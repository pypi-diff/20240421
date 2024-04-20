# Comparing `tmp/matrix_alertbot-0.2.1.tar.gz` & `tmp/matrix_alertbot-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrix_alertbot-0.2.1.tar", last modified: Thu Apr 18 10:15:39 2024, max compression
+gzip compressed data, was "matrix_alertbot-0.2.2.tar", last modified: Sat Apr 20 22:36:05 2024, max compression
```

## Comparing `matrix_alertbot-0.2.1.tar` & `matrix_alertbot-0.2.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.089432 matrix_alertbot-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      384 2024-04-17 14:30:34.000000 matrix_alertbot-0.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2368 2024-04-17 14:42:10.000000 matrix_alertbot-0.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1491 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)    34523 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4553 2024-04-18 10:15:39.089432 matrix_alertbot-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2031 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     3977 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.1/SETUP.md
--rw-rw-rw-   0 root         (0) root         (0)     2922 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.1/config.sample.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.073432 matrix_alertbot-0.2.1/docker/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/docker/.env
--rw-rw-rw-   0 root         (0) root         (0)     3127 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/docker/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     2757 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/docker/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.073432 matrix_alertbot-0.2.1/docker/alertmanager/
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/docker/alertmanager/alertmanager.sample.yml
--rwxrwxrwx   0 root         (0) root         (0)      910 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/docker/build_and_install_libolm.sh
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/docker/docker-compose.yml
--rw-rw-rw-   0 root         (0) root         (0)      366 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/docker/matrix-alertbot.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.073432 matrix_alertbot-0.2.1/docker/prometheus/
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/docker/prometheus/prometheus.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.073432 matrix_alertbot-0.2.1/docker/prometheus/rules.d/
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/docker/prometheus/rules.d/health.yml
--rwxrwxrwx   0 root         (0) root         (0)      202 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/matrix-alertbot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.077432 matrix_alertbot-0.2.1/matrix_alertbot/
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/matrix_alertbot/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-18 10:15:38.000000 matrix_alertbot-0.2.1/matrix_alertbot/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/matrix_alertbot/alert.py
--rw-rw-rw-   0 root         (0) root         (0)     7762 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/matrix_alertbot/alertmanager.py
--rw-rw-rw-   0 root         (0) root         (0)    18555 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.1/matrix_alertbot/callback.py
--rw-rw-rw-   0 root         (0) root         (0)     3559 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/matrix_alertbot/chat_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    12279 2024-04-18 09:59:20.000000 matrix_alertbot-0.2.1/matrix_alertbot/command.py
--rw-rw-rw-   0 root         (0) root         (0)     7659 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.1/matrix_alertbot/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1477 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/matrix_alertbot/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/matrix_alertbot/main.py
--rw-rw-rw-   0 root         (0) root         (0)     9654 2024-01-22 10:50:25.000000 matrix_alertbot-0.2.1/matrix_alertbot/matrix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.065432 matrix_alertbot-0.2.1/matrix_alertbot/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.077432 matrix_alertbot-0.2.1/matrix_alertbot/resources/templates/
--rw-rw-rw-   0 root         (0) root         (0)      205 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/matrix_alertbot/resources/templates/alert.html.j2
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/matrix_alertbot/resources/templates/alert.txt.j2
--rw-rw-rw-   0 root         (0) root         (0)     8276 2024-01-22 10:43:28.000000 matrix_alertbot-0.2.1/matrix_alertbot/webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.081432 matrix_alertbot-0.2.1/matrix_alertbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4553 2024-04-18 10:15:38.000000 matrix_alertbot-0.2.1/matrix_alertbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1523 2024-04-18 10:15:39.000000 matrix_alertbot-0.2.1/matrix_alertbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 10:15:38.000000 matrix_alertbot-0.2.1/matrix_alertbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-18 10:15:38.000000 matrix_alertbot-0.2.1/matrix_alertbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 10:15:38.000000 matrix_alertbot-0.2.1/matrix_alertbot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      695 2024-04-18 10:15:38.000000 matrix_alertbot-0.2.1/matrix_alertbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 10:15:38.000000 matrix_alertbot-0.2.1/matrix_alertbot.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      222 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-17 14:42:10.000000 matrix_alertbot-0.2.1/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.077432 matrix_alertbot-0.2.1/scripts-dev/
--rwxrwxrwx   0 root         (0) root         (0)      360 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/scripts-dev/lint.sh
--rw-rw-rw-   0 root         (0) root         (0)     1936 2024-04-18 10:15:39.089432 matrix_alertbot-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.081432 matrix_alertbot-0.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 10:15:13.000000 matrix_alertbot-0.2.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.065432 matrix_alertbot-0.2.1/tests/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.081432 matrix_alertbot-0.2.1/tests/resources/config/
--rw-rw-rw-   0 root         (0) root         (0)     3502 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.1/tests/resources/config/config.full.yml
--rw-rw-rw-   0 root         (0) root         (0)      959 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/tests/resources/config/config.minimal.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:15:39.081432 matrix_alertbot-0.2.1/tests/resources/templates/
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/tests/resources/templates/alert.html.j2
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/tests/resources/templates/alert.txt.j2
--rw-rw-rw-   0 root         (0) root         (0)     6039 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.1/tests/test_alert.py
--rw-rw-rw-   0 root         (0) root         (0)    35542 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.1/tests/test_alertmanager.py
--rw-rw-rw-   0 root         (0) root         (0)    51407 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.1/tests/test_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     7908 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.1/tests/test_chat_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    27816 2024-04-18 10:06:38.000000 matrix_alertbot-0.2.1/tests/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)    15777 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.1/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11433 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.1/tests/test_matrix.py
--rw-rw-rw-   0 root         (0) root         (0)    22094 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.1/tests/test_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.074903 matrix_alertbot-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      384 2024-04-17 14:30:34.000000 matrix_alertbot-0.2.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2368 2024-04-17 14:42:10.000000 matrix_alertbot-0.2.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)    34523 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4553 2024-04-20 22:36:05.074903 matrix_alertbot-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     3977 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.2/SETUP.md
+-rw-rw-rw-   0 root         (0) root         (0)     2922 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.2/config.sample.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.034902 matrix_alertbot-0.2.2/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/docker/.env
+-rw-rw-rw-   0 root         (0) root         (0)     3127 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/docker/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     2757 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/docker/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.038902 matrix_alertbot-0.2.2/docker/alertmanager/
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/docker/alertmanager/alertmanager.sample.yml
+-rwxrwxrwx   0 root         (0) root         (0)      910 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/docker/build_and_install_libolm.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/docker/docker-compose.yml
+-rw-rw-rw-   0 root         (0) root         (0)      366 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/docker/matrix-alertbot.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.038902 matrix_alertbot-0.2.2/docker/prometheus/
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/docker/prometheus/prometheus.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.038902 matrix_alertbot-0.2.2/docker/prometheus/rules.d/
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/docker/prometheus/rules.d/health.yml
+-rwxrwxrwx   0 root         (0) root         (0)      202 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/matrix-alertbot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.046902 matrix_alertbot-0.2.2/matrix_alertbot/
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/matrix_alertbot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-20 22:36:04.000000 matrix_alertbot-0.2.2/matrix_alertbot/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/matrix_alertbot/alert.py
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/matrix_alertbot/alertmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)    18774 2024-04-20 15:56:58.000000 matrix_alertbot-0.2.2/matrix_alertbot/callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3559 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/matrix_alertbot/chat_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12279 2024-04-18 09:59:20.000000 matrix_alertbot-0.2.2/matrix_alertbot/command.py
+-rw-rw-rw-   0 root         (0) root         (0)     7659 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.2/matrix_alertbot/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/matrix_alertbot/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/matrix_alertbot/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     9698 2024-04-20 15:49:31.000000 matrix_alertbot-0.2.2/matrix_alertbot/matrix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.018901 matrix_alertbot-0.2.2/matrix_alertbot/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.050902 matrix_alertbot-0.2.2/matrix_alertbot/resources/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      205 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/matrix_alertbot/resources/templates/alert.html.j2
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/matrix_alertbot/resources/templates/alert.txt.j2
+-rw-rw-rw-   0 root         (0) root         (0)     8276 2024-01-22 10:43:28.000000 matrix_alertbot-0.2.2/matrix_alertbot/webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.062902 matrix_alertbot-0.2.2/matrix_alertbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4553 2024-04-20 22:36:04.000000 matrix_alertbot-0.2.2/matrix_alertbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-04-20 22:36:05.000000 matrix_alertbot-0.2.2/matrix_alertbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 22:36:04.000000 matrix_alertbot-0.2.2/matrix_alertbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-20 22:36:04.000000 matrix_alertbot-0.2.2/matrix_alertbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 22:36:04.000000 matrix_alertbot-0.2.2/matrix_alertbot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      695 2024-04-20 22:36:04.000000 matrix_alertbot-0.2.2/matrix_alertbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-20 22:36:04.000000 matrix_alertbot-0.2.2/matrix_alertbot.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-17 14:42:10.000000 matrix_alertbot-0.2.2/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.050902 matrix_alertbot-0.2.2/scripts-dev/
+-rwxrwxrwx   0 root         (0) root         (0)      360 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/scripts-dev/lint.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2024-04-20 22:36:05.078903 matrix_alertbot-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.058902 matrix_alertbot-0.2.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-20 22:35:40.000000 matrix_alertbot-0.2.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.022901 matrix_alertbot-0.2.2/tests/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.058902 matrix_alertbot-0.2.2/tests/resources/config/
+-rw-rw-rw-   0 root         (0) root         (0)     3502 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.2/tests/resources/config/config.full.yml
+-rw-rw-rw-   0 root         (0) root         (0)      959 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/tests/resources/config/config.minimal.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 22:36:05.062902 matrix_alertbot-0.2.2/tests/resources/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/tests/resources/templates/alert.html.j2
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/tests/resources/templates/alert.txt.j2
+-rw-rw-rw-   0 root         (0) root         (0)     6039 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.2/tests/test_alert.py
+-rw-rw-rw-   0 root         (0) root         (0)    35542 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.2/tests/test_alertmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)    52799 2024-04-20 15:56:58.000000 matrix_alertbot-0.2.2/tests/test_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     7908 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.2/tests/test_chat_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    27816 2024-04-18 10:06:38.000000 matrix_alertbot-0.2.2/tests/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)    15777 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.2/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11433 2024-04-18 08:19:14.000000 matrix_alertbot-0.2.2/tests/test_matrix.py
+-rw-rw-rw-   0 root         (0) root         (0)    22094 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.2/tests/test_webhook.py
```

### Comparing `matrix_alertbot-0.2.1/.gitlab-ci.yml` & `matrix_alertbot-0.2.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/CONTRIBUTING.md` & `matrix_alertbot-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/LICENSE` & `matrix_alertbot-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/PKG-INFO` & `matrix_alertbot-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrix-alertbot
-Version: 0.2.1
+Version: 0.2.2
 Summary: A matrix bot to manage alerts from Alertmanager
 Home-page: https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot
 Project-URL: Documentation, https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot/-/blob/master/README.md
 Project-URL: Source, https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot
 Project-URL: Tracker, https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot/-/issues
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `matrix_alertbot-0.2.1/README.md` & `matrix_alertbot-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/SETUP.md` & `matrix_alertbot-0.2.2/SETUP.md`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/config.sample.yaml` & `matrix_alertbot-0.2.2/config.sample.yaml`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/docker/Dockerfile` & `matrix_alertbot-0.2.2/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/docker/README.md` & `matrix_alertbot-0.2.2/docker/README.md`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/docker/build_and_install_libolm.sh` & `matrix_alertbot-0.2.2/docker/build_and_install_libolm.sh`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/docker/docker-compose.yml` & `matrix_alertbot-0.2.2/docker/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/docker/prometheus/prometheus.yml` & `matrix_alertbot-0.2.2/docker/prometheus/prometheus.yml`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot/alert.py` & `matrix_alertbot-0.2.2/matrix_alertbot/alert.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot/alertmanager.py` & `matrix_alertbot-0.2.2/matrix_alertbot/alertmanager.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot/callback.py` & `matrix_alertbot-0.2.2/matrix_alertbot/callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         user_id_patterns = []
         for user_id in self.config.user_ids:
             user, homeserver = user_id.split(":")
             username = user[1:]
             user_id_patterns.append(rf"@?{username}(:{homeserver})?")
 
         pattern = re.compile(
-            rf"(^|\s+)({'|'.join(user_id_patterns)})(\s+|$)",
+            rf"(^|\s+)({'|'.join(user_id_patterns)}):?(?=\s+|$)",
             re.IGNORECASE | re.MULTILINE,
         )
         if pattern.search(msg) is None:
             logger.debug(
                 f"Bot {self.matrix_client.user_id} | Room ID {room.room_id} | "
                 f"Event ID {event.event_id} | Sender {event.sender} | "
                 f"Cannot process message: Bot was not mentionned."
@@ -119,14 +119,19 @@
                 f"Bot {self.matrix_client.user_id} | Room ID {room.room_id} | "
                 f"Event ID {event.event_id} | Sender {event.sender} | "
                 f"Command received is in reply to event ID {reacted_to_event_id}"
             )
 
         # Remove the mention of the bot
         cmd = pattern.sub(" ", msg).strip()
