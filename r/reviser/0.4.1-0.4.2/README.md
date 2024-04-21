# Comparing `tmp/reviser-0.4.1.tar.gz` & `tmp/reviser-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviser-0.4.1.tar", max compression
+gzip compressed data, was "reviser-0.4.2.tar", max compression
```

## Comparing `reviser-0.4.1.tar` & `reviser-0.4.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1078 2024-03-02 02:02:29.561668 reviser-0.4.1/LICENSE
--rw-r--r--   0        0        0    40957 2024-03-02 02:02:53.135869 reviser-0.4.1/README.md
--rw-r--r--   0        0        0     2690 2024-03-02 02:02:29.562668 reviser-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      838 2024-03-02 02:02:29.562668 reviser-0.4.1/reviser/__init__.py
--rw-r--r--   0        0        0     4780 2024-03-02 02:02:29.562668 reviser-0.4.1/reviser/bundling/__init__.py
--rw-r--r--   0        0        0     4930 2024-03-02 02:02:29.562668 reviser-0.4.1/reviser/bundling/_installer.py
--rw-r--r--   0        0        0     2855 2024-03-02 02:02:29.562668 reviser-0.4.1/reviser/cli.py
--rw-r--r--   0        0        0     1555 2024-03-02 02:02:29.562668 reviser-0.4.1/reviser/commands/__init__.py
--rw-r--r--   0        0        0     4767 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/aliaser.py
--rw-r--r--   0        0        0     2392 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/bundler.py
--rw-r--r--   0        0        0      851 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/configer.py
--rw-r--r--   0        0        0     2009 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/deployer.py
--rw-r--r--   0        0        0      637 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/exiter.py
--rw-r--r--   0        0        0     1800 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/helper/__init__.py
--rw-r--r--   0        0        0      198 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/helper/help.jinja2
--rw-r--r--   0        0        0     5193 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/invoker.py
--rw-r--r--   0        0        0     1268 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/lister.py
--rw-r--r--   0        0        0     8356 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/pruner.py
--rw-r--r--   0        0        0      876 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/pusher.py
--rw-r--r--   0        0        0     2471 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/region_switcher.py
--rw-r--r--   0        0        0     2543 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/reloader.py
--rw-r--r--   0        0        0     4698 2024-03-02 02:02:29.563668 reviser-0.4.1/reviser/commands/reporter.py
--rw-r--r--   0        0        0     5378 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/commands/selector.py
--rw-r--r--   0        0        0     1361 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/commands/sheller.py
--rw-r--r--   0        0        0     5009 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/commands/tailer.py
--rw-r--r--   0        0        0     1250 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/__init__.py
--rw-r--r--   0        0        0     5855 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/abstracts.py
--rw-r--r--   0        0        0     2248 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/aws.py
--rw-r--r--   0        0        0     3699 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/configurations/__init__.py
--rw-r--r--   0        0        0     9767 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/configurations/bundling.py
--rw-r--r--   0        0        0     9839 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/configurations/depending.py
--rw-r--r--   0        0        0     3989 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/configurations/enviromentals.py
--rw-r--r--   0        0        0     2262 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/configurations/imaging.py
--rw-r--r--   0        0        0     3053 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/configurations/layering.py
--rw-r--r--   0        0        0     9876 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/configurations/targeting.py
--rw-r--r--   0        0        0     3415 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/contexts.py
--rw-r--r--   0        0        0     1127 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/enumerations.py
--rw-r--r--   0        0        0     9690 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/infomatics.py
--rw-r--r--   0        0        0      570 2024-03-02 02:02:29.564668 reviser-0.4.1/reviser/definitions/selections.py
--rw-r--r--   0        0        0     2954 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/deploying/__init__.py
--rw-r--r--   0        0        0     6391 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/deploying/publisher.py
--rw-r--r--   0        0        0     6559 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/deploying/updater.py
--rw-r--r--   0        0        0     2383 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/deploying/uploader.py
--rw-r--r--   0        0        0      509 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/interactivity/__init__.py
--rw-r--r--   0        0        0     4153 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/interactivity/completions.py
--rw-r--r--   0        0        0     1592 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/interactivity/runner.py
--rw-r--r--   0        0        0     9639 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/interactivity/shells/__init__.py
--rw-r--r--   0        0        0      293 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/interactivity/shells/execution_result.jinja2
--rw-r--r--   0        0        0      514 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/interactivity/shells/prompt.jinja2
--rw-r--r--   0        0        0      277 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/interactivity/shells/splash.jinja2
--rw-r--r--   0        0        0     4469 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/parsing.py
--rw-r--r--   0        0        0      554 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/servicer/__init__.py
--rw-r--r--   0        0        0     3404 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/servicer/functioning/__init__.py
--rw-r--r--   0        0        0      334 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/servicer/functioning/echo_versions.jinja2
--rw-r--r--   0        0        0     4099 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/servicer/layering.py
--rw-r--r--   0        0        0     2395 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/templating/__init__.py
--rw-r--r--   0        0        0      260 2024-03-02 02:02:29.565668 reviser-0.4.1/reviser/templating/error.jinja2
--rw-r--r--   0        0        0     1827 2024-03-02 02:02:29.569668 reviser-0.4.1/reviser/utils.py
--rw-r--r--   0        0        0    42430 1970-01-01 00:00:00.000000 reviser-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-21 13:30:45.825712 reviser-0.4.2/LICENSE
+-rw-r--r--   0        0        0    40957 2024-04-21 13:31:02.975243 reviser-0.4.2/README.md
+-rw-r--r--   0        0        0     2548 2024-04-21 13:30:45.826712 reviser-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      838 2024-04-21 13:30:45.826712 reviser-0.4.2/reviser/__init__.py
+-rw-r--r--   0        0        0     4780 2024-04-21 13:30:45.826712 reviser-0.4.2/reviser/bundling/__init__.py
+-rw-r--r--   0        0        0     4930 2024-04-21 13:30:45.826712 reviser-0.4.2/reviser/bundling/_installer.py
+-rw-r--r--   0        0        0     2855 2024-04-21 13:30:45.826712 reviser-0.4.2/reviser/cli.py
+-rw-r--r--   0        0        0     1555 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/__init__.py
+-rw-r--r--   0        0        0     4767 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/aliaser.py
+-rw-r--r--   0        0        0     2392 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/bundler.py
+-rw-r--r--   0        0        0      851 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/configer.py
+-rw-r--r--   0        0        0     2009 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/deployer.py
+-rw-r--r--   0        0        0      637 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/exiter.py
+-rw-r--r--   0        0        0     1800 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/helper/__init__.py
+-rw-r--r--   0        0        0      198 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/helper/help.jinja2
+-rw-r--r--   0        0        0     5193 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/invoker.py
+-rw-r--r--   0        0        0     1268 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/lister.py
+-rw-r--r--   0        0        0     8356 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/pruner.py
+-rw-r--r--   0        0        0      876 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/pusher.py
+-rw-r--r--   0        0        0     2471 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/region_switcher.py
+-rw-r--r--   0        0        0     2543 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/reloader.py
+-rw-r--r--   0        0        0     4698 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/reporter.py
+-rw-r--r--   0        0        0     5378 2024-04-21 13:30:45.827712 reviser-0.4.2/reviser/commands/selector.py
+-rw-r--r--   0        0        0     1361 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/commands/sheller.py
+-rw-r--r--   0        0        0     5009 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/commands/tailer.py
+-rw-r--r--   0        0        0     1250 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/__init__.py
+-rw-r--r--   0        0        0     5855 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/abstracts.py
+-rw-r--r--   0        0        0     2248 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/aws.py
+-rw-r--r--   0        0        0     3699 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/configurations/__init__.py
+-rw-r--r--   0        0        0     9767 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/configurations/bundling.py
+-rw-r--r--   0        0        0     9839 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/configurations/depending.py
+-rw-r--r--   0        0        0     3989 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/configurations/enviromentals.py
+-rw-r--r--   0        0        0     2262 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/configurations/imaging.py
+-rw-r--r--   0        0        0     3053 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/configurations/layering.py
+-rw-r--r--   0        0        0     9876 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/configurations/targeting.py
+-rw-r--r--   0        0        0     3415 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/contexts.py
+-rw-r--r--   0        0        0     1127 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/enumerations.py
+-rw-r--r--   0        0        0     9690 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/infomatics.py
+-rw-r--r--   0        0        0      570 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/definitions/selections.py
+-rw-r--r--   0        0        0     2954 2024-04-21 13:30:45.828712 reviser-0.4.2/reviser/deploying/__init__.py
+-rw-r--r--   0        0        0     6391 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/deploying/publisher.py
+-rw-r--r--   0        0        0     6559 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/deploying/updater.py
+-rw-r--r--   0        0        0     2383 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/deploying/uploader.py
+-rw-r--r--   0        0        0      509 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/interactivity/__init__.py
+-rw-r--r--   0        0        0     4153 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/interactivity/completions.py
+-rw-r--r--   0        0        0     1592 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/interactivity/runner.py
+-rw-r--r--   0        0        0     9639 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/interactivity/shells/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/interactivity/shells/execution_result.jinja2
+-rw-r--r--   0        0        0      514 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/interactivity/shells/prompt.jinja2
+-rw-r--r--   0        0        0      277 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/interactivity/shells/splash.jinja2
+-rw-r--r--   0        0        0     4469 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/parsing.py
+-rw-r--r--   0        0        0      554 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/servicer/__init__.py
+-rw-r--r--   0        0        0     3404 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/servicer/functioning/__init__.py
+-rw-r--r--   0        0        0      334 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/servicer/functioning/echo_versions.jinja2
+-rw-r--r--   0        0        0     4099 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/servicer/layering.py
+-rw-r--r--   0        0        0     2395 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/templating/__init__.py
+-rw-r--r--   0        0        0      260 2024-04-21 13:30:45.829712 reviser-0.4.2/reviser/templating/error.jinja2
+-rw-r--r--   0        0        0     1827 2024-04-21 13:30:45.833712 reviser-0.4.2/reviser/utils.py
+-rw-r--r--   0        0        0    42301 1970-01-01 00:00:00.000000 reviser-0.4.2/PKG-INFO
```

### Comparing `reviser-0.4.1/LICENSE` & `reviser-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/README.md` & `reviser-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/pyproject.toml` & `reviser-0.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reviser"
-version = "0.4.1"
+version = "0.4.2"
 description = "AWS Lambda function/layer version deployment manager."
 authors = [
   "Scott Ernst <swernst@gmail.com>",
   "Kevin Schiroo",
   "Rigo Silva"
 ]
 license = "MIT"
