# Comparing `tmp/django-clite-0.2.9.tar.gz` & `tmp/django-clite-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-clite-0.2.9.tar", last modified: Wed Mar 18 16:51:23 2020, max compression
+gzip compressed data, was "dist/django-clite-0.3.0.tar", last modified: Tue Mar 24 03:05:00 2020, max compression
```

## Comparing `django-clite-0.2.9.tar` & `django-clite-0.3.0.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/
--rw-rw-rw-   0 root         (0) root         (0)     1407 2020-03-18 16:51:16.000000 django-clite-0.2.9/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1516 2020-03-18 16:51:16.000000 django-clite-0.2.9/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      154 2020-03-18 16:51:16.000000 django-clite-0.2.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3430 2020-03-18 16:51:23.000000 django-clite-0.2.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1771 2020-03-18 16:51:16.000000 django-clite-0.2.9/README.md
--rwxrwxrwx   0 root         (0) root         (0)     1965 2020-03-18 16:51:16.000000 django-clite-0.2.9/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/
--rw-rw-rw-   0 root         (0) root         (0)       89 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/
--rw-rw-rw-   0 root         (0) root         (0)      182 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/creator/
--rw-rw-rw-   0 root         (0) root         (0)       92 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/creator/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       50 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11291 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/helpers/creator.py
--rw-rw-rw-   0 root         (0) root         (0)     6533 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/creator/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1564 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/Pipfile.tpl
--rw-rw-rw-   0 root         (0) root         (0)     1880 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/README.tpl
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/admin-init.tpl
--rw-rw-rw-   0 root         (0) root         (0)       97 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/app_json.tpl
--rw-rw-rw-   0 root         (0) root         (0)      178 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/apps.tpl
--rw-rw-rw-   0 root         (0) root         (0)      284 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/bitbucket-pipelines.tpl
--rw-rw-rw-   0 root         (0) root         (0)     2308 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/ckeditor.tpl
--rw-rw-rw-   0 root         (0) root         (0)     1189 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/docker-compose.tpl
--rw-rw-rw-   0 root         (0) root         (0)      207 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/docker-entrypoint.tpl
--rw-rw-rw-   0 root         (0) root         (0)      769 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/dockerfile.tpl
--rw-rw-rw-   0 root         (0) root         (0)       63 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/dokku_checks.tpl
--rw-rw-rw-   0 root         (0) root         (0)       13 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/dokku_scale.tpl
--rw-rw-rw-   0 root         (0) root         (0)     1164 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/env.tpl
--rw-rw-rw-   0 root         (0) root         (0)     1372 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/gitignore.tpl
--rw-rw-rw-   0 root         (0) root         (0)       32 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/procfile.tpl
--rw-rw-rw-   0 root         (0) root         (0)     2470 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/rest-framework.tpl
--rw-rw-rw-   0 root         (0) root         (0)      434 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/router.tpl
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/seeds.tpl
--rw-rw-rw-   0 root         (0) root         (0)     8480 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/settings.tpl
--rw-rw-rw-   0 root         (0) root         (0)      487 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/storage.tpl
--rw-rw-rw-   0 root         (0) root         (0)      541 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/travis-yml.tpl
--rw-rw-rw-   0 root         (0) root         (0)      178 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/creator/templates/urls.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/destroyer/
--rw-rw-rw-   0 root         (0) root         (0)      299 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/destroyer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/destroyer/helpers/
--rw-rw-rw-   0 root         (0) root         (0)      666 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/destroyer/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7283 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/destroyer/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/generator/
--rw-rw-rw-   0 root         (0) root         (0)      327 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/
--rw-rw-rw-   0 root         (0) root         (0)      352 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1729 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/fixture.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/form.py
--rw-rw-rw-   0 root         (0) root         (0)     1942 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3080 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/template.py
--rw-rw-rw-   0 root         (0) root         (0)     1769 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/test.py
--rw-rw-rw-   0 root         (0) root         (0)     2936 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/view.py
--rw-rw-rw-   0 root         (0) root         (0)     1481 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/helpers/viewset.py
--rw-rw-rw-   0 root         (0) root         (0)    12815 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/generator/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/admin-import.tpl
--rw-rw-rw-   0 root         (0) root         (0)       54 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/admin-inline-import.tpl
--rw-rw-rw-   0 root         (0) root         (0)      174 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/admin-inline.tpl
--rw-rw-rw-   0 root         (0) root         (0)      464 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/admin-user.tpl
--rw-rw-rw-   0 root         (0) root         (0)      845 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/admin.tpl
--rw-rw-rw-   0 root         (0) root         (0)      317 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/fixture.tpl
--rw-rw-rw-   0 root         (0) root         (0)       52 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/form-import.tpl
--rw-rw-rw-   0 root         (0) root         (0)      378 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/form-user.tpl
--rw-rw-rw-   0 root         (0) root         (0)      204 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/form.tpl
--rw-rw-rw-   0 root         (0) root         (0)      342 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/identifier.tpl
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/import.tpl
--rw-rw-rw-   0 root         (0) root         (0)       56 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/manager-import.tpl
--rw-rw-rw-   0 root         (0) root         (0)      725 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/manager.tpl
--rw-rw-rw-   0 root         (0) root         (0)       86 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/model-admin.tpl
--rw-rw-rw-   0 root         (0) root         (0)      138 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/model-field.tpl
--rw-rw-rw-   0 root         (0) root         (0)       48 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/model-import.tpl
--rw-rw-rw-   0 root         (0) root         (0)      525 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/model-test.tpl
--rw-rw-rw-   0 root         (0) root         (0)     1937 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/model-user.tpl
--rw-rw-rw-   0 root         (0) root         (0)     2645 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/model.tpl
--rw-rw-rw-   0 root         (0) root         (0)       58 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/serializer-import.tpl
--rw-rw-rw-   0 root         (0) root         (0)     2700 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/serializer-test.tpl
--rw-rw-rw-   0 root         (0) root         (0)      371 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/serializer-user.tpl
--rw-rw-rw-   0 root         (0) root         (0)      567 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/serializer.tpl
--rw-rw-rw-   0 root         (0) root         (0)      302 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/sql-migration.tpl
--rw-rw-rw-   0 root         (0) root         (0)      442 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/sql-model.tpl
--rw-rw-rw-   0 root         (0) root         (0)      299 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/template.tpl
--rw-rw-rw-   0 root         (0) root         (0)       56 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/test-import.tpl
--rw-rw-rw-   0 root         (0) root         (0)      106 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/view-class-import.tpl
--rw-rw-rw-   0 root         (0) root         (0)      750 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/view-class.tpl
--rw-rw-rw-   0 root         (0) root         (0)       41 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/view-function-import.tpl
--rw-rw-rw-   0 root         (0) root         (0)      671 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/view-function.tpl
--rw-rw-rw-   0 root         (0) root         (0)       55 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/viewset-import.tpl
--rw-rw-rw-   0 root         (0) root         (0)      529 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/generator/templates/viewset.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/inspector/
--rw-rw-rw-   0 root         (0) root         (0)       47 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/inspector/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/inspector/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       66 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/inspector/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2754 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/inspector/helpers/inspector.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/inspector/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/runner/
--rw-rw-rw-   0 root         (0) root         (0)      258 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/runner/helpers/
--rw-rw-rw-   0 root         (0) root         (0)      264 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/helpers/build.py
--rw-rw-rw-   0 root         (0) root         (0)     2186 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/helpers/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     2996 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/helpers/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/helpers/fixture.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/helpers/migration.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/helpers/runner.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/helpers/server.py
--rw-rw-rw-   0 root         (0) root         (0)     7925 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/commands/runner/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1189 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/templates/docker-compose.tpl
--rw-rw-rw-   0 root         (0) root         (0)      189 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/templates/docker-entrypoint.tpl
--rw-rw-rw-   0 root         (0) root         (0)      769 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/commands/runner/templates/dockerfile.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite/helpers/
--rw-rw-rw-   0 root         (0) root         (0)      343 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12357 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/helpers/field_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/helpers/finders.py
--rw-rw-rw-   0 root         (0) root         (0)    14510 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/helpers/fs.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/helpers/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/helpers/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2020-03-18 16:51:16.000000 django-clite-0.2.9/django_clite/helpers/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3430 2020-03-18 16:51:22.000000 django-clite-0.2.9/django_clite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6322 2020-03-18 16:51:23.000000 django-clite-0.2.9/django_clite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-03-18 16:51:22.000000 django-clite-0.2.9/django_clite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2020-03-18 16:51:22.000000 django-clite-0.2.9/django_clite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-03-18 16:51:22.000000 django-clite-0.2.9/django_clite.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       94 2020-03-18 16:51:22.000000 django-clite-0.2.9/django_clite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2020-03-18 16:51:22.000000 django-clite-0.2.9/django_clite.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      371 2020-03-18 16:51:23.000000 django-clite-0.2.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1900 2020-03-18 16:51:16.000000 django-clite-0.2.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)      138 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/tests/creator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/creator/test_new_app.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/creator/test_new_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/tests/destroyer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/destroyer/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/destroyer/test_form.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/destroyer/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/destroyer/test_resource.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/destroyer/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/destroyer/test_template.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/destroyer/test_view.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/destroyer/test_viewset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/tests/generator/
--rw-rw-rw-   0 root         (0) root         (0)      267 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/generator/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/generator/test_form.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/generator/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)      308 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/generator/test_resource.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/generator/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/generator/test_template.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/generator/test_test.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/generator/test_view.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/generator/test_viewset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-18 16:51:23.000000 django-clite-0.2.9/tests/runner/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/runner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2020-03-18 16:51:16.000000 django-clite-0.2.9/tests/runner/test_create_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.227869 django-clite-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (115)     1407 2020-03-24 03:04:48.000000 django-clite-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (115)     1516 2020-03-24 03:04:48.000000 django-clite-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      154 2020-03-24 03:04:48.000000 django-clite-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (115)     3367 2020-03-24 03:05:00.227869 django-clite-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     1717 2020-03-24 03:04:48.000000 django-clite-0.3.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (115)     1965 2020-03-24 03:04:48.000000 django-clite-0.3.0/app.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.215869 django-clite-0.3.0/django_clite/
+-rw-r--r--   0 runner    (1001) docker     (115)       89 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.215869 django-clite-0.3.0/django_clite/commands/
+-rw-r--r--   0 runner    (1001) docker     (115)      182 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.215869 django-clite-0.3.0/django_clite/commands/creator/
+-rw-r--r--   0 runner    (1001) docker     (115)       92 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.215869 django-clite-0.3.0/django_clite/commands/creator/helpers/
+-rw-r--r--   0 runner    (1001) docker     (115)       50 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11291 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/helpers/creator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6529 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/main.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.219869 django-clite-0.3.0/django_clite/commands/creator/templates/
+-rw-r--r--   0 runner    (1001) docker     (115)     1564 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/Pipfile.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)     1880 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/README.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      248 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/admin-init.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       97 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/app_json.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      178 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/apps.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      284 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/bitbucket-pipelines.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)     2308 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/ckeditor.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)     1188 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/docker-compose.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      207 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/docker-entrypoint.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      769 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/dockerfile.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       63 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/dokku_checks.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       13 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/dokku_scale.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)     1164 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/env.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)     1372 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/gitignore.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       32 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/procfile.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)     2470 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/rest-framework.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      434 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/router.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/seeds.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)     8480 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/settings.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      487 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/storage.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      541 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/travis-yml.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      178 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/creator/templates/urls.tpl
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.219869 django-clite-0.3.0/django_clite/commands/destroyer/
+-rw-r--r--   0 runner    (1001) docker     (115)      299 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/destroyer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.219869 django-clite-0.3.0/django_clite/commands/destroyer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (115)      666 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/destroyer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7283 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/destroyer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.219869 django-clite-0.3.0/django_clite/commands/generator/
+-rw-r--r--   0 runner    (1001) docker     (115)      327 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.219869 django-clite-0.3.0/django_clite/commands/generator/helpers/
+-rw-r--r--   0 runner    (1001) docker     (115)      352 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2045 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/helpers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1729 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/helpers/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1654 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/helpers/form.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1942 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/helpers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3080 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/helpers/model.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1620 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/helpers/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1274 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/helpers/template.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1769 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/helpers/test.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2936 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/helpers/view.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1521 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/helpers/viewset.py
+-rw-r--r--   0 runner    (1001) docker     (115)    12815 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/main.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.223869 django-clite-0.3.0/django_clite/commands/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)       53 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/admin-import.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       54 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/admin-inline-import.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      174 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/admin-inline.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      464 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/admin-user.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      845 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/admin.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      317 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/fixture.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       52 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/form-import.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      378 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/form-user.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      204 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/form.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      342 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/identifier.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/import.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       56 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/manager-import.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      725 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/manager.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       86 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/model-admin.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      138 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/model-field.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       48 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/model-import.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      525 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/model-test.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)     1937 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/model-user.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)     2645 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/model.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       58 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/serializer-import.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)     2700 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/serializer-test.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      371 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/serializer-user.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      567 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/serializer.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      302 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/sql-migration.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      442 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/sql-model.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      299 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/template.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       56 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/test-import.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      106 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/view-class-import.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      750 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/view-class.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       41 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/view-function-import.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      671 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/view-function.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)       55 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/viewset-import.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      529 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/generator/templates/viewset.tpl
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.223869 django-clite-0.3.0/django_clite/commands/inspector/
+-rw-r--r--   0 runner    (1001) docker     (115)       47 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/inspector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.223869 django-clite-0.3.0/django_clite/commands/inspector/helpers/
+-rw-r--r--   0 runner    (1001) docker     (115)       66 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/inspector/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3304 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/inspector/helpers/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1303 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/inspector/main.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.223869 django-clite-0.3.0/django_clite/commands/runner/
+-rw-r--r--   0 runner    (1001) docker     (115)      258 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.227869 django-clite-0.3.0/django_clite/commands/runner/helpers/
+-rw-r--r--   0 runner    (1001) docker     (115)      264 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      897 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/helpers/build.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2186 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/helpers/docker.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2996 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (115)      345 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/helpers/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1641 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/helpers/migration.py
+-rw-r--r--   0 runner    (1001) docker     (115)      198 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/helpers/runner.py
+-rw-r--r--   0 runner    (1001) docker     (115)      632 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/helpers/server.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7925 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/main.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.227869 django-clite-0.3.0/django_clite/commands/runner/templates/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1188 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/templates/docker-compose.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      189 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/templates/docker-entrypoint.tpl
+-rw-r--r--   0 runner    (1001) docker     (115)      769 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/commands/runner/templates/dockerfile.tpl
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.227869 django-clite-0.3.0/django_clite/helpers/
+-rw-r--r--   0 runner    (1001) docker     (115)      343 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    12357 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/helpers/field_parser.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5033 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/helpers/finders.py
+-rw-r--r--   0 runner    (1001) docker     (115)    14510 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/helpers/fs.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2279 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/helpers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (115)      262 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/helpers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (115)      399 2020-03-24 03:04:48.000000 django-clite-0.3.0/django_clite/helpers/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.215869 django-clite-0.3.0/django_clite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     3367 2020-03-24 03:04:59.000000 django-clite-0.3.0/django_clite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     6322 2020-03-24 03:05:00.000000 django-clite-0.3.0/django_clite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-24 03:04:59.000000 django-clite-0.3.0/django_clite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       71 2020-03-24 03:04:59.000000 django-clite-0.3.0/django_clite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-24 03:04:59.000000 django-clite-0.3.0/django_clite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (115)       94 2020-03-24 03:04:59.000000 django-clite-0.3.0/django_clite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       13 2020-03-24 03:04:59.000000 django-clite-0.3.0/django_clite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      371 2020-03-24 03:05:00.231869 django-clite-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     1891 2020-03-24 03:04:48.000000 django-clite-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.227869 django-clite-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)      138 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.227869 django-clite-0.3.0/tests/creator/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/creator/test_new_app.py
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/creator/test_new_project.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.227869 django-clite-0.3.0/tests/destroyer/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/destroyer/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/destroyer/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/destroyer/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/destroyer/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/destroyer/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/destroyer/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/destroyer/test_view.py
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/destroyer/test_viewset.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.227869 django-clite-0.3.0/tests/generator/
+-rw-r--r--   0 runner    (1001) docker     (115)      267 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/generator/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (115)      295 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/generator/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (115)      299 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/generator/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (115)      308 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/generator/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (115)      319 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/generator/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (115)      311 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/generator/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (115)      295 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/generator/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (115)      295 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/generator/test_view.py
+-rw-r--r--   0 runner    (1001) docker     (115)      307 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/generator/test_viewset.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-24 03:05:00.227869 django-clite-0.3.0/tests/runner/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      230 2020-03-24 03:04:48.000000 django-clite-0.3.0/tests/runner/test_create_settings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-clite-0.2.9/.gitignore` & `django-clite-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/LICENSE.txt` & `django-clite-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/PKG-INFO` & `django-clite-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: django-clite
-Version: 0.2.9
+Version: 0.3.0
 Summary: CLI for managing Django projects
