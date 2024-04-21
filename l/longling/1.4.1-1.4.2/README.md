# Comparing `tmp/longling-1.4.1.tar.gz` & `tmp/longling-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longling-1.4.1.tar", last modified: Sun Apr 21 04:53:43 2024, max compression
+gzip compressed data, was "longling-1.4.2.tar", last modified: Sun Apr 21 13:32:02 2024, max compression
```

## Comparing `longling-1.4.1.tar` & `longling-1.4.2.tar`

### file list

```diff
@@ -1,43 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.775459 longling-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-04-21 04:53:40.000000 longling-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-21 04:53:40.000000 longling-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-21 04:53:43.775459 longling-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-21 04:53:40.000000 longling-1.4.1/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-21 04:53:40.000000 longling-1.4.1/longling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-21 04:53:40.000000 longling-1.4.1/longling/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.763460 longling-1.4.1/longling/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.763460 longling-1.4.1/longling/infrastructure/meta_docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.763460 longling-1.4.1/longling/infrastructure/meta_docs/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/infrastructure/meta_docs/docs/mxnet/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-21 04:53:40.000000 longling-1.4.1/longling/infrastructure/meta_docs/docs/mxnet/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/infrastructure/meta_docs/docs/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-21 04:53:40.000000 longling-1.4.1/longling/infrastructure/meta_docs/docs/sphinx/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-21 04:53:40.000000 longling-1.4.1/longling/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/spider/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/download_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/spider/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/lib/get_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/spider/meta_data/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/meta_data/IPpool.json
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/meta_data/user_agents.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/spider/parser/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/parser/lxml_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 04:53:40.000000 longling-1.4.1/longling/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-21 04:53:40.000000 longling-1.4.1/longling/toolbox/toc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-21 04:53:43.775459 longling-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-21 04:53:40.000000 longling-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:02.006899 longling-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-04-21 13:31:54.000000 longling-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-21 13:31:54.000000 longling-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-21 13:32:02.006899 longling-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-21 13:31:54.000000 longling-1.4.2/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.994898 longling-1.4.2/longling/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-21 13:31:54.000000 longling-1.4.2/longling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-21 13:31:54.000000 longling-1.4.2/longling/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.990898 longling-1.4.2/longling/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.994898 longling-1.4.2/longling/infrastructure/meta_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/.pypirc.template
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/.travis.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.994898 longling-1.4.2/longling/infrastructure/meta_docs/Dockerfile/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/Dockerfile/nginx.docker
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/Dockerfile/python-cli.docker
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/Dockerfile/python-flask.docker
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/Makefile.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.994898 longling-1.4.2/longling/infrastructure/meta_docs/chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/chart/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/chart/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.998899 longling-1.4.2/longling/infrastructure/meta_docs/chart/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/chart/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/chart/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/chart/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/chart/templates/ingress.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/chart/templates/secret.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/chart/templates/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/chart/templates/serviceaccount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.998899 longling-1.4.2/longling/infrastructure/meta_docs/chart/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/chart/templates/tests/test-connection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/chart/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.998899 longling-1.4.2/longling/infrastructure/meta_docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/docs/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.998899 longling-1.4.2/longling/infrastructure/meta_docs/docs/mxnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/docs/mxnet/.math.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/docs/mxnet/conf.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/docs/mxnet/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.998899 longling-1.4.2/longling/infrastructure/meta_docs/docs/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/docs/sphinx/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.998899 longling-1.4.2/longling/infrastructure/meta_docs/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.998899 longling-1.4.2/longling/infrastructure/meta_docs/github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.998899 longling-1.4.2/longling/infrastructure/meta_docs/gitignore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/gitignore/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/gitignore/docs.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/gitignore/python.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/gitignore/web.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.998899 longling-1.4.2/longling/infrastructure/meta_docs/gitlab-ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/gitlab-ci/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/gitlab-ci/helm_install.gitlab-ci.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/gitlab-ci/nginx.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/gitlab-ci/python.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/gitlab-ci/vue.gitlab-ci.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:02.002899 longling-1.4.2/longling/infrastructure/meta_docs/nni/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/nni/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/nni/_search_space.json
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/setup.cfg.template
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-21 13:31:54.000000 longling-1.4.2/longling/infrastructure/meta_docs/setup.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-21 13:31:54.000000 longling-1.4.2/longling/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:01.990898 longling-1.4.2/longling/spider/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:02.002899 longling-1.4.2/longling/spider/meta_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 13:31:54.000000 longling-1.4.2/longling/spider/meta_data/IPpool.json
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-21 13:31:54.000000 longling-1.4.2/longling/spider/meta_data/user_agents.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:32:02.002899 longling-1.4.2/longling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-21 13:32:01.000000 longling-1.4.2/longling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-21 13:32:01.000000 longling-1.4.2/longling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:32:01.000000 longling-1.4.2/longling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 13:32:01.000000 longling-1.4.2/longling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-21 13:32:01.000000 longling-1.4.2/longling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 13:32:01.000000 longling-1.4.2/longling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-21 13:31:54.000000 longling-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-21 13:32:02.010899 longling-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-21 13:31:54.000000 longling-1.4.2/setup.py
```

### Comparing `longling-1.4.1/LICENSE` & `longling-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `longling-1.4.1/PKG-INFO` & `longling-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: longling
-Version: 1.4.1
+Version: 1.4.2
 Summary: This project aims to provide some handy toolkit functions to help construct the architecture.
 Home-page: https://gitlab.com/tswsxk/longling.git
 Author: Sherlock, Shiwei Tong
 Author-email: tongsw@mail.ustc.edu.cn
 License: LICENSE.txt
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pip
 Requires-Dist: tqdm
 Requires-Dist: fire
 Requires-Dist: PyYAML>=5.1
 Requires-Dist: toml
 Requires-Dist: multiprocess
```