@@ -14,52 +14,48 @@
 documentation = "https://gitlab.com/rocket-boosters/reviser"
 keywords = ["aws", "lambda"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Utilities",
   "Typing :: Typed"
 ]
 exclude = ["reviser/tests"]
 
 [tool.poetry.scripts]
 reviser = 'reviser.cli:main'
 reviser-shell = 'reviser:main_shell'
 
 [tool.poetry.dependencies]
-python = ">=3.8.0, <3.13.0"
-boto3 = { version = ">=1.16.11", optional = true }
+python = ">=3.10.2, <3.13.0"
+boto3 = { version = ">=1.34.45", optional = true }
 colorama = { version = ">=0.4.4", optional = true }
 Jinja2 = { version = ">=2.11.2", optional = true }
 prompt-toolkit = { version = ">=3.0.8", optional = true }
 PyYAML = { version = ">=5.3.0", optional = true }
 pipper = { version = ">=0.10.0", optional = true }
 toml = { version = ">=0.10.0", optional = true }
 wheel = { version = ">=0.37.1", optional = true }
-# AWS is not currently compatible with 2+
-urllib3 = "<2.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 black = "*"
 coverage = "*"
 pytest-cov = "*"
 lobotomy = ">=0.3.0"
 flake8 = "*"
 flake8-black = "*"
 mypy = "*"