+        logger.debug(
+            "Bot {self.matrix_client.user_id} | Room ID {room.room_id} | "
+            f"Event ID {event.event_id} | Sender {event.sender} | "
+            f"Processing command {cmd}"
+        )
         try:
             command = CommandFactory.create(
                 cmd,
                 self.matrix_client,
                 self.cache,
                 self.alertmanager_client,
                 self.config,
```

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot/chat_functions.py` & `matrix_alertbot-0.2.2/matrix_alertbot/chat_functions.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot/command.py` & `matrix_alertbot-0.2.2/matrix_alertbot/command.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot/config.py` & `matrix_alertbot-0.2.2/matrix_alertbot/config.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot/errors.py` & `matrix_alertbot-0.2.2/matrix_alertbot/errors.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot/main.py` & `matrix_alertbot-0.2.2/matrix_alertbot/main.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot/matrix.py` & `matrix_alertbot-0.2.2/matrix_alertbot/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import os
 import random
+from asyncio.exceptions import TimeoutError
 from typing import Dict, List, Optional, Tuple
 
 from aiohttp import ClientConnectionError, ServerDisconnectedError
 from diskcache import Cache
 from nio.client import AsyncClient, AsyncClientConfig
 from nio.events import (
     InviteMemberEvent,
```

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot/webhook.py` & `matrix_alertbot-0.2.2/matrix_alertbot/webhook.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot.egg-info/PKG-INFO` & `matrix_alertbot-0.2.2/matrix_alertbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrix-alertbot
-Version: 0.2.1
+Version: 0.2.2
 Summary: A matrix bot to manage alerts from Alertmanager
 Home-page: https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot
 Project-URL: Documentation, https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot/-/blob/master/README.md
 Project-URL: Source, https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot
 Project-URL: Tracker, https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot/-/issues
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot.egg-info/SOURCES.txt` & `matrix_alertbot-0.2.2/matrix_alertbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/matrix_alertbot.egg-info/requires.txt` & `matrix_alertbot-0.2.2/matrix_alertbot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/setup.cfg` & `matrix_alertbot-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/tests/resources/config/config.full.yml` & `matrix_alertbot-0.2.2/tests/resources/config/config.full.yml`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/tests/resources/config/config.minimal.yml` & `matrix_alertbot-0.2.2/tests/resources/config/config.minimal.yml`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/tests/test_alert.py` & `matrix_alertbot-0.2.2/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/tests/test_alertmanager.py` & `matrix_alertbot-0.2.2/tests/test_alertmanager.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/tests/test_callback.py` & `matrix_alertbot-0.2.2/tests/test_callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,14 +303,47 @@
             fake_message_event.sender,
             fake_message_event.event_id,
             "some alert event id",
             (),
         )
         fake_command.return_value.process.assert_called_once()
 
