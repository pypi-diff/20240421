# Comparing `tmp/rnaseqc-0.0.2.tar.gz` & `tmp/rnaseqc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rnaseqc-0.0.2.tar", last modified: Wed May 13 16:58:22 2020, max compression
+gzip compressed data, was "rnaseqc-0.0.3.tar", last modified: Sun Apr 21 06:01:42 2024, max compression
```

## Comparing `rnaseqc-0.0.2.tar` & `rnaseqc-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 aarong   (1067564159) 1594166068        0 2020-05-13 16:58:22.000000 rnaseqc-0.0.2/
--rw-r--r--   0 aarong   (1067564159) 1594166068     2582 2020-05-13 16:58:22.000000 rnaseqc-0.0.2/PKG-INFO
--rw-r--r--   0 aarong   (1067564159) 1594166068     1705 2020-05-11 22:03:25.000000 rnaseqc-0.0.2/README.md
-drwxr-xr-x   0 aarong   (1067564159) 1594166068        0 2020-05-13 16:58:22.000000 rnaseqc-0.0.2/rnaseqc/
--rw-r--r--   0 aarong   (1067564159) 1594166068       22 2020-05-13 16:57:46.000000 rnaseqc-0.0.2/rnaseqc/__init__.py
--rw-r--r--   0 aarong   (1067564159) 1594166068     2587 2020-05-13 16:56:17.000000 rnaseqc-0.0.2/rnaseqc/__main__.py
--rw-r--r--   0 aarong   (1067564159) 1594166068     6388 2020-05-12 22:07:31.000000 rnaseqc-0.0.2/rnaseqc/aggregate.py
--rw-r--r--   0 aarong   (1067564159) 1594166068     2073 2020-05-11 21:36:48.000000 rnaseqc-0.0.2/rnaseqc/create_notebook.py
--rw-r--r--   0 aarong   (1067564159) 1594166068     4546 2020-05-11 21:37:00.000000 rnaseqc-0.0.2/rnaseqc/insert_size_intervals.py
--rw-r--r--   0 aarong   (1067564159) 1594166068     4151 2020-05-11 21:47:53.000000 rnaseqc-0.0.2/rnaseqc/legacy_exon_remap.py
--rw-r--r--   0 aarong   (1067564159) 1594166068     4135 2020-05-11 20:23:30.000000 rnaseqc-0.0.2/rnaseqc/nb_encode.py
--rw-r--r--   0 aarong   (1067564159) 1594166068    19808 2020-05-11 19:58:18.000000 rnaseqc-0.0.2/rnaseqc/plot.py
--rw-r--r--   0 aarong   (1067564159) 1594166068     6971 2020-05-11 21:37:15.000000 rnaseqc-0.0.2/rnaseqc/report.py
--rw-r--r--   0 aarong   (1067564159) 1594166068     3216 2020-05-13 16:55:07.000000 rnaseqc-0.0.2/rnaseqc/run.py
-drwxr-xr-x   0 aarong   (1067564159) 1594166068        0 2020-05-13 16:58:22.000000 rnaseqc-0.0.2/rnaseqc.egg-info/
--rw-r--r--   0 aarong   (1067564159) 1594166068     2582 2020-05-13 16:58:22.000000 rnaseqc-0.0.2/rnaseqc.egg-info/PKG-INFO
--rw-r--r--   0 aarong   (1067564159) 1594166068      392 2020-05-13 16:58:22.000000 rnaseqc-0.0.2/rnaseqc.egg-info/SOURCES.txt
--rw-r--r--   0 aarong   (1067564159) 1594166068        1 2020-05-13 16:58:22.000000 rnaseqc-0.0.2/rnaseqc.egg-info/dependency_links.txt
--rw-r--r--   0 aarong   (1067564159) 1594166068       52 2020-05-13 16:58:22.000000 rnaseqc-0.0.2/rnaseqc.egg-info/requires.txt
--rw-r--r--   0 aarong   (1067564159) 1594166068        8 2020-05-13 16:58:22.000000 rnaseqc-0.0.2/rnaseqc.egg-info/top_level.txt
--rw-r--r--   0 aarong   (1067564159) 1594166068       38 2020-05-13 16:58:22.000000 rnaseqc-0.0.2/setup.cfg
--rw-r--r--   0 aarong   (1067564159) 1594166068      946 2020-05-11 21:57:04.000000 rnaseqc-0.0.2/setup.py
+drwxrwxr-x   0 aguet     (1001) aguet     (1002)        0 2024-04-21 06:01:42.866390 rnaseqc-0.0.3/
+-rw-r--r--   0 aguet     (1001) aguet     (1002)     2176 2024-04-21 06:01:42.866390 rnaseqc-0.0.3/PKG-INFO
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)     1705 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/README.md
+drwxrwxr-x   0 aguet     (1001) aguet     (1002)        0 2024-04-21 06:01:42.866390 rnaseqc-0.0.3/rnaseqc/
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)       22 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/rnaseqc/__init__.py
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)     2587 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/rnaseqc/__main__.py
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)     6642 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/rnaseqc/aggregate.py
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)     2638 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/rnaseqc/create_notebook.py
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)     4482 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/rnaseqc/insert_size_intervals.py
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)     3960 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/rnaseqc/legacy_exon_remap.py
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)     4135 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/rnaseqc/nb_encode.py
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)    25390 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/rnaseqc/plot.py
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)     9550 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/rnaseqc/report.py
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)     3216 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/rnaseqc/run.py
+drwxrwxr-x   0 aguet     (1001) aguet     (1002)        0 2024-04-21 06:01:42.866390 rnaseqc-0.0.3/rnaseqc.egg-info/
+-rw-r--r--   0 aguet     (1001) aguet     (1002)     2176 2024-04-21 06:01:42.000000 rnaseqc-0.0.3/rnaseqc.egg-info/PKG-INFO
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)      392 2024-04-21 06:01:42.000000 rnaseqc-0.0.3/rnaseqc.egg-info/SOURCES.txt
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)        1 2024-04-21 06:01:42.000000 rnaseqc-0.0.3/rnaseqc.egg-info/dependency_links.txt
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)       52 2024-04-21 06:01:42.000000 rnaseqc-0.0.3/rnaseqc.egg-info/requires.txt
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)        8 2024-04-21 06:01:42.000000 rnaseqc-0.0.3/rnaseqc.egg-info/top_level.txt
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)       38 2024-04-21 06:01:42.866390 rnaseqc-0.0.3/setup.cfg
+-rw-rw-r--   0 aguet     (1001) aguet     (1002)      946 2024-04-21 00:25:47.000000 rnaseqc-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rnaseqc-0.0.2/PKG-INFO` & `rnaseqc-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,78 @@
 Metadata-Version: 2.1
 Name: rnaseqc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Multi-sample visualization of metrics from RNA-SeQC
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: # RNA-SeQC Python utilities
-        
-        This module contains utility code for RNA-SeQC
-        
-        ## Installing
-        
-        * From pip: `pip install rnaseqc`
-        * From the git repo: `pip install -e python` (Invoke from root of git repo)
-        
-        ## Usage
-        
-        This does not install a console entrypoint. You can invoke the utilities in one of three ways:
-        
-        * From the main module: `python3 -m rnaseqc ...`
-        * Calling the target module: `python3 -m rnaseqc.example ...`
-        * Calling scripts directly: `python3 python/rnaseqc/example.py`
-        
-        ## Utilities
-        
-        The `rnaseqc` module contains 5 main utilities. To get more help with each utility,
-        invoke the utility with the `-h` or `--help` option
-        
-        ### Aggregation
-        
-        Aggregates RNA-SeQC outputs from multiple samples
-        
-        ```
-        python3 -m rnaseqc aggregate [-h] [--parquet] [-o OUTPUT_DIR] results_dir prefix
-        ```
-        
-        ### Jupyter Notebooks
-        
-        Creates a jupyter notebook with several figures for comparing samples
-        
-        ```
-        python3 -m rnaseqc notebook [-h] [-t TPM] [-i INSERT_SIZE] [-c COHORT] [-d DATE] metrics output
-        ```
-        
-        ### Figures
-        
-        Generates figures from an aggregated RNA-SeQC metrics table
-        
-        ```
-        python3 -m rnaseqc report [-h] [--tpm TPM] [--insert-size INSERT_SIZE] [--cohort COHORT] [--output-dir OUTPUT_DIR] [--dpi DPI] metrics prefix
-        ```
-        
-        ### Insert Size distributions
-        
-        Generates a BED file with intervals used by RNA-SeQC for estimating a sample's insert size distribution
-        
-        ```
-        python3 -m rnaseqc insert-size [-h] [--min-length MIN_LENGTH] [--min-mappability MIN_MAPPABILITY] [--output-dir OUTPUT_DIR] gtf_path mappability_bigwig prefix
-        ```
-        
-        ### Exon remapping
-        
-        Convert exon names in an `*.exon_reads.gct` file from RNA-SeQC 2.X.X to match names
-        as reported by RNA-SeQC 1.1.9
-        
-        ```
-        python3 -m rnaseqc legacy-exons gct gtf
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: qtl
+Requires-Dist: agutil
+Requires-Dist: nbformat
+
+# RNA-SeQC Python utilities
+
+This module contains utility code for RNA-SeQC
+
+## Installing
+
+* From pip: `pip install rnaseqc`
+* From the git repo: `pip install -e python` (Invoke from root of git repo)
+
+## Usage
+
+This does not install a console entrypoint. You can invoke the utilities in one of three ways:
+
+* From the main module: `python3 -m rnaseqc ...`
+* Calling the target module: `python3 -m rnaseqc.example ...`
+* Calling scripts directly: `python3 python/rnaseqc/example.py`
+
+## Utilities
+
+The `rnaseqc` module contains 5 main utilities. To get more help with each utility,
+invoke the utility with the `-h` or `--help` option
+
+### Aggregation
+
+Aggregates RNA-SeQC outputs from multiple samples
+
+```
+python3 -m rnaseqc aggregate [-h] [--parquet] [-o OUTPUT_DIR] results_dir prefix
+```
+
+### Jupyter Notebooks
+
+Creates a jupyter notebook with several figures for comparing samples
+
+```
+python3 -m rnaseqc notebook [-h] [-t TPM] [-i INSERT_SIZE] [-c COHORT] [-d DATE] metrics output
+```
+
+### Figures
+
+Generates figures from an aggregated RNA-SeQC metrics table
+
+```
+python3 -m rnaseqc report [-h] [--tpm TPM] [--insert-size INSERT_SIZE] [--cohort COHORT] [--output-dir OUTPUT_DIR] [--dpi DPI] metrics prefix
+```
+
+### Insert Size distributions
+
+Generates a BED file with intervals used by RNA-SeQC for estimating a sample's insert size distribution
+
+```
+python3 -m rnaseqc insert-size [-h] [--min-length MIN_LENGTH] [--min-mappability MIN_MAPPABILITY] [--output-dir OUTPUT_DIR] gtf_path mappability_bigwig prefix
+```
+
+### Exon remapping
+
+Convert exon names in an `*.exon_reads.gct` file from RNA-SeQC 2.X.X to match names
+as reported by RNA-SeQC 1.1.9
+
+```
+python3 -m rnaseqc legacy-exons gct gtf
+```
```

