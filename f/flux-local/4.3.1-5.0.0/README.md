# Comparing `tmp/flux-local-4.3.1.tar.gz` & `tmp/flux_local-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-local-4.3.1.tar", last modified: Sun Jan 21 18:32:41 2024, max compression
+gzip compressed data, was "flux_local-5.0.0.tar", last modified: Sun Apr 21 00:58:00 2024, max compression
```

## Comparing `flux-local-4.3.1.tar` & `flux_local-5.0.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 18:32:41.094024 flux-local-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-21 18:32:31.000000 flux-local-4.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-01-21 18:32:41.094024 flux-local-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-01-21 18:32:31.000000 flux-local-4.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 18:32:41.086024 flux-local-4.3.1/flux_local/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25623 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)    21389 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 18:32:41.090024 flux-local-4.3.1/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/tool/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-01-21 18:32:31.000000 flux-local-4.3.1/flux_local/tool/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 18:32:41.094024 flux-local-4.3.1/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-01-21 18:32:41.000000 flux-local-4.3.1/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-21 18:32:41.000000 flux-local-4.3.1/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 18:32:41.000000 flux-local-4.3.1/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-21 18:32:41.000000 flux-local-4.3.1/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-21 18:32:41.000000 flux-local-4.3.1/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-21 18:32:41.000000 flux-local-4.3.1/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-01-21 18:32:41.094024 flux-local-4.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-21 18:32:31.000000 flux-local-4.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 18:32:41.090024 flux-local-4.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/test_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 18:32:41.090024 flux-local-4.3.1/tests/tool/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/tool/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/tool/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/tool/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/tool/test_diff_hr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/tool/test_diff_ks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/tool/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/tool/test_get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/tool/test_get_hr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/tool/test_get_ks.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-21 18:32:31.000000 flux-local-4.3.1/tests/tool/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.709360 flux_local-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 00:57:53.000000 flux_local-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-21 00:58:00.709360 flux_local-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-21 00:57:53.000000 flux_local-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.705361 flux_local-5.0.0/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27320 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.705361 flux_local-5.0.0/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/tool/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/tool/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-21 00:57:53.000000 flux_local-5.0.0/flux_local/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.709360 flux_local-5.0.0/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-21 00:58:00.000000 flux_local-5.0.0/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-21 00:58:00.000000 flux_local-5.0.0/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 00:58:00.000000 flux_local-5.0.0/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 00:58:00.000000 flux_local-5.0.0/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-21 00:58:00.000000 flux_local-5.0.0/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 00:58:00.000000 flux_local-5.0.0/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-21 00:58:00.709360 flux_local-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-21 00:57:53.000000 flux_local-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.705361 flux_local-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.709360 flux_local-5.0.0/tests/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/tool/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/tool/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/tool/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/tool/test_diff_hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/tool/test_diff_ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/tool/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/tool/test_get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/tool/test_get_hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/tool/test_get_ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-21 00:57:53.000000 flux_local-5.0.0/tests/tool/test_test.py
```

### Comparing `flux-local-4.3.1/LICENSE` & `flux_local-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/PKG-INFO` & `flux_local-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 4.3.1
+Version: 5.0.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles>=22.1.0
 Requires-Dist: nest_asyncio>=1.5.6
-Requires-Dist: pydantic>=2.5.2
 Requires-Dist: python-slugify>=8.0.0
 Requires-Dist: GitPython>=3.1.30
 Requires-Dist: PyYAML>=6.0
+Requires-Dist: mashumaro>=3.12
 Requires-Dist: pytest>=7.2.1
 Requires-Dist: pytest-asyncio>=0.20.3
 
 flux-local is a set of tools and libraries for managing a local flux gitops repository focused on validation steps to help improve quality of commits, PRs, and general local testing.
 
 This library uses command line tools like kustomize and helm to replicate the behavior of
 flux to gather objects in the cluster. It only looks at the local git repo, and not a live
@@ -115,15 +115,15 @@
 ```
 
 ### flux-local diff
 
 You may also use `flux-local` to verify your local changes to cluster resources have the desird
 effect. This is similar to `flux diff` but entirely local. This will run a local `kustomize build`
 first against the local repo then again against a prior repo revision, then prints the output:
-```bash
+```diff
 $ flux-local diff ks apps
 ---
 
 +++
 
 @@ -2,6 +2,13 @@
 
@@ -174,15 +174,15 @@
 On branch dev
 Your branch is up to date with 'origin/dev'.
 
 Changes not staged for commit:
 	modified:   home/dev/hajimari-values.yaml
 
 $ export DIFF="dyff between --omit-header --color on"
-# flux-local diff ks home --path clusters/dev/
+$ flux-local diff ks home --path clusters/dev/
 
 spec.chart.spec.version  (HelmRelease/hajimari/hajimari)
   ± value change
     - 2.0.2
     + 2.0.1
 
 $ flux-local diff hr hajimari -n hajimari --path clusters/dev/
@@ -268,16 +268,16 @@
 or that ingress objects are valid).
 
 This example will run `flux-local test` against the cluster in `clusters/prod` with
 helm release expansion enabled.
 
 ```yaml
 - name: Setup Flux CLI
-  uses: fluxcd/flux2/action@v2
-- uses: allenporter/flux-local/test@2.0.0
+  uses: fluxcd/flux2/action@v2.2.2
+- uses: allenporter/flux-local/action/test@4.3.1
   with:
     path: clusters/prod
     enable-helm: true
     enable-kyverno: false
 ```
 
 ### diff action
@@ -287,16 +287,16 @@
 how kustomzations may be affected, this action also supports overlays and multiple
 clusters showing you the final output.
 
 This is an example that diffs a `HelmRelease`:
 
 ```yaml
 - name: Setup Flux CLI
-  uses: fluxcd/flux2/action@v2
-- uses: allenporter/flux-local/action/diff@2.0.0
+  uses: fluxcd/flux2/action@v2.2.3
+- uses: allenporter/flux-local/action/diff@4.3.1
   id: diff
   with:
     live-branch: main
     path: clusters/prod
     resource: helmrelease
 - name: PR Comments
   uses: mshick/add-pr-comment@v2
@@ -324,16 +324,16 @@
           - clusters/dev
           - clusters/prod
         resource:
           - helmrelease
           - kustomization
     steps:
       - name: Setup Flux CLI
-        uses: fluxcd/flux2/action@v2
-      - uses: allenporter/flux-local/action/diff@2.0.0
+        uses: fluxcd/flux2/action@v2.2.3
+      - uses: allenporter/flux-local/action/diff@4.3.1
         id: diff
         with:
           live-branch: main
           path: ${{ matrix.cluster_path }}
           resource: ${{ matrix.resource }}
       - name: PR Comments
         uses: mshick/add-pr-comment@v2