+    @patch.object(matrix_alertbot.command, "AckAlertCommand", autospec=True)
+    async def test_message_ack_in_reply_with_multi_mentions(
+        self, fake_command: Mock
+    ) -> None:
+        """Tests the callback for RoomMessageText with a mention of the bot"""
+        # Tests that the bot process messages in the room that contain a command
+        fake_message_event = Mock(spec=nio.RoomMessageText)
+        fake_message_event.event_id = "some event id"
+        fake_message_event.sender = "@some_other_fake_user:example.com"
+        fake_message_event.body = "@fake_user:example.com @fake_user:example.com: ack"
+        fake_message_event.source = {
+            "content": {
+                "m.relates_to": {"m.in_reply_to": {"event_id": "some alert event id"}}
+            }
+        }
+
+        # Pretend that we received a text message event
+        await self.callbacks.message(self.fake_room, fake_message_event)
+
+        # Check that the command was not executed
+        fake_command.assert_called_once_with(
+            self.fake_matrix_client,
+            self.fake_cache,
+            self.fake_alertmanager_client,
+            self.fake_config,
+            self.fake_room,
+            fake_message_event.sender,
+            fake_message_event.event_id,
+            "some alert event id",
+            (),
+        )
+        fake_command.return_value.process.assert_called_once()
+
     @patch.object(matrix_alertbot.callback, "UnackAlertCommand", autospec=True)
     async def test_message_unack_not_in_reply_with_mention(
         self, fake_command: Mock
     ) -> None:
         """Tests the callback for RoomMessageText with a mention of the bot"""
         # Tests that the bot process messages in the room that contain a command
         fake_message_event = Mock(spec=nio.RoomMessageText)
```

### Comparing `matrix_alertbot-0.2.1/tests/test_chat_functions.py` & `matrix_alertbot-0.2.2/tests/test_chat_functions.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/tests/test_command.py` & `matrix_alertbot-0.2.2/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/tests/test_config.py` & `matrix_alertbot-0.2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/tests/test_matrix.py` & `matrix_alertbot-0.2.2/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `matrix_alertbot-0.2.1/tests/test_webhook.py` & `matrix_alertbot-0.2.2/tests/test_webhook.py`

 * *Files identical despite different names*