### Comparing `rnaseqc-0.0.2/README.md` & `rnaseqc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rnaseqc-0.0.2/rnaseqc/__main__.py` & `rnaseqc-0.0.3/rnaseqc/__main__.py`

 * *Files identical despite different names*

### Comparing `rnaseqc-0.0.2/rnaseqc/aggregate.py` & `rnaseqc-0.0.3/rnaseqc/aggregate.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,58 +26,57 @@
     # allocate
     gct_df = pd.DataFrame(0, index=df.index, columns=['Description']+list(sample_ids), dtype=dtype)
     gct_df['Description'] = df['Description']
     gct_df[sample_id] = df[sample_id].astype(dtype)
 
     for k,sample_id in enumerate(sample_ids[1:], 2):
         if verbose:
-            print('\r  * loading GCT {}/{}'.format(k, len(path_dict)), end='', flush=True)
+            print(f'\r  * loading GCT {k}/{len(path_dict)}', end='', flush=True)
         df = pd.read_csv(path_dict[sample_id], sep='\t', skiprows=3, header=None,
                          usecols=[0,2],  index_col=0, names=['Name', sample_id],
                          dtype={'Name':str, sample_id:dtype})
         gct_df[sample_id] = df[sample_id]
     if verbose:
         print()
 
     return gct_df
 
 
 def write_gct(df, gct_file, float_format='%.6g', compresslevel=6):
     """Write pd.DataFrame to GCT format"""
 
-    assert df.index.name=='Name' and df.columns[0]=='Description'
+    assert df.index.name == 'Name' and df.columns[0] == 'Description'
 
     if gct_file.endswith('.gct.gz'):
         opener = gzip.open(gct_file, 'wt', compresslevel=compresslevel)
     else:
         opener = open(gct_file, 'w')
 
     with opener as gct:
-        gct.write('#1.2\n{0:d}\t{1:d}\n'.format(df.shape[0], df.shape[1]-1))
+        gct.write(f'#1.2\n{df.shape[0]:d}\t{df.shape[1]-1:d}\n')
         df.to_csv(gct, sep='\t', float_format=float_format)
 
 
 def combine_metrics(path_dict):
     """Aggregate single-sample metrics files."""
     metrics_df = []
     for k,sample_id in enumerate(sorted(path_dict), 1):
-        metrics_df.append(pd.read_csv(path_dict[sample_id], sep='\t', index_col=0).astype(np.float32))
+        metrics_df.append(pd.read_csv(path_dict[sample_id], sep='\t', index_col=0, dtype=str))
     metrics_df = pd.concat(metrics_df, axis=1).T
     metrics_df.index.name = 'sample_id'
     return metrics_df
 
 
-def combine_insert_sizes(path_dict):
+def combine_distributions(path_dict):
     """Aggregate single-sample insert sizes distributions."""
-    insertsize_df = []
+    distr_df = []
     for k,sample_id in enumerate(sorted(path_dict), 1):
-        insertsize_df.append(pd.read_csv(path_dict[sample_id], sep='\t', index_col=0, squeeze=True).rename(sample_id))
-    insertsize_df = pd.concat(insertsize_df, axis=1).fillna(0).astype(np.int32)
-    return insertsize_df
-
+        distr_df.append(pd.read_csv(path_dict[sample_id], sep='\t', index_col=0).squeeze('columns').rename(sample_id))
+    distr_df = pd.concat(distr_df, axis=1).fillna(0).astype(np.int32)
+    return distr_df
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Aggregate RNA-SeQC outputs')
     parser.add_argument('results_dir', help='Directory containing RNA-SeQC outputs for all samples to be combined.')
     parser.add_argument('prefix', help='Prefix for output files, e.g., <prefix>.gct.gz')
     parser.add_argument('--parquet', action='store_true', help='Write to parquet format instead of GCT')
@@ -90,51 +89,57 @@
     # if os.path.isdir(args.results):
     gene_reads_gcts =  {os.path.basename(i).split('.')[0]:i for i in glob.glob(os.path.join(args.results_dir, '**/*gene_reads.gct*'), recursive=True)}
     gene_fragm_gcts =  {os.path.basename(i).split('.')[0]:i for i in glob.glob(os.path.join(args.results_dir, '**/*gene_fragments.gct*'), recursive=True)}
     gene_tpm_gcts =    {os.path.basename(i).split('.')[0]:i for i in glob.glob(os.path.join(args.results_dir, '**/*gene_tpm.gct*'), recursive=True)}
     exon_reads_gcts =  {os.path.basename(i).split('.')[0]:i for i in glob.glob(os.path.join(args.results_dir, '**/*exon_reads.gct*'), recursive=True)}
     metrics_files =    {os.path.basename(i).split('.')[0]:i for i in glob.glob(os.path.join(args.results_dir, '**/*metrics.tsv*'), recursive=True)}
     insertsize_files = {os.path.basename(i).split('.')[0]:i for i in glob.glob(os.path.join(args.results_dir, '**/*fragmentSizes.txt*'), recursive=True)}
+    gc_content_files = {os.path.basename(i).split('.')[0]:i for i in glob.glob(os.path.join(args.results_dir, '**/*gc_content.tsv*'), recursive=True)}
     # coverage files don't get aggregated
     # coverage_files =   {os.path.basename(i).split('.')[0]:i for i in glob.glob(os.path.join(args.results, '*coverage.tsv*'))}
 
     if len(metrics_files) > 0:
         print('Aggregating metrics')
         metrics_df = combine_metrics(metrics_files)
-        metrics_df.to_csv(os.path.join(args.output_dir, '{}.metrics.txt.gz'.format(args.prefix)), sep='\t', float_format='%.6g')
+        metrics_df.to_csv(os.path.join(args.output_dir, f'{args.prefix}.metrics.txt.gz'), sep='\t')
 
     if len(insertsize_files) > 0:
         print('Aggregating insert size distributions')
-        insertsize_df = combine_insert_sizes(insertsize_files)
-        insertsize_df.to_csv(os.path.join(args.output_dir, '{}.insert_size_hists.txt.gz'.format(args.prefix)), sep='\t')
+        insertsize_df = combine_distributions(insertsize_files)
+        insertsize_df.to_csv(os.path.join(args.output_dir, f'{args.prefix}.insert_size_hists.txt.gz'), sep='\t')
+
+    if len(gc_content_files) > 0:
+        print('Aggregating GC content distributions')
+        gc_df = combine_distributions(gc_content_files)
+        gc_df.to_csv(os.path.join(args.output_dir, f'{args.prefix}.gc_content_hists.txt.gz'), sep='\t')
 
     if len(gene_reads_gcts) > 0:
         print('Aggregating read count GCTs')
         gct_df = combine_gcts(gene_reads_gcts)
         if args.parquet:
-            gct_df.to_parquet(os.path.join(args.output_dir, '{}.gene_reads.parquet'.format(args.prefix)))
+            gct_df.to_parquet(os.path.join(args.output_dir, f'{args.prefix}.gene_reads.parquet'))
         else:
-            write_gct(gct_df, os.path.join(args.output_dir, '{}.gene_reads.gct.gz'.format(args.prefix)))
+            write_gct(gct_df, os.path.join(args.output_dir, f'{args.prefix}.gene_reads.gct.gz'))
 
     if len(gene_fragm_gcts) > 0:
         print('Aggregating fragment count GCTs')
         gct_df = combine_gcts(gene_fragm_gcts)
         if args.parquet:
-            gct_df.to_parquet(os.path.join(args.output_dir, '{}.gene_fragments.parquet'.format(args.prefix)))
+            gct_df.to_parquet(os.path.join(args.output_dir, f'{args.prefix}.gene_fragments.parquet'))
         else:
-            write_gct(gct_df, os.path.join(args.output_dir, '{}.gene_fragments.gct.gz'.format(args.prefix)))
+            write_gct(gct_df, os.path.join(args.output_dir, f'{args.prefix}.gene_fragments.gct.gz'))
 
     if len(gene_tpm_gcts) > 0:
         print('Aggregating TPM GCTs')
         gct_df = combine_gcts(gene_tpm_gcts)
         if args.parquet:
-            gct_df.to_parquet(os.path.join(args.output_dir, '{}.gene_tpm.parquet'.format(args.prefix)))
+            gct_df.to_parquet(os.path.join(args.output_dir, f'{args.prefix}.gene_tpm.parquet'))
         else:
-            write_gct(gct_df, os.path.join(args.output_dir, '{}.gene_tpm.gct.gz'.format(args.prefix)))
+            write_gct(gct_df, os.path.join(args.output_dir, f'{args.prefix}.gene_tpm.gct.gz'))
 
     if len(exon_reads_gcts) > 0:
         print('Aggregating exon read count GCTs')
         gct_df = combine_gcts(exon_reads_gcts)
         if args.parquet:
-            gct_df.to_parquet(os.path.join(args.output_dir, '{}.exon_reads.parquet'.format(args.prefix)))
+            gct_df.to_parquet(os.path.join(args.output_dir, f'{args.prefix}.exon_reads.parquet'))
         else:
-            write_gct(gct_df, os.path.join(args.output_dir, '{}.exon_reads.gct.gz'.format(args.prefix)))
+            write_gct(gct_df, os.path.join(args.output_dir, f'{args.prefix}.exon_reads.gct.gz'))
```

### Comparing `rnaseqc-0.0.2/rnaseqc/create_notebook.py` & `rnaseqc-0.0.3/rnaseqc/create_notebook.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,27 +13,35 @@
 
     nb.add_code_cell([
         'import pandas as pd',
         'import qtl.io',
         'import rnaseqc.report'
     ])
 