```

### Comparing `flux-local-4.3.1/README.md` & `flux_local-5.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 ```
 
 ### flux-local diff
 
 You may also use `flux-local` to verify your local changes to cluster resources have the desird
 effect. This is similar to `flux diff` but entirely local. This will run a local `kustomize build`
 first against the local repo then again against a prior repo revision, then prints the output:
-```bash
+```diff
 $ flux-local diff ks apps
 ---
 
 +++
 
 @@ -2,6 +2,13 @@
 
@@ -153,15 +153,15 @@
 On branch dev
 Your branch is up to date with 'origin/dev'.
 
 Changes not staged for commit:
 	modified:   home/dev/hajimari-values.yaml
 
 $ export DIFF="dyff between --omit-header --color on"
-# flux-local diff ks home --path clusters/dev/
+$ flux-local diff ks home --path clusters/dev/
 
 spec.chart.spec.version  (HelmRelease/hajimari/hajimari)
   ± value change
     - 2.0.2
     + 2.0.1
 
 $ flux-local diff hr hajimari -n hajimari --path clusters/dev/
@@ -247,16 +247,16 @@
 or that ingress objects are valid).
 
 This example will run `flux-local test` against the cluster in `clusters/prod` with
 helm release expansion enabled.
 
 ```yaml
 - name: Setup Flux CLI
-  uses: fluxcd/flux2/action@v2
-- uses: allenporter/flux-local/test@2.0.0
+  uses: fluxcd/flux2/action@v2.2.2
+- uses: allenporter/flux-local/action/test@4.3.1
   with:
     path: clusters/prod
     enable-helm: true
     enable-kyverno: false
 ```
 
 ### diff action
@@ -266,16 +266,16 @@
 how kustomzations may be affected, this action also supports overlays and multiple
 clusters showing you the final output.
 
 This is an example that diffs a `HelmRelease`:
 
 ```yaml
 - name: Setup Flux CLI
-  uses: fluxcd/flux2/action@v2
-- uses: allenporter/flux-local/action/diff@2.0.0
+  uses: fluxcd/flux2/action@v2.2.3
+- uses: allenporter/flux-local/action/diff@4.3.1
   id: diff
   with:
     live-branch: main
     path: clusters/prod
     resource: helmrelease
 - name: PR Comments
   uses: mshick/add-pr-comment@v2
@@ -303,16 +303,16 @@
           - clusters/dev
           - clusters/prod
         resource:
           - helmrelease
           - kustomization
     steps:
       - name: Setup Flux CLI
-        uses: fluxcd/flux2/action@v2
-      - uses: allenporter/flux-local/action/diff@2.0.0
+        uses: fluxcd/flux2/action@v2.2.3
+      - uses: allenporter/flux-local/action/diff@4.3.1
         id: diff
         with:
           live-branch: main
           path: ${{ matrix.cluster_path }}
           resource: ${{ matrix.resource }}
       - name: PR Comments
         uses: mshick/add-pr-comment@v2
```

### Comparing `flux-local-4.3.1/flux_local/command.py` & `flux_local-5.0.0/flux_local/command.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local/context.py` & `flux_local-5.0.0/flux_local/context.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local/git_repo.py` & `flux_local-5.0.0/flux_local/git_repo.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 
 import asyncio
 import contextlib
 from dataclasses import dataclass, field
 import logging
 import os
 import tempfile
-from collections.abc import Callable, Awaitable, Iterable
+from collections import deque
+from collections.abc import Callable, Awaitable
 from functools import cache
 from pathlib import Path
-import queue
 from typing import Any, Generator
 
 import git
 
-from . import kustomize, helm
+from . import kustomize, values
 from .exceptions import FluxException, KustomizePathException
 from .manifest import (
     CRD_KIND,
     FLUXTOMIZE_DOMAIN,
     KUSTOMIZE_DOMAIN,
     Cluster,
     ClusterPolicy,
@@ -390,14 +390,22 @@
         if cmd := self._cache.get(key):
             return cmd
         cmd = kustomize.flux_build(kustomization, path)
         cmd = await cmd.stash()
         self._cache[key] = cmd
         return cmd
 
+    def remove(self, kustomization: Kustomization) -> None:
+        """Remove the kustomization value from the cache."""
+        target_key = f"{kustomization.namespaced_name} @"
+        for key in list(self._cache.keys()):
+            if key.startswith(target_key):
+                _LOGGER.debug("Invalidated cache %s", key)
+                del self._cache[key]
+
 
 async def visit_kustomization(
     selector: PathSelector,
     builder: CachableBuilder,
     path: Path,
     visit_ks: Kustomization | None,
 ) -> list[Kustomization]:
@@ -454,21 +462,21 @@
 ) -> list[Kustomization]:
     """Search for kustomizations in the specified path."""
 
     response_kustomizations: list[Kustomization] = []
     visited_paths: set[Path] = set()  # Relative paths within the cluster
     visited_ks: set[str] = set()
 
-    path_queue: queue.Queue[tuple[Path, Kustomization | None]] = queue.Queue()
-    path_queue.put((selector.relative_path, None))
-    while not path_queue.empty():
+    path_queue: deque[tuple[Path, Kustomization | None]] = deque()
+    path_queue.append((selector.relative_path, None))
+    while path_queue:
         # Fully empty the queue, running all tasks in parallel
         tasks = []
-        while not path_queue.empty():
-            (path, visit_ks) = path_queue.get()
+        while path_queue:
+            (path, visit_ks) = path_queue.popleft()
 
             if path in visited_paths:
                 _LOGGER.debug("Already visited %s", path)
                 continue
             visited_paths.add(path)
 
             tasks.append(visit_kustomization(selector, builder, path, visit_ks))
@@ -490,15 +498,15 @@
                 ks.name,
                 ks.source_kind,
                 ks.source_name,
             )
             if not (ks_path := adjust_ks_path(ks, selector)):
                 continue
             ks.path = str(ks_path)
-            path_queue.put((ks_path, ks))
+            path_queue.append((ks_path, ks))
             response_kustomizations.append(ks)
 
     response_kustomizations.sort(key=lambda x: (x.namespace, x.name))
     return response_kustomizations
 
 
 def node_name(ks: Kustomization) -> str:
@@ -512,36 +520,30 @@
 
 async def build_kustomization(
     kustomization: Kustomization,
     cluster_path: Path,
     selector: ResourceSelector,
     kustomize_flags: list[str],
     builder: CachableBuilder,
-) -> tuple[
-    Iterable[HelmRepository],
-    Iterable[HelmRelease],
-    Iterable[ClusterPolicy],
-    Iterable[ConfigMap],
-    Iterable[Secret],
-]:
-    """Build helm objects for the Kustomization."""
+) -> None:
+    """Build helm objects for the Kustomization and update state."""
 
     root: Path = selector.path.root
     kustomization_selector: MetadataSelector = selector.kustomization
     helm_repo_selector: MetadataSelector = selector.helm_repo
     helm_release_selector: MetadataSelector = selector.helm_release
     cluster_policy_selector: MetadataSelector = selector.cluster_policy
     if (
         not kustomization_selector.enabled
         and not helm_repo_selector.enabled
         and not helm_release_selector.enabled
         and not cluster_policy_selector.enabled
         and not selector.doc_visitor
     ):
-        return ([], [], [], [], [])
+        return
 
     with trace_context(f"Build '{kustomization.namespaced_name}'"):
         cmd = await builder.build(kustomization, root / kustomization.path)
         skips = []
         if kustomization_selector.skip_crds:
             skips.append(CRD_KIND)
         if kustomization_selector.skip_secrets:
@@ -560,72 +562,96 @@
             await kustomization_selector.visitor.func(
                 Path(kustomization.path),
                 kustomization,
                 cmd,
             )
 
         kinds = []
+        # Needed for expanding postbuild substitutions and value references
+        kinds.append(CONFIG_MAP_KIND)
         if helm_repo_selector.enabled:
             kinds.append(HELM_REPO_KIND)
         if helm_release_selector.enabled:
             kinds.append(HELM_RELEASE_KIND)
             # Needed for expanding value references
-            kinds.append(CONFIG_MAP_KIND)
             kinds.append(SECRET_KIND)
         if cluster_policy_selector.enabled:
             kinds.append(CLUSTER_POLICY_KIND)
         if selector.doc_visitor:
             kinds.extend(selector.doc_visitor.kinds)
         if not kinds:
-            return ([], [], [], [], [])
+            return
 
         regexp = f"kind=^({'|'.join(kinds)})$"
         docs = await cmd.grep(regexp).objects(
             target_namespace=kustomization.target_namespace
         )
 
         if selector.doc_visitor:
             doc_kinds = set(selector.doc_visitor.kinds)
             for doc in docs:
                 if doc.get("kind") not in doc_kinds:
                     continue
                 selector.doc_visitor.func(kustomization.namespaced_name, doc)
 
-        return (
+        kustomization.helm_repos = list(
             filter(
                 helm_repo_selector.predicate,
                 [
                     HelmRepository.parse_doc(doc)
                     for doc in docs
                     if doc.get("kind") == HELM_REPO_KIND
                 ],
-            ),
+            )
+        )
+        kustomization.helm_releases = list(
             filter(
                 helm_release_selector.predicate,
                 [
                     HelmRelease.parse_doc(doc)
                     for doc in docs
                     if doc.get("kind") == HELM_RELEASE_KIND
                 ],
-            ),
+            )
+        )
+        kustomization.cluster_policies = list(
             filter(
                 cluster_policy_selector.predicate,
                 [
                     ClusterPolicy.parse_doc(doc)
                     for doc in docs
                     if doc.get("kind") == CLUSTER_POLICY_KIND
                 ],
-            ),
-            [
-                ConfigMap.parse_doc(doc)
-                for doc in docs
-                if doc.get("kind") == CONFIG_MAP_KIND
-            ],
-            [Secret.parse_doc(doc) for doc in docs if doc.get("kind") == SECRET_KIND],
+            )
         )
+        kustomization.config_maps = [
+            ConfigMap.parse_doc(doc)
+            for doc in docs
+            if doc.get("kind") == CONFIG_MAP_KIND
+        ]
+        kustomization.secrets = [
+            Secret.parse_doc(doc) for doc in docs if doc.get("kind") == SECRET_KIND
+        ]
+
+
+def _ready_kustomizations(kustomizations: list[Kustomization], visited: set[str]) -> tuple[Kustomization, Kustomization]:
+    """Split the kustomizations into those that are ready vs pending."""
+    ready = []
+    pending = []
+    for kustomization in kustomizations:
+        if not_ready := (set(kustomization.depends_on or {}) - visited):
+            _LOGGER.debug(
+                "Kustomization %s waiting for %s",
+                kustomization.namespaced_name,
+                not_ready,
+            )
+            pending.append(kustomization)
+        else:
+            ready.append(kustomization)
+    return (ready, pending)
 
 
 async def build_manifest(
     path: Path | None = None,
     selector: ResourceSelector = ResourceSelector(),
     options: Options = Options(),
 ) -> Manifest:
@@ -654,58 +680,66 @@
                 kustomizations=[
                     ks for ks in results if selector.kustomization.predicate(ks)
                 ],
             )
         ]
 
         async def update_kustomization(cluster: Cluster) -> None:
-            build_tasks = []
-            for kustomization in cluster.kustomizations:
-                _LOGGER.debug(
-                    "Processing kustomization '%s': %s",
-                    kustomization.name,
-                    kustomization.path,
-                )
-                build_tasks.append(
-                    build_kustomization(
-                        kustomization,
-                        Path(cluster.path),
-                        selector,
-                        options.kustomize_flags,
-                        builder,
+            queue = [*cluster.kustomizations]
+            visited: set[str] = set()
+            while queue:
+                build_tasks = []
+                (ready, pending) = _ready_kustomizations(queue, visited)
+                for kustomization in ready:
+                    _LOGGER.debug("Processing kustomization '%s': %s", kustomization.name, kustomization.path)
+
+                    if kustomization.postbuild_substitute_from:
+                        values.expand_postbuild_substitute_reference(
+                            kustomization,
+                            values.ks_cluster_config(cluster.kustomizations),
+                        )
+                        # Clear the cache to remove any previous builds that are
+                        # missing the postbuild substitutions.
+                        builder.remove(kustomization)
+
+                    build_tasks.append(
+                        build_kustomization(
+                            kustomization,
+                            Path(cluster.path),
+                            selector,
+                            options.kustomize_flags,
+                            builder,
+                        )
                     )
-                )
-            results = list(await asyncio.gather(*build_tasks))
-            for kustomization, (
-                helm_repos,
-                helm_releases,
-                cluster_policies,
-                config_maps,
-                secrets,
-            ) in zip(
-                cluster.kustomizations,
-                results,
-            ):
-                kustomization.helm_repos = list(helm_repos)
-                kustomization.helm_releases = list(helm_releases)
-                kustomization.cluster_policies = list(cluster_policies)
-                kustomization.config_maps = list(config_maps)
-                kustomization.secrets = list(secrets)
+                if not build_tasks:
+                    raise FluxException(
+                        "Internal error: Unexpected loop without build tasks"
+                    )
+                await asyncio.gather(*build_tasks)
+                visited.update([ks.namespaced_name for ks in ready])
+                queue = pending
+
+        # Validate all Kustomizations have valid dependsOn attributes since later
+        # we'll be using them to order processing.
+        for cluster in clusters:
+            all_ks = set([ks.namespaced_name for ks in cluster.kustomizations])
+            for ks in cluster.kustomizations:
+                ks.validate_depends_on(all_ks)
 
         kustomization_tasks = []
         # Expand and visit Kustomizations
         for cluster in clusters:
             kustomization_tasks.append(update_kustomization(cluster))
         await asyncio.gather(*kustomization_tasks)
 
         # Handle any HelmRelease value references
         for cluster in clusters:
             for kustomization in cluster.kustomizations:
                 kustomization.helm_releases = [
-                    helm.expand_value_references(helm_release, kustomization)
+                    values.expand_value_references(helm_release, kustomization)
                     for helm_release in kustomization.helm_releases
                 ]
 
         # Visit Helm resources
         for cluster in clusters:
             if selector.helm_repo.visitor:
                 for kustomization in cluster.kustomizations:
```

### Comparing `flux-local-4.3.1/flux_local/image.py` & `flux_local-5.0.0/flux_local/image.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local/kustomize.py` & `flux_local-5.0.0/flux_local/kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local/manifest.py` & `flux_local-5.0.0/flux_local/manifest.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,99 +2,102 @@
 
 A manifest may be built directly from the local context of a cluster, or may be
 serialized and stored and checked into the cluster for use in other applications
 e.g. such as writing management plan for resources.
 """
 
 import base64
+from dataclasses import dataclass, field
+import logging
 from pathlib import Path
 from typing import Any, Optional, cast
 
 import aiofiles
-import yaml
-
-from pydantic import BaseModel, Field
+from mashumaro.codecs.yaml import yaml_decode, yaml_encode
+from mashumaro import DataClassDictMixin, field_options
+from mashumaro.config import BaseConfig
 
 from .exceptions import InputException
 
 __all__ = [
     "read_manifest",
     "write_manifest",
     "Manifest",
     "Cluster",
     "Kustomization",
     "HelmRepository",
     "HelmRelease",
     "HelmChart",
     "ClusterPolicy",
+    "ConfigMap",
+    "Secret",
 ]
 
+_LOGGER = logging.getLogger(__name__)
+
+
 # Match a prefix of apiVersion to ensure we have the right type of object.
 # We don't check specific versions for forward compatibility on upgrade.
 FLUXTOMIZE_DOMAIN = "kustomize.toolkit.fluxcd.io"
 KUSTOMIZE_DOMAIN = "kustomize.config.k8s.io"
 HELM_REPO_DOMAIN = "source.toolkit.fluxcd.io"
 HELM_RELEASE_DOMAIN = "helm.toolkit.fluxcd.io"
 CLUSTER_POLICY_DOMAIN = "kyverno.io"
 CRD_KIND = "CustomResourceDefinition"
 SECRET_KIND = "Secret"
 CONFIG_MAP_KIND = "ConfigMap"
 DEFAULT_NAMESPACE = "flux-system"
-VALUE_PLACEHOLDER = "**PLACEHOLDER**"
+VALUE_PLACEHOLDER = "!!PLACEHOLDER!!"
 VALUE_B64_PLACEHOLDER = base64.b64encode(VALUE_PLACEHOLDER.encode())
 
 REPO_TYPE_DEFAULT = "default"
 REPO_TYPE_OCI = "oci"
 
 
 def _check_version(doc: dict[str, Any], version: str) -> None:
     """Assert that the resource has the specified version."""
     if not (api_version := doc.get("apiVersion")):
         raise InputException(f"Invalid object missing apiVersion: {doc}")
     if not api_version.startswith(version):
         raise InputException(f"Invalid object expected '{version}': {doc}")
 
 
-class BaseManifest(BaseModel):
+@dataclass
+class BaseManifest(DataClassDictMixin):
     """Base class for all manifest objects."""
 
-    def compact_dict(self, exclude: dict[str, Any] | None = None) -> dict[str, Any]:
+    def compact_dict(self) -> dict[str, Any]:
         """Return a compact dictionary representation of the object.
 
         This is similar to `dict()` but with a specific implementation for serializing
         with variable fields removed.
         """
-        if exclude is None:
-            exclude = self.compact_exclude_fields()
-        return self.model_dump(exclude=exclude, exclude_unset=True, exclude_none=True)
-
-    @classmethod
-    def compact_exclude_fields(cls) -> dict[str, Any]:
-        """Return a dictionary of fields to exclude from compact_dict."""
-        return {}
+        return self.to_dict()
 
     @classmethod
     def parse_yaml(cls, content: str) -> "BaseManifest":
         """Parse a serialized manifest."""
-        doc = next(yaml.load_all(content, Loader=yaml.Loader), None)
-        return cls.model_validate(doc)
+        return yaml_decode(content, cls)
 
     def yaml(self, exclude: dict[str, Any] | None = None) -> str:
         """Return a YAML string representation of compact_dict."""
-        data = self.compact_dict(exclude)
-        return yaml.dump(data, sort_keys=False, explicit_start=True)
+        return yaml_encode(self, self.__class__)
 
+    class Config(BaseConfig):
+        omit_none = True
 
+
+@dataclass
 class HelmChart(BaseManifest):
     """A representation of an instantiation of a chart for a HelmRelease."""
 
     name: str
     """The name of the chart within the HelmRepository."""
 
-    version: Optional[str] = None
+    version: Optional[str] = field(metadata={"serialize":"omit"})
     """The version of the chart."""
 
     repo_name: str
     """The short name of the HelmRepository."""
 
     repo_namespace: str
     """The namespace of the HelmRepository."""
@@ -131,58 +134,54 @@
         return f"{self.repo_namespace}-{self.repo_name}"
 
     @property
     def chart_name(self) -> str:
         """Identifier for the HelmChart."""
         return f"{self.repo_full_name}/{self.name}"
 
-    @classmethod
-    def compact_exclude_fields(cls) -> dict[str, Any]:
-        """Return a dictionary of fields to exclude from compact_dict."""
-        return {"version": True}
-
 
+@dataclass
 class ValuesReference(BaseManifest):
     """A reference to a resource containing values for a HelmRelease."""
 
     kind: str
     """The kind of resource."""
 
     name: str
     """The name of the resource."""
 
-    values_key: str = Field(alias="valuesKey", default="values.yaml")
+    values_key: str = field(metadata=field_options(alias="valuesKey"), default="values.yaml")
     """The key in the resource that contains the values."""
 
-    target_path: Optional[str] = Field(alias="targetPath", default=None)
+    target_path: Optional[str] = field(metadata=field_options(alias="targetPath"), default=None)
     """The path in the HelmRelease values to store the values."""
 
     optional: bool = False
     """Whether the reference is optional."""
 
-
+@dataclass
 class HelmRelease(BaseManifest):
     """A representation of a Flux HelmRelease."""
 
     name: str
     """The name of the HelmRelease."""
 
     namespace: str
     """The namespace that owns the HelmRelease."""
 
     chart: HelmChart
     """A mapping to a specific helm chart for this HelmRelease."""
 
-    values: Optional[dict[str, Any]] = None
+    values: Optional[dict[str, Any]] = field(metadata={"serialize":"omit"})
     """The values to install in the chart."""
 
-    values_from: Optional[list[ValuesReference]]
+    values_from: Optional[list[ValuesReference]] = field(metadata={"serialize":"omit"})
     """A list of values to reference from an ConfigMap or Secret."""
 
-    images: list[str] = Field(default_factory=list)
+    images: list[str] | None = field(default=None)
     """The list of images referenced in the HelmRelease."""
 
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "HelmRelease":
         """Parse a HelmRelease from a kubernetes resource object."""
         _check_version(doc, HELM_RELEASE_DOMAIN)
         if not (metadata := doc.get("metadata")):
@@ -191,16 +190,16 @@
             raise InputException(f"Invalid {cls} missing metadata.name: {doc}")
         if not (namespace := metadata.get("namespace")):
             raise InputException(f"Invalid {cls} missing metadata.namespace: {doc}")
         chart = HelmChart.parse_doc(doc, namespace)
         spec = doc["spec"]
         values_from: list[ValuesReference] | None = None
         if values_from_dict := spec.get("valuesFrom"):
-            values_from = [ValuesReference(**subdoc) for subdoc in values_from_dict]
-        return cls(
+            values_from = [ValuesReference.from_dict(subdoc) for subdoc in values_from_dict]
+        return HelmRelease(
             name=name,
             namespace=namespace,
             chart=chart,
             values=spec.get("values"),
             values_from=values_from,
         )
 
@@ -215,24 +214,16 @@
         return f"{self.chart.repo_namespace}-{self.chart.repo_name}"
 
     @property
     def namespaced_name(self) -> str:
         """Return the namespace and name concatenated as an id."""
         return f"{self.namespace}/{self.name}"
 
-    @classmethod
-    def compact_exclude_fields(cls) -> dict[str, Any]:
-        """Return a dictionary of fields to exclude from compact_dict."""
-        return {
-            "values": True,
-            "values_from": True,
-            "chart": HelmChart.compact_exclude_fields(),
-        }
-
 
+@dataclass
 class HelmRepository(BaseManifest):
     """A representation of a flux HelmRepository."""
 
     name: str
     """The name of the HelmRepository."""
 
     namespace: str
@@ -267,24 +258,25 @@
 
     @property
     def repo_name(self) -> str:
         """Identifier for the HelmRepository."""
         return f"{self.namespace}-{self.name}"
 
 
+@dataclass
 class ClusterPolicy(BaseManifest):
     """A kyverno policy object."""
 
     name: str
     """The name of the kustomization."""
 
     namespace: str | None = None
     """The namespace of the kustomization."""
 
-    doc: dict[str, Any] | None = None
+    doc: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
     """The raw ClusterPolicy document."""
 
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "ClusterPolicy":
         """Parse a cluster policy object from a kubernetes resource."""
         _check_version(doc, CLUSTER_POLICY_DOMAIN)
         if not (metadata := doc.get("metadata")):
@@ -292,35 +284,29 @@
         if not (name := metadata.get("name")):
             raise InputException(f"Invalid {cls} missing metadata.name: {doc}")
         namespace = metadata.get("namespace")
         if not doc.get("spec"):
             raise InputException(f"Invalid {cls} missing spec: {doc}")
         return ClusterPolicy(name=name, namespace=namespace, doc=doc)
 
-    @classmethod
-    def compact_exclude_fields(cls) -> dict[str, Any]:
-        """Return a dictionary of fields to exclude from compact_dict."""
-        return {
-            "doc": True,
-        }
-
 
+@dataclass
 class ConfigMap(BaseManifest):
     """A ConfigMap is an API object used to store data in key-value pairs."""
 
     name: str
     """The name of the kustomization."""
 
     namespace: str | None = None
     """The namespace of the kustomization."""
 
-    data: dict[str, Any] | None = None
+    data: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
     """The data in the ConfigMap."""
 
-    binary_data: dict[str, Any] | None = None
+    binary_data: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
     """The binary data in the ConfigMap."""
 
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "ConfigMap":
         """Parse a config map object from a kubernetes resource."""
         _check_version(doc, "v1")
         if not (metadata := doc.get("metadata")):
@@ -328,39 +314,32 @@
         if not (name := metadata.get("name")):
             raise InputException(f"Invalid {cls} missing metadata.name: {doc}")
         namespace = metadata.get("namespace")
         return ConfigMap(
             name=name,
             namespace=namespace,
             data=doc.get("data"),
-            binaryData=doc.get("binaryData"),
+            binary_data=doc.get("binaryData"),
         )
 
-    @classmethod
-    def compact_exclude_fields(cls) -> dict[str, Any]:
-        """Return a dictionary of fields to exclude from compact_dict."""
-        return {
-            "data": True,
-            "binaryData": True,
-        }
-
 
+@dataclass
 class Secret(BaseManifest):
     """A Secret contains a small amount of sensitive data."""
 
     name: str
     """The name of the kustomization."""
 
     namespace: str | None = None
     """The namespace of the kustomization."""
 
-    data: dict[str, Any] | None = None
+    data: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
     """The data in the Secret."""
 
-    string_data: dict[str, Any] | None = None
+    string_data: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
     """The string data in the Secret."""
 
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "Secret":
         """Parse a secret object from a kubernetes resource."""
         _check_version(doc, "v1")
         if not (metadata := doc.get("metadata")):
@@ -376,76 +355,91 @@
         if string_data := doc.get("stringData"):
             for key, value in string_data.items():
                 string_data[key] = VALUE_PLACEHOLDER
         return Secret(
             name=name, namespace=namespace, data=data, string_data=string_data
         )
 
-    @classmethod
-    def compact_exclude_fields(cls) -> dict[str, Any]:
-        """Return a dictionary of fields to exclude from compact_dict."""
-        return {
-            "data": True,
-            "stringData": True,
-        }
 
+@dataclass
+class SubstituteReference(BaseManifest):
+    """SubstituteReference contains a reference to a resource containing the variables name and value."""
 
+    kind: str
+    """The kind of resource."""
+
+    name: str
+    """The name of the resource."""
+
+    optional: bool = False
+    """Whether the reference is optional."""
+
+@dataclass
 class Kustomization(BaseManifest):
     """A Kustomization is a set of declared cluster artifacts.
 
     This represents a flux Kustomization that points to a path that
     contains typical `kustomize` Kustomizations on local disk that
     may be flat or contain overlays.
     """
 
     name: str
     """The name of the kustomization."""
 
-    namespace: str | None = None
+    namespace: str | None
     """The namespace of the kustomization."""
 
     path: str
     """The local repo path to the kustomization contents."""
 
-    helm_repos: list[HelmRepository] = Field(default_factory=list)
+    helm_repos: list[HelmRepository] = field(default_factory=list)
     """The set of HelmRepositories represented in this kustomization."""
 
-    helm_releases: list[HelmRelease] = Field(default_factory=list)
+    helm_releases: list[HelmRelease] = field(default_factory=list)
     """The set of HelmRelease represented in this kustomization."""
 
-    cluster_policies: list[ClusterPolicy] = Field(default_factory=list)
+    cluster_policies: list[ClusterPolicy] = field(default_factory=list)
     """The set of ClusterPolicies represented in this kustomization."""
 
-    config_maps: list[ConfigMap] = Field(default_factory=list)
+    config_maps: list[ConfigMap] = field(default_factory=list)
     """The list of config maps referenced in the kustomization."""
 
-    secrets: list[Secret] = Field(default_factory=list)
+    secrets: list[Secret] = field(default_factory=list)
     """The list of secrets referenced in the kustomization."""
 
-    source_path: str | None = None
+    source_path: str | None = field(metadata={"serialize":"omit"}, default=None)
     """Optional source path for this Kustomization, relative to the build path."""
 
-    source_kind: str | None = None
+    source_kind: str | None = field(metadata={"serialize":"omit"}, default=None)
     """The sourceRef kind that provides this Kustomization e.g. GitRepository etc."""
 
-    source_name: str | None = None
+    source_name: str | None = field(metadata={"serialize":"omit"}, default=None)
     """The name of the sourceRef that provides this Kustomization."""
 
-    source_namespace: str | None = None
+    source_namespace: str | None = field(metadata={"serialize":"omit"}, default=None)
     """The namespace of the sourceRef that provides this Kustomization."""
 
-    target_namespace: str | None = None
+    target_namespace: str | None = field(metadata={"serialize":"omit"}, default=None)
     """The namespace to target when performing the operation."""
 
-    contents: dict[str, Any] | None = None
+    contents: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
     """Contents of the raw Kustomization document."""
 
-    images: list[str] = Field(default_factory=list)
+    images: list[str] | None = field(default=None)
     """The list of images referenced in the kustomization."""
 
+    postbuild_substitute: Optional[dict[str, Any]] = field(metadata={"serialize":"omit"}, default=None)
+    """A map of key/value pairs to substitute into the final YAML manifest, after building."""
+
+    postbuild_substitute_from: Optional[list[SubstituteReference]] = field(metadata={"serialize":"omit"}, default=None)
+    """A list of substitutions to reference from an ConfigMap or Secret."""
+
+    depends_on: list[str] | None = field(metadata={"serialize":"omit"}, default=None)
+    """A list of namespaced names that this Kustomization depends on."""
+
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "Kustomization":
         """Parse a partial Kustomization from a kubernetes resource."""
         _check_version(doc, FLUXTOMIZE_DOMAIN)
         if not (metadata := doc.get("metadata")):
             raise InputException(f"Invalid {cls} missing metadata: {doc}")
         if not (name := metadata.get("name")):
@@ -453,72 +447,87 @@
         if not (namespace := metadata.get("namespace")):
             raise InputException(f"Invalid {cls} missing metadata.namespace: {doc}")
         if not (spec := doc.get("spec")):
             raise InputException(f"Invalid {cls} missing spec: {doc}")
         path = spec.get("path", "")
         source_path = metadata.get("annotations", {}).get("config.kubernetes.io/path")
         source_ref = spec.get("sourceRef", {})
+        postbuild = spec.get("postBuild", {})
+        substitute_from: list[SubstituteReference] | None = None
+        if substitute_from_dict := postbuild.get("substituteFrom"):
+            substitute_from = [
+                SubstituteReference(**subdoc) for subdoc in substitute_from_dict
+            ]
+        depends_on = []
+        for dependency in spec.get("dependsOn", ()):
+            if not (dep_name := dependency.get("name")):
+                raise InputException(f"Invalid {cls} missing dependsOn.name: {doc}")
+            dep_namespace = dependency.get("namespace", namespace)
+            depends_on.append(f"{dep_namespace}/{dep_name}")
         return Kustomization(
             name=name,
             namespace=namespace,
             path=path,
             source_path=source_path,
             source_kind=source_ref.get("kind"),
             source_name=source_ref.get("name"),
             source_namespace=source_ref.get("namespace", namespace),
             target_namespace=spec.get("targetNamespace"),
             contents=doc,
+            postbuild_substitute=postbuild.get("substitute"),
+            postbuild_substitute_from=substitute_from,
+            depends_on=depends_on,
         )
 
     @property
     def id_name(self) -> str:
         """Identifier for the Kustomization in tests"""
         return f"{self.path}"
 
     @property
     def namespaced_name(self) -> str:
         """Return the namespace and name concatenated as an id."""
         return f"{self.namespace}/{self.name}"
 
-    @classmethod
-    def compact_exclude_fields(cls) -> dict[str, Any]:
-        """Return a dictionary of fields to exclude from compact_dict."""
-        return {
-            "helm_releases": {
-                "__all__": HelmRelease.compact_exclude_fields(),
-            },
-            "cluster_policies": {
-                "__all__": ClusterPolicy.compact_exclude_fields(),
-            },
-            "config_maps": {
-                "__all__": ConfigMap.compact_exclude_fields(),
-            },
-            "secrets": {
-                "__all__": Secret.compact_exclude_fields(),
-            },
-            "source_path": True,
-            "source_name": True,
-            "source_namespace": True,
-            "source_kind": True,
-            "target_namespace": True,
-            "contents": True,
-        }
 
+    def validate_depends_on(self, all_ks: set[str]) -> None:
+        """Validate depends_on values are all correct given the list of Kustomizations."""
+        depends_on = set(self.depends_on or {})
+        if missing := (depends_on - all_ks):
+            _LOGGER.warning(
+                "Kustomization %s has dependsOn with invalid names: %s",
+                self.namespaced_name,
+                missing,
+            )
+            self.depends_on = list(depends_on - missing)
+    
+    def update_postbuild_substitutions(self, substitutions: dict[str, Any]) -> None:
+        """Update the postBuild.substitutions in the extracted values and raw doc contents."""
+        if self.postbuild_substitute is None:
+            self.postbuild_substitute = {}
+        self.postbuild_substitute.update(substitutions)
+        if self.contents:
+            post_build = self.contents["spec"]["postBuild"]
+            if (substitute := post_build.get("substitute")) is None:
+                substitute = {}
+                post_build["substitute"] = substitute
+            substitute.update(substitutions)
 
+@dataclass
 class Cluster(BaseManifest):
     """A set of nodes that run containerized applications.
 
     Many flux git repos will only have a single flux cluster, though
     a repo may also contain multiple (e.g. dev an prod).
     """
 
     path: str
     """The local git repo path to the Kustomization objects for the cluster."""
 
-    kustomizations: list[Kustomization] = Field(default_factory=list)
+    kustomizations: list[Kustomization] = field(default_factory=list)
     """A list of flux Kustomizations for the cluster."""
 
     @property
     def id_name(self) -> str:
         """Identifier for the Cluster in tests."""
         return f"{self.path}"
 
@@ -545,38 +554,22 @@
         """Return the list of ClusterPolicy objects from all Kustomizations."""
         return [
             policy
             for kustomization in self.kustomizations
             for policy in kustomization.cluster_policies
         ]
 
-    @classmethod
-    def compact_exclude_fields(cls) -> dict[str, Any]:
-        """Return a dictionary of fields to exclude from compact_dict."""
-        return {
-            "kustomizations": {
-                "__all__": Kustomization.compact_exclude_fields(),
-            }
-        }
-
 
+@dataclass
 class Manifest(BaseManifest):
     """Holds information about cluster and applications contained in a repo."""
 
     clusters: list[Cluster]
     """A list of Clusters represented in the repo."""
 
-    @classmethod
-    def compact_exclude_fields(cls) -> dict[str, Any]:
-        """Return a dictionary of fields to exclude from compact_dict."""
-        return {
-            "clusters": {
-                "__all__": Cluster.compact_exclude_fields(),
-            }
-        }
 
 
 async def read_manifest(manifest_path: Path) -> Manifest:
     """Return the contents of a serialized manifest file.
 
     A manifest file is typically created by `flux-local get cluster -o yaml` or
     similar command.
```

### Comparing `flux-local-4.3.1/flux_local/tool/build.py` & `flux_local-5.0.0/flux_local/tool/build.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local/tool/diagnostics.py` & `flux_local-5.0.0/flux_local/tool/diagnostics.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local/tool/diff.py` & `flux_local-5.0.0/flux_local/tool/diff.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local/tool/flux_local.py` & `flux_local-5.0.0/flux_local/tool/flux_local.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local/tool/format.py` & `flux_local-5.0.0/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local/tool/get.py` & `flux_local-5.0.0/flux_local/tool/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             cols.extend(["helmrepos", "releases"])
         if query.kustomization.namespace is None:
             cols.insert(0, "namespace")
         if len(manifest.clusters) > 1:
             cols.insert(0, "cluster")
         for cluster in manifest.clusters:
             for ks in cluster.kustomizations:
-                value = ks.dict(include=set(cols))
+                value = { k: v for k, v in ks.compact_dict().items() if k in cols }
                 if output == "wide":
                     value["helmrepos"] = len(ks.helm_repos)
                     value["releases"] = len(ks.helm_releases)
                 value["cluster"] = cluster.path
                 results.append(value)
 
         if not results:
@@ -122,15 +122,15 @@
 
         cols = ["name", "revision", "chart", "source"]
         if query.helm_release.namespace is None:
             cols.insert(0, "namespace")
         results: list[dict[str, Any]] = []
         for cluster in manifest.clusters:
             for helmrelease in cluster.helm_releases:
-                value = helmrelease.dict(include=set(cols))
+                value = { k: v for k, v in helmrelease.compact_dict().items() if k in cols }
                 value["revision"] = str(helmrelease.chart.version)
                 value["chart"] = f"{helmrelease.namespace}-{helmrelease.chart.name}"
                 value["source"] = helmrelease.chart.repo_name
                 results.append(value)
 
         if not results:
             print(selector.not_found("HelmRelease", query.helm_release))
@@ -226,15 +226,15 @@
             with open(output_file, "w") as file:
                 YamlFormatter().print([manifest.compact_dict()], file=file)
             return
 
         cols = ["path", "kustomizations"]
         results: list[dict[str, Any]] = []
         for cluster in manifest.clusters:
-            value: dict[str, Any] = cluster.dict(include=set(cols))
+            value = { k: v for k, v in cluster.compact_dict().items() if k in cols }
             value["kustomizations"] = len(cluster.kustomizations)
             results.append(value)
 
         with open(output_file, "w") as file:
             if not results:
                 print(
                     selector.not_found("flux cluster Kustmization", query.cluster),
```

### Comparing `flux-local-4.3.1/flux_local/tool/selector.py` & `flux_local-5.0.0/flux_local/tool/selector.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local/tool/test.py` & `flux_local-5.0.0/flux_local/tool/test.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local/tool/visitor.py` & `flux_local-5.0.0/flux_local/tool/visitor.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/flux_local.egg-info/PKG-INFO` & `flux_local-5.0.0/flux_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 4.3.1
+Version: 5.0.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles>=22.1.0
 Requires-Dist: nest_asyncio>=1.5.6
-Requires-Dist: pydantic>=2.5.2
 Requires-Dist: python-slugify>=8.0.0
 Requires-Dist: GitPython>=3.1.30
 Requires-Dist: PyYAML>=6.0
+Requires-Dist: mashumaro>=3.12
 Requires-Dist: pytest>=7.2.1
 Requires-Dist: pytest-asyncio>=0.20.3
 
 flux-local is a set of tools and libraries for managing a local flux gitops repository focused on validation steps to help improve quality of commits, PRs, and general local testing.
 
 This library uses command line tools like kustomize and helm to replicate the behavior of
 flux to gather objects in the cluster. It only looks at the local git repo, and not a live
@@ -115,15 +115,15 @@
 ```
 
 ### flux-local diff
 
 You may also use `flux-local` to verify your local changes to cluster resources have the desird
 effect. This is similar to `flux diff` but entirely local. This will run a local `kustomize build`
 first against the local repo then again against a prior repo revision, then prints the output:
-```bash
+```diff
 $ flux-local diff ks apps
 ---
 
 +++
 
 @@ -2,6 +2,13 @@
 
@@ -174,15 +174,15 @@
 On branch dev
 Your branch is up to date with 'origin/dev'.
 
 Changes not staged for commit:
 	modified:   home/dev/hajimari-values.yaml
 
 $ export DIFF="dyff between --omit-header --color on"
-# flux-local diff ks home --path clusters/dev/
+$ flux-local diff ks home --path clusters/dev/
 
 spec.chart.spec.version  (HelmRelease/hajimari/hajimari)
   ± value change
     - 2.0.2
     + 2.0.1
 
 $ flux-local diff hr hajimari -n hajimari --path clusters/dev/
@@ -268,16 +268,16 @@
 or that ingress objects are valid).
 
 This example will run `flux-local test` against the cluster in `clusters/prod` with
 helm release expansion enabled.
 
 ```yaml
 - name: Setup Flux CLI
-  uses: fluxcd/flux2/action@v2
-- uses: allenporter/flux-local/test@2.0.0
+  uses: fluxcd/flux2/action@v2.2.2
+- uses: allenporter/flux-local/action/test@4.3.1
   with:
     path: clusters/prod
     enable-helm: true
     enable-kyverno: false
 ```
 
 ### diff action
@@ -287,16 +287,16 @@
 how kustomzations may be affected, this action also supports overlays and multiple
 clusters showing you the final output.
 
 This is an example that diffs a `HelmRelease`:
 
 ```yaml
 - name: Setup Flux CLI
-  uses: fluxcd/flux2/action@v2
-- uses: allenporter/flux-local/action/diff@2.0.0
+  uses: fluxcd/flux2/action@v2.2.3
+- uses: allenporter/flux-local/action/diff@4.3.1
   id: diff
   with:
     live-branch: main
     path: clusters/prod
     resource: helmrelease
 - name: PR Comments
   uses: mshick/add-pr-comment@v2
@@ -324,16 +324,16 @@
           - clusters/dev
           - clusters/prod
         resource:
           - helmrelease
           - kustomization
     steps:
       - name: Setup Flux CLI
-        uses: fluxcd/flux2/action@v2
-      - uses: allenporter/flux-local/action/diff@2.0.0
+        uses: fluxcd/flux2/action@v2.2.3
+      - uses: allenporter/flux-local/action/diff@4.3.1
         id: diff
         with:
           live-branch: main
           path: ${{ matrix.cluster_path }}
           resource: ${{ matrix.resource }}
       - name: PR Comments
         uses: mshick/add-pr-comment@v2
```

### Comparing `flux-local-4.3.1/flux_local.egg-info/SOURCES.txt` & `flux_local-5.0.0/flux_local.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 flux_local/context.py
 flux_local/exceptions.py
 flux_local/git_repo.py
 flux_local/helm.py
 flux_local/image.py
 flux_local/kustomize.py
 flux_local/manifest.py
+flux_local/values.py
 flux_local.egg-info/PKG-INFO
 flux_local.egg-info/SOURCES.txt
 flux_local.egg-info/dependency_links.txt
 flux_local.egg-info/entry_points.txt
 flux_local.egg-info/requires.txt
 flux_local.egg-info/top_level.txt
 flux_local/tool/__init__.py
@@ -29,14 +30,15 @@
 flux_local/tool/visitor.py
 tests/test_command.py
 tests/test_git_repo.py
 tests/test_helm.py
 tests/test_image.py
 tests/test_kustomize.py
 tests/test_manifest.py
+tests/test_values.py
 tests/tool/__init__.py
 tests/tool/test_build.py
 tests/tool/test_diagnostics.py
 tests/tool/test_diff.py
 tests/tool/test_diff_hr.py
 tests/tool/test_diff_ks.py
 tests/tool/test_format.py
```

### Comparing `flux-local-4.3.1/setup.cfg` & `flux_local-5.0.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 4.3.1
+version = 5.0.0
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
@@ -15,18 +15,18 @@
 
 [options]
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	aiofiles>=22.1.0
 	nest_asyncio>=1.5.6
-	pydantic>=2.5.2
 	python-slugify>=8.0.0
 	GitPython>=3.1.30
 	PyYAML>=6.0
+	mashumaro>=3.12
 	pytest>=7.2.1
 	pytest-asyncio>=0.20.3
 
 [options.packages.find]
 exclude = 
 	tests
 	venv
```

### Comparing `flux-local-4.3.1/tests/test_command.py` & `flux_local-5.0.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/test_git_repo.py` & `flux_local-5.0.0/tests/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/test_image.py` & `flux_local-5.0.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/test_kustomize.py` & `flux_local-5.0.0/tests/test_kustomize.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         },
     }
 
 
 async def test_flux_build_path_is_not_dir() -> None:
     """Test case where the flux build path does not exist."""
     cmd = kustomize.flux_build(
-        manifest.Kustomization(name="example", path="./"),
+        manifest.Kustomization(name="example", path="./", namespace="flux-system"),
         Path(TESTDATA_DIR) / "does-not-exist",
     )
     with pytest.raises(exceptions.FluxException, match="not a directory"):
         await cmd.objects()
 
 
 async def test_flux_build() -> None:
```

### Comparing `flux-local-4.3.1/tests/test_manifest.py` & `flux_local-5.0.0/tests/test_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,15 @@
                 path="./example",
                 kustomizations=[],
             )
         ]
     )
     await write_manifest(tmp_path / "file.yaml", manifest)
     new_manifest = await read_manifest(tmp_path / "file.yaml")
-    assert new_manifest.model_dump() == {
+    assert new_manifest.compact_dict() == {
         "clusters": [
             {
                 "path": "./example",
                 "kustomizations": [],
             },
         ]
     }
-    assert new_manifest.compact_dict() == new_manifest.model_dump()
-    assert new_manifest.compact_dict() == manifest.model_dump()
```

### Comparing `flux-local-4.3.1/tests/tool/test_build.py` & `flux_local-5.0.0/tests/tool/test_build.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/tool/test_diagnostics.py` & `flux_local-5.0.0/tests/tool/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/tool/test_diff.py` & `flux_local-5.0.0/tests/tool/test_diff.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/tool/test_diff_hr.py` & `flux_local-5.0.0/tests/tool/test_diff_hr.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/tool/test_diff_ks.py` & `flux_local-5.0.0/tests/tool/test_diff_ks.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/tool/test_format.py` & `flux_local-5.0.0/tests/tool/test_format.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/tool/test_get_cluster.py` & `flux_local-5.0.0/tests/tool/test_get_cluster.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/tool/test_get_hr.py` & `flux_local-5.0.0/tests/tool/test_get_hr.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/tool/test_get_ks.py` & `flux_local-5.0.0/tests/tool/test_get_ks.py`

 * *Files identical despite different names*

### Comparing `flux-local-4.3.1/tests/tool/test_test.py` & `flux_local-5.0.0/tests/tool/test_test.py`

 * *Files identical despite different names*