-pydocstyle = "^6.1.1"
-radon = "^5.0.1"
+pydocstyle = ">=6.1.1"
+radon = ">=5.0.1"
 yamllint = "^1.26.1"
 taskipy = ">=1.4.0"
 
 [tool.taskipy.tasks]
 # https://github.com/illBeRoy/taskipy
 black = "black ."
 black_lint = "black . --check"
```

### Comparing `reviser-0.4.1/reviser/__init__.py` & `reviser-0.4.2/reviser/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/bundling/__init__.py` & `reviser-0.4.2/reviser/bundling/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/bundling/_installer.py` & `reviser-0.4.2/reviser/bundling/_installer.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/cli.py` & `reviser-0.4.2/reviser/cli.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/__init__.py` & `reviser-0.4.2/reviser/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/aliaser.py` & `reviser-0.4.2/reviser/commands/aliaser.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/bundler.py` & `reviser-0.4.2/reviser/commands/bundler.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/configer.py` & `reviser-0.4.2/reviser/commands/configer.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/deployer.py` & `reviser-0.4.2/reviser/commands/deployer.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/exiter.py` & `reviser-0.4.2/reviser/commands/exiter.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/helper/__init__.py` & `reviser-0.4.2/reviser/commands/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/invoker.py` & `reviser-0.4.2/reviser/commands/invoker.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/lister.py` & `reviser-0.4.2/reviser/commands/lister.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/pruner.py` & `reviser-0.4.2/reviser/commands/pruner.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/pusher.py` & `reviser-0.4.2/reviser/commands/pusher.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/region_switcher.py` & `reviser-0.4.2/reviser/commands/region_switcher.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/reloader.py` & `reviser-0.4.2/reviser/commands/reloader.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/reporter.py` & `reviser-0.4.2/reviser/commands/reporter.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/selector.py` & `reviser-0.4.2/reviser/commands/selector.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/sheller.py` & `reviser-0.4.2/reviser/commands/sheller.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/commands/tailer.py` & `reviser-0.4.2/reviser/commands/tailer.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/__init__.py` & `reviser-0.4.2/reviser/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/abstracts.py` & `reviser-0.4.2/reviser/definitions/abstracts.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/aws.py` & `reviser-0.4.2/reviser/definitions/aws.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/configurations/__init__.py` & `reviser-0.4.2/reviser/definitions/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/configurations/bundling.py` & `reviser-0.4.2/reviser/definitions/configurations/bundling.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/configurations/depending.py` & `reviser-0.4.2/reviser/definitions/configurations/depending.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/configurations/enviromentals.py` & `reviser-0.4.2/reviser/definitions/configurations/enviromentals.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/configurations/imaging.py` & `reviser-0.4.2/reviser/definitions/configurations/imaging.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/configurations/layering.py` & `reviser-0.4.2/reviser/definitions/configurations/layering.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/configurations/targeting.py` & `reviser-0.4.2/reviser/definitions/configurations/targeting.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/contexts.py` & `reviser-0.4.2/reviser/definitions/contexts.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/enumerations.py` & `reviser-0.4.2/reviser/definitions/enumerations.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/infomatics.py` & `reviser-0.4.2/reviser/definitions/infomatics.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/definitions/selections.py` & `reviser-0.4.2/reviser/definitions/selections.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/deploying/__init__.py` & `reviser-0.4.2/reviser/deploying/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/deploying/publisher.py` & `reviser-0.4.2/reviser/deploying/publisher.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/deploying/updater.py` & `reviser-0.4.2/reviser/deploying/updater.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/deploying/uploader.py` & `reviser-0.4.2/reviser/deploying/uploader.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/interactivity/completions.py` & `reviser-0.4.2/reviser/interactivity/completions.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/interactivity/runner.py` & `reviser-0.4.2/reviser/interactivity/runner.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/interactivity/shells/__init__.py` & `reviser-0.4.2/reviser/interactivity/shells/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/interactivity/shells/prompt.jinja2` & `reviser-0.4.2/reviser/interactivity/shells/prompt.jinja2`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/parsing.py` & `reviser-0.4.2/reviser/parsing.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/servicer/__init__.py` & `reviser-0.4.2/reviser/servicer/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/servicer/functioning/__init__.py` & `reviser-0.4.2/reviser/servicer/functioning/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/servicer/layering.py` & `reviser-0.4.2/reviser/servicer/layering.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/templating/__init__.py` & `reviser-0.4.2/reviser/templating/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/reviser/utils.py` & `reviser-0.4.2/reviser/utils.py`

 * *Files identical despite different names*