-    nb.add_code_cell([
+    cell = [
         "# load inputs",
         "metrics_df = pd.read_csv('{}', sep='\\t', index_col=0)".format(args.metrics),
-        "tpm_df = qtl.io.read_gct('{}')".format(args.tpm),
-        "cohort_s = pd.read_csv('{}', sep='\\t', index_col=0, header=None, squeeze=True)".format(args.cohort),
-        "insertsize_df = pd.read_csv('{}', sep='\\t', index_col=0)".format(args.insert_size),
-    ])
+    ]
+    if args.tpm is not None:
+        cell.append("tpm_df = qtl.io.read_gct('{}')".format(args.tpm))
+    if args.cohort is not None:
+        cell.append("cohort_s = pd.read_csv('{}', sep='\\t', index_col=0, header=None).squeeze('columns')".format(args.cohort))
+    if args.date is not None:
+        cell.append("date_s = pd.read_csv('{}', sep='\\t', index_col=0, header=None).squeeze('columns')".format(args.date))
+    if args.insert_size is not None:
+        cell.append("insertsize_df = pd.read_csv('{}', sep='\\t', index_col=0)".format(args.insert_size))
+    nb.add_code_cell(cell)
 
     nb.add_code_cell([
         "thresholds = {'Exonic Rate': 0.7}",
-        'rnaseqc.report.plot_qc_figures(metrics_df, cohort_s=cohort_s, cohort_colors=None, date_s=None,',
+        'rnaseqc.report.plot_qc_figures(metrics_df, cohort_s={}, cohort_colors=None, date_s={},'.format(
+            'cohort_s' if args.cohort is not None else 'None', 'date_s' if args.date is not None else 'None'),
         '                               show_legend=True, ms=12, alpha=1, highlight_ids=None,',
-        '                               thresholds=thresholds, insertsize_df=insertsize_df, tpm_df=tpm_df)',
+        '                               thresholds=thresholds, insertsize_df={}, tpm_df={})'.format(
+            'insertsize_df' if args.insert_size is not None else 'None', 'tpm_df' if args.tpm is not None else 'None'),
     ])
 
     nb.add_code_cell('')
     nb.write(args.output)
 
 
 
@@ -51,8 +59,8 @@
                         help='TSV file mapping sample IDs to dates')
     args = parser.parse_args()
 
     # generate notebook
     main(args)
 
     # execute notebook
-    subprocess.check_call('jupyter nbconvert --execute --inplace {}'.format(args.output.name), shell=True)
+    subprocess.check_call('jupyter nbconvert --execute --ExecutePreprocessor.timeout=300 --inplace {}'.format(args.output.name), shell=True)
```

### Comparing `rnaseqc-0.0.2/rnaseqc/insert_size_intervals.py` & `rnaseqc-0.0.3/rnaseqc/insert_size_intervals.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,50 +50,50 @@
 
     bw = pyBigWig.open(mappability_bw)
     gintervals = {}
     for c in annot.chr_list:
         exon_coords = []
         for g in annot.chr_genes[c]:
             for t in g.transcripts:
-                if (t.type!='retained_intron') and (('tags' not in t.attributes) or len(set(t.attributes['tags']).intersection(exclude))==0):
+                if (t.type not in exclude) and (('tags' not in t.attributes) or len(set(t.attributes['tags']).intersection(exclude)) == 0):
                     for e in t.exons:
                         exon_coords.append((e.start_pos, e.end_pos))
 
         v = np.array(intersect_overlap(exon_coords))  # intersect all exons on current chr
         l = v[:,1]-v[:,0]+1
         gintervals[c] = v[l >= min_length, :]
         # filter by mappability
         gintervals[c] = np.array([i for i in gintervals[c] if bw.stats(c, int(i[0])-1, int(i[1]), exact=True)[0] >= min_mappability])
     bw.close()
 
     # all intervals
-    with open(os.path.join(output_dir, '{}_geq{}bp.bed'.format(prefix, min_length)), 'w') as f:
+    with open(os.path.join(output_dir, f'{prefix}_geq{min_length}bp.bed'), 'w') as f:
         f.write('#chr\tstart\tend\n')
         for c in annot.chr_list:
             for i in range(gintervals[c].shape[0]):
-                f.write('{0:s}\t{1:d}\t{2:d}\n'.format(c, gintervals[c][i][0]-1, gintervals[c][i][1]))  # BED is 0-indexed, [..)
+                f.write(f'{c}\t{gintervals[c][i][0]-1}\t{gintervals[c][i][1]}\n')  # BED is 0-indexed, [..)
 
     # single-isoform genes
     gintervals_1iso = {}
     for c in annot.chr_list:
         ec = []
         for g in annot.chr_genes[c]:
             if len(g.transcripts) == 1:
                 for e in g.transcripts[0].exons:
                     if e.length >= min_length:
                         ec.append([e.start_pos, e.end_pos])
         ec = list(set([tuple(i) for i in ec]).intersection(set([tuple(i) for i in gintervals[c]])))
         ec.sort(key=lambda x: (x[0],x[1]))
         gintervals_1iso[c] = np.array(ec)
 
-    with open(os.path.join(output_dir, '{}_geq{}bp_1iso.bed'.format(prefix, min_length)), 'w') as f:
+    with open(os.path.join(output_dir, f'{prefix}_geq{min_length}bp_1iso.bed'), 'w') as f:
         f.write('#chr\tstart\tend\n')
         for c in annot.chr_list:
             for i in range(gintervals_1iso[c].shape[0]):
-                f.write('{0:s}\t{1:d}\t{2:d}\n'.format(c, gintervals_1iso[c][i][0]-1, gintervals_1iso[c][i][1]))
+                f.write(f'{c}\t{gintervals_1iso[c][i][0]-1}\t{gintervals_1iso[c][i][1]}\n')
 
 
 if __name__=='__main__':
 
     parser = argparse.ArgumentParser(description='Parse long exons/UTRs with high mappability for estimating insert size distribution.')
     parser.add_argument('gtf_path', help='Reference annotation in GTF format.')
     parser.add_argument('mappability_bigwig', help='Mappability track in bigWig format.')
```

### Comparing `rnaseqc-0.0.2/rnaseqc/legacy_exon_remap.py` & `rnaseqc-0.0.3/rnaseqc/legacy_exon_remap.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,53 +15,51 @@
     reader = csv.DictReader(args.gct, delimiter='\t')
     w = tempfile.NamedTemporaryFile('w')
     w.write(header)
     writer = csv.DictWriter(w, reader.fieldnames, delimiter='\t', lineterminator='\n')
     writer.writeheader()
     current = None
     features = []
-    with status_bar(numRows) as bar:
-        for line in reader:
-            bar.update(bar.current + 1)
-            gene = '_'.join(line['Name'].split('_')[:-1])
-            if gene != current:
-                if current is not None:
-                    ref = gtf.get_gene(current)
+    for line in status_bar.iter(reader, maximum=numRows):
+        gene = '_'.join(line['Name'].split('_')[:-1])
+        if gene != current:
+            if current is not None:
+                ref = gtf.get_gene(current)
+                try:
+                    if len(ref):
+                        ref = ref[0]
+                except:
+                    pass
+                exons = {exon.id:exon for transcript in ref.transcripts for exon in transcript.exons}
+                raw_size = len(exons)
+                for exon in [exon for exon in exons]:
                     try:
-                        if len(ref):
-                            ref = ref[0]
+                        if exon.isdigit() and int(exon) <= raw_size:
+                            exons[current+'_'+exon] = exons[exon]
                     except:
                         pass