### Comparing `longling-1.4.1/longling/__init__.py` & `longling-1.4.2/longling/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 from longling.utils import regex
 from longling.utils import stream
 from longling.utils import utilog
 from longling.utils import candylib
 from longling.utils import path
 from longling.utils import parser
 
-__version__ = '1.4.1'
+__version__ = '1.4.2'
```

### Comparing `longling-1.4.1/longling/main.py` & `longling-1.4.2/longling/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 def cli():  # pragma: no cover
     fire.Fire(
         {
             "train_valid_test": train_valid_test_cli,
             "train_test": train_test_cli,
             "kfold": kfold_cli,
             "toc": toc,
+            "infra": arch,
             "arch": arch,
             "tarch": tarch,
             "arch-cli": ArchCli,
             "max": select_max_cli,
             "amax": arg_select_max_cli,
             "min": select_min_cli,
             "amin": arg_select_min_cli,
```

### Comparing `longling-1.4.1/longling/spider/meta_data/user_agents.txt` & `longling-1.4.2/longling/spider/meta_data/user_agents.txt`

 * *Files identical despite different names*

### Comparing `longling-1.4.1/longling.egg-info/PKG-INFO` & `longling-1.4.2/longling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: longling
-Version: 1.4.1
+Version: 1.4.2
 Summary: This project aims to provide some handy toolkit functions to help construct the architecture.
 Home-page: https://gitlab.com/tswsxk/longling.git
 Author: Sherlock, Shiwei Tong
 Author-email: tongsw@mail.ustc.edu.cn
 License: LICENSE.txt
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pip
 Requires-Dist: tqdm
 Requires-Dist: fire
 Requires-Dist: PyYAML>=5.1
 Requires-Dist: toml
 Requires-Dist: multiprocess
```

### Comparing `longling-1.4.1/longling.egg-info/requires.txt` & `longling-1.4.2/longling.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longling-1.4.1/setup.py` & `longling-1.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # coding: utf-8
 # created by tongshiwei on 17-12-17
-import logging
 import io
 import os
 import re
-from distutils.core import setup
 
-from setuptools import find_packages
+from setuptools import find_packages, setup
 
 test_deps = [
     'pytest>=4',
     'pytest-cov>=2.6.0',
     'flake8'
 ]
 
@@ -86,32 +84,24 @@
 
 setup(
     name='longling',
     version=VERSION,
     author='Sherlock, Shiwei Tong',
     author_email='tongsw@mail.ustc.edu.cn',
     include_package_data=True,
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     packages=find_packages(
         include=[
             "longling",
-            "*.toolbox", "*.toolbox.*",
-            "*.lib", "*.lib.*",
-            "*.spider", "*.spider.*",
-            "*.Architecture", "*.Architecture.*",
-            "*.ML*",
         ],
         exclude=[
-            "*.mx_example", "*.gluon_example*", "*.gluon_exp*",
-            "*.mxnet_old*",
         ]
     ),
     entry_points={
         "console_scripts": [
-            "glue = longling.ML.MxnetHelper.glue.glue:cli",
             "longling = longling.main:cli"
         ],
     },
     url='https://gitlab.com/tswsxk/longling.git',
     license='LICENSE.txt',
     description='This project aims to provide some handy toolkit functions to help construct the architecture.',
     long_description=open('README.txt', encoding="utf-8").read(),
@@ -133,19 +123,20 @@
         'ml-viz': ml_base_deps + viz_deps,
         'viz': viz_deps,
         'ml-full': ml_full_deps,
         "spider": spider_deps,
         "full": full_deps
     },
     classifiers=[
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         "Environment :: Other Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