-Home-page: https://bitbucket.org/oleoneto/django-clite
+Home-page: https://github.com/oleoneto/django-clite
 Author: Leo Neto
 Author-email: leo@ekletik.com
 License: BSD
-Project-URL: Documentation, https://bitbucket.org/oleoneto/django-clite/
-Project-URL: Source Code, https://bitbucket.org/oleoneto/django-clite/
+Project-URL: Documentation, https://github.com/oleoneto/django-clite/
+Project-URL: Source Code, https://github.com/oleoneto/django-clite/
 Description: # django-clite
         
         A CLI tool that handles creating and managing Django projects
         
-        ![PyPI - License](https://img.shields.io/pypi/l/django-clite?style=flat-square)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-clite?style=flat-square)
-        ![PyPI](https://img.shields.io/pypi/v/django-clite?style=flat-square)
-        ![Bitbucket Pipelines](https://img.shields.io/bitbucket/pipelines/oleoneto/django-clite/development?style=flat-square)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/django-clite?style=flat-square)
+        ![publish](https://github.com/oleoneto/django-clite/workflows/publish/badge.svg?branch=master)
+        ![PyPI - Package](https://img.shields.io/pypi/v/django-clite)
+        ![PyPI - Python](https://img.shields.io/pypi/pyversions/django-clite)
+        ![PyPI - License](https://img.shields.io/pypi/l/django-clite)
+        ![PyPI - Downloads](https://img.shields.io/pypi/dm/django-clite)
         
         
         - [Introduction](#django-clite)
         - [Interactive Docs](#interactive-docs)
         - [Dependencies](#dependencies)
         - [Installation](#installation)
         - [To Do](#to-do)
@@ -52,15 +52,15 @@
         ```
         D
         django-clite
         djc
         ```
         
         ## To Do
-        [Check out our open issues](/issues).
+        [Check out our open issues](https://github.com/oleoneto/django-clite/issues).
         
         ## Pull requests
         Found a bug? See a typo? Have an idea for new command?
         Feel free to submit a pull request with your contributions. They are much welcome and appreciated.
         
         ## LICENSE
         **django-clite** is [BSD Licensed](LICENSE.txt).
```

### Comparing `django-clite-0.2.9/README.md` & `django-clite-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # django-clite
 
 A CLI tool that handles creating and managing Django projects
 
-![PyPI - License](https://img.shields.io/pypi/l/django-clite?style=flat-square)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-clite?style=flat-square)
-![PyPI](https://img.shields.io/pypi/v/django-clite?style=flat-square)
-![Bitbucket Pipelines](https://img.shields.io/bitbucket/pipelines/oleoneto/django-clite/development?style=flat-square)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/django-clite?style=flat-square)
+![publish](https://github.com/oleoneto/django-clite/workflows/publish/badge.svg?branch=master)
+![PyPI - Package](https://img.shields.io/pypi/v/django-clite)
+![PyPI - Python](https://img.shields.io/pypi/pyversions/django-clite)
+![PyPI - License](https://img.shields.io/pypi/l/django-clite)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/django-clite)
 
 
 - [Introduction](#django-clite)
 - [Interactive Docs](#interactive-docs)
 - [Dependencies](#dependencies)
 - [Installation](#installation)
 - [To Do](#to-do)
@@ -42,15 +42,15 @@
 ```
 D
 django-clite
 djc
 ```
 
 ## To Do
-[Check out our open issues](/issues).
+[Check out our open issues](https://github.com/oleoneto/django-clite/issues).
 
 ## Pull requests
 Found a bug? See a typo? Have an idea for new command?
 Feel free to submit a pull request with your contributions. They are much welcome and appreciated.
 
 ## LICENSE
 **django-clite** is [BSD Licensed](LICENSE.txt).
```

### Comparing `django-clite-0.2.9/app.py` & `django-clite-0.3.0/app.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/creator/helpers/creator.py` & `django-clite-0.3.0/django_clite/commands/creator/helpers/creator.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/creator/main.py` & `django-clite-0.3.0/django_clite/commands/creator/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import inquirer
 from django_clite.helpers import get_project_name
 from django_clite.helpers import find_project_files
 from django_clite.helpers.logger import *
 from .helpers import *
 from django_clite.commands.inspector.main import InspectorHelper
-from django_clite.commands.inspector.main import apps as inspect_apps
+from django_clite.commands.inspector.main import inspect
 
 
 def wrong_place_warning(ctx):
     if (ctx.obj['path'] and ctx.obj['project_name']) is None:
         log_error(DEFAULT_MANAGEMENT_ERROR)
         log_standard('')
         log_standard(DEFAULT_MANAGEMENT_ERROR_HELP)
@@ -179,11 +179,11 @@
         dry=ctx.obj['dry'],
         default=ctx.obj['default'],
         verbose=ctx.obj['verbose']
     )
 
     if not ignore_apps:
         ctx.obj['helper'] = InspectorHelper(cwd=ctx.obj['management'])
-        apps = ctx.invoke(inspect_apps, no_stdout=True)
+        apps = ctx.invoke(inspect, scope='apps', no_stdout=True)
         h.create_settings(project=ctx.obj['project_name'], apps=apps)
     else:
         h.create_settings(project=ctx.obj['project_name'])
```

### Comparing `django-clite-0.2.9/django_clite/commands/creator/templates/Pipfile.tpl` & `django-clite-0.3.0/django_clite/commands/creator/templates/Pipfile.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/creator/templates/README.tpl` & `django-clite-0.3.0/django_clite/commands/creator/templates/README.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/creator/templates/ckeditor.tpl` & `django-clite-0.3.0/django_clite/commands/creator/templates/ckeditor.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/creator/templates/docker-compose.tpl` & `django-clite-0.3.0/django_clite/commands/creator/templates/docker-compose.tpl`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 version: '3'
 
 services:
   web:
     container_name: "{{ project }}_web"
     labels:
-        com.{{ project }}.web.description = "{{ project }}: Web Application"
+        com.{{ project }}.web.description: "{{ project }}: Web Application"
     build:
         context: .
     volumes:
         - .:/app
     env_file:
         - .env
     environment:
```

### Comparing `django-clite-0.2.9/django_clite/commands/creator/templates/dockerfile.tpl` & `django-clite-0.3.0/django_clite/commands/creator/templates/dockerfile.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/creator/templates/env.tpl` & `django-clite-0.3.0/django_clite/commands/creator/templates/env.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/creator/templates/gitignore.tpl` & `django-clite-0.3.0/django_clite/commands/creator/templates/gitignore.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/creator/templates/rest-framework.tpl` & `django-clite-0.3.0/django_clite/commands/creator/templates/rest-framework.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/creator/templates/settings.tpl` & `django-clite-0.3.0/django_clite/commands/creator/templates/settings.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/creator/templates/travis-yml.tpl` & `django-clite-0.3.0/django_clite/commands/creator/templates/travis-yml.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/destroyer/helpers/__init__.py` & `django-clite-0.3.0/django_clite/commands/destroyer/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/destroyer/main.py` & `django-clite-0.3.0/django_clite/commands/destroyer/main.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/helpers/admin.py` & `django-clite-0.3.0/django_clite/commands/generator/helpers/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import inflection
 from django_clite.helpers.logger import *
+from django_clite.helpers import sanitized_string
 from django_clite.helpers import FSHelper
 
 BASE_DIR = os.path.dirname(os.path.abspath(__file__)).rsplit('/', 1)[0]
 
 TEMPLATE_DIR = os.path.join(BASE_DIR, 'templates')
 
 TEMPLATES = [f for f in os.listdir(TEMPLATE_DIR) if f.endswith('tpl')]
 
 
 class AdminHelper(FSHelper):
 
     def create(self, model, fields=None, **kwargs):
+        model = sanitized_string(model)
 
         scope = "Admin"
         template = 'admin.tpl' \
             if not kwargs.get('template') \
             else kwargs.get('template')
         template_import = 'admin-import.tpl' \
             if not kwargs.get('template_import') \
```

### Comparing `django-clite-0.2.9/django_clite/commands/generator/helpers/fixture.py` & `django-clite-0.3.0/django_clite/commands/generator/helpers/fixture.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/helpers/form.py` & `django-clite-0.3.0/django_clite/commands/generator/helpers/form.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 TEMPLATES = [f for f in os.listdir(TEMPLATE_DIR) if f.endswith('tpl')]
 
 
 class FormHelper(FSHelper):
 
     def create(self, model, **kwargs):
+        model = sanitized_string(model)
 
         template = 'form.tpl' \
             if not kwargs.get('template') \
             else kwargs.get('template')
         template_import = 'form-import.tpl' \
             if not kwargs.get('template_import') \
             else kwargs.get('template_import')
```

### Comparing `django-clite-0.2.9/django_clite/commands/generator/helpers/manager.py` & `django-clite-0.3.0/django_clite/commands/generator/helpers/manager.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/helpers/model.py` & `django-clite-0.3.0/django_clite/commands/generator/helpers/model.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/helpers/serializer.py` & `django-clite-0.3.0/django_clite/commands/generator/helpers/viewset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 import os
 import inflection
 from django_clite.helpers.logger import *
+from django_clite.helpers import sanitized_string
+from django_clite.helpers import rendered_file_template
 from django_clite.helpers import FSHelper
 
 BASE_DIR = os.path.dirname(os.path.abspath(__file__)).rsplit('/', 1)[0]
 
 TEMPLATE_DIR = os.path.join(BASE_DIR, 'templates')
 
 TEMPLATES = [f for f in os.listdir(TEMPLATE_DIR) if f.endswith('tpl')]
 
 
-class SerializerHelper(FSHelper):
+class ViewSetHelper(FSHelper):
 
-    def create(self, model, **kwargs):
+    def create(self, model, read_only=False):
+        model = sanitized_string(model)
 
-        template = 'serializer.tpl' \
-            if not kwargs.get('template') \
-            else kwargs.get('template')
-        template_import = 'serializer-import.tpl' \
-            if not kwargs.get('template_import') \
-            else kwargs.get('template_import')
+        template = 'viewset.tpl'
+        template_import = 'viewset-import.tpl'
+
+        # TODO: Ensure serializer already exists
 
         self.default_create(
             model,
             templates_directory=TEMPLATE_DIR,
             template=template,
             template_import=template_import,
-            scope='Serializer',
-            context={'model': model}
+            scope='ViewSet',
+            context={
+                'model': model,
+                'read_only': read_only,
+                'route': inflection.pluralize(model),
+            }
         )
 
     def delete(self, model):
         model = self.check_noun(model)
         classname = inflection.camelize(model)
 
         filename = f"{model}.py"
-        template_import = 'serializer-import.tpl'
+        template_import = 'viewset-import.tpl'
 
         if self.default_destroy_file(
             model=model,
             templates_directory=TEMPLATE_DIR,
             template_import=template_import
         ):
 
-            resource = f"{classname}Serializer"
+            resource = f"{classname}ViewSet"
             log_success(DEFAULT_DELETE_MESSAGE.format(filename, resource))
-
-    def create_auth_user(self):
-        self.create(
-            model='User',
-            template='serializer-user.tpl'
-        )
```

### Comparing `django-clite-0.2.9/django_clite/commands/generator/helpers/template.py` & `django-clite-0.3.0/django_clite/commands/generator/helpers/template.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/helpers/test.py` & `django-clite-0.3.0/django_clite/commands/generator/helpers/test.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/helpers/view.py` & `django-clite-0.3.0/django_clite/commands/generator/helpers/view.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/helpers/viewset.py` & `django-clite-0.3.0/django_clite/commands/generator/helpers/serializer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 import os
 import inflection
 from django_clite.helpers.logger import *
 from django_clite.helpers import sanitized_string
-from django_clite.helpers import rendered_file_template
 from django_clite.helpers import FSHelper
 
 BASE_DIR = os.path.dirname(os.path.abspath(__file__)).rsplit('/', 1)[0]
 
 TEMPLATE_DIR = os.path.join(BASE_DIR, 'templates')
 
 TEMPLATES = [f for f in os.listdir(TEMPLATE_DIR) if f.endswith('tpl')]
 
 
-class ViewSetHelper(FSHelper):
+class SerializerHelper(FSHelper):
 
-    def create(self, model, read_only=False):
+    def create(self, model, **kwargs):
+        model = sanitized_string(model)
 
-        template = 'viewset.tpl'
-        template_import = 'viewset-import.tpl'
-
-        # TODO: Ensure serializer already exists
+        template = 'serializer.tpl' \
+            if not kwargs.get('template') \
+            else kwargs.get('template')
+        template_import = 'serializer-import.tpl' \
+            if not kwargs.get('template_import') \
+            else kwargs.get('template_import')
 
         self.default_create(
             model,
             templates_directory=TEMPLATE_DIR,
             template=template,
             template_import=template_import,
-            scope='ViewSet',
-            context={
-                'model': model,
-                'read_only': read_only,
-                'route': inflection.pluralize(model),
-            }
+            scope='Serializer',
+            context={'model': model}
         )
 
     def delete(self, model):
         model = self.check_noun(model)
         classname = inflection.camelize(model)
 
         filename = f"{model}.py"
-        template_import = 'viewset-import.tpl'
+        template_import = 'serializer-import.tpl'
 
         if self.default_destroy_file(
             model=model,
             templates_directory=TEMPLATE_DIR,
             template_import=template_import
         ):
 
-            resource = f"{classname}ViewSet"
+            resource = f"{classname}Serializer"
             log_success(DEFAULT_DELETE_MESSAGE.format(filename, resource))
+
+    def create_auth_user(self):
+        self.create(
+            model='User',
+            template='serializer-user.tpl'
+        )
```

### Comparing `django-clite-0.2.9/django_clite/commands/generator/main.py` & `django-clite-0.3.0/django_clite/commands/generator/main.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/templates/admin.tpl` & `django-clite-0.3.0/django_clite/commands/generator/templates/admin.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/templates/manager.tpl` & `django-clite-0.3.0/django_clite/commands/generator/templates/manager.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/templates/model-test.tpl` & `django-clite-0.3.0/django_clite/commands/generator/templates/model-test.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/templates/model-user.tpl` & `django-clite-0.3.0/django_clite/commands/generator/templates/model-user.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/templates/model.tpl` & `django-clite-0.3.0/django_clite/commands/generator/templates/model.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/templates/serializer-test.tpl` & `django-clite-0.3.0/django_clite/commands/generator/templates/serializer-test.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/templates/serializer.tpl` & `django-clite-0.3.0/django_clite/commands/generator/templates/serializer.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/templates/view-class.tpl` & `django-clite-0.3.0/django_clite/commands/generator/templates/view-class.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/templates/view-function.tpl` & `django-clite-0.3.0/django_clite/commands/generator/templates/view-function.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/generator/templates/viewset.tpl` & `django-clite-0.3.0/django_clite/commands/generator/templates/viewset.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/inspector/helpers/inspector.py` & `django-clite-0.3.0/django_clite/commands/inspector/helpers/inspector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
+import fileinput
 from django_clite.helpers import FSHelper
 from django_clite.helpers.logger import log_info, log_standard, log_verbose
+import re
 
 
 class InspectorHelper(FSHelper):
 
     def get_apps(self, show_paths=False, no_stdout=False):
         """
         Traverse file system in search for AppConfig files.
@@ -23,15 +25,15 @@
 
             if not no_stdout:
                 log_standard(f'{app}', bold=True)
                 
                 if show_paths:
                     log_standard(f'{path}\n')
 
-        return current_apps
+        return sorted(current_apps)
 
     def get_app_paths(self):
         """
         Traverse file system in search for apps and their paths.
 
         :return: list of app paths
         """
@@ -42,58 +44,64 @@
             if 'apps.py' in files
         ])
 
         [log_info(path) for path in current_paths]
 
         return current_paths
 
-    def get_models(self, show_paths=False, no_stdout=False):
+    def get_classes(self, scope, show_paths=False, no_stdout=False):
         """
         Retrieve models under each app's models package.
 
         :return:
         """
 
         models = []
 
         excluded_dirs = [
-            'signals', 'tests', 'helpers',
-            'validators', 'managers', '__pycache__'
+            'signals', 'tests', 'helpers', 'abstract', 'abstracts',
+            'validators', 'managers', 'permissions', 'inlines', '__pycache__'
         ]
 
         excluded_files = [
             "__init__.py"
         ]
 
         current_apps = {
             c.rsplit('/', 1)[-1]: c
             for c, _, files in os.walk(self.cwd) if 'apps.py' in files
         }
 
+        # One day... one day I'll refactor this
         for app, path in sorted(current_apps.items()):
 
-            models_directory = path + "/models"
+            if scope == 'managers':
+                scope = 'models/managers'
 
-            for root, dirs, files in os.walk(models_directory):
+            resource_directory = f'{path}/{scope}'
+
+            for root, dirs, files in os.walk(resource_directory):
                 dirs[:] = [d for d in dirs if d not in excluded_dirs]
                 files[:] = [f for f in files if f not in excluded_files]
 
                 if files and not no_stdout:
+                    log_standard('')
                     log_standard(app, bold=True)
 
                     if show_paths:
                         if not no_stdout:
-                            log_standard(f'  {path}', bold=True)
-
-                    for f in sorted(files):
-                        models.append({app: f})
-                        if not no_stdout:
-                            log_verbose(
-                                header=None,
-                                message='    {0:20}'.format(f),
-                            )
-                    log_standard('')
+                            log_standard(f'  {resource_directory}', bold=True)
 
+                for file in sorted(files):
+                    models.append({app: file})
+                    model_file = resource_directory + f'/{file}'
+
+                    for line in fileinput.input(model_file):
+                        if re.match(r'^class ', line):  # in line and "Meta:" not in line:
+                            model_name = line.split('class ')[-1].split('(')[0]
+                            if not no_stdout:
+                                log_verbose(
+                                    header=None,
+                                    message='    {0:20}'.format(model_name),
+                                )
+                    fileinput.close()
         return models
-
-    def parse_model_attributes(self):
-        pass
```

### Comparing `django-clite-0.2.9/django_clite/commands/runner/helpers/build.py` & `django-clite-0.3.0/django_clite/commands/runner/helpers/build.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/runner/helpers/docker.py` & `django-clite-0.3.0/django_clite/commands/runner/helpers/docker.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/runner/helpers/environment.py` & `django-clite-0.3.0/django_clite/commands/runner/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/runner/helpers/migration.py` & `django-clite-0.3.0/django_clite/commands/runner/helpers/migration.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/runner/helpers/server.py` & `django-clite-0.3.0/django_clite/commands/runner/helpers/server.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/runner/main.py` & `django-clite-0.3.0/django_clite/commands/runner/main.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/commands/runner/templates/docker-compose.tpl` & `django-clite-0.3.0/django_clite/commands/runner/templates/docker-compose.tpl`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 version: '3'
 
 services:
   web:
     container_name: "{{ project }}_web"
     labels:
-        com.{{ project }}.web.description = "{{ project }}: Web Application"
+        com.{{ project }}.web.description: "{{ project }}: Web Application"
     build:
         context: .
     volumes:
         - .:/app
     env_file:
         - .env
     environment:
```

### Comparing `django-clite-0.2.9/django_clite/commands/runner/templates/dockerfile.tpl` & `django-clite-0.3.0/django_clite/commands/runner/templates/dockerfile.tpl`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/helpers/field_parser.py` & `django-clite-0.3.0/django_clite/helpers/field_parser.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/helpers/finders.py` & `django-clite-0.3.0/django_clite/helpers/finders.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/helpers/fs.py` & `django-clite-0.3.0/django_clite/helpers/fs.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite/helpers/logger.py` & `django-clite-0.3.0/django_clite/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/django_clite.egg-info/PKG-INFO` & `django-clite-0.3.0/django_clite.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: django-clite
-Version: 0.2.9
+Version: 0.3.0
 Summary: CLI for managing Django projects
-Home-page: https://bitbucket.org/oleoneto/django-clite
+Home-page: https://github.com/oleoneto/django-clite
 Author: Leo Neto
 Author-email: leo@ekletik.com
 License: BSD
-Project-URL: Documentation, https://bitbucket.org/oleoneto/django-clite/
-Project-URL: Source Code, https://bitbucket.org/oleoneto/django-clite/
+Project-URL: Documentation, https://github.com/oleoneto/django-clite/
+Project-URL: Source Code, https://github.com/oleoneto/django-clite/
 Description: # django-clite
         
         A CLI tool that handles creating and managing Django projects
         
-        ![PyPI - License](https://img.shields.io/pypi/l/django-clite?style=flat-square)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-clite?style=flat-square)
-        ![PyPI](https://img.shields.io/pypi/v/django-clite?style=flat-square)
-        ![Bitbucket Pipelines](https://img.shields.io/bitbucket/pipelines/oleoneto/django-clite/development?style=flat-square)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/django-clite?style=flat-square)
+        ![publish](https://github.com/oleoneto/django-clite/workflows/publish/badge.svg?branch=master)
+        ![PyPI - Package](https://img.shields.io/pypi/v/django-clite)
+        ![PyPI - Python](https://img.shields.io/pypi/pyversions/django-clite)
+        ![PyPI - License](https://img.shields.io/pypi/l/django-clite)
+        ![PyPI - Downloads](https://img.shields.io/pypi/dm/django-clite)
         
         
         - [Introduction](#django-clite)
         - [Interactive Docs](#interactive-docs)
         - [Dependencies](#dependencies)
         - [Installation](#installation)
         - [To Do](#to-do)
@@ -52,15 +52,15 @@
         ```
         D
         django-clite
         djc
         ```
         
         ## To Do
-        [Check out our open issues](/issues).
+        [Check out our open issues](https://github.com/oleoneto/django-clite/issues).
         
         ## Pull requests
         Found a bug? See a typo? Have an idea for new command?
         Feel free to submit a pull request with your contributions. They are much welcome and appreciated.
         
         ## LICENSE
         **django-clite** is [BSD Licensed](LICENSE.txt).
```

### Comparing `django-clite-0.2.9/django_clite.egg-info/SOURCES.txt` & `django-clite-0.3.0/django_clite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-clite-0.2.9/setup.py` & `django-clite-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="django-clite",
-    version="0.2.9",
+    version="0.3.0",
     author="Leo Neto",
     author_email="leo@ekletik.com",
-    url="https://bitbucket.org/oleoneto/django-clite",
+    url="https://github.com/oleoneto/django-clite",
     description="CLI for managing Django projects",
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords="django automate cli command line tools rails ember python framework",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
@@ -43,16 +43,16 @@
         'faker',
         'inquirer',
     ],
     zip_safe=False,
     include_package_data=True,
     packages=find_packages(),
     project_urls={
-        "Documentation": "https://bitbucket.org/oleoneto/django-clite/",
-        "Source Code": "https://bitbucket.org/oleoneto/django-clite/",
+        "Documentation": "https://github.com/oleoneto/django-clite/",
+        "Source Code": "https://github.com/oleoneto/django-clite/",
     },
     entry_points={
         'console_scripts': [
             'D=app:main',
             'djc=app:main',
             'django-clite=app:main',
         ]
```