-                    exons = {exon.id:exon for transcript in ref.transcripts for exon in transcript.exons}
-                    raw_size = len(exons)
-                    for exon in [exon for exon in exons]:
-                        try:
-                            if exon.isdigit() and int(exon) <= raw_size:
-                                exons[current+'_'+exon] = exons[exon]
-                        except:
-                            pass
-                    features.sort(
-                        key=lambda feat:(
-                            1 if exons[feat['Name']].length == 1 else 0,
-                            exons[feat['Name']].start_pos,
-                            exons[feat['Name']].end_pos
-                        )
+                features.sort(
+                    key=lambda feat:(
+                        1 if exons[feat['Name']].length == 1 else 0,
+                        exons[feat['Name']].start_pos,
+                        exons[feat['Name']].end_pos
                     )
-                    for i in range(len(features)):
-                        parts = features[i]['Name'].split('_')
-                        prefix = '_'.join(parts[:-1])
-                        suffix = parts[-1]
-                        if exons[features[i]['Name']].length == 1:
-                            features[i][reader.fieldnames[-1]] = 0
-                        suffix = str(i)
-                        features[i]['Name'] = prefix+'_'+suffix
-                    writer.writerows(features)
-                current = gene
-                features = []
-            features.append({k:v for k,v in line.items()})
+                )
+                for i in range(len(features)):
+                    parts = features[i]['Name'].split('_')
+                    prefix = '_'.join(parts[:-1])
+                    suffix = parts[-1]
+                    if exons[features[i]['Name']].length == 1:
+                        features[i][reader.fieldnames[-1]] = 0
+                    suffix = str(i)
+                    features[i]['Name'] = prefix+'_'+suffix
+                writer.writerows(features)
+            current = gene
+            features = []
+        features.append({k:v for k,v in line.items()})
     if len(features):
         ref = gtf.get_gene(current)
         try:
             if len(ref):
                 ref = ref[0]
         except:
             pass
```

### Comparing `rnaseqc-0.0.2/rnaseqc/nb_encode.py` & `rnaseqc-0.0.3/rnaseqc/nb_encode.py`

 * *Files identical despite different names*

### Comparing `rnaseqc-0.0.2/rnaseqc/plot.py` & `rnaseqc-0.0.3/rnaseqc/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,186 +13,240 @@
     if nc > 5:
         cohort_colors = {i:j for i,j in zip(cohorts, plt.cm.get_cmap('Spectral', nc)(np.random.permutation(np.arange(nc)))[:,:-1])}
     else:
         cohort_colors = {i:j for i,j in zip(cohorts, plt.cm.get_cmap('tab10', 10)(np.arange(nc))[:,:-1])}
     return cohort_colors
 
 
-def mismatch_rates(metrics_df, cohort_s=None, cohort_colors=None, ms=12, alpha=1,
-                   aw=2, end1_threshold=None, end2_threshold=None):
+def sort_samples(sample_ix, cohort_s=None, cohort_order=None, date_s=None):
+    """Sort samples by date and cohort label"""
+    if cohort_s is None and date_s is None:
+        return sample_ix
+
+    if cohort_s is not None:
+        assert sample_ix.isin(cohort_s.index).all()
+        cohort_s = cohort_s[sample_ix]
+    if date_s is not None:
+        assert sample_ix.isin(cohort_s.index).all()
+        date_s = date_s[sample_ix]
+
+    if date_s is not None:
+        if cohort_s is not None:  # sort samples by date and cohort
+            sorted_ix = pd.concat([
+                pd.to_datetime(date_s).rename('date'), cohort_s.rename('cohort')], axis=1
+            ).sort_values(['date', 'cohort'], na_position='first').index
+        else:
+            sorted_ix = pd.to_datetime(date_s).sort_values(na_position='first').index
+    else:  # sort by cohort only
+        if cohort_order is None:
+            sorted_ix = cohort_s.sort_values(na_position='first').index
+        else:
+            sorted_ix = cohort_s.map({j:i for i,j in enumerate(cohort_order)}).sort_values(na_position='first').index
+
+    return sorted_ix
+
+
+def mismatch_rates(metrics_df, cohort_s=None, cohort_order=None, cohort_colors=None, ms=12, alpha=1, aw=2,
+                   end1_threshold=None, end2_threshold=None,
+                   end1_limit=0.01, end2_limit=0.025):
     """Plot base mismatch rates ('NM' tag) for read mate 1 vs read mate 2."""
 
     if cohort_s is not None:
         assert metrics_df.index.isin(cohort_s.index).all()
+        cohort_s = cohort_s.loc[metrics_df.index]
     else:
         cohort_s = pd.Series('NA', index=metrics_df.index)
 
     ax = qtl.plot.setup_figure(aw, aw)
 
     x = metrics_df['End 1 Mismatch Rate'].copy()
     y = metrics_df['End 2 Mismatch Rate'].copy()
-    x[x>0.01] = 0.01
-    y[y>0.025] = 0.025
+    x[x>end1_limit] = end1_limit
+    y[y>end2_limit] = end2_limit
 
-    cohorts = cohort_s.unique()
+    sorted_ix = sort_samples(metrics_df.index, cohort_s=cohort_s, cohort_order=cohort_order)
+    cohorts = cohort_s.loc[sorted_ix].unique()
     if cohort_colors is None:
         cohort_colors = get_cohort_colors(cohorts)
 
     for t in cohorts:
         ix = cohort_s[cohort_s==t].index
         ax.scatter(x[ix], y[ix], s=ms, edgecolor='none', label=t,
             c=[cohort_colors[t]], alpha=alpha, clip_on=False, rasterized=True)
 
     if end1_threshold is not None:
         ax.plot(2*[end1_threshold], [0,0.2], '--',  color=[0.6]*3, zorder=0, lw=1, alpha=0.8)
     if end2_threshold is not None:
         ax.plot([0,0.02], 2*[end2_threshold], '--', color=[0.6]*3, zorder=0, lw=1, alpha=0.8)
     if end1_threshold is not None or end2_threshold is not None:
         ix = (x > end1_threshold) | (y > end2_threshold)
-        ax.scatter(x[ix], y[ix], c='none', edgecolor='k', s=ms, lw=1, label=None)
+        ax.scatter(x[ix], y[ix], c='none', edgecolor='k', s=ms, lw=1, label=None, clip_on=False, rasterized=True)
 
-    ax.set_xlim([0, 0.01])
-    ax.set_ylim([0, 0.025])
     qtl.plot.format_plot(ax, fontsize=10)
+    ax.set_xlim([0, end1_limit])
+    ax.set_ylim([0, end2_limit])
 
     ax.spines['left'].set_position(('outward', 6))
     ax.spines['bottom'].set_position(('outward', 6))
-    ax.plot([0, 0.01], [0, 0.01], '--', c=[0.6]*3, lw=1, zorder=0)
+    ax.plot([0, end1_limit], [0, end1_limit], '--', c=[0.6]*3, lw=1, zorder=0)
 
     ax.set_xlabel('End 1 mismatch rate', fontsize=12)
     ax.set_ylabel('End 2 mismatch rate', fontsize=12)
 
 
-def metrics(metric_s, cohort_s=None, ylim=None, ms=12, alpha=1, ylabel=None, cohort_colors=None,
-            date_s=None, threshold=None, threshold_dir=None, show_legend=False,
+def metrics(metric_s, cohort_s=None, cohort_order=None, cohort_colors=None, date_s=None,
+            threshold=None, threshold_dir=None, outlier_method='threshold', plot_density=True, show_legend=False,
+            ms=12, alpha=1, ylim=None, ylabel=None,
             show_xticklabels=False, highlight_ids=None,
             dl=0.85, aw=6, ds=0.2, daw=0.5, dr=0.25,
-            db=0.75, ah=2, dt=0.25):
+            db=0.75, ah=2, dt=0.25, fontsize=10, rasterized=True):
     """Plot a single QC metric sorted by cohort and/or date"""
 
     if ylabel is None:
         ylabel = metric_s.name
 
     if metric_s.median() > 1e5:
         metric_s = metric_s.copy() / 1e6
         if threshold is not None:
             threshold = threshold / 1e6
         ylabel += ' (millions)'
 
     if cohort_s is not None:
         assert metric_s.index.isin(cohort_s.index).all()
+        cohort_s = cohort_s.loc[metric_s.index]
     else:
         cohort_s = pd.Series('NA', index=metric_s.index)
 
     if show_xticklabels:
         db += 0.75
 
-    fw = dl + aw + ds + daw + dr
+    if plot_density:
+        fw = dl + aw + ds + daw + dr
+    else:
+        fw = dl + aw + dr
     fh = db + ah + dt
     fig = plt.figure(facecolor=(1,1,1), figsize=(fw,fh))
     ax = fig.add_axes([dl/fw, db/fh, aw/fw, ah/fh])
-    dax = fig.add_axes([(dl+aw+ds)/fw, db/fh, daw/fw, ah/fh], sharey=ax)
+    if plot_density:
+        dax = fig.add_axes([(dl+aw+ds)/fw, db/fh, daw/fw, ah/fh], sharey=ax)
 
-    if date_s is not None:  # sort samples by date and cohort
-        # date_ix = pd.to_datetime(date_s).sort_values(na_position='first').index
-        date_ix = pd.concat([pd.to_datetime(date_s).rename('date'), cohort_s.rename('cohort')], axis=1).sort_values(['date', 'cohort'], na_position='first').index
+    if date_s is not None:
         xlabel = 'Samples, ordered by date'
     else:
-        date_ix = metric_s.index
         xlabel = 'Samples'
 
-    cohorts = cohort_s.loc[date_ix].unique()
+    sorted_ix = sort_samples(metric_s.index, cohort_s=cohort_s, cohort_order=cohort_order, date_s=date_s)
+    cohorts = cohort_s.loc[sorted_ix].unique()
     if cohort_colors is None:
         cohort_colors = get_cohort_colors(cohorts)
 
     ns = len(metric_s)
-    xpos = pd.Series(np.arange(1,ns+1), index=date_ix)
+    xpos = pd.Series(np.arange(1,ns+1), index=sorted_ix)
 
     # plot
     for t in cohorts:
         ix = cohort_s[cohort_s==t].index
-        # ix = xpos.index[xpos.index.isin(cohort_s[cohort_s==t].index)]
         ax.scatter(xpos[ix], metric_s[ix], s=ms, edgecolor='none', label=t,
-            c=cohort_colors[t].reshape(1,-1), alpha=alpha, clip_on=False, rasterized=True)
+                   c=[cohort_colors[t]], alpha=alpha, clip_on=False, rasterized=rasterized)
 
     if highlight_ids is not None:
-        ax.scatter(xpos[highlight_ids], metric_s[highlight_ids], marker='s', edgecolor='k', facecolor='none')
+        ax.scatter(xpos[highlight_ids], metric_s[highlight_ids], marker='s',
+                   edgecolor='k', facecolor='none', clip_on=False, rasterized=rasterized)
 
     if threshold is not None:
         ax.plot([-0.02*ns, 1.02*ns], 2*[threshold], '--', color=[0.6,0.6,0.6], lw=1, alpha=0.8)
-        if threshold_dir=='gt':
-            ix = metric_s > threshold
-        elif threshold_dir=='lt':
-            ix = metric_s < threshold
-        ax.scatter(xpos[np.where(ix)[0]], metric_s[ix], c='none', edgecolor='k', s=ms, lw=1, label=None)
 
-    sns.kdeplot(metric_s, ax=dax, vertical=True, legend=False, shade=True)
+    if outlier_method.lower() == 'iqr':
+        p = np.percentile(metric_s, [25, 75])
+        if threshold_dir == 'gt':
+            ix = metric_s[metric_s > p[1] + 1.5*(p[1]-p[0])].index
+        elif threshold_dir == 'lt':
+            ix = metric_s[metric_s < p[0] - 1.5*(p[1]-p[0])].index
+        if any(ix):
+            ax.scatter(xpos[ix], metric_s[ix], c='none', edgecolor='k', s=ms, lw=1, label=None, clip_on=False, rasterized=rasterized)
+    elif outlier_method.lower() == 'threshold' and threshold is not None:
+        if threshold_dir == 'gt':
+            ix = metric_s[metric_s > threshold].index
+        elif threshold_dir == 'lt':
+            ix = metric_s[metric_s < threshold].index
+        if any(ix):
+            ax.scatter(xpos[ix], metric_s[ix], c='none', edgecolor='k', s=ms, lw=1, label=None, clip_on=False, rasterized=rasterized)
+
+    # plot density
+    if plot_density:
+        sns.kdeplot(y=metric_s, ax=dax, legend=False, fill=True, lw=1.5)
+        dax.set_ylabel(None)
+        qtl.plot.format_plot(dax, fontsize=fontsize, hide=['top', 'right', 'bottom'])
+        plt.setp(dax.get_yticklabels(), visible=False)
+        dax.set_xticks([])
+        dax.set_xlabel('Freq.', ha='left', x=0, fontsize=fontsize, labelpad=7)
 
-    qtl.plot.format_plot(ax, fontsize=10)
-    qtl.plot.format_plot(dax, fontsize=10, hide=['top', 'right', 'bottom'])
+    qtl.plot.format_plot(ax, fontsize=fontsize)
     ax.spines['left'].set_position(('outward', 8))
-    plt.setp(dax.get_yticklabels(), visible=False)
 
     ax.set_xlim([1, ns])
     if ylim is None:
         ax.set_ylim([0, ax.get_ylim()[1]])
     else:
         ax.set_ylim(ylim)
 
     if show_xticklabels:
         ax.set_xticks(xpos)
-        ax.set_xticklabels(date_ix, rotation=45, ha='right', va='top')
+        ax.set_xticklabels(sorted_ix, rotation=45, ha='right', va='top')
     else:
         ax.xaxis.set_major_locator(ticker.MaxNLocator(integer=True))
 