### Comparing `reviser-0.4.1/PKG-INFO` & `reviser-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: reviser
-Version: 0.4.1
+Version: 0.4.2
 Summary: AWS Lambda function/layer version deployment manager.
 Home-page: https://gitlab.com/rocket-boosters/reviser
 License: MIT
 Keywords: aws,lambda
 Author: Scott Ernst
 Author-email: swernst@gmail.com
-Requires-Python: >=3.8.0,<3.13.0
+Requires-Python: >=3.10.2,<3.13.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: shell
 Requires-Dist: Jinja2 (>=2.11.2) ; extra == "shell"
 Requires-Dist: PyYAML (>=5.3.0) ; extra == "shell"
-Requires-Dist: boto3 (>=1.16.11) ; extra == "shell"
+Requires-Dist: boto3 (>=1.34.45) ; extra == "shell"
 Requires-Dist: colorama (>=0.4.4) ; extra == "shell"
 Requires-Dist: pipper (>=0.10.0) ; extra == "shell"
 Requires-Dist: prompt-toolkit (>=3.0.8) ; extra == "shell"
 Requires-Dist: toml (>=0.10.0) ; extra == "shell"
-Requires-Dist: urllib3 (<2.0)
 Requires-Dist: wheel (>=0.37.1) ; extra == "shell"
 Project-URL: Documentation, https://gitlab.com/rocket-boosters/reviser
 Project-URL: Repository, https://gitlab.com/rocket-boosters/reviser
 Description-Content-Type: text/markdown
 
 # Reviser
```