-    ax.set_ylabel(ylabel, fontsize=14)
-    ax.set_xlabel(xlabel, fontsize=14)
-    ax.tick_params(labelsize=12)
-    dax.set_xticks([])
-    dax.set_xlabel('Freq.', ha='left', x=0, fontsize=12, labelpad=7)
+    ax.set_ylabel(ylabel, fontsize=fontsize+2)
+    ax.set_xlabel(xlabel, fontsize=fontsize+2)
 
     if show_legend:
         ax.legend(fontsize=9, handlelength=1, labelspacing=0.5, title=cohort_s.name)
 
-    return ax, dax
+    if plot_density:
+        return ax, dax
+    else:
+        return ax
 
 
-def detection_bias(metrics_df, bias_metric="Median 3' bias", c='Duplicate Rate of Mapped'):
+def detection_bias(metrics_df, bias_metric="Median 3' bias", c='Duplicate Rate of Mapped',
+                   ah=2, aw=2, ct=0, rasterized=False):
     """Plot genes detected vs a bias metric (e.g., Median Exon CV)"""
 
-    ax, cax = qtl.plot.setup_figure(2, 2, xspace=[0.75, 0.75],
-                                    colorbar=True, ds=0.05, cw=0.1)
+    ax, cax = qtl.plot.setup_figure(ah, aw, xspace=[0.75, 0.75],
+                                    colorbar=True, ds=0.05, cw=0.1, ct=ct)
 
     ix = metrics_df[c].sort_values().index
     h = ax.scatter(metrics_df.loc[ix, 'Genes Detected'], metrics_df.loc[ix, bias_metric],
                    c=metrics_df.loc[ix, c], cmap=plt.cm.GnBu,
                    clip_on=False, s=36, edgecolor='k',lw=0.5,
-                   vmin=0, vmax=1)
+                   vmin=0, vmax=1, rasterized=rasterized)
 
     ax.set_xlabel('Genes detected', fontsize=12)
     ax.set_ylabel(bias_metric, fontsize=12)
     qtl.plot.format_plot(ax, fontsize=10)
+    ax.autoscale(True)
     ax.spines['left'].set_position(('outward', 6))
     ax.spines['bottom'].set_position(('outward', 6))
     hc = plt.colorbar(h, cax=cax)
     hc.set_label('Duplicate Rate', fontsize=12, labelpad=6)
     return ax, cax
 
 
-def mapping_sense(metrics_df, cohort_s=None, cohort_colors=None, width=0.8,
+def mapping_sense(metrics_df, cohort_s=None, cohort_order=None, cohort_colors=None, date_s=None, width=0.8,
                   dl=0.75, aw=4, dr=1.5, db=0.5, ah=2, dt=0.25, ds=0.066, dc=0.1):
     """Summary of sense/antisense alignments.
 
     For stranded protocols, most reads should be 'End 1 Antisense' and 'End 2 Sense',
     or vice versa, depending on protocol.
     For unstranded protocols, the 4 categories are expected to be of equal proportion (~0.25).
     """
-    df = metrics_df[['End 1 Sense', 'End 1 Antisense', 'End 2 Sense', 'End 2 Antisense']]
+    sorted_ix = sort_samples(metrics_df.index, cohort_s=cohort_s,
+                             cohort_order=cohort_order, date_s=date_s)
+    df = metrics_df.loc[sorted_ix, ['End 1 Sense', 'End 1 Antisense', 'End 2 Sense', 'End 2 Antisense']]
     df = df / np.sum(df.values, axis=1, keepdims=True)
-    # df = df.loc[df.max(1).sort_values().index]
 
     fw = dl + aw + dr
     fh = db + ah + dt
     fig = plt.figure(facecolor=(1,1,1), figsize=(fw,fh))
     ax = fig.add_axes([dl/fw, db/fh, aw/fw, ah/fh])
     df.reset_index(drop=True).plot(kind='bar', width=width,
                                    stacked=True, xticks=[], ax=ax,
@@ -208,75 +262,76 @@
     ax.set_ylabel('Proportion of mapped reads', fontsize=12)
     ax.set_xlabel('Samples', fontsize=12)
     ax.set_xlim([-width/2, metrics_df.shape[0]-width/2])
 
     if cohort_s is not None:
         cax = fig.add_axes([dl/fw, (db+ah+ds)/fh, aw/fw, dc/fh], sharex=ax)
         cax.set_yticks([])
-        _plot_cohort_labels(cax, cohort_s, cohort_colors=cohort_colors,
+        _plot_cohort_labels(cax, cohort_s.loc[df.index], cohort_colors=cohort_colors,
                             lax=ax, legend=False, orientation='horizontal')
 
 
 def calculate_expression_cdfs(tpm_df):
     """Sort and compute CDF for each sample independently"""
     cdf_df = tpm_df.reset_index(drop=True).copy()
     if 'Description' in cdf_df:
         cdf_df.drop('Description', axis=1, inplace=True)
     for c in cdf_df:
         cdf_df[c] = np.cumsum(cdf_df[c].sort_values(ascending=False).values) / 1e6
     return cdf_df
 
 
-def cumulative_expression(cdf_df, cohort_s=None, cohort_colors=None, ax=None, cmap=plt.cm.Spectral_r,
-                          reference_df=None, reference_name=None, alpha=0.5, mode='lines', lw=1, legend=False):
+def cumulative_expression(cdf_df, cohort_s=None, cohort_colors=None, ax=None, cmap=plt.cm.Spectral_r, c=[0.6,0.6,0.6],
+                          reference_df=None, reference_name=None, alpha=0.5, mode='lines', lw=1, legend=False, rasterized=False):
     """
     Plot cumulative gene expression for each sample.
     This enables identification of samples with dominant expression of few genes.
 
     With mode='ci', median and confidence intervals are shown instead of individual samples.
     """
     if cohort_s is None:
         cohort_s = pd.Series('_NA', index=cdf_df.columns)
 
     if cohort_colors is None:
         cohorts = cohort_s.unique()
         nc = len(cohorts)
         if nc==1:
-            cohort_colors = {cohorts[0]: [0.6,0.6,0.6]}
+            cohort_colors = {cohorts[0]: c}
         else:
             cohort_colors = {i:j for i,j in zip(cohorts, plt.cm.get_cmap(cmap.name, nc)(np.arange(nc)))}
 
     if ax is None:
         ax = qtl.plot.setup_figure(4, 2.5)
     ax.set_xscale('log')
 
     if reference_df is not None:  # plot reference distribution
         # mu = reference_df.mean(axis=1)
         s = reference_df.std(axis=1)
         mu = reference_df.median(axis=1)
         # s = np.median(np.abs(gtex_cdf-mu), axis=0) / 0.6745
         if mode=='ci':
             ax.fill_between(np.arange(reference_df.shape[0])+1, mu-1.96*s, mu+1.96*s, facecolor='k', edgecolor='k', alpha=0.2, label=None, zorder=20)
-            ax.plot(mu, 'k', lw=2, alpha=0.8, rasterized=False, label=reference_name, zorder=30)
+            ax.plot(mu, 'k', lw=2, alpha=0.8, rasterized=rasterized, label=reference_name, zorder=30)
         else:
-            ax.fill_between(np.arange(reference_df.shape[0])+1, mu-1.96*s, mu+1.96*s, facecolor='k', edgecolor='none', alpha=0.2, label='{} 95% CI'.format(reference_name), zorder=20)
-            ax.plot(mu, 'k', lw=1.5, alpha=0.8, rasterized=False, label='{} mean'.format(reference_name), zorder=30)
+            ax.fill_between(np.arange(reference_df.shape[0])+1, mu-1.96*s, mu+1.96*s, facecolor='k', edgecolor='none', alpha=0.2, label=f'{reference_name} 95% CI', zorder=20)
+            ax.plot(mu, 'k', lw=1.5, alpha=0.8, rasterized=rasterized, label=f'{reference_name} mean', zorder=30)
 
     for c in cohort_s.unique():
+        x = np.arange(1, cdf_df.shape[0]+1)
         ix = cohort_s[cohort_s==c].index
         if mode == 'ci':  # plot confidence intervals
             mu = cdf_df[ix].median(axis=1)
             s = cdf_df[ix].std(axis=1)  # replace with MAD?
             fc = cohort_colors[c]
-            pc = ax.fill_between(np.arange(cdf_df.shape[0])+1, mu-1.96*s, mu+1.96*s, facecolor=fc, edgecolor=fc, alpha=0.2, label=None, zorder=20, lw=1)
-            ax.plot(mu, '-', color=cohort_colors[c], lw=2, alpha=0.8, rasterized=False, label=c, zorder=30)
+            pc = ax.fill_between(x, mu-1.96*s, mu+1.96*s, facecolor=fc, edgecolor=fc, alpha=0.2, label=None, zorder=20, lw=1)
+            ax.plot(mu, '-', color=cohort_colors[c], lw=2, alpha=0.8, rasterized=rasterized, label=c, zorder=30)
         else:
-            ax.plot(cdf_df[ix[0]], color=cohort_colors[c], alpha=alpha, lw=lw, rasterized=False, label=c)  # plot first one w/ label
+            ax.plot(x, cdf_df[ix[0]], color=cohort_colors[c], alpha=alpha, lw=lw, rasterized=rasterized, label=c)  # plot first one w/ label
             if len(ix)>1:
-                ax.plot(cdf_df[ix[1:]], color=cohort_colors[c], alpha=alpha, lw=lw, rasterized=False)
+                ax.plot(x, cdf_df[ix[1:]], color=cohort_colors[c], alpha=alpha, lw=lw, rasterized=rasterized)
 
     ax.set_ylim([0,1])
     ax.set_xlim([1,10000])
     qtl.plot.format_plot(ax, fontsize=10)
     ax.set_xlabel('Number of genes', fontsize=12)
     ax.set_ylabel('Cumulative transcriptional output', fontsize=12)
     ax.spines['left'].set_position(('outward', 6))
@@ -293,46 +348,48 @@
     """Internal function for adding a cohort color legend to a figure (in a separate axis)"""
 
     cohort_index_dict = {i:k for k,i in enumerate(np.unique(cohort_s))}
     if cohort_colors is None:
         n = len(cohort_index_dict)
         cmap = ListedColormap(plt.cm.get_cmap('Spectral', n)(np.arange(n)), 'indexed')
     else:
-        cmap = ListedColormap(np.stack(pd.Series(cohort_index_dict).sort_values().index.map(cohort_colors)))
+        cmap = ListedColormap(pd.Series(cohort_index_dict).sort_values().index.map(cohort_colors))
 
     if orientation == 'vertical':
         ax.imshow(cohort_s.map(cohort_index_dict).values.reshape(-1,1), aspect='auto', cmap=cmap)
     else:
         ax.imshow(cohort_s.map(cohort_index_dict).values.reshape(1,-1), aspect='auto', cmap=cmap)
 
     if lax is None:
         lax = ax
     for k,i in cohort_index_dict.items():
-        lax.scatter([], [], marker='s', c=[cmap(i)], label='{}'.format(k))
+        lax.scatter([], [], marker='s', c=[cmap(i)], label=f'{k}')
     if legend:
         lax.legend(loc='upper left', borderaxespad=None, bbox_to_anchor=(1,1), handlelength=1, title='Cohort')
 
 
-def insert_sizes(insertsize_df, cohort_s=None, cohort_colors=None, sort_order='mean', max_size=1000,
+def insert_sizes(insertsize_df, cohort_s=None, cohort_colors=None,
+                 cohort_order=None, sort_order='mean', max_size=1000,
                  legend=False, dl=0.75, aw=3, dr=0.5, db=0.5, ah=2, dt=0.25):
     """Plot heat map of insert size distributions"""
 
     # expand to 'max_size' bp
     df = insertsize_df.reindex(np.arange(1,max_size+1)).fillna(0).astype(np.int32).T
 
     # sort by mean if > 100000 reads
     mu = df.mul(df.columns.values, axis=1).sum(1)
     n = df.sum(1).sort_values()
     si = n[n<100000].index.tolist() + mu.loc[n[n>=100000].index].sort_values().index.tolist()
 
-    size_s = cohort_s.value_counts()
-    if sort_order == 'cohort':
+    if cohort_s is not None and sort_order == 'cohort':  # sort within each cohort
+        if cohort_order is None:
+            cohort_order = cohort_s.value_counts().index
         sort_s = pd.Series(cohort_s[si], index=si)
         si = []
-        for c in size_s.index:
+        for c in cohort_order:
             si.extend(sort_s[sort_s==c].index)
 
     # set up figure
     if cohort_s is not None:
         cw = 0.1
         ds = 0.05
     else:
@@ -359,94 +416,166 @@
 
     ax.imshow(df.loc[si], interpolation='none', aspect='auto', norm=LogNorm())
     ax.set_xlabel('Insert size (bp)', fontsize=12)
     ax.set_xlim([1, max_size])
     return ax
 
 
+def gc_content(gc_content_df, cohort_s=None, cohort_colors=None,
+               cohort_order=None, sort_order='mean', legend=False,
+               dl=0.75, aw=3, dr=0.5, db=0.5, ah=2, dt=0.25):
+    """Plot heat map of GC content distributions"""
+
+    # sort by mean
+    x = gc_content_df.index.values
+    mu = (gc_content_df * x.reshape(-1,1)).sum()
+    si = mu.sort_values().index
+
+    if cohort_s is not None and sort_order == 'cohort':  # sort within each cohort
+        if cohort_order is None:
+            cohort_order = cohort_s.value_counts().index
+        sort_s = pd.Series(cohort_s[si], index=si)
+        si = []
+        for c in cohort_order:
+            si.extend(sort_s[sort_s==c].index)
+
+    # set up figure
+    if cohort_s is not None:
+        ch = 0.1
+        ds = 0.05
+    else:
+        ch = 0
+        ds = 0
+    fw = dl + aw + dr
+    fh = db + ah + ch + ds + dt
+    fig = plt.figure(facecolor=(1,1,1), figsize=(fw,fh))
+    ax = fig.add_axes([dl/fw, db/fh, aw/fw, ah/fh])
+
+    # add cohort information and legend
+    if cohort_s is not None:
+        # set up axes
+        cax = fig.add_axes([dl/fw, (db+ah+ds)/fh, aw/fw, ch/fh], sharex=ax)
+        plt.setp(cax.get_xticklabels(), visible=False);
+        for line in cax.xaxis.get_ticklines():
+            line.set_markersize(0)
+            line.set_markeredgewidth(0)
+        cax.set_yticks([])
+
+        # plot labels
+        _plot_cohort_labels(cax, cohort_s[si], orientation='horizontal',
+                            cohort_colors=cohort_colors, lax=ax, legend=legend)
+
+    ax.imshow(gc_content_df[si], origin='lower', interpolation='none', aspect='auto', norm=LogNorm())
+    ax.set_xlabel('Samples', fontsize=12)
+    ax.set_ylabel('Fragment GC Content', fontsize=12)
+    y = np.arange(0, 120, 20)
+    ax.set_yticks(y)
+    ax.set_yticklabels(y/100)
+    return ax
+
+
 def xy_expression(tpm_df, sex_s=None, flag_klinefelter=True, highlight_ids=None,
-                  x_threshold=5, y_threshold=30, s=24, verbose=True):
+                  x_threshold=5, y_threshold=30, s=24, verbose=True, rasterized=False, **kwargs):
     """Expression of sex-specific genes (XIST and RPS4Y1) to identify sample swaps.
 
     sex_s: pd.Series annotating the sex of each sample, as Male/Female.
     """
 
     x_id = tpm_df.index[tpm_df.index.str.startswith('ENSG00000229807')][0]  # XIST
     y_id = tpm_df.index[tpm_df.index.str.startswith('ENSG00000129824')][0]  # RPS4Y1
     x_s = tpm_df.loc[x_id].rename('XIST')
     y_s = tpm_df.loc[y_id].rename('RPS4Y1')
 
-    ax = qtl.plot.setup_figure(3, 3)
+    ax = qtl.plot.setup_figure(3, 3, xspace=[0.75, 1.75])
     ax.set_xscale('symlog')
     ax.set_yscale('symlog')
 
     if sex_s is not None:  # flag potential swaps based on thresholds
         assert tpm_df.columns.isin(sex_s.index).all()
-        res_s = pd.Series('NA', index=sex_s.index, name='inferred_sex')
+        res_s = pd.Series('NA', index=sex_s.index[sex_s.index.isin(tpm_df.columns)], name='inferred_sex')
 
-        args = {'edgecolors':'none', 'lw':0, 'rasterized':False, 'clip_on':False, 's':s, 'alpha':0.2}
-        args2 = {'edgecolors':'k', 'lw':1, 'rasterized':False, 'clip_on':False, 's':s+6, 'alpha':1}
+        args =  {'ec':'none', 'lw':0, 'rasterized':rasterized, 'clip_on':False, 's':s, 'alpha':0.33}
+        args.update(kwargs)
+        args2 = {**args, 'ec':'k', 'lw':1, 's':s+6, 'alpha':1}
+
+        # infer missing labels based on thresholds
+        ix = sex_s[sex_s.isnull() & (x_s <= x_threshold) & (y_s > y_threshold)].index
+        if len(ix) > 0:
+            ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0.6,0.8,0.7]).reshape(1,-1), **args, label=f"Male* ({len(ix)})")
+            res_s[ix] = 'Male'
+        ix = sex_s[sex_s.isnull() & (x_s > x_threshold) & (y_s <= y_threshold)].index
+        if len(ix) > 0:
+            ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0,0.8,0.7]).reshape(1,-1), **args, label=f"Female* ({len(ix)})")
+            res_s[ix] = 'Female'
+        ix = sex_s[sex_s.isnull() & (x_s > x_threshold) & (y_s > y_threshold)].index
+        if len(ix) > 0:
+            ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0.75,0.8,0.7]).reshape(1,-1), **args, label=f"XXY* ({len(ix)})")
+            res_s[ix] = 'Klinefelter (XXY)'
+        ix = sex_s[sex_s.isnull() & (x_s <= x_threshold) & (y_s <= y_threshold)].index
+        if len(ix) > 0:
+            ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0.0,0,0.7]).reshape(1,-1), **args, label=f"? ({len(ix)})")
+            res_s[ix] = np.NaN
 
         # matching samples
         ix = sex_s[(sex_s == 'Male') & (x_s <= x_threshold)].index
         if len(ix) > 0:
-            ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0.6,0.8,0.7]).reshape(1,-1), label='Male ({})'.format(len(ix)), **args)
             res_s[ix] = 'Male'
+            ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0.6,0.8,0.7]).reshape(1,-1), label=f"Male ({len(ix)})", **args)
         ix = sex_s[(sex_s == 'Female') & (y_s <= y_threshold)].index
         if len(ix) > 0:
-            ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0,0.8,0.7]).reshape(1,-1), label='Female ({})'.format(len(ix)), **args)
             res_s[ix] = 'Female'
+            ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0,0.8,0.7]).reshape(1,-1), label=f"Female ({len(ix)})", **args)
 
         # mismatches
         if flag_klinefelter:
             ix = sex_s[(sex_s == 'Male') & (x_s > x_threshold) & (y_s <= y_threshold)].index
             if len(ix) > 0:
-                ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0.6,1,0.9]).reshape(1,-1), label='M > F swap ({})'.format(len(ix)), **args2)
+                ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0.6,1,0.9]).reshape(1,-1), label=f'M > F swap ({len(ix)})', **args2)
                 if verbose:
-                    print('F mislabeled as M:\n{}'.format(ix.tolist()))
+                    print(f'F mislabeled as M:\n{ix.tolist()}')
                 res_s[ix] = 'Female'
             ix = sex_s[(sex_s == 'Female') & (y_s > y_threshold) & (x_s <= x_threshold)].index
             if len(ix) > 0:
-                ax.scatter(x_s[ix], y_s[ix], c=[[0.9, 0, 0, 1]], label='F > M swap ({})'.format(len(ix)), **args2)
+                ax.scatter(x_s[ix], y_s[ix], c=[[0.9, 0, 0, 1]], label=f'F > M swap ({len(ix)})', **args2)
                 if verbose:
-                    print('M mislabeled as F:\n{}'.format(ix.tolist()))
+                    print(f'M mislabeled as F:\n{ix.tolist()}')
                 res_s[ix] = 'Male'
 
             # Klinefelter
             ix = sex_s[(sex_s == 'Male') & (x_s > x_threshold) & (y_s > y_threshold)].index
             if len(ix) > 0:
-                ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0.6,1,0.9]).reshape(1,-1), label='XXY? ({})'.format(len(ix)), **args2)
+                ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0.75,1,0.9]).reshape(1,-1), label=f'XXY? ({len(ix)})', **args2)
                 if verbose:
-                    print('Possible Klinefelter (XXY): {}'.format(ix.tolist()))
+                    print(f'Possible Klinefelter (XXY): {ix.tolist()}')
                 res_s[ix] = 'Possible Klinefelter (XXY)'
             ix = sex_s[(sex_s == 'Female') & (y_s > y_threshold) & (x_s > x_threshold)].index
             if len(ix) > 0:
-                ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0,1,0.9]).reshape(1,-1), label='XXY? ({})'.format(len(ix)), **args2)
+                ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0,1,0.9]).reshape(1,-1), label=f'XXY? ({len(ix)})', **args2)
                 if verbose:
-                    print('Possible Klinefelter (XXY): {}'.format(ix.tolist()))
+                    print(f'Possible Klinefelter (XXY): {ix.tolist()}')
                 res_s[ix] = 'Possible Klinefelter (XXY)'
 
         else:
             ix = sex_s[(sex_s == 'Male') & (x_s > x_threshold)].index
             if len(ix) > 0:
-                ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0.6,1,0.9]).reshape(1,-1), label='M > F swap ({})'.format(len(ix)), **args2)
+                ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0.6,1,0.9]).reshape(1,-1), label=f'M > F swap ({len(ix)})', **args2)
                 if verbose:
-                    print('F mislabeled as M:\n{}'.format(ix.tolist()))
+                    print(f'F mislabeled as M:\n{ix.tolist()}')
                 res_s[ix] = 'Female'
             ix = sex_s[(sex_s == 'Female') & (y_s > y_threshold)].index
             if len(ix) > 0:
-                ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0,1,0.9]).reshape(1,-1), label='F > M swap ({})'.format(len(ix)), **args2)
+                ax.scatter(x_s[ix], y_s[ix], c=hsv_to_rgb([0,1,0.9]).reshape(1,-1), label=f'F > M swap ({len(ix)})', **args2)
                 if verbose:
-                    print('M mislabeled as F:\n{}'.format(ix.tolist()))
+                    print(f'M mislabeled as F:\n{ix.tolist()}')
                 res_s[ix] = 'Male'
     else:
         ax.scatter(x_s, y_s, s=s, alpha=0.5, edgecolors='none', lw=0.5, rasterized=True, clip_on=False)
 
     if highlight_ids is not None:  # highlight selected samples
-        ax.scatter(x_s[highlight_ids], y_s[highlight_ids], c='r', s=s, alpha=0.5, edgecolors='none', lw=0.5, rasterized=True, label=None)
+        ax.scatter(x_s[highlight_ids], y_s[highlight_ids], c=[hsv_to_rgb([0.075,1,1])], s=s+12, alpha=1, edgecolors='k', lw=1, zorder=50, rasterized=False, clip_on=False, label=None)
 
     qtl.plot.format_plot(ax, fontsize=12)
     ax.spines['left'].set_position(('outward', 6))
     ax.spines['bottom'].set_position(('outward', 6))
     ax.set_xlabel('XIST expression (TPM)', fontsize=14)
     ax.set_ylabel('RPS4Y1 expression (TPM)', fontsize=14)
 
@@ -459,9 +588,8 @@
     ax.set_xlim(xlim)
     ax.set_ylim(ylim)
 
     if sex_s is not None:
         leg = ax.legend(loc='upper left', fontsize=12, handlelength=0.5, labelspacing=0.2, bbox_to_anchor=(1,1))
         for lh in leg.legendHandles:
             lh.set_alpha(1)
-
-    return ax
+        return res_s
```

### Comparing `rnaseqc-0.0.2/rnaseqc/report.py` & `rnaseqc-0.0.3/rnaseqc/report.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,65 +6,79 @@
 import matplotlib.pyplot as plt
 import qtl.io
 
 sys.path.insert(1, os.path.dirname(__file__))
 from .plot import *
 
 
-def plot_qc_figures(metrics_df, cohort_s=None, cohort_colors=None, date_s=None,
-                    prefix=None, output_dir=None, dpi=300, show_legend=True,
-                    ms=12, alpha=1, show_xticklabels=False, highlight_ids=None,
-                    thresholds=None, insertsize_df=None, tpm_df=None):
+def plot_qc_figures(metrics_df, cohort_s=None, cohort_order=None, cohort_colors=None, date_s=None,
+                    insertsize_df=None, gc_content_df=None, tpm_df=None,
+                    thresholds=None, lims=None, outlier_method='threshold',
+                    show_legend=True, legend_cols=5, lw=4, lh=1, ms=12, alpha=1, show_xticklabels=False,
+                    highlight_ids=None, prefix=None, output_dir=None, dpi=300):
     """
     metrics_df: output from RNA-SeQC
     cohort_s: mapping of sample ID to cohort/cluster/etc.
     """
     if cohort_s is None:
         cohort_s = pd.Series('All samples', index=metrics_df.index)
+    else:
+        assert metrics_df.index.isin(cohort_s.index).all() and cohort_s.loc[metrics_df.index].notnull().all()
+
+    if date_s is not None:
+        assert metrics_df.index.isin(date_s.index).all() and date_s.loc[metrics_df.index].notnull().all()
 
     if output_dir is not None:
         assert prefix is not None
 
-    cohorts = np.unique(cohort_s)
+    cohorts = np.unique(cohort_s.loc[metrics_df.index])
     if cohort_colors is None:
         cohort_colors = get_cohort_colors(cohorts)
 
     metrics_args = {
         'cohort_s': cohort_s,
+        'cohort_order': cohort_order,
         'cohort_colors': cohort_colors,
+        'date_s': date_s,
         'show_xticklabels': show_xticklabels,
         'ms': ms,
         'alpha': alpha,
-        'highlight_ids': highlight_ids
+        'highlight_ids': highlight_ids,
+        'aw': 6,
+        'ah': 2,
     }
 
     metrics_list = [
         'Mapped Reads',  # Unique Mapping, Vendor QC Passed Reads that were mapped
         'Mapping Rate',
         'Duplicate Rate of Mapped',
         'Exonic Rate',
         'Intronic Rate',
         'Intergenic Rate',
         'Chimeric Alignment Rate',
         'rRNA Rate',
         # 'Mapped Unique Reads',  # Duplicate Rate of Mapped is more representative
         "Median 3' bias",
         'Median Exon CV',
+        'Fragment GC Content Mean',
         'Average Fragment Length',
     ]
 
     threshold_dir_dict = {
         'Mapped Reads': 'lt',
         'Mapping Rate': 'lt',
         'Duplicate Rate of Mapped': 'gt',
         'Exonic Rate': 'lt',
         'Intronic Rate': 'gt',
         'Intergenic Rate': 'gt',
         'Chimeric Alignment Rate': 'gt',
         'rRNA Rate': 'gt',
+        "Median 3' bias": 'gt',
+        'Median Exon CV': 'gt',
+        'Average Fragment Length': 'lt',
     }
 
     threshold_dict = {
         'Mapped Reads': 50e6,
         'Mapping Rate': 0.9,
         # 'Duplicate Rate of Mapped': 0.6,
         'Exonic Rate': 0.7,
@@ -81,67 +95,94 @@
         'Mapping Rate': [0,1],
         'Duplicate Rate of Mapped': [0, 1],
         'Exonic Rate': [0, 1],
         'Intronic Rate': [0, 1],
         'Intergenic Rate': [0, 1],
         'Chimeric Alignment Rate': [0, 0.1],
         'rRNA Rate': [0, 1],
-        "Median 3' bias": None,
+        "Median 3' bias": [0, 1],
         'Median Exon CV': None,
+        'Fragment GC Content Mean': [0, 1],
         'Average Fragment Length': None,
     }
 
+    if lims is not None:
+        ylim_dict.update(lims)
+
+    if cohort_order is None:
+        cohort_order = cohorts
+
     # plot cohort legend
     if show_legend:
-        ax = qtl.plot.setup_figure(0.5,0.5)
-        for c in cohorts:
-            ax.scatter([], [], s=48, marker='s', c=cohort_colors[c].reshape(1,-1), label=c)
-        ax.legend(loc='upper left', handlelength=1, ncol=5, bbox_to_anchor=(1,1))
+        ax = qtl.plot.setup_figure(lw, lh, xspace=[0,0], yspace=[0,0])
+        for c in cohort_order:
+            ax.scatter([], [], s=48, marker='s', color=cohort_colors[c], label=c)
+        ax.scatter([], [], fc='w', ec='k', lw=1, s=30, label='Outliers')
+        ax.legend(loc='center left', handlelength=1, ncol=legend_cols)
         plt.axis('off')
+        if output_dir is not None:
+            plt.savefig(os.path.join(output_dir, f'{prefix}.legend.pdf'), dpi=dpi)
 
     # distributions for selected/key metrics
     for k,metric in enumerate(metrics_list, 1):
-        if metric in metrics_df:
-            ylim = [0,1]
-            metrics(metrics_df[metric], ylim=ylim_dict[metric],
+        if metric in metrics_df and not (metrics_df[metric] == 0).all():
+            if metric == 'Duplicate Rate of Mapped' and 'Duplicate Rate of Mapped, excluding Globins' in metrics_df:
+                metric_s = metrics_df['Duplicate Rate of Mapped, excluding Globins'].rename('Duplicate Rate of Mapped')
+            else:
+                metric_s = metrics_df[metric]
+            metrics(metric_s, ylim=ylim_dict[metric],
                          threshold=threshold_dict.get(metric, None),
                          threshold_dir=threshold_dir_dict.get(metric, None),
+                         outlier_method=outlier_method,
                          **metrics_args)
             if output_dir is not None:
                 plt.savefig(os.path.join(output_dir, '{}.{}.pdf'.format(prefix, metric.lower().replace("3'",'3prime').replace(' ','_'))), dpi=dpi)
 
     # genes detected vs bias and duplication rate
-    detection_bias(metrics_df, bias_metric="Median 3' bias", c='Duplicate Rate of Mapped')
-    if output_dir is not None:
-        plt.savefig(os.path.join(output_dir, '{}.genes_detected_vs_median_3prime_bias.pdf'.format(prefix)), dpi=dpi)
+    if "Median 3' bias" in metrics_df:
+        c = 'Duplicate Rate of Mapped, excluding Globins' if 'Duplicate Rate of Mapped, excluding Globins' in metrics_df else 'Duplicate Rate of Mapped'
+        detection_bias(metrics_df, bias_metric="Median 3' bias", c=c)
+        if output_dir is not None:
+            plt.savefig(os.path.join(output_dir, f'{prefix}.genes_detected_vs_median_3prime_bias.pdf'), dpi=dpi)
 
     # mismatch rates
-    mismatch_rates(metrics_df, cohort_s=cohort_s, cohort_colors=cohort_colors)
-    if output_dir is not None:
-        plt.savefig(os.path.join(output_dir, '{}.end_mismatch_rates.pdf'.format(prefix)), dpi=dpi)
+    if not metrics_df['End 1 Mismatch Rate'].isnull().all():
+        mismatch_rates(metrics_df, cohort_s=cohort_s, cohort_order=cohort_order, cohort_colors=cohort_colors,
+                       end1_threshold=threshold_dict.get('End 1 mismatch rate', None),
+                       end2_threshold=threshold_dict.get('End 2 mismatch rate', None))
+        if output_dir is not None:
+            plt.savefig(os.path.join(output_dir, f'{prefix}.end_mismatch_rates.pdf'), dpi=dpi)
 
-    mapping_sense(metrics_df, cohort_s, cohort_colors=cohort_colors)
+    mapping_sense(metrics_df, cohort_s=cohort_s, cohort_order=cohort_order,
+                  cohort_colors=cohort_colors, date_s=date_s, width=1)
     if output_dir is not None:
-        plt.savefig(os.path.join(output_dir, '{}.mapping_sense.pdf'.format(prefix)), dpi=dpi)
+        plt.savefig(os.path.join(output_dir, f'{prefix}.mapping_sense.pdf'), dpi=dpi)
 
     # insert size distributions (if supplied)
     if insertsize_df is not None:
-        insert_sizes(insertsize_df, cohort_s, cohort_colors=cohort_colors, sort_order='mean')
+        insert_sizes(insertsize_df, cohort_s=cohort_s, cohort_order=cohort_order,
+                     cohort_colors=cohort_colors, sort_order='cohort')
+        if output_dir is not None:
+            plt.savefig(os.path.join(output_dir, f'{prefix}.insert_sizes.pdf'), dpi=dpi)
+
+    if gc_content_df is not None:
+        gc_content(gc_content_df, cohort_s=cohort_s, cohort_colors=cohort_colors,
+                   cohort_order=cohort_order, sort_order='cohort')
         if output_dir is not None:
-            plt.savefig(os.path.join(output_dir, '{}.insert_sizes.pdf'.format(prefix)), dpi=dpi)
+            plt.savefig(os.path.join(output_dir, f'{prefix}.gc_content.pdf'), dpi=dpi)
 
     if tpm_df is not None:
         cdf_df = calculate_expression_cdfs(tpm_df)
         if tpm_df.shape[1] < 50:
             mode = 'lines'
         else:
             mode = 'ci'
         cumulative_expression(cdf_df, cohort_s=cohort_s, cohort_colors=cohort_colors, mode=mode)
         if output_dir is not None:
-            plt.savefig(os.path.join(output_dir, '{}.cumulative_expression.pdf'.format(prefix)), dpi=dpi)
+            plt.savefig(os.path.join(output_dir, f'{prefix}.cumulative_expression.pdf'), dpi=dpi)
 
 
 def load_inputs(args):
 
     if args.metrics.endswith('.parquet'):
         metrics_df = pd.read_parquet(args.metrics)
     else:
@@ -149,38 +190,45 @@
 
     if args.tpm is not None:
         tpm_df = qtl.io.read_gct(args.tpm, load_description=False)
     else:
         tpm_df = None
 
     if args.cohort is not None:
-        cohort_s = pd.read_csv(args.cohort, sep='\t', index_col=0, header=None, squeeze=True)
+        cohort_s = pd.read_csv(args.cohort, sep='\t', index_col=0, header=None).squeeze('columns')
         assert metrics_df.index.isin(cohort_s.index).all()
     else:
         cohort_s = None
 
-    if args.cohort is not None:
+    if args.date is not None:
+        date_s = pd.read_csv(args.date, sep='\t', index_col=0, header=None).squeeze('columns')
+        assert metrics_df.index.isin(date_s.index).all()
+    else:
+        date_s = None
+
+    if args.insert_size is not None:
         insertsize_df = pd.read_csv(args.insert_size, sep='\t', index_col=0)
     else:
         insertsize_df = None
 
-    return metrics_df, tpm_df, cohort_s, insertsize_df
+    return metrics_df, tpm_df, cohort_s, date_s, insertsize_df
 
 
 if __name__ == '__main__':
 
     parser = argparse.ArgumentParser(description='Generate QC report from RNA-SeQC metrics table.')
     parser.add_argument('metrics', help='Aggregated QC metrics from RNA-SeQC.')
     parser.add_argument('prefix', help='Name for output files.')
     parser.add_argument('--tpm', default=None, help='Aggregated TPM matrix from RNA-SeQC.')
     parser.add_argument('--insert-size', default=None, help='Aggregated insert sizes from RNA-SeQC.')
     parser.add_argument('--cohort', default=None, help='Cohort or batch annotation. TSV file mapping sample IDs to annotation.')
+    parser.add_argument('--date', default=None, help='Date annotation. TSV file mapping sample IDs to dates.')
     parser.add_argument('--output-dir', default='.', help='If specified, figures are saved here.')
     parser.add_argument('--dpi', type=int, default=300, help='Figure resolution.')
     args = parser.parse_args()
 
-    metrics_df, tpm_df, cohort_s, insertsize_df = load_inputs(args)
+    metrics_df, tpm_df, cohort_s, date_s, insertsize_df = load_inputs(args)
 
-    plot_qc_figures(metrics_df, cohort_s=cohort_s, cohort_colors=None, date_s=None,
+    plot_qc_figures(metrics_df, cohort_s=cohort_s, cohort_colors=None, date_s=date_s,
                     prefix=args.prefix, output_dir=args.output_dir, dpi=args.dpi, show_legend=True,
                     ms=12, alpha=1, show_xticklabels=False, highlight_ids=None,
                     thresholds=None, insertsize_df=insertsize_df, tpm_df=tpm_df)
```

### Comparing `rnaseqc-0.0.2/rnaseqc/run.py` & `rnaseqc-0.0.3/rnaseqc/run.py`

 * *Files identical despite different names*

### Comparing `rnaseqc-0.0.2/rnaseqc.egg-info/PKG-INFO` & `rnaseqc-0.0.3/rnaseqc.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,78 @@
 Metadata-Version: 2.1
 Name: rnaseqc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Multi-sample visualization of metrics from RNA-SeQC
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: # RNA-SeQC Python utilities
-        
-        This module contains utility code for RNA-SeQC
-        
-        ## Installing
-        
-        * From pip: `pip install rnaseqc`
-        * From the git repo: `pip install -e python` (Invoke from root of git repo)
-        
-        ## Usage
-        
-        This does not install a console entrypoint. You can invoke the utilities in one of three ways:
-        
-        * From the main module: `python3 -m rnaseqc ...`
-        * Calling the target module: `python3 -m rnaseqc.example ...`
-        * Calling scripts directly: `python3 python/rnaseqc/example.py`
-        
-        ## Utilities
-        
-        The `rnaseqc` module contains 5 main utilities. To get more help with each utility,
-        invoke the utility with the `-h` or `--help` option
-        
-        ### Aggregation
-        
-        Aggregates RNA-SeQC outputs from multiple samples
-        
-        ```
-        python3 -m rnaseqc aggregate [-h] [--parquet] [-o OUTPUT_DIR] results_dir prefix
-        ```
-        
-        ### Jupyter Notebooks
-        
-        Creates a jupyter notebook with several figures for comparing samples
-        
-        ```
-        python3 -m rnaseqc notebook [-h] [-t TPM] [-i INSERT_SIZE] [-c COHORT] [-d DATE] metrics output
-        ```
-        
-        ### Figures
-        
-        Generates figures from an aggregated RNA-SeQC metrics table
-        
-        ```
-        python3 -m rnaseqc report [-h] [--tpm TPM] [--insert-size INSERT_SIZE] [--cohort COHORT] [--output-dir OUTPUT_DIR] [--dpi DPI] metrics prefix
-        ```
-        
-        ### Insert Size distributions
-        
-        Generates a BED file with intervals used by RNA-SeQC for estimating a sample's insert size distribution
-        
-        ```
-        python3 -m rnaseqc insert-size [-h] [--min-length MIN_LENGTH] [--min-mappability MIN_MAPPABILITY] [--output-dir OUTPUT_DIR] gtf_path mappability_bigwig prefix
-        ```
-        
-        ### Exon remapping
-        
-        Convert exon names in an `*.exon_reads.gct` file from RNA-SeQC 2.X.X to match names
-        as reported by RNA-SeQC 1.1.9
-        
-        ```
-        python3 -m rnaseqc legacy-exons gct gtf
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: qtl
+Requires-Dist: agutil
+Requires-Dist: nbformat
+
+# RNA-SeQC Python utilities
+
+This module contains utility code for RNA-SeQC
+
+## Installing
+
+* From pip: `pip install rnaseqc`
+* From the git repo: `pip install -e python` (Invoke from root of git repo)
+
+## Usage
+
+This does not install a console entrypoint. You can invoke the utilities in one of three ways:
+
+* From the main module: `python3 -m rnaseqc ...`
+* Calling the target module: `python3 -m rnaseqc.example ...`
+* Calling scripts directly: `python3 python/rnaseqc/example.py`
+
+## Utilities
+
+The `rnaseqc` module contains 5 main utilities. To get more help with each utility,
+invoke the utility with the `-h` or `--help` option
+
+### Aggregation
+
+Aggregates RNA-SeQC outputs from multiple samples
+
+```
+python3 -m rnaseqc aggregate [-h] [--parquet] [-o OUTPUT_DIR] results_dir prefix
+```
+
+### Jupyter Notebooks
+
+Creates a jupyter notebook with several figures for comparing samples
+
+```
+python3 -m rnaseqc notebook [-h] [-t TPM] [-i INSERT_SIZE] [-c COHORT] [-d DATE] metrics output
+```
+
+### Figures
+
+Generates figures from an aggregated RNA-SeQC metrics table
+
+```
+python3 -m rnaseqc report [-h] [--tpm TPM] [--insert-size INSERT_SIZE] [--cohort COHORT] [--output-dir OUTPUT_DIR] [--dpi DPI] metrics prefix
+```
+
+### Insert Size distributions
+
+Generates a BED file with intervals used by RNA-SeQC for estimating a sample's insert size distribution
+
+```
+python3 -m rnaseqc insert-size [-h] [--min-length MIN_LENGTH] [--min-mappability MIN_MAPPABILITY] [--output-dir OUTPUT_DIR] gtf_path mappability_bigwig prefix
+```
+
+### Exon remapping
+
+Convert exon names in an `*.exon_reads.gct` file from RNA-SeQC 2.X.X to match names
+as reported by RNA-SeQC 1.1.9
+
+```
+python3 -m rnaseqc legacy-exons gct gtf
+```
```

### Comparing `rnaseqc-0.0.2/setup.py` & `rnaseqc-0.0.3/setup.py`

 * *Files identical despite different names*

