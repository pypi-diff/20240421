# Comparing `tmp/wagtail_fedit-1.5.1a3.tar.gz` & `tmp/wagtail_fedit-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.1a3.tar", last modified: Fri Apr 19 16:35:49 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.2.tar", last modified: Sat Apr 20 23:41:16 2024, max compression
```

## Comparing `wagtail_fedit-1.5.1a3.tar` & `wagtail_fedit-1.5.2.tar`

### file list

```diff
@@ -1,128 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.377062 wagtail_fedit-1.5.1a3/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/MANIFEST.in
--rw-rw-rw-   0        0        0    12614 2024-04-19 16:35:49.377062 wagtail_fedit-1.5.1a3/PKG-INFO
--rw-rw-rw-   0        0        0    11357 2024-04-18 16:00:13.000000 wagtail_fedit-1.5.1a3/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/pyproject.toml
--rw-rw-rw-   0        0        0     1188 2024-04-19 16:35:49.377062 wagtail_fedit-1.5.1a3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.700359 wagtail_fedit-1.5.1a3/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.778473 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0     6121 2024-04-18 20:22:02.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     4828 2024-04-18 20:24:20.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     1943 2024-04-18 21:37:23.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.809803 wagtail_fedit-1.5.1a3/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1765 2024-04-18 20:28:58.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4214 2024-04-16 18:40:39.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.590607 wagtail_fedit-1.5.1a3/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.590607 wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.841058 wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.841058 wagtail_fedit-1.5.1a3/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.841058 wagtail_fedit-1.5.1a3/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.590607 wagtail_fedit-1.5.1a3/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.605035 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.878071 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5245 2024-04-18 15:52:31.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.904056 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    19376 2024-04-18 15:41:23.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.622185 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.904056 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.904056 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.935345 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:48.966515 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      889 2024-04-18 15:45:49.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5980 2024-04-16 13:14:54.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.013475 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.013475 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.045132 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.048488 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.058142 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     9382 2024-04-18 14:55:09.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     6749 2024-04-18 14:55:07.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.058142 wagtail_fedit-1.5.1a3/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.088461 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.140723 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.219894 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    10055 2024-04-16 10:53:49.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.259044 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    17203 2024-04-18 15:56:15.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.298620 wagtail_fedit-1.5.1a3/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6429 2024-04-18 14:10:27.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.377062 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     1881 2024-04-16 18:44:29.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:35:49.377062 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    12614 2024-04-19 16:35:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4162 2024-04-19 16:35:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 16:35:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-19 16:35:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 16:35:48.000000 wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.873446 wagtail_fedit-1.5.2/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    19504 2024-04-20 23:41:16.873446 wagtail_fedit-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    18306 2024-04-20 20:08:53.000000 wagtail_fedit-1.5.2/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-04-20 23:41:16.883842 wagtail_fedit-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.221848 wagtail_fedit-1.5.2/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.2/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.326428 wagtail_fedit-1.5.2/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0     9235 2024-04-20 14:51:04.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.2/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.350268 wagtail_fedit-1.5.2/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.2/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.2/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1765 2024-04-18 20:28:58.000000 wagtail_fedit-1.5.2/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4214 2024-04-16 18:40:39.000000 wagtail_fedit-1.5.2/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.143468 wagtail_fedit-1.5.2/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.144478 wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.360361 wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.361344 wagtail_fedit-1.5.2/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.2/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.362902 wagtail_fedit-1.5.2/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.2/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0      351 2024-04-19 19:34:54.000000 wagtail_fedit-1.5.2/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.146470 wagtail_fedit-1.5.2/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.146470 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.381574 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.411358 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.147469 wagtail_fedit-1.5.2/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.413871 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.423951 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.434737 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.466914 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      889 2024-04-18 15:45:49.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5980 2024-04-16 13:14:54.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.506469 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.516207 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.526812 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.540306 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.544828 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10007 2024-04-19 19:46:13.000000 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7503 2024-04-19 19:46:11.000000 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.556205 wagtail_fedit-1.5.2/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.576661 wagtail_fedit-1.5.2/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.594087 wagtail_fedit-1.5.2/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.664638 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    11767 2024-04-20 20:40:55.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.752638 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.2/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.2/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.2/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.796489 wagtail_fedit-1.5.2/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.2/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6516 2024-04-19 19:15:42.000000 wagtail_fedit-1.5.2/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.2/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.2/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.871923 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     1881 2024-04-16 18:44:29.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.265798 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    19504 2024-04-20 23:41:16.000000 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3905 2024-04-20 23:41:16.000000 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 23:41:16.000000 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-20 23:41:16.000000 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-20 23:41:16.000000 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.1a3/LICENSE` & `wagtail_fedit-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/PKG-INFO` & `wagtail_fedit-1.5.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: wagtail_fedit
-Version: 1.5.1a3
-Summary: Frontend editing for your Wagtail site
-Home-page: https://github.com/Nigel2392/wagtail_fedit
-Author: Nigel
-Author-email: nigel@goodadvice.it
-License: GPL-2.0-only
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.2
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 5
-Classifier: Framework :: Wagtail :: 6
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=5.2
-
 wagtail_fedit
 =============
 
 ![Wagtail FEdit Example](https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
 
@@ -42,22 +10,28 @@
 - [Getting Started](#getting-started)
 - [Getting Editing!](#getting-editing)
 - [Permissions](#permissions)
 - [Revisions](#revisions)
 - [Workflows](#workflows)
 - [Logs](#logs)
 - [Caveats](#caveats)
-- [Adapters Python](#adapters-python)
-- [Adapters Javascript](#adapters-javascript)
+- [Adapters](#adapters)
+  - [Adapters Python](#adapters-python)
+  - [Adapters Javascript](#adapters-javascript)
 - [Hooks](#hooks)
   - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
   - [Register Type Renderer](#wagtail_feditregister_type_renderer)
   - [Register Field Renderer](#wagtail_feditregister_field_renderer)
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
+  - [Register CSS](#wagtail_feditregister_css)
+  - [Register JS](#wagtail_feditregister_js)
+  - [Field Editor Size](#wagtail_feditfield_editor_size)
+- [Settings](#settings)
+  - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
 - [How your content is rendered](#how-your-content-is-rendered)
   - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
 
@@ -66,14 +40,15 @@
    ```
    INSTALLED_APPS = [
    ...,
    'wagtail_fedit',
    ]
    ```
 2. Run `py ./manage.py collectstatic`.
+3. Run `py ./manage.py adapter_help` to see all your options and their requirements.
 
 ## Getting Editing!
 
 1. Make sure the models you wish to edit inherit from PreviewableMixin.
 
    **This is a requirement.**
 2. Define a template for your model.
@@ -84,29 +59,31 @@
    {% load fedit static wagtailuserbar %} {# Load the required template tag libraries #}
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
-       <link rel="stylesheet" href="{% static 'wagtail_fedit/css/frontend.css' %}">
+       {# Load all registered CSS required for the adapters. Only included inside edit view! #}
+       {% fedit_scripts "css" %}
    </head>
    <body>
        {# Adress the model.field or model.my.related.field you wish to edit. #}
-       {# Editable fields get a special `inline` argument. #}
-       {# if True the button is not placed with an absolute CSS position. #}
-       <h1>{% fedit field self.title inline=True or False %}</h1>
+       {# For help on arguments for the adapters please run the adapter_help command. #}
+       {# Example: `python3 ./manage.py adapter_help` #}
+       <h1>{% fedit field self.title inline %}</h1>
 
        <main class="my-streamfield-content">
            {% fedit field self.content %}
        </main>
 
        {% wagtailuserbar %}
 
-       <script src="{% static 'wagtail_fedit/js/frontend.js' %}"></script>
+       {# Load all registered Javascript required for the adapters. Only included inside edit view! #}
+       {% fedit_scripts "js" %}
    </body>
    </html>
 
 
    ```
 3. If your needs some special form of rendering; we allow your model to define a custom render method.
    The format of the method name should be `render_fedit_{fieldname}`.
@@ -228,21 +205,179 @@
 ```django-html
 {% for item in self.items.bound_blocks %}
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
-## Adapters Python
+## Adapters
+
+Creating a custom adapter is relatively simple.  
+We highly recommend you to inherit from `BaseFieldFuncAdapter` or `BaseBlockFuncAdapter`.  
+These adapters are basically pre-setup to callback to a javascript function on successful form submission.  
+This will save you the most amount of work.
+
+We will create an adapter to change the color of a text field.
+
+Our adapter will be called `colorizer`.
+
+1. Our model is defined as follows:
+
+```python
+from wagtail.models import Page
+from wagtail.admin.panels import FieldPanel
+from django.db import models
+
+class MyPage(Page):
+    COLOR_CHOICES = [
+        ("#000000", "Black"),
+        ("#FFFFFF", "White"),
+        ("#FF0000", "Red"),
+        ("#00FF00", "Green"),
+        ("#0000FF", "Blue"),
+    ]
+
+    color = models.CharField(max_length=7, default="#000000", choices=COLOR_CHOICES)
+
+    content_panels = Page.content_panels + [
+        FieldPanel("color"),
+    ]
+```
+
+2. We have the following HTML template:
+
+```django-html
+...
+
+{% load fedit %}
+{% fedit colorizer page.color target=".my-colorized-div" %}
+<div class="my-colorized-div" style="color: {{ page.color }}">
+    <h1>Colorized Text!</h1>
+</div>
+
+...
+```
+
+###  Adapters Python
+
+We will get started creating the adapter definition.  
+Adapters can be defined anywhere; we recommend a separate `adapters.py` file.
+
+Adapter instances also have access to the following variables:
+
+* `self.object` - The model instance.
+* `self.field_name` - The field name.
+* `self.meta_field` - The models.Field instance.
+* `self.field_value` - The field value (Retrieved with `self.meta_field.value_from_object(self.object)`)
+* `self.request` - The django HTTP request object.
+* `self.kwargs` - Any shared context / keyword arguments for this adapter.
+
+```python
+# myapp/adapters.py
+
+from wagtail_fedit.adapters import (
+    BaseFieldFuncAdapter,
+    VARIABLES,
+)
+
+class ColorizerAdapter(BaseFieldFuncAdapter):
+    # Required keyword arguments for the template tag are defined by the superclass.
+    # required_kwargs = [
+    #   "target",
+    #   "name", # the function name, override in __init__ method.
+    # ]
+
+    # Optional kwargs are used to inform inside of the adapter_help command.
+    # They are only for developer convenience.
+    # optional_kwargs = []
+
+    # How the adapter will be adressed inside of the template tag.
+    identifier = "colorizer"
+
+    # A simple description of what this adapter does.
+    usage_description = "Change the color of the text for the given target element."
+
+    # Optional explanation of keyword arguments
+    help_text_dict = {
+        "target": "The target element to apply the color to.",
+    }
+
+    def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
+        kwargs["name"] = "myColorizerJavascriptFunction"
+        super().__init__(object, field_name, request, **kwargs)
+
+    def render_content(self, parent_context=None):
+        # This is not required; we will replace a CSS variable; thus we are not returning any actual content.
+        return ""
+        
+    def get_response_data(self, parent_context=None):
+        """
+        Return the data to be sent to the frontend adapter.
+        """
+        data = super().get_response_data(parent_context)
+        return data | {
+            "color": self.field_value,
+        }
+
+    def get_form_attrs(self) -> dict:
+        """
+        Return form attributes for the form inside of the edit modal.
+        This can be used to control editor size.
+        """
+        attrs = super().get_form_attrs()
+        attrs[VARIABLES.FORM_SIZE_VAR] = "full" # Fullscreen, there is also `large`.
+        return attrs
+```
+
+We must then register the adapter to make sure it is available for templates.
 
-* TBA
+This should be done in a `wagtail_hooks.py` file.
+
+```python
+# myapp/wagtail_hooks.py
+
+from wagtail_fedit.adapters import adapter_registry
+from myapp.adapters import ColorizerAdapter
+
+adapter_registry.register(ColorizerAdapter)
+```
 
-## Adapters Javascript
+###  Adapters Javascript
 
-* TBA
+We now need to create the javascript function to actually apply the color to the styles of the element.  
+This function will be called `myColorizerJavascriptFunction`, as defined in the adapter's `__init__` method.
+
+```javascript
+// myapp/static/myapp/js/custom.js
+function myColorizerJavascriptFunction(element, response) {
+    element.style.color = response.color;
+}
+```
+
+We must then register this javascript file to be included in the frontend editing interface.
+
+This should be done in a `wagtail_hooks.py` file.
+
+```python
+# myapp/wagtail_hooks.py
+
+from django.utils.html import format_html
+from django.templatetags.static import static
+from wagtail_fedit.hooks import REGISTER_JS
+from wagtail import hooks
+
+@hooks.register(REGISTER_JS)
+def register_js(request):
+    return [
+        format_html(
+            '<script src="{0}"></script>',
+            static('myapp/js/custom.js')
+        ),
+    ]
+```
 
 ## Hooks
 
 ### wagtail_fedit.construct_adapter_toolbar
 
 Construct the toolbar for the given adapter.
 This is used to display the edit icon for the given adapter.
@@ -271,14 +406,63 @@
     # It will render the Page model as a simple h2 tag.
     renderer_map[Page] = lambda request, context, instance, value: format_html(
         '<h2>{0}</h2>',
         value.title
     )
 ```
 
+### wagtail_fedit.register_css
+
+Register a custom CSS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
+
+Example of how this hook is used in wagtail_hooks.py:
+    
+```python
+@hooks.register(REGISTER_CSS)
+def register_css(request):
+    return [
+        format_html(
+            '<link rel="stylesheet" href="{0}">',
+            static('css/custom.css')
+        ),
+    ]
+```
+
+### wagtail_fedit.field_editor_size
+
+Control the size of the editor for the given model-field type.
+
+Example of how this hook is called:
+    
+```python
+for hook in hooks.get_hooks(FEDIT_FIELD_EDITOR_SIZE):
+    size = hook(model_instance, model_field)
+    if size:
+        return size
+```
+
+### wagtail_fedit.register_js
+
+Register a custom JS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
+
+This can be used to register custom adapter JS.
+
+Example of how this hook is used in wagtail_hooks.py:
+    
+    ```python
+    @hooks.register(REGISTER_JS)
+    def register_js(request):
+        return [
+            format_html(
+                '<script src="{0}"></script>',
+                static('js/custom.js')
+            ),
+        ]
+    ```
+
 ### wagtail_fedit.register_field_renderer
 
 Register a custom renderer for a field.
 
 Example of how this type of renderer is used in wagtail_hooks/renderers.py:
 
 ```python
@@ -325,14 +509,25 @@
 ```python
 for hook in hooks.get_hooks(ACTION_MENU_ITEM_IS_SHOWN):
     result = hook(context, instance)
     if result is not None:
         return result # <- bool
 ```
 
+## Settings
+
+### `WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT`
+
+Default: `True`
+
+Sign the shared context with a secret key.  
+This is useful to prevent tampering with the shared context.  
+It will also be compressed with zlib if available.  
+It might not be in your site's security model to need this.
+
 ## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
 ### Rendered editable output HTML
```

#### html2text {}

```diff
@@ -1,49 +1,42 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.1a3 Summary: Frontend
-editing for your Wagtail site Home-page: https://github.com/Nigel2392/
-wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
-only Classifier: Environment :: Web Environment Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
-Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
-:: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
-Dynamic Content Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: Django>=4.2 Requires-Dist: Wagtail>=5.2
 wagtail_fedit ============= ![Wagtail FEdit Example](https://github.com/
 Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
-(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters Python]
-(#adapters-python) - [Adapters Javascript](#adapters-javascript) - [Hooks]
-(#hooks) - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
-- [Register Type Renderer](#wagtail_feditregister_type_renderer) - [Register
-Field Renderer](#wagtail_feditregister_field_renderer) - [Exclude Related
-Forms](#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
-(#wagtail_feditaction_menu_item_is_shown) - [How your content is rendered]
-(#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
-output-html) - [Implemented](#implemented) Getting Started --------------- 1.
-Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
+(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters](#adapters) -
+[Adapters Python](#adapters-python) - [Adapters Javascript](#adapters-
+javascript) - [Hooks](#hooks) - [Construct Adapter Toolbar]
+(#wagtail_feditconstruct_adapter_toolbar) - [Register Type Renderer]
+(#wagtail_feditregister_type_renderer) - [Register Field Renderer]
+(#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
+(#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
+(#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
+(#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
+[Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
+[Sign Shared Context](#wagtail_fedit_sign_shared_context) - [How your content
+is rendered](#how-your-content-is-rendered) - [Rendered output HTML](#rendered-
+editable-output-html) - [Implemented](#implemented) Getting Started -----------
+---- 1. Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
 INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
-collectstatic`. ## Getting Editing! 1. Make sure the models you wish to edit
-inherit from PreviewableMixin. **This is a requirement.** 2. Define a template
-for your model. Example: ```django-html {% load fedit static wagtailuserbar %}
-{# Load the required template tag libraries #}
-{# Adress the model.field or model.my.related.field you wish to edit. #} {#
-Editable fields get a special `inline` argument. #} {# if True the button is
-not placed with an absolute CSS position. #}
-************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee==TTrruuee oorr FFaallssee %%}} ************
-{% fedit field self.content %} {% wagtailuserbar %}
+collectstatic`. 3. Run `py ./manage.py adapter_help` to see all your options
+and their requirements. ## Getting Editing! 1. Make sure the models you wish to
+edit inherit from PreviewableMixin. **This is a requirement.** 2. Define a
+template for your model. Example: ```django-html {% load fedit static
+wagtailuserbar %} {# Load the required template tag libraries #}
+{# Load all registered CSS required for the adapters. Only included inside edit
+view! #} {% fedit_scripts "css" %}
+{# Adress the model.field or model.my.related.field you wish to edit. #} {# For
+help on arguments for the adapters please run the adapter_help command. #} {#
+Example: `python3 ./manage.py adapter_help` #}
+************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee %%}} ************
+{% fedit field self.content %} {% wagtailuserbar %} {# Load all registered
+Javascript required for the adapters. Only included inside edit view! #} {%
+fedit_scripts "js" %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
 fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by {# fedit
@@ -100,48 +93,124 @@
 %} {% include_block item %} {# No access to ID! Cannot edit! #} {% endfor %}
 ``` To make this an editable block instead; we would slightly change the loop
 to make the block's `id` available. This is done by accessing the
 `bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for
 the toplevel block!)* Our new loop would then be: ```django-html {% for item in
 self.items.bound_blocks %} {# Field name and model are the same arguments as in
 the first example! #} {% fedit block my_model_instance_var.content_field
-block=item block_id=item.id %} {% endfor %} ``` ## Adapters Python * TBA ##
-Adapters Javascript * TBA ## Hooks ### wagtail_fedit.construct_adapter_toolbar
-Construct the toolbar for the given adapter. This is used to display the edit
-icon for the given adapter. How it is called: ```python items =
-[ FeditAdapterEditButton(), ] for hook in hooks.get_hooks
-(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter) ``` ###
-wagtail_fedit.register_type_renderer Register a custom renderer for a type.
-Example of how this type of renderer can be used: ```python @hooks.register
-(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): # This is a
-custom renderer for the Page model. # It will render the Page model as a simple
-h2 tag. renderer_map[Page] = lambda request, context, instance, value:
-format_html( '
+block=item block_id=item.id %} {% endfor %} ``` ## Adapters Creating a custom
+adapter is relatively simple. We highly recommend you to inherit from
+`BaseFieldFuncAdapter` or `BaseBlockFuncAdapter`. These adapters are basically
+pre-setup to callback to a javascript function on successful form submission.
+This will save you the most amount of work. We will create an adapter to change
+the color of a text field. Our adapter will be called `colorizer`. 1. Our model
+is defined as follows: ```python from wagtail.models import Page from
+wagtail.admin.panels import FieldPanel from django.db import models class
+MyPage(Page): COLOR_CHOICES = [ ("#000000", "Black"), ("#FFFFFF", "White"),
+("#FF0000", "Red"), ("#00FF00", "Green"), ("#0000FF", "Blue"), ] color =
+models.CharField(max_length=7, default="#000000", choices=COLOR_CHOICES)
+content_panels = Page.content_panels + [ FieldPanel("color"), ] ``` 2. We have
+the following HTML template: ```django-html ... {% load fedit %} {% fedit
+colorizer page.color target=".my-colorized-div" %}
+************ CCoolloorriizzeedd TTeexxtt!! ************
+... ``` ### Adapters Python We will get started creating the adapter
+definition. Adapters can be defined anywhere; we recommend a separate
+`adapters.py` file. Adapter instances also have access to the following
+variables: * `self.object` - The model instance. * `self.field_name` - The
+field name. * `self.meta_field` - The models.Field instance. *
+`self.field_value` - The field value (Retrieved with
+`self.meta_field.value_from_object(self.object)`) * `self.request` - The django
+HTTP request object. * `self.kwargs` - Any shared context / keyword arguments
+for this adapter. ```python # myapp/adapters.py from wagtail_fedit.adapters
+import ( BaseFieldFuncAdapter, VARIABLES, ) class ColorizerAdapter
+(BaseFieldFuncAdapter): # Required keyword arguments for the template tag are
+defined by the superclass. # required_kwargs = [ # "target", # "name", # the
+function name, override in __init__ method. # ] # Optional kwargs are used to
+inform inside of the adapter_help command. # They are only for developer
+convenience. # optional_kwargs = [] # How the adapter will be adressed inside
+of the template tag. identifier = "colorizer" # A simple description of what
+this adapter does. usage_description = "Change the color of the text for the
+given target element." # Optional explanation of keyword arguments
+help_text_dict = { "target": "The target element to apply the color to.", } def
+__init__(self, object, field_name: str, request: HttpRequest, **kwargs): kwargs
+["name"] = "myColorizerJavascriptFunction" super().__init__(object, field_name,
+request, **kwargs) def render_content(self, parent_context=None): # This is not
+required; we will replace a CSS variable; thus we are not returning any actual
+content. return "" def get_response_data(self, parent_context=None): """ Return
+the data to be sent to the frontend adapter. """ data = super
+().get_response_data(parent_context) return data | { "color": self.field_value,
+} def get_form_attrs(self) -> dict: """ Return form attributes for the form
+inside of the edit modal. This can be used to control editor size. """ attrs =
+super().get_form_attrs() attrs[VARIABLES.FORM_SIZE_VAR] = "full" # Fullscreen,
+there is also `large`. return attrs ``` We must then register the adapter to
+make sure it is available for templates. This should be done in a
+`wagtail_hooks.py` file. ```python # myapp/wagtail_hooks.py from
+wagtail_fedit.adapters import adapter_registry from myapp.adapters import
+ColorizerAdapter adapter_registry.register(ColorizerAdapter) ``` ### Adapters
+Javascript We now need to create the javascript function to actually apply the
+color to the styles of the element. This function will be called
+`myColorizerJavascriptFunction`, as defined in the adapter's `__init__` method.
+```javascript // myapp/static/myapp/js/custom.js function
+myColorizerJavascriptFunction(element, response) { element.style.color =
+response.color; } ``` We must then register this javascript file to be included
+in the frontend editing interface. This should be done in a `wagtail_hooks.py`
+file. ```python # myapp/wagtail_hooks.py from django.utils.html import
+format_html from django.templatetags.static import static from
+wagtail_fedit.hooks import REGISTER_JS from wagtail import hooks
+@hooks.register(REGISTER_JS) def register_js(request): return [ format_html( '
+', static('myapp/js/custom.js') ), ] ``` ## Hooks ###
+wagtail_fedit.construct_adapter_toolbar Construct the toolbar for the given
+adapter. This is used to display the edit icon for the given adapter. How it is
+called: ```python items = [ FeditAdapterEditButton(), ] for hook in
+hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter)
+``` ### wagtail_fedit.register_type_renderer Register a custom renderer for a
+type. Example of how this type of renderer can be used: ```python
+@hooks.register(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): #
+This is a custom renderer for the Page model. # It will render the Page model
+as a simple h2 tag. renderer_map[Page] = lambda request, context, instance,
+value: format_html( '
 ********** {{00}} **********
-', value.title ) ``` ### wagtail_fedit.register_field_renderer Register a
-custom renderer for a field. Example of how this type of renderer is used in
-wagtail_hooks/renderers.py: ```python @hooks.register(REGISTER_FIELD_RENDERER)
-def register_renderers(renderer_map): # This is a custom renderer for RichText
-fields. # It will render the RichText field as a RichText block. renderer_map
-[RichTextField] =\ lambda request, context, instance, value: richtext(value)
-``` ### wagtail_fedit.exclude_related_forms Exclude the given model type from
-the related forms. This is used internally to exclude the Page, Image, and
-Document models from the related forms. This way; the user will have the actual
-widget for the field instead of the related form. Example of how this hook is
-called and how it is used internally: ```python def use_related_form(field:
-models.Field) -> bool: for hook in hooks.get_hooks(EXCLUDE_FROM_RELATED_FORMS):
-if hook(field): return False return True @hooks.register
-(EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field): if
-field.related_model in [Page, Image, Document]: return True return False ```
+', value.title ) ``` ### wagtail_fedit.register_css Register a custom CSS file
+to be included when the utils.FEDIT_PREVIEW_VAR is set to True. Example of how
+this hook is used in wagtail_hooks.py: ```python @hooks.register(REGISTER_CSS)
+def register_css(request): return [ format_html( '
+', static('css/custom.css') ), ] ``` ### wagtail_fedit.field_editor_size
+Control the size of the editor for the given model-field type. Example of how
+this hook is called: ```python for hook in hooks.get_hooks
+(FEDIT_FIELD_EDITOR_SIZE): size = hook(model_instance, model_field) if size:
+return size ``` ### wagtail_fedit.register_js Register a custom JS file to be
+included when the utils.FEDIT_PREVIEW_VAR is set to True. This can be used to
+register custom adapter JS. Example of how this hook is used in
+wagtail_hooks.py: ```python @hooks.register(REGISTER_JS) def register_js
+(request): return [ format_html( '
+', static('js/custom.js') ), ] ``` ### wagtail_fedit.register_field_renderer
+Register a custom renderer for a field. Example of how this type of renderer is
+used in wagtail_hooks/renderers.py: ```python @hooks.register
+(REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
+custom renderer for RichText fields. # It will render the RichText field as a
+RichText block. renderer_map[RichTextField] =\ lambda request, context,
+instance, value: richtext(value) ``` ### wagtail_fedit.exclude_related_forms
+Exclude the given model type from the related forms. This is used internally to
+exclude the Page, Image, and Document models from the related forms. This way;
+the user will have the actual widget for the field instead of the related form.
+Example of how this hook is called and how it is used internally: ```python def
+use_related_form(field: models.Field) -> bool: for hook in hooks.get_hooks
+(EXCLUDE_FROM_RELATED_FORMS): if hook(field): return False return True
+@hooks.register(EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field):
+if field.related_model in [Page, Image, Document]: return True return False ```
 ### wagtail_fedit.action_menu_item_is_shown Decide if the action menu item
 should be shown for the given instance. Return None if you cannot decide, False
 if you want to hide the item, and True if you want to show the item. Example of
 how this hook is called: ```python for hook in hooks.get_hooks
 (ACTION_MENU_ITEM_IS_SHOWN): result = hook(context, instance) if result is not
-None: return result # <- bool ``` ## How your content is rendered
+None: return result # <- bool ``` ## Settings ###
+`WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT` Default: `True` Sign the shared context
+with a secret key. This is useful to prevent tampering with the shared context.
+It will also be compressed with zlib if available. It might not be in your
+site's security model to need this. ## How your content is rendered
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
 or even at all for most content - **if** you don't get hyperspecific with your
 CSS selectors and structure your templates well.) Your block and field are
 wrapped in a `div`, any CSS for your templates should keep this in mind. ###
 Rendered editable output HTML ```html
 % if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
 { edit_url }}">
```

### Comparing `wagtail_fedit-1.5.1a3/setup.cfg` & `wagtail_fedit-1.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3161 330d 0a64 6573 6372 6970 7469 6f6e  1a3..description
-00000040: 203d 2046 726f 6e74 656e 6420 6564 6974   = Frontend edit
-00000050: 696e 6720 666f 7220 796f 7572 2057 6167  ing for your Wag
-00000060: 7461 696c 2073 6974 650d 0a6c 6f6e 675f  tail site..long_
-00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-000000a0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-000000b0: 6578 742f 6d61 726b 646f 776e 0d0a 6175  ext/markdown..au
-000000c0: 7468 6f72 203d 204e 6967 656c 0d0a 6175  thor = Nigel..au
-000000d0: 7468 6f72 5f65 6d61 696c 203d 206e 6967  thor_email = nig
-000000e0: 656c 4067 6f6f 6461 6476 6963 652e 6974  el@goodadvice.it
-000000f0: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000100: 6769 7468 7562 2e63 6f6d 2f4e 6967 656c  github.com/Nigel
-00000110: 3233 3932 2f77 6167 7461 696c 5f66 6564  2392/wagtail_fed
-00000120: 6974 0d0a 6c69 6365 6e73 6520 3d20 4750  it..license = GP
-00000130: 4c2d 322e 302d 6f6e 6c79 0d0a 636c 6173  L-2.0-only..clas
-00000140: 7369 6669 6572 7320 3d20 0d0a 0945 6e76  sifiers = ...Env
-00000150: 6972 6f6e 6d65 6e74 203a 3a20 5765 6220  ironment :: Web 
-00000160: 456e 7669 726f 6e6d 656e 740d 0a09 4672  Environment...Fr
-00000170: 616d 6577 6f72 6b20 3a3a 2044 6a61 6e67  amework :: Djang
-00000180: 6f0d 0a09 4672 616d 6577 6f72 6b20 3a3a  o...Framework ::
-00000190: 2044 6a61 6e67 6f20 3a3a 2034 2e32 0d0a   Django :: 4.2..
-000001a0: 0946 7261 6d65 776f 726b 203a 3a20 5761  .Framework :: Wa
-000001b0: 6774 6169 6c0d 0a09 4672 616d 6577 6f72  gtail...Framewor
-000001c0: 6b20 3a3a 2057 6167 7461 696c 203a 3a20  k :: Wagtail :: 
-000001d0: 350d 0a09 4672 616d 6577 6f72 6b20 3a3a  5...Framework ::
-000001e0: 2057 6167 7461 696c 203a 3a20 360d 0a09   Wagtail :: 6...
-000001f0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-00000200: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
-00000210: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-00000220: 2041 7070 726f 7665 6420 3a3a 2047 4e55   Approved :: GNU
-00000230: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-00000240: 4c69 6365 6e73 6520 7632 206f 7220 6c61  License v2 or la
-00000250: 7465 7220 2847 504c 7632 2b29 0d0a 094f  ter (GPLv2+)...O
-00000260: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000270: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000280: 740d 0a09 5072 6f67 7261 6d6d 696e 6720  t...Programming 
-00000290: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002a0: 6f6e 0d0a 0950 726f 6772 616d 6d69 6e67  on...Programming
-000002b0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002c0: 686f 6e20 3a3a 2033 0d0a 0950 726f 6772  hon :: 3...Progr
-000002d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000002e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 203a  :: Python :: 3 :
-000002f0: 3a20 4f6e 6c79 0d0a 0950 726f 6772 616d  : Only...Program
-00000300: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000310: 2050 7974 686f 6e20 3a3a 2033 2e38 0d0a   Python :: 3.8..
-00000320: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000330: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000340: 3a3a 2033 2e39 0d0a 0950 726f 6772 616d  :: 3.9...Program
-00000350: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000360: 2050 7974 686f 6e20 3a3a 2033 2e31 300d   Python :: 3.10.
-00000370: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000380: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000390: 203a 3a20 332e 3131 0d0a 0954 6f70 6963   :: 3.11...Topic
-000003a0: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
-000003b0: 5757 572f 4854 5450 0d0a 0954 6f70 6963  WWW/HTTP...Topic
-000003c0: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
-000003d0: 5757 572f 4854 5450 203a 3a20 4479 6e61  WWW/HTTP :: Dyna
-000003e0: 6d69 6320 436f 6e74 656e 740d 0a0d 0a5b  mic Content....[
-000003f0: 6f70 7469 6f6e 735d 0d0a 696e 636c 7564  options]..includ
-00000400: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
-00000410: 2074 7275 650d 0a70 6163 6b61 6765 7320   true..packages 
-00000420: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
-00000430: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
-00000440: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-00000450: 6573 203d 200d 0a09 446a 616e 676f 203e  es = ...Django >
-00000460: 3d20 342e 320d 0a09 5761 6774 6169 6c20  = 4.2...Wagtail 
-00000470: 3e3d 2035 2e32 0d0a 0d0a 5b65 6767 5f69  >= 5.2....[egg_i
-00000480: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-00000490: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000004a0: 0d0a 0d0a                                ....
+00000030: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
+00000040: 2046 726f 6e74 656e 6420 6564 6974 696e   Frontend editin
+00000050: 6720 666f 7220 796f 7572 2057 6167 7461  g for your Wagta
+00000060: 696c 2073 6974 650d 0a6c 6f6e 675f 6465  il site..long_de
+00000070: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+00000080: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
+00000090: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+000000a0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+000000b0: 742f 6d61 726b 646f 776e 0d0a 6175 7468  t/markdown..auth
+000000c0: 6f72 203d 204e 6967 656c 0d0a 6175 7468  or = Nigel..auth
+000000d0: 6f72 5f65 6d61 696c 203d 206e 6967 656c  or_email = nigel
+000000e0: 4067 6f6f 6461 6476 6963 652e 6974 0d0a  @goodadvice.it..
+000000f0: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
+00000100: 7468 7562 2e63 6f6d 2f4e 6967 656c 3233  thub.com/Nigel23
+00000110: 3932 2f77 6167 7461 696c 5f66 6564 6974  92/wagtail_fedit
+00000120: 0d0a 6c69 6365 6e73 6520 3d20 4750 4c2d  ..license = GPL-
+00000130: 322e 302d 6f6e 6c79 0d0a 636c 6173 7369  2.0-only..classi
+00000140: 6669 6572 7320 3d20 0d0a 0945 6e76 6972  fiers = ...Envir
+00000150: 6f6e 6d65 6e74 203a 3a20 5765 6220 456e  onment :: Web En
+00000160: 7669 726f 6e6d 656e 740d 0a09 4672 616d  vironment...Fram
+00000170: 6577 6f72 6b20 3a3a 2044 6a61 6e67 6f0d  ework :: Django.
+00000180: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
+00000190: 6a61 6e67 6f20 3a3a 2034 2e32 0d0a 0946  jango :: 4.2...F
+000001a0: 7261 6d65 776f 726b 203a 3a20 5761 6774  ramework :: Wagt
+000001b0: 6169 6c0d 0a09 4672 616d 6577 6f72 6b20  ail...Framework 
+000001c0: 3a3a 2057 6167 7461 696c 203a 3a20 350d  :: Wagtail :: 5.
+000001d0: 0a09 4672 616d 6577 6f72 6b20 3a3a 2057  ..Framework :: W
+000001e0: 6167 7461 696c 203a 3a20 360d 0a09 496e  agtail :: 6...In
+000001f0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000200: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
+00000210: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000220: 7070 726f 7665 6420 3a3a 2047 4e55 2047  pproved :: GNU G
+00000230: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
+00000240: 6365 6e73 6520 7632 206f 7220 6c61 7465  cense v2 or late
+00000250: 7220 2847 504c 7632 2b29 0d0a 094f 7065  r (GPLv2+)...Ope
+00000260: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000270: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000280: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000290: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002a0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000002b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002c0: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
+000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002e0: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
+000002f0: 4f6e 6c79 0d0a 0950 726f 6772 616d 6d69  Only...Programmi
+00000300: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000310: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
+00000320: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000330: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000340: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
+00000350: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000360: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
+00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000380: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000390: 3a20 332e 3131 0d0a 0954 6f70 6963 203a  : 3.11...Topic :
+000003a0: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
+000003b0: 572f 4854 5450 0d0a 0954 6f70 6963 203a  W/HTTP...Topic :
+000003c0: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
+000003d0: 572f 4854 5450 203a 3a20 4479 6e61 6d69  W/HTTP :: Dynami
+000003e0: 6320 436f 6e74 656e 740d 0a0d 0a5b 6f70  c Content....[op
+000003f0: 7469 6f6e 735d 0d0a 696e 636c 7564 655f  tions]..include_
+00000400: 7061 636b 6167 655f 6461 7461 203d 2074  package_data = t
+00000410: 7275 650d 0a70 6163 6b61 6765 7320 3d20  rue..packages = 
+00000420: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
+00000430: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
+00000440: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000450: 203d 200d 0a09 446a 616e 676f 203e 3d20   = ...Django >= 
+00000460: 342e 320d 0a09 5761 6774 6169 6c20 3e3d  4.2...Wagtail >=
+00000470: 2035 2e32 0d0a 0d0a 5b65 6767 5f69 6e66   5.2....[egg_inf
+00000480: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000490: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+000004a0: 0d0a                                     ..
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.2/wagtail_fedit/adapters/block.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,48 +18,86 @@
     AdapterError,
     VARIABLES,
 )
 from ..forms import (
     blocks as block_forms,
 )
 from .. import utils
-
+from wagtail.admin.admin_url_finder import (
+    AdminURLFinder,
+)
+from ..toolbar import (
+    FeditAdapterComponent,
+    FeditAdapterAdminLinkButton,
+)
 
 
 
 class BlockAdapter(BlockFieldReplacementAdapter):
     """
     An adapter for editing Wagtail blocks.
     This will render the block and replace it on the frontend
     on successful form submission.
     """
     identifier = "block"
-    required_kwargs = ["block"]
+    usage_description = "This adapter is used to edit a block of a streamfield."
+    help_text_dict = {
+        "block": "the block instance to edit. This can be a regular block isntance or a BoundBlock.",
+        "block_id": "the ID of the block to edit, required if block is not a BoundBlock.",
+        "admin": "if passed; the adapter will a quick- link to the Wagtail Admin for this block.",
+    }
+    required_kwargs = [
+        "block",
+    ]
+    optional_kwargs = [
+        "block_id",
+    ]
+    absolute_tokens = [ # override; remove "inline"
+        "admin", # allows for displaying admin URLs
+    ]
 
     def __init__(self, object: models.Model, field_name: str, request: HttpRequest, **kwargs):
         super().__init__(object, field_name, request, **kwargs)
 
         self.block = self.kwargs.pop("block", None)
         if self.block:
-            if not isinstance(self.block, BoundBlock):
-                raise AdapterError("Invalid block type")
+            if not hasattr(self.block, "id") and not "block_id" in self.kwargs:
+                raise AdapterError("Invalid block type, block must have an `id` attribute or provide a `block_id`")
+            
+            if hasattr(self.block, "id"):
+                self.kwargs["block_id"] = self.block.id
 
-            self.kwargs["block_id"] = self.block.id
         else:
             block_id = self.kwargs.get("block_id", None)
             if block_id is None:
                 raise AdapterError("Block ID is required")
             
             self.streamfield: StreamValue = getattr(self.object, self.field_name)
             result = utils.find_block(block_id, self.streamfield)
             if not result:
                 raise AdapterError("Block not found; did you provide the correct block ID?")
             
             self.block, _ = result
 
+    def get_admin_url(self) -> str:
+        finder = AdminURLFinder(self.request.user)
+        url = finder.get_edit_url(self.object)
+        hash = f"#block-{self.kwargs['block_id']}-section"
+        return f"{url}{hash}"
+
+    def get_toolbar_buttons(self) -> list[FeditAdapterComponent]:
+        buttons = super().get_toolbar_buttons()
+        if not self.kwargs.get("admin", False):
+            return buttons
+        
+        buttons.append(FeditAdapterAdminLinkButton(
+            self.request, self,
+        ))
+        return buttons
+
     def get_header_title(self):
 
         model_string = getattr(self.object, "get_admin_display_title", None)
         if model_string:
             model_string = model_string()
         else:
             model_string = getattr(self.object, "title", str(self.object))
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.2/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.2/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.2/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.2/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.2/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.2/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/models.py` & `wagtail_fedit-1.5.2/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,20 @@
     left: unset;
     right: unset;
 }
 
 /* .wagtail-fedit-field-wrapper > .wagtail-fedit-buttons { */
     /* position: relative; */
 /* } */
+.wagtail-fedit-adapter-wrapper > .wagtail-fedit-buttons .wagtail-fedit-toolbar-button,
 .wagtail-fedit-adapter-wrapper > .wagtail-fedit-buttons button {
     display: inline-block;
     vertical-align: middle;
 }
+.wagtail-fedit-buttons .wagtail-fedit-toolbar-button,
 .wagtail-fedit-buttons button {
     border: none;
     background-color: white;
     padding: 0.1em;
     border-radius: 0.25em;
     width: 24px;
     height: 24px;
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -560,15 +560,24 @@
         }
     }
 }
 
 
 function wagtailFeditBackgroundImageAdapter(element, response) {
     const url = response.url;
-    element.style.backgroundImage = `url(${url})`;
+    const cssVar = response.css_variable_name;
+    if (cssVar) {
+        if (cssVar.startsWith("--")) {
+            element.style.setProperty(cssVar, `url(${url})`);
+        } else {
+            element.style.setProperty(cssVar, `url(${url})`);
+        }
+    } else {
+        element.style.backgroundImage = `url(${url})`;
+    }
 }
 
 
 document.addEventListener("DOMContentLoaded", initFEditors);
 
 
 window.wagtailFedit = {
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% load i18n %}
-<button class="wagtail-fedit-block-edit wagtail-fedit-edit-button">
-    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-pencil-square" viewBox="0 0 16 16" aria-label="{% translate "Edit block" %}">
+<button class="wagtail-fedit-adapter-edit wagtail-fedit-toolbar-button wagtail-fedit-edit-button">
+    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-pencil-square" viewBox="0 0 16 16" aria-label="{% translate "Edit Field" %}">
         <!-- The MIT License (MIT) -->
         <!-- Copyright (c) 2011-2024 The Bootstrap Authors -->
         <path d="M15.502 1.94a.5.5 0 0 1 0 .706L14.459 3.69l-2-2L13.502.646a.5.5 0 0 1 .707 0l1.293 1.293zm-1.75 2.456-2-2L4.939 9.21a.5.5 0 0 0-.121.196l-.805 2.414a.25.25 0 0 0 .316.316l2.414-.805a.5.5 0 0 0 .196-.12l6.813-6.814z"/>
         <path fill-rule="evenodd" d="M1 13.5A1.5 1.5 0 0 0 2.5 15h11a1.5 1.5 0 0 0 1.5-1.5v-6a.5.5 0 0 0-1 0v6a.5.5 0 0 1-.5.5h-11a.5.5 0 0 1-.5-.5v-11a.5.5 0 0 1 .5-.5H9a.5.5 0 0 0 0-1H2.5A1.5 1.5 0 0 0 1 2.5z"/>
     </svg>
 </button>
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-00000000: 7b25 206c 6f61 6420 6931 386e 2025 7d0d  {% load i18n %}.
-00000010: 0a3c 6275 7474 6f6e 2063 6c61 7373 3d22  .<button class="
-00000020: 7761 6774 6169 6c2d 6665 6469 742d 626c  wagtail-fedit-bl
-00000030: 6f63 6b2d 6564 6974 2077 6167 7461 696c  ock-edit wagtail
-00000040: 2d66 6564 6974 2d65 6469 742d 6275 7474  -fedit-edit-butt
-00000050: 6f6e 223e 0d0a 2020 2020 3c73 7667 2078  on">..    <svg x
-00000060: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
-00000070: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
-00000080: 2220 7769 6474 683d 2231 3622 2068 6569  " width="16" hei
-00000090: 6768 743d 2231 3622 2066 696c 6c3d 2263  ght="16" fill="c
-000000a0: 7572 7265 6e74 436f 6c6f 7222 2063 6c61  urrentColor" cla
-000000b0: 7373 3d22 6269 2062 692d 7065 6e63 696c  ss="bi bi-pencil
-000000c0: 2d73 7175 6172 6522 2076 6965 7742 6f78  -square" viewBox
-000000d0: 3d22 3020 3020 3136 2031 3622 2061 7269  ="0 0 16 16" ari
-000000e0: 612d 6c61 6265 6c3d 227b 2520 7472 616e  a-label="{% tran
-000000f0: 736c 6174 6520 2245 6469 7420 626c 6f63  slate "Edit bloc
-00000100: 6b22 2025 7d22 3e0d 0a20 2020 2020 2020  k" %}">..       
-00000110: 203c 212d 2d20 5468 6520 4d49 5420 4c69   <!-- The MIT Li
-00000120: 6365 6e73 6520 284d 4954 2920 2d2d 3e0d  cense (MIT) -->.
-00000130: 0a20 2020 2020 2020 203c 212d 2d20 436f  .        <!-- Co
-00000140: 7079 7269 6768 7420 2863 2920 3230 3131  pyright (c) 2011
-00000150: 2d32 3032 3420 5468 6520 426f 6f74 7374  -2024 The Bootst
-00000160: 7261 7020 4175 7468 6f72 7320 2d2d 3e0d  rap Authors -->.
-00000170: 0a20 2020 2020 2020 203c 7061 7468 2064  .        <path d
-00000180: 3d22 4d31 352e 3530 3220 312e 3934 612e  ="M15.502 1.94a.
-00000190: 352e 3520 3020 3020 3120 3020 2e37 3036  5.5 0 0 1 0 .706
-000001a0: 4c31 342e 3435 3920 332e 3639 6c2d 322d  L14.459 3.69l-2-
-000001b0: 324c 3133 2e35 3032 2e36 3436 612e 352e  2L13.502.646a.5.
-000001c0: 3520 3020 3020 3120 2e37 3037 2030 6c31  5 0 0 1 .707 0l1
-000001d0: 2e32 3933 2031 2e32 3933 7a6d 2d31 2e37  .293 1.293zm-1.7
-000001e0: 3520 322e 3435 362d 322d 324c 342e 3933  5 2.456-2-2L4.93
-000001f0: 3920 392e 3231 612e 352e 3520 3020 3020  9 9.21a.5.5 0 0 
-00000200: 302d 2e31 3231 2e31 3936 6c2d 2e38 3035  0-.121.196l-.805
-00000210: 2032 2e34 3134 612e 3235 2e32 3520 3020   2.414a.25.25 0 
-00000220: 3020 3020 2e33 3136 2e33 3136 6c32 2e34  0 0 .316.316l2.4
-00000230: 3134 2d2e 3830 3561 2e35 2e35 2030 2030  14-.805a.5.5 0 0
-00000240: 2030 202e 3139 362d 2e31 326c 362e 3831   0 .196-.12l6.81
-00000250: 332d 362e 3831 347a 222f 3e0d 0a20 2020  3-6.814z"/>..   
-00000260: 2020 2020 203c 7061 7468 2066 696c 6c2d       <path fill-
-00000270: 7275 6c65 3d22 6576 656e 6f64 6422 2064  rule="evenodd" d
-00000280: 3d22 4d31 2031 332e 3541 312e 3520 312e  ="M1 13.5A1.5 1.
-00000290: 3520 3020 3020 3020 322e 3520 3135 6831  5 0 0 0 2.5 15h1
-000002a0: 3161 312e 3520 312e 3520 3020 3020 3020  1a1.5 1.5 0 0 0 
-000002b0: 312e 352d 312e 3576 2d36 612e 352e 3520  1.5-1.5v-6a.5.5 
-000002c0: 3020 3020 302d 3120 3076 3661 2e35 2e35  0 0 0-1 0v6a.5.5
-000002d0: 2030 2030 2031 2d2e 352e 3568 2d31 3161   0 0 1-.5.5h-11a
-000002e0: 2e35 2e35 2030 2030 2031 2d2e 352d 2e35  .5.5 0 0 1-.5-.5
-000002f0: 762d 3131 612e 352e 3520 3020 3020 3120  v-11a.5.5 0 0 1 
-00000300: 2e35 2d2e 3548 3961 2e35 2e35 2030 2030  .5-.5H9a.5.5 0 0
-00000310: 2030 2030 2d31 4832 2e35 4131 2e35 2031   0 0-1H2.5A1.5 1
-00000320: 2e35 2030 2030 2030 2031 2032 2e35 7a22  .5 0 0 0 1 2.5z"
-00000330: 2f3e 0d0a 2020 2020 3c2f 7376 673e 0d0a  />..    </svg>..
-00000340: 3c2f 6275 7474 6f6e 3e                   </button>
+00000000: 7b25 2065 7874 656e 6473 2022 7761 6774  {% extends "wagt
+00000010: 6169 6c61 646d 696e 2f75 7365 7262 6172  ailadmin/userbar
+00000020: 2f69 7465 6d5f 6261 7365 2e68 746d 6c22  /item_base.html"
+00000030: 2025 7d0d 0a7b 2520 6c6f 6164 2069 3138   %}..{% load i18
+00000040: 6e20 7761 6774 6169 6c61 646d 696e 5f74  n wagtailadmin_t
+00000050: 6167 7320 257d 0d0a 0d0a 7b25 2062 6c6f  ags %}....{% blo
+00000060: 636b 2069 7465 6d5f 636f 6e74 656e 7420  ck item_content 
+00000070: 257d 0d0a 2020 2020 3c61 2068 7265 663d  %}..    <a href=
+00000080: 227b 7b20 6c69 7665 5f75 726c 7c73 6166  "{{ live_url|saf
+00000090: 6520 7d7d 2220 7461 7267 6574 3d22 5f73  e }}" target="_s
+000000a0: 656c 6622 2072 6f6c 653d 226d 656e 7569  elf" role="menui
+000000b0: 7465 6d22 2069 643d 2277 6167 7461 696c  tem" id="wagtail
+000000c0: 2d66 6564 6974 2d6c 6976 652d 6275 7474  -fedit-live-butt
+000000d0: 6f6e 223e 0d0a 2020 2020 2020 2020 3c73  on">..        <s
+000000e0: 7667 2078 6d6c 6e73 3d22 6874 7470 3a2f  vg xmlns="http:/
+000000f0: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
+00000100: 2f73 7667 2220 6669 6c6c 3d22 6375 7272  /svg" fill="curr
+00000110: 656e 7443 6f6c 6f72 2220 636c 6173 733d  entColor" class=
+00000120: 2277 2d61 6374 696f 6e2d 6963 6f6e 2220  "w-action-icon" 
+00000130: 7669 6577 426f 783d 2230 2030 2031 3620  viewBox="0 0 16 
+00000140: 3136 223e 0d0a 2020 2020 2020 2020 2020  16">..          
+00000150: 2020 3c21 2d2d 2054 6865 204d 4954 204c    <!-- The MIT L
+00000160: 6963 656e 7365 2028 4d49 5429 202d 2d3e  icense (MIT) -->
+00000170: 0d0a 2020 2020 2020 2020 2020 2020 3c21  ..            <!
+00000180: 2d2d 2043 6f70 7972 6967 6874 2028 6329  -- Copyright (c)
+00000190: 2032 3031 312d 3230 3234 2054 6865 2042   2011-2024 The B
+000001a0: 6f6f 7473 7472 6170 2041 7574 686f 7273  ootstrap Authors
+000001b0: 202d 2d3e 0d0a 2020 2020 2020 2020 2020   -->..          
+000001c0: 2020 3c70 6174 6820 643d 226d 372e 3634    <path d="m7.64
+000001d0: 3620 392e 3335 342d 332e 3739 3220 332e  6 9.354-3.792 3.
+000001e0: 3739 3261 2e35 2e35 2030 2030 2030 202e  792a.5.5 0 0 0 .
+000001f0: 3335 332e 3835 3468 372e 3538 3661 2e35  353.854h7.586a.5
+00000200: 2e35 2030 2030 2030 202e 3335 342d 2e38  .5 0 0 0 .354-.8
+00000210: 3534 4c38 2e33 3534 2039 2e33 3534 612e  54L8.354 9.354a.
+00000220: 352e 3520 3020 3020 302d 2e37 3038 2030  5.5 0 0 0-.708 0
+00000230: 222f 3e0d 0a20 2020 2020 2020 2020 2020  "/>..           
+00000240: 203c 7061 7468 2064 3d22 4d31 312e 3431   <path d="M11.41
+00000250: 3420 3131 4831 342e 3561 2e35 2e35 2030  4 11H14.5a.5.5 0
+00000260: 2030 2030 202e 352d 2e35 762d 3761 2e35   0 0 .5-.5v-7a.5
+00000270: 2e35 2030 2030 2030 2d2e 352d 2e35 682d  .5 0 0 0-.5-.5h-
+00000280: 3133 612e 352e 3520 3020 3020 302d 2e35  13a.5.5 0 0 0-.5
+00000290: 2e35 7637 612e 352e 3520 3020 3020 3020  .5v7a.5.5 0 0 0 
+000002a0: 2e35 2e35 6833 2e30 3836 6c2d 3120 3148  .5.5h3.086l-1 1H
+000002b0: 312e 3541 312e 3520 312e 3520 3020 3020  1.5A1.5 1.5 0 0 
+000002c0: 3120 3020 3130 2e35 762d 3741 312e 3520  1 0 10.5v-7A1.5 
+000002d0: 312e 3520 3020 3020 3120 312e 3520 3268  1.5 0 0 1 1.5 2h
+000002e0: 3133 4131 2e35 2031 2e35 2030 2030 2031  13A1.5 1.5 0 0 1
+000002f0: 2031 3620 332e 3576 3761 312e 3520 312e   16 3.5v7a1.5 1.
+00000300: 3520 3020 3020 312d 312e 3520 312e 3568  5 0 0 1-1.5 1.5h
+00000310: 2d32 2e30 3836 7a22 2f3e 0d0a 2020 2020  -2.086z"/>..    
+00000320: 2020 2020 2020 3c2f 7376 673e 0d0a 2020        </svg>..  
+00000330: 2020 2020 2020 7b25 2074 7261 6e73 2027        {% trans '
+00000340: 5669 6577 204c 6976 6520 5061 6765 2720  View Live Page' 
+00000350: 257d 0d0a 2020 2020 3c2f 613e 0d0a 7b25  %}..    </a>..{%
+00000360: 2065 6e64 626c 6f63 6b20 257d             endblock %}
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files 8% similar despite different names*

```diff
@@ -30,21 +30,23 @@
                                     <td>
                                         {% if entry.revision %}<span class="report__results--text">{% endif %}
                                         {{ entry.message }}
                                         {% if entry.revision %}</span>{% endif %}
                                         {% if entry.comment %}
                                             <span class="report__results--comment">{% trans "Comment" %}: <em>{{ entry.comment }}</em></span>
                                         {% endif %}
-                                        {% if entry.revision and entry.content_changed and is_page %}
+                                        {% if entry.revision and entry.content_changed and LOG_ACTION_TEMPLATES_AVAILABLE %}
                                             {% if entry.revision == view.object.latest_revision %}{% trans 'Current draft' as status_label %}{% status status_label classname="w-status--primary" %}{% endif %}
                                             {% include "wagtailadmin/pages/revisions/_actions.html" with revision=entry.revision page=view.object %}
                                         {% endif %}
                                     </td>
                                 {% else %}
-                                    {% include "wagtailsnippets/snippets/revisions/_actions.html" with instance=entry value=entry.message object=view.object revision_enabled=True can_publish=True draftstate_enabled=True %}
+                                    <td>
+
+                                    </td>
                                 {% endif %}
                                 <td>
                                     {% include "wagtailadmin/shared/user_avatar.html" with user=entry.user username=entry.user_display_name %}
                                 </td>
                                 <td class="updated">{% human_readable_date entry.timestamp %}</td>
                             </tr>
                         {% endfor %}
```

#### html2text {}

```diff
@@ -1,33 +1,32 @@
 {% extends "./action_confirm.html" %} {% load i18n wagtailadmin_tags %} {%
 block form_content %} {% if log_entries %}
 {% translate "Changes since last publish" as panel_heading %} {% panel
 id="wagtail-fedit-log-actions" icon="draft" heading=panel_heading %}
-{{%% ttrraannss ''AAccttiioonn'' %%}}        {{%% ttrraannss ''UUsseerr'' %%}}               {{%% ttrraannss ''DDaattee //
-                                                             TTiimmee'' %%}}
+                               {{%%
+{{%% ttrraannss ''AAccttiioonn'' %%}}           ttrraannss  {{%% ttrraannss ''DDaattee // TTiimmee'' %%}}
+                               ''UUsseerr''
+                               %%}}
 {% if entry.revision %}{%
-endif %} {{ entry.message
-}} {% if entry.revision %}
-{% endif %} {% if
-entry.comment %} {% trans
-"Comment" %}: {{
-{{ eennttrryy..ccoommmmeenntt }}}} {% endif
-%} {% if entry.revision and
-entry.content_changed and
-is_page %} {% if            {% include "wagtailadmin/shared/
-entry.revision ==           user_avatar.html" with           {%
-view.object.latest_revision user=entry.user                  human_readable_date
-%}{% trans 'Current draft'  username=entry.user_display_name entry.timestamp %}
-as status_label %}{% status %}
+endif %} {{ entry.message }}
+{% if entry.revision %}{%
+endif %} {% if entry.comment
+%} {% trans "Comment" %}: {{
+{{ eennttrryy..ccoommmmeenntt }}}} {% endif %}
+{% if entry.revision and
+entry.content_changed and             {% include "wagtailadmin/shared/
+LOG_ACTION_TEMPLATES_AVAILABLE        user_avatar.html" with           {%
+%} {% if entry.revision ==            user=entry.user                  human_readable_date
+view.object.latest_revision %}        username=entry.user_display_name entry.timestamp %}
+{% trans 'Current draft' as           %}
+status_label %}{% status
 status_label classname="w-
-status--primary" %}{% endif
-%} {% include
-"wagtailadmin/pages/
-revisions/_actions.html"
-with
-revision=entry.revision
-page=view.object %} {%
-endif %}
-{% blocktrans trimmed with view_more_url=view_more_url%} This object has more
-changes. _V_i_e_w_ _a_l_l_ _c_h_a_n_g_e_s_. {% endblocktrans %}
+status--primary" %}{% endif %}
+{% include "wagtailadmin/
+pages/revisions/_actions.html"
+with revision=entry.revision
+page=view.object %} {% endif
+%}
+{% blocktrans trimmed with view_more_url=view_more_url%} This object
+has more changes. _V_i_e_w_ _a_l_l_ _c_h_a_n_g_e_s_. {% endblocktrans %}
 {% endpanel %}
 {% endif %} {{ block.super }} {% endblock %}
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,34 +1,35 @@
 magic:    0xa70d0d0a
-moddate:  0x4b342166 (Thu Apr 18 14:55:07 2024 UTC)
-files sz: 6749
+moddate:  0x03ca2266 (Fri Apr 19 19:46:11 2024 UTC)
+files sz: 7503
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 9
+   stacksize : 11
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
       055a050100640064036c066d075a070100640064046c086d095a096d0a5a
       0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f01
       00640064076c106d115a110100640064086c126d135a130100640064096c
       145a14640a640b6c156d165a166d175a176d185a186d195a190100640a64
-      0c6c1a6d1b5a1b6d1c5a1c6d1d5a1d0100640a640d6c136d1e5a1e6d1f5a
-      1f0100020065036a200000000000000000a6000000ab0000000000000000
-      005a21640e5a22640f5a23020047006410840064116504a6030000ab0300
-      000000000000005a246521a0250000000000000000000000000000000000
-      0000006412ac13a6010000ab010000000000000000641465096415650a66
-      0464168404a6000000ab0000000000000000005a266521a0270000000000
-      0000000000000000000000000000006417ac18a6010000ab010000000000
-      00000064196507641a6518641b65286606641c8404a6000000ab00000000
-      00000000005a296521a02a00000000000000000000000000000000000000
-      00641d641e6417ac1fa6030000ab030000000000000000641b652b660264
-      208404a6000000ab0000000000000000005a2c6424641465096421652d65
-      28190000000000000000006422652d652819000000000000000000641b65
-      2b6608642384055a2e64095300
+      0c6c1a6d1b5a1b6d1c5a1c6d1d5a1d6d1e5a1e0100640a640d6c136d1f5a
+      1f6d205a200100020065036a210000000000000000a6000000ab00000000
+      00000000005a22640e5a23640f5a24020047006410840064116504a60300
+      00ab0300000000000000005a256522a02600000000000000000000000000
+      00000000000000651eac12a6010000ab0100000000000000006413650964
+      14650a660464158404a6000000ab0000000000000000005a276522a02800
+      000000000000000000000000000000000000006416ac17a6010000ab0100
+      000000000000006418650764196518641a65296606641b8404a6000000ab
+      0000000000000000005a2a6522a02b000000000000000000000000000000
+      0000000000641c641d6416ac1ea6030000ab030000000000000000641a65
+      2c6602641f8404a6000000ab0000000000000000005a2d64246413650964
+      20652e6529190000000000000000006421652e6529190000000000000000
+      006422652e652919000000000000000000641a652c660a642384055a2f64
+      095300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Type',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Type)
                 10 STORE_NAME               1 (Type)
@@ -106,197 +107,203 @@
                136 IMPORT_FROM             24 (BaseAdapter)
                138 STORE_NAME              24 (BaseAdapter)
                140 IMPORT_FROM             25 (AdapterError)
                142 STORE_NAME              25 (AdapterError)
                144 POP_TOP
    
     26         146 LOAD_CONST              10 (2)
-               148 LOAD_CONST              12 (('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR'))
+               148 LOAD_CONST              12 (('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME'))
                150 IMPORT_NAME             26 (utils)
                152 IMPORT_FROM             27 (wrap_adapter)
                154 STORE_NAME              27 (wrap_adapter)
                156 IMPORT_FROM             28 (_can_edit)
                158 STORE_NAME              28 (_can_edit)
                160 IMPORT_FROM             29 (FEDIT_PREVIEW_VAR)
                162 STORE_NAME              29 (FEDIT_PREVIEW_VAR)
-               164 POP_TOP
-   
-    31         166 LOAD_CONST              10 (2)
-               168 LOAD_CONST              13 (('REGISTER_CSS', 'REGISTER_JS'))
-               170 IMPORT_NAME             19 (hooks)
-               172 IMPORT_FROM             30 (REGISTER_CSS)
-               174 STORE_NAME              30 (REGISTER_CSS)
-               176 IMPORT_FROM             31 (REGISTER_JS)
-               178 STORE_NAME              31 (REGISTER_JS)
-               180 POP_TOP
-   
-    37         182 PUSH_NULL
-               184 LOAD_NAME                3 (library)
-               186 LOAD_ATTR               32 (Library)
-               196 PRECALL                  0
-               200 CALL                     0
-               210 STORE_NAME              33 (register)
-   
-    40         212 LOAD_CONST              14 ('Field name is not available in the context for %(object)s.')
-               214 STORE_NAME              34 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-   
-    41         216 LOAD_CONST              15 ('Model instance is not available in the context for %(object)s.')
-               218 STORE_NAME              35 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-   
-    45         220 PUSH_NULL
-               222 LOAD_BUILD_CLASS
-               224 LOAD_CONST              16 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 45>)
-               226 MAKE_FUNCTION            0
-               228 LOAD_CONST              17 ('AdapterNode')
-               230 LOAD_NAME                4 (Node)
-               232 PRECALL                  3
-               236 CALL                     3
-               246 STORE_NAME              36 (AdapterNode)
-   
-   122         248 LOAD_NAME               33 (register)
-               250 LOAD_METHOD             37 (tag)
-               272 LOAD_CONST              18 ('fedit')
-               274 KW_NAMES                19
-               276 PRECALL                  1
-               280 CALL                     1
-   
-   123         290 LOAD_CONST              20 ('parser')
-               292 LOAD_NAME                9 (Parser)
-               294 LOAD_CONST              21 ('token')
-               296 LOAD_NAME               10 (Token)
-               298 BUILD_TUPLE              4
-               300 LOAD_CONST              22 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 122>)
-               302 MAKE_FUNCTION            4 (annotations)
-   
-   122         304 PRECALL                  0
-               308 CALL                     0
-   
-   123         318 STORE_NAME              38 (do_render_fedit)
-   
-   162         320 LOAD_NAME               33 (register)
-               322 LOAD_METHOD             39 (simple_tag)
-               344 LOAD_CONST              23 (True)
-               346 KW_NAMES                24
-               348 PRECALL                  1
-               352 CALL                     1
-   
-   163         362 LOAD_CONST              25 ('context')
-               364 LOAD_NAME                7 (Context)
-               366 LOAD_CONST              26 ('adapter')
-               368 LOAD_NAME               24 (BaseAdapter)
-               370 LOAD_CONST              27 ('return')
-               372 LOAD_NAME               40 (str)
-               374 BUILD_TUPLE              6
-               376 LOAD_CONST              28 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 162>)
-               378 MAKE_FUNCTION            4 (annotations)
-   
-   162         380 PRECALL                  0
-               384 CALL                     0
-   
-   163         394 STORE_NAME              41 (render_adapter)
-   
-   179         396 LOAD_NAME               33 (register)
-               398 LOAD_METHOD             42 (inclusion_tag)
-               420 LOAD_CONST              29 ('wagtail_fedit/_hook_output.html')
-               422 LOAD_CONST              30 ('fedit_scripts')
-               424 LOAD_CONST              23 (True)
-               426 KW_NAMES                31
-               428 PRECALL                  3
-               432 CALL                     3
-   
-   180         442 LOAD_CONST              27 ('return')
-               444 LOAD_NAME               43 (dict)
-               446 BUILD_TUPLE              2
-               448 LOAD_CONST              32 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 179>)
-               450 MAKE_FUNCTION            4 (annotations)
-   
-   179         452 PRECALL                  0
-               456 CALL                     0
-   
-   180         466 STORE_NAME              44 (static_hook_output)
-   
-   210         468 LOAD_CONST              36 ((None,))
-               470 LOAD_CONST              20 ('parser')
-               472 LOAD_NAME                9 (Parser)
-               474 LOAD_CONST              33 ('tokens')
-               476 LOAD_NAME               45 (list)
-               478 LOAD_NAME               40 (str)
-               480 BINARY_SUBSCR
-               490 LOAD_CONST              34 ('kwarg_list')
-               492 LOAD_NAME               45 (list)
-               494 LOAD_NAME               40 (str)
-               496 BINARY_SUBSCR
-               506 LOAD_CONST              27 ('return')
-               508 LOAD_NAME               43 (dict)
-               510 BUILD_TUPLE              8
-               512 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 210>)
-               514 MAKE_FUNCTION            5 (defaults, annotations)
-               516 STORE_NAME              46 (get_kwargs)
-               518 LOAD_CONST               9 (None)
-               520 RETURN_VALUE
+               164 IMPORT_FROM             30 (TEMPLATE_TAG_NAME)
+               166 STORE_NAME              30 (TEMPLATE_TAG_NAME)
+               168 POP_TOP
+   
+    32         170 LOAD_CONST              10 (2)
+               172 LOAD_CONST              13 (('REGISTER_CSS', 'REGISTER_JS'))
+               174 IMPORT_NAME             19 (hooks)
+               176 IMPORT_FROM             31 (REGISTER_CSS)
+               178 STORE_NAME              31 (REGISTER_CSS)
+               180 IMPORT_FROM             32 (REGISTER_JS)
+               182 STORE_NAME              32 (REGISTER_JS)
+               184 POP_TOP
+   
+    38         186 PUSH_NULL
+               188 LOAD_NAME                3 (library)
+               190 LOAD_ATTR               33 (Library)
+               200 PRECALL                  0
+               204 CALL                     0
+               214 STORE_NAME              34 (register)
+   
+    41         216 LOAD_CONST              14 ('Field name is not available in the context for %(object)s.')
+               218 STORE_NAME              35 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+   
+    42         220 LOAD_CONST              15 ('Model instance is not available in the context for %(object)s.')
+               222 STORE_NAME              36 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+   
+    46         224 PUSH_NULL
+               226 LOAD_BUILD_CLASS
+               228 LOAD_CONST              16 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 46>)
+               230 MAKE_FUNCTION            0
+               232 LOAD_CONST              17 ('AdapterNode')
+               234 LOAD_NAME                4 (Node)
+               236 PRECALL                  3
+               240 CALL                     3
+               250 STORE_NAME              37 (AdapterNode)
+   
+   123         252 LOAD_NAME               34 (register)
+               254 LOAD_METHOD             38 (tag)
+               276 LOAD_NAME               30 (TEMPLATE_TAG_NAME)
+               278 KW_NAMES                18
+               280 PRECALL                  1
+               284 CALL                     1
+   
+   124         294 LOAD_CONST              19 ('parser')
+               296 LOAD_NAME                9 (Parser)
+               298 LOAD_CONST              20 ('token')
+               300 LOAD_NAME               10 (Token)
+               302 BUILD_TUPLE              4
+               304 LOAD_CONST              21 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 123>)
+               306 MAKE_FUNCTION            4 (annotations)
+   
+   123         308 PRECALL                  0
+               312 CALL                     0
+   
+   124         322 STORE_NAME              39 (do_render_fedit)
+   
+   168         324 LOAD_NAME               34 (register)
+               326 LOAD_METHOD             40 (simple_tag)
+               348 LOAD_CONST              22 (True)
+               350 KW_NAMES                23
+               352 PRECALL                  1
+               356 CALL                     1
+   
+   169         366 LOAD_CONST              24 ('context')
+               368 LOAD_NAME                7 (Context)
+               370 LOAD_CONST              25 ('adapter')
+               372 LOAD_NAME               24 (BaseAdapter)
+               374 LOAD_CONST              26 ('return')
+               376 LOAD_NAME               41 (str)
+               378 BUILD_TUPLE              6
+               380 LOAD_CONST              27 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 168>)
+               382 MAKE_FUNCTION            4 (annotations)
+   
+   168         384 PRECALL                  0
+               388 CALL                     0
+   
+   169         398 STORE_NAME              42 (render_adapter)
+   
+   185         400 LOAD_NAME               34 (register)
+               402 LOAD_METHOD             43 (inclusion_tag)
+               424 LOAD_CONST              28 ('wagtail_fedit/_hook_output.html')
+               426 LOAD_CONST              29 ('fedit_scripts')
+               428 LOAD_CONST              22 (True)
+               430 KW_NAMES                30
+               432 PRECALL                  3
+               436 CALL                     3
+   
+   186         446 LOAD_CONST              26 ('return')
+               448 LOAD_NAME               44 (dict)
+               450 BUILD_TUPLE              2
+               452 LOAD_CONST              31 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 185>)
+               454 MAKE_FUNCTION            4 (annotations)
+   
+   185         456 PRECALL                  0
+               460 CALL                     0
+   
+   186         470 STORE_NAME              45 (static_hook_output)
+   
+   216         472 LOAD_CONST              36 ((None, None))
+               474 LOAD_CONST              19 ('parser')
+               476 LOAD_NAME                9 (Parser)
+               478 LOAD_CONST              32 ('tokens')
+               480 LOAD_NAME               46 (list)
+               482 LOAD_NAME               41 (str)
+               484 BINARY_SUBSCR
+               494 LOAD_CONST              33 ('kwarg_list')
+               496 LOAD_NAME               46 (list)
+               498 LOAD_NAME               41 (str)
+               500 BINARY_SUBSCR
+               510 LOAD_CONST              34 ('absolute_tokens')
+               512 LOAD_NAME               46 (list)
+               514 LOAD_NAME               41 (str)
+               516 BINARY_SUBSCR
+               526 LOAD_CONST              26 ('return')
+               528 LOAD_NAME               44 (dict)
+               530 BUILD_TUPLE             10
+               532 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 216>)
+               534 MAKE_FUNCTION            5 (defaults, annotations)
+               536 STORE_NAME              47 (get_kwargs)
+               538 LOAD_CONST               9 (None)
+               540 RETURN_VALUE
    consts
       0
       ('Type',)
       ('library', 'Node', 'TemplateSyntaxError')
       ('Context',)
       ('Parser', 'Token', 'FilterExpression')
       ('HttpRequest',)
       ('reverse',)
       ('signing',)
       ('hooks',)
       None
       2
       ('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError')
-      ('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR')
+      ('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME')
       ('REGISTER_CSS', 'REGISTER_JS')
       'Field name is not available in the context for %(object)s.'
       'Model instance is not available in the context for %(object)s.'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a02020065036a040000000000000000a6000000ab
             0000000000000000005a0564016506650719000000000000000000640265
             0864036509650a190000000000000000006606640484045a0b640584005a
             0c640684005a0d64075300
-          45           0 RESUME                   0
+          46           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdapterNode')
                        8 STORE_NAME               2 (__qualname__)
          
-          46          10 PUSH_NULL
+          47          10 PUSH_NULL
                       12 LOAD_NAME                3 (signing)
                       14 LOAD_ATTR                4 (TimestampSigner)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_NAME               5 (signer)
          
-          48          40 LOAD_CONST               1 ('adapter')
+          49          40 LOAD_CONST               1 ('adapter')
                       42 LOAD_NAME                6 (Type)
                       44 LOAD_NAME                7 (BaseAdapter)
                       46 BINARY_SUBSCR
                       56 LOAD_CONST               2 ('model')
                       58 LOAD_NAME                8 (FilterExpression)
                       60 LOAD_CONST               3 ('getters')
                       62 LOAD_NAME                9 (list)
                       64 LOAD_NAME               10 (str)
                       66 BINARY_SUBSCR
                       76 BUILD_TUPLE              6
-                      78 LOAD_CONST               4 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 48>)
+                      78 LOAD_CONST               4 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 49>)
                       80 MAKE_FUNCTION            4 (annotations)
                       82 STORE_NAME              11 (__init__)
          
-          54          84 LOAD_CONST               5 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 54>)
+          55          84 LOAD_CONST               5 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 55>)
                       86 MAKE_FUNCTION            0
                       88 STORE_NAME              12 (_resolve_expressions)
          
-          64          90 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 64>)
+          65          90 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 65>)
                       92 MAKE_FUNCTION            0
                       94 STORE_NAME              13 (render)
                       96 LOAD_CONST               7 (None)
                       98 RETURN_VALUE
          consts
             'AdapterNode'
             'adapter'
@@ -307,42 +314,42 @@
                nlocals   : 5
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   007c037c005f0200000000000000007c047c005f03000000000000000064
                   005300
-                48           0 RESUME                   0
+                49           0 RESUME                   0
                
-                49           2 LOAD_FAST                1 (adapter)
+                50           2 LOAD_FAST                1 (adapter)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (adapter)
                
-                50          16 LOAD_FAST                2 (model)
+                51          16 LOAD_FAST                2 (model)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (model)
                
-                51          30 LOAD_FAST                3 (getters)
+                52          30 LOAD_FAST                3 (getters)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (getters)
                
-                52          44 LOAD_FAST                4 (kwargs)
+                53          44 LOAD_FAST                4 (kwargs)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (kwargs)
                             58 LOAD_CONST               0 (None)
                             60 RETURN_VALUE
                consts
                   None
                names      ('adapter', 'model', 'getters', 'kwargs')
                varnames   ('self', 'adapter', 'model', 'getters', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 48
+               firstlineno 49
                lnotab 0x02010e010e010e01
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
                flags     : 11
                code
@@ -350,70 +357,70 @@
                   00ab00000000000000000044005d325c0200007d047d0574030000000000
                   00000000007c05740400000000000000000000a6020000ab020000000000
                   00000072187c05a00300000000000000000000000000000000000000007c
                   01a6010000ab0100000000000000007c037c043c0000008c337403000000
                   000000000000007c02740400000000000000000000a6020000ab02000000
                   000000000072157c02a00300000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d027c027c0366025300
-                54           0 RESUME                   0
+                55           0 RESUME                   0
                
-                55           2 LOAD_FAST                3 (kwargs)
+                56           2 LOAD_FAST                3 (kwargs)
                              4 LOAD_METHOD              0 (items)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 GET_ITER
                        >>   42 FOR_ITER                50 (to 144)
                             44 UNPACK_SEQUENCE          2
                             48 STORE_FAST               4 (k)
                             50 STORE_FAST               5 (v)
                
-                56          52 LOAD_GLOBAL              3 (NULL + isinstance)
+                57          52 LOAD_GLOBAL              3 (NULL + isinstance)
                             64 LOAD_FAST                5 (v)
                             66 LOAD_GLOBAL              4 (FilterExpression)
                             78 PRECALL                  2
                             82 CALL                     2
                             92 POP_JUMP_FORWARD_IF_FALSE    24 (to 142)
                
-                57          94 LOAD_FAST                5 (v)
+                58          94 LOAD_FAST                5 (v)
                             96 LOAD_METHOD              3 (resolve)
                            118 LOAD_FAST                1 (context)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 LOAD_FAST                3 (kwargs)
                            136 LOAD_FAST                4 (k)
                            138 STORE_SUBSCR
                        >>  142 JUMP_BACKWARD           51 (to 42)
                
-                59     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
+                60     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
                            156 LOAD_FAST                2 (model)
                            158 LOAD_GLOBAL              4 (FilterExpression)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 POP_JUMP_FORWARD_IF_FALSE    21 (to 228)
                
-                60         186 LOAD_FAST                2 (model)
+                61         186 LOAD_FAST                2 (model)
                            188 LOAD_METHOD              3 (resolve)
                            210 LOAD_FAST                1 (context)
                            212 PRECALL                  1
                            216 CALL                     1
                            226 STORE_FAST               2 (model)
                
-                62     >>  228 LOAD_FAST                2 (model)
+                63     >>  228 LOAD_FAST                2 (model)
                            230 LOAD_FAST                3 (kwargs)
                            232 BUILD_TUPLE              2
                            234 RETURN_VALUE
                consts
                   None
                names      ('items', 'isinstance', 'FilterExpression', 'resolve')
                varnames   ('self', 'context', 'model', 'kwargs', 'k', 'v')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '_resolve_expressions'
-               firstlineno 54
+               firstlineno 55
                lnotab 0x020132012a0132022a012a02
             code
                argcount  : 2
                nlocals   : 12
                stacksize : 8
                flags     : 3
                code
@@ -443,254 +450,254 @@
                   00ab0100000000000000007d0a02007c006a07000000000000000064097c
                   067c057c0a64089c037c04a4018e017d0b7c0ba015000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007210742d00
                   0000000000000000007c0a7c06a6020000ab02000000000000000073157c
                   0ba01700000000000000000000000000000000000000007c01a6010000ab
                   01000000000000000053007431000000000000000000007c0a7c0b7c01a6
                   030000ab0300000000000000005300
-                64           0 RESUME                   0
+                65           0 RESUME                   0
                
-                65           2 LOAD_FAST                0 (self)
+                66           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (model)
                             14 STORE_FAST               2 (model)
                
-                66          16 LOAD_FAST                0 (self)
+                67          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (getters)
                             28 STORE_FAST               3 (getters)
                
-                68          30 PUSH_NULL
+                69          30 PUSH_NULL
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                2 (_resolve_expressions)
                
-                69          44 LOAD_FAST                1 (context)
+                70          44 LOAD_FAST                1 (context)
                             46 LOAD_FAST                2 (model)
                
-                68          48 BUILD_TUPLE              2
+                69          48 BUILD_TUPLE              2
                             50 BUILD_MAP                0
                
-                69          52 LOAD_FAST                0 (self)
+                70          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (kwargs)
                
-                68          64 DICT_MERGE               1
+                69          64 DICT_MERGE               1
                             66 CALL_FUNCTION_EX         1
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               2 (model)
                             74 STORE_FAST               4 (kwargs)
                
-                72          76 LOAD_CONST               1 ('wagtail_fedit_field')
+                73          76 LOAD_CONST               1 ('wagtail_fedit_field')
                             78 LOAD_FAST                1 (context)
                             80 CONTAINS_OP              0
                             82 POP_JUMP_FORWARD_IF_FALSE    24 (to 132)
                
-                73          84 LOAD_CONST               2 ('wagtail_fedit_instance')
+                74          84 LOAD_CONST               2 ('wagtail_fedit_instance')
                             86 LOAD_FAST                1 (context)
                             88 CONTAINS_OP              0
                             90 POP_JUMP_FORWARD_IF_FALSE    20 (to 132)
                
-                74          92 LOAD_FAST                2 (model)
+                75          92 LOAD_FAST                2 (model)
                
-                73          94 POP_JUMP_FORWARD_IF_TRUE    18 (to 132)
+                74          94 POP_JUMP_FORWARD_IF_TRUE    18 (to 132)
                
-                76          96 LOAD_FAST                1 (context)
+                77          96 LOAD_FAST                1 (context)
                             98 LOAD_CONST               1 ('wagtail_fedit_field')
                            100 BINARY_SUBSCR
                            110 STORE_FAST               5 (field_name)
                
-                77         112 LOAD_FAST                1 (context)
+                78         112 LOAD_FAST                1 (context)
                            114 LOAD_CONST               2 ('wagtail_fedit_instance')
                            116 BINARY_SUBSCR
                            126 STORE_FAST               6 (obj)
                            128 EXTENDED_ARG             1
                            130 JUMP_FORWARD           264 (to 660)
                
-                81     >>  132 LOAD_FAST                2 (model)
+                82     >>  132 LOAD_FAST                2 (model)
                            134 POP_JUMP_FORWARD_IF_TRUE   132 (to 400)
                
-                82         136 LOAD_GLOBAL              9 (NULL + warnings)
+                83         136 LOAD_GLOBAL              9 (NULL + warnings)
                            148 LOAD_ATTR                5 (warn)
                
-                83         158 LOAD_GLOBAL             12 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+                84         158 LOAD_GLOBAL             12 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
                
-                84         170 LOAD_CONST               3 ('object')
+                85         170 LOAD_CONST               3 ('object')
                            172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                7 (adapter)
                            184 LOAD_ATTR                8 (__name__)
                
-                83         194 BUILD_MAP                1
+                84         194 BUILD_MAP                1
                            196 BINARY_OP                6 (%)
                
-                86         200 LOAD_GLOBAL             18 (RuntimeWarning)
+                87         200 LOAD_GLOBAL             18 (RuntimeWarning)
                
-                82         212 PRECALL                  2
+                83         212 PRECALL                  2
                            216 CALL                     2
                            226 POP_TOP
                
-                89         228 LOAD_FAST                1 (context)
+                90         228 LOAD_FAST                1 (context)
                            230 LOAD_METHOD             10 (flatten)
                            252 PRECALL                  0
                            256 CALL                     0
                            266 STORE_FAST               1 (context)
                
-                91         268 NOP
+                92         268 NOP
                
-                92         270 PUSH_NULL
+                93         270 PUSH_NULL
                            272 LOAD_FAST                0 (self)
                            274 LOAD_ATTR                7 (adapter)
                            284 LOAD_ATTR               11 (render_from_kwargs)
                
-                93         294 LOAD_FAST                1 (context)
+                94         294 LOAD_FAST                1 (context)
                
-                92         296 BUILD_TUPLE              1
+                93         296 BUILD_TUPLE              1
                            298 BUILD_MAP                0
                
-                93         300 LOAD_FAST                4 (kwargs)
+                94         300 LOAD_FAST                4 (kwargs)
                
-                92         302 DICT_MERGE               1
+                93         302 DICT_MERGE               1
                            304 CALL_FUNCTION_EX         1
                            306 RETURN_VALUE
                        >>  308 PUSH_EXC_INFO
                
-                95         310 LOAD_GLOBAL             24 (AdapterError)
+                96         310 LOAD_GLOBAL             24 (AdapterError)
                            322 CHECK_EXC_MATCH
                            324 POP_JUMP_FORWARD_IF_FALSE    33 (to 392)
                            326 STORE_FAST               7 (e)
                
-                96         328 LOAD_GLOBAL             27 (NULL + TemplateSyntaxError)
+                97         328 LOAD_GLOBAL             27 (NULL + TemplateSyntaxError)
                            340 LOAD_GLOBAL             29 (NULL + str)
                            352 LOAD_FAST                7 (e)
                            354 PRECALL                  1
                            358 CALL                     1
                            368 PRECALL                  1
                            372 CALL                     1
                            382 RAISE_VARARGS            1
                        >>  384 LOAD_CONST               0 (None)
                            386 STORE_FAST               7 (e)
                            388 DELETE_FAST              7 (e)
                            390 RERAISE                  1
                
-                95     >>  392 RERAISE                  0
+                96     >>  392 RERAISE                  0
                        >>  394 COPY                     3
                            396 POP_EXCEPT
                            398 RERAISE                  1
                
-                98     >>  400 LOAD_FAST                3 (getters)
+                99     >>  400 LOAD_FAST                3 (getters)
                            402 LOAD_GLOBAL             31 (NULL + len)
                            414 LOAD_FAST                3 (getters)
                            416 PRECALL                  1
                            420 CALL                     1
                            430 LOAD_CONST               4 (1)
                            432 BINARY_OP               10 (-)
                            436 BINARY_SUBSCR
                            446 STORE_FAST               5 (field_name)
                
-                99         448 LOAD_FAST                2 (model)
+               100         448 LOAD_FAST                2 (model)
                            450 STORE_FAST               6 (obj)
                
-               100         452 LOAD_GLOBAL             33 (NULL + range)
+               101         452 LOAD_GLOBAL             33 (NULL + range)
                            464 LOAD_GLOBAL             31 (NULL + len)
                            476 LOAD_FAST                3 (getters)
                            478 PRECALL                  1
                            482 CALL                     1
                            492 LOAD_CONST               4 (1)
                            494 BINARY_OP               10 (-)
                            498 PRECALL                  1
                            502 CALL                     1
                            512 GET_ITER
                        >>  514 FOR_ITER                72 (to 660)
                            516 STORE_FAST               8 (i)
                
-               101         518 LOAD_FAST                3 (getters)
+               102         518 LOAD_FAST                3 (getters)
                            520 LOAD_FAST                8 (i)
                            522 BINARY_SUBSCR
                            532 STORE_FAST               9 (getter)
                
-               102         534 NOP
+               103         534 NOP
                
-               103         536 LOAD_GLOBAL             35 (NULL + getattr)
+               104         536 LOAD_GLOBAL             35 (NULL + getattr)
                            548 LOAD_FAST                6 (obj)
                            550 LOAD_FAST                9 (getter)
                            552 PRECALL                  2
                            556 CALL                     2
                            566 STORE_FAST               6 (obj)
                            568 JUMP_BACKWARD           28 (to 514)
                        >>  570 PUSH_EXC_INFO
                
-               104         572 LOAD_GLOBAL             36 (AttributeError)
+               105         572 LOAD_GLOBAL             36 (AttributeError)
                            584 CHECK_EXC_MATCH
                            586 POP_JUMP_FORWARD_IF_FALSE    32 (to 652)
                            588 POP_TOP
                
-               105         590 LOAD_GLOBAL             37 (NULL + AttributeError)
+               106         590 LOAD_GLOBAL             37 (NULL + AttributeError)
                            602 LOAD_CONST               5 ('Object ')
                            604 LOAD_FAST                2 (model)
                            606 LOAD_ATTR               19 (__class__)
                            616 LOAD_ATTR                8 (__name__)
                            626 FORMAT_VALUE             0
                            628 LOAD_CONST               6 (' does not have attribute ')
                            630 LOAD_FAST                9 (getter)
                            632 FORMAT_VALUE             0
                            634 BUILD_STRING             4
                            636 PRECALL                  1
                            640 CALL                     1
                            650 RAISE_VARARGS            1
                
-               104     >>  652 RERAISE                  0
+               105     >>  652 RERAISE                  0
                        >>  654 COPY                     3
                            656 POP_EXCEPT
                            658 RERAISE                  1
                
-               107     >>  660 LOAD_FAST                1 (context)
+               108     >>  660 LOAD_FAST                1 (context)
                            662 LOAD_METHOD             20 (get)
                            684 LOAD_CONST               7 ('request')
                            686 PRECALL                  1
                            690 CALL                     1
                            700 STORE_FAST              10 (request)
                
-               108         702 PUSH_NULL
+               109         702 PUSH_NULL
                            704 LOAD_FAST                0 (self)
                            706 LOAD_ATTR                7 (adapter)
                            716 LOAD_CONST               9 (())
                
-               109         718 LOAD_FAST                6 (obj)
+               110         718 LOAD_FAST                6 (obj)
                
-               110         720 LOAD_FAST                5 (field_name)
+               111         720 LOAD_FAST                5 (field_name)
                
-               111         722 LOAD_FAST               10 (request)
+               112         722 LOAD_FAST               10 (request)
                
-               108         724 LOAD_CONST               8 (('object', 'field_name', 'request'))
+               109         724 LOAD_CONST               8 (('object', 'field_name', 'request'))
                            726 BUILD_CONST_KEY_MAP      3
                
-               112         728 LOAD_FAST                4 (kwargs)
+               113         728 LOAD_FAST                4 (kwargs)
                
-               108         730 DICT_MERGE               1
+               109         730 DICT_MERGE               1
                            732 CALL_FUNCTION_EX         1
                            734 STORE_FAST              11 (adapter)
                
-               115         736 LOAD_FAST               11 (adapter)
+               116         736 LOAD_FAST               11 (adapter)
                            738 LOAD_METHOD             21 (check_permissions)
                            760 PRECALL                  0
                            764 CALL                     0
                            774 POP_JUMP_FORWARD_IF_FALSE    16 (to 808)
                
-               116         776 LOAD_GLOBAL             45 (NULL + _can_edit)
+               117         776 LOAD_GLOBAL             45 (NULL + _can_edit)
                            788 LOAD_FAST               10 (request)
                            790 LOAD_FAST                6 (obj)
                            792 PRECALL                  2
                            796 CALL                     2
                
-               115         806 POP_JUMP_FORWARD_IF_TRUE    21 (to 850)
+               116         806 POP_JUMP_FORWARD_IF_TRUE    21 (to 850)
                
-               117     >>  808 LOAD_FAST               11 (adapter)
+               118     >>  808 LOAD_FAST               11 (adapter)
                            810 LOAD_METHOD             23 (render_content)
                            832 LOAD_FAST                1 (context)
                            834 PRECALL                  1
                            838 CALL                     1
                            848 RETURN_VALUE
                
-               119     >>  850 LOAD_GLOBAL             49 (NULL + wrap_adapter)
+               120     >>  850 LOAD_GLOBAL             49 (NULL + wrap_adapter)
                            862 LOAD_FAST               10 (request)
                            864 LOAD_FAST               11 (adapter)
                            866 LOAD_FAST                1 (context)
                            868 PRECALL                  3
                            872 CALL                     3
                            882 RETURN_VALUE
                ExceptionTable:
@@ -713,31 +720,30 @@
                   ()
                names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'adapter', '__name__', 'RuntimeWarning', 'flatten', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'render_content', 'wrap_adapter')
                varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 64
+               firstlineno 65
                lnotab
                   0x02010e010e020e0104ff04010cff0c040801080102ff02031001140404
                   0116010c0118ff06030cfc100728020201180102ff040102ff0803120140
                   ff080330010401420110010201240112013eff08032a0110010201020102
                   fd040402fc060728011eff02022a02
             None
          names      ('__name__', '__module__', '__qualname__', 'signing', 'TimestampSigner', 'signer', 'Type', 'BaseAdapter', 'FilterExpression', 'list', 'str', '__init__', '_resolve_expressions', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'AdapterNode'
-         firstlineno 45
+         firstlineno 46
          lnotab 0x0a011e022c06060a
       'AdapterNode'
-      'fedit'
       ('name',)
       'parser'
       'token'
       code
          argcount  : 2
          nlocals   : 10
          stacksize : 7
@@ -757,158 +763,165 @@
             0000007c07a6010000ab01000000000000000064066b0000000000721b7c
             0764011900000000000000000064076b0300000000720f74090000000000
             00000000006408a6010000ab0100000000000000008201740d0000000000
             00000000007c07a6010000ab01000000000000000064096b040000000072
             287c00a00700000000000000000000000000000000000000007c07a00100
             000000000000000000000000000000000000006401a6010000ab01000000
             0000000000a6010000ab0100000000000000007d06741100000000000000
-            0000007c007c027c056a090000000000000000a6030000ab030000000000
-            0000007d09741500000000000000000000640b7c057c067c07640a9c037c
-            09a4018e015300
-         122           0 RESUME                   0
+            0000007c007c027c056a0900000000000000007c056a0a00000000000000
+            00a6040000ab0400000000000000007d0974170000000000000000000064
+            0b7c057c067c07640a9c037c09a4018e015300
+         123           0 RESUME                   0
          
-         125           2 LOAD_FAST                1 (token)
+         126           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         127          42 LOAD_FAST                2 (tokens)
+         128          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         128          84 LOAD_FAST                2 (tokens)
+         129          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (adapter_id)
          
-         130         126 NOP
+         131         126 NOP
          
-         131         128 LOAD_GLOBAL              4 (adapter_registry)
+         132         128 LOAD_GLOBAL              4 (adapter_registry)
                      140 LOAD_FAST                4 (adapter_id)
                      142 BINARY_SUBSCR
                      152 STORE_FAST               5 (adapter)
                      154 JUMP_FORWARD            33 (to 222)
                  >>  156 PUSH_EXC_INFO
          
-         132         158 LOAD_GLOBAL              6 (RegistryLookUpError)
+         133         158 LOAD_GLOBAL              6 (RegistryLookUpError)
                      170 CHECK_EXC_MATCH
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
                      174 POP_TOP
          
-         133         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         134         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
                      188 LOAD_CONST               2 ("No adapter found with identifier '")
                      190 LOAD_FAST                4 (adapter_id)
                      192 FORMAT_VALUE             0
                      194 LOAD_CONST               3 ("'")
                      196 BUILD_STRING             3
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         132     >>  214 RERAISE                  0
+         133     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         135     >>  222 LOAD_CONST               4 ((None, None))
+         136     >>  222 LOAD_CONST               4 ((None, None))
                      224 UNPACK_SEQUENCE          2
                      228 STORE_FAST               6 (model)
                      230 STORE_FAST               7 (model_tokens)
          
-         136         232 LOAD_FAST                2 (tokens)
+         137         232 LOAD_FAST                2 (tokens)
                      234 POP_JUMP_FORWARD_IF_FALSE   147 (to 530)
          
-         137         236 LOAD_FAST                2 (tokens)
+         138         236 LOAD_FAST                2 (tokens)
                      238 LOAD_METHOD              1 (pop)
                      260 LOAD_CONST               1 (0)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST               8 (model__field)
          
-         138         278 LOAD_FAST                8 (model__field)
+         139         278 LOAD_FAST                8 (model__field)
                      280 LOAD_METHOD              5 (split)
                      302 LOAD_CONST               5 ('.')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               7 (model_tokens)
          
-         140         320 LOAD_GLOBAL             13 (NULL + len)
+         141         320 LOAD_GLOBAL             13 (NULL + len)
                      332 LOAD_FAST                7 (model_tokens)
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_CONST               6 (2)
                      350 COMPARE_OP               0 (<)
                      356 POP_JUMP_FORWARD_IF_FALSE    27 (to 412)
          
-         141         358 LOAD_FAST                7 (model_tokens)
+         142         358 LOAD_FAST                7 (model_tokens)
                      360 LOAD_CONST               1 (0)
                      362 BINARY_SUBSCR
                      372 LOAD_CONST               7 ('from_context')
                      374 COMPARE_OP               3 (!=)
                      380 POP_JUMP_FORWARD_IF_FALSE    15 (to 412)
          
-         142         382 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         143         382 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
          
-         143         394 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
+         144         394 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
          
-         142         396 PRECALL                  1
+         143         396 PRECALL                  1
                      400 CALL                     1
                      410 RAISE_VARARGS            1
          
-         146     >>  412 LOAD_GLOBAL             13 (NULL + len)
+         147     >>  412 LOAD_GLOBAL             13 (NULL + len)
                      424 LOAD_FAST                7 (model_tokens)
                      426 PRECALL                  1
                      430 CALL                     1
                      440 LOAD_CONST               9 (1)
                      442 COMPARE_OP               4 (>)
                      448 POP_JUMP_FORWARD_IF_FALSE    40 (to 530)
          
-         149         450 LOAD_FAST                0 (parser)
+         150         450 LOAD_FAST                0 (parser)
                      452 LOAD_METHOD              7 (compile_filter)
                      474 LOAD_FAST                7 (model_tokens)
                      476 LOAD_METHOD              1 (pop)
                      498 LOAD_CONST               1 (0)
                      500 PRECALL                  1
                      504 CALL                     1
                      514 PRECALL                  1
                      518 CALL                     1
                      528 STORE_FAST               6 (model)
          
-         151     >>  530 LOAD_GLOBAL             17 (NULL + get_kwargs)
-                     542 LOAD_FAST                0 (parser)
-                     544 LOAD_FAST                2 (tokens)
-                     546 LOAD_FAST                5 (adapter)
+         152     >>  530 LOAD_GLOBAL             17 (NULL + get_kwargs)
+         
+         153         542 LOAD_FAST                0 (parser)
+         
+         154         544 LOAD_FAST                2 (tokens)
+         
+         155         546 LOAD_FAST                5 (adapter)
                      548 LOAD_ATTR                9 (required_kwargs)
-                     558 PRECALL                  3
-                     562 CALL                     3
-                     572 STORE_FAST               9 (kwargs)
          
-         153         574 LOAD_GLOBAL             21 (NULL + AdapterNode)
-                     586 LOAD_CONST              11 (())
+         156         558 LOAD_FAST                5 (adapter)
+                     560 LOAD_ATTR               10 (absolute_tokens)
+         
+         152         570 PRECALL                  4
+                     574 CALL                     4
+                     584 STORE_FAST               9 (kwargs)
+         
+         159         586 LOAD_GLOBAL             23 (NULL + AdapterNode)
+                     598 LOAD_CONST              11 (())
          
-         154         588 LOAD_FAST                5 (adapter)
+         160         600 LOAD_FAST                5 (adapter)
          
-         155         590 LOAD_FAST                6 (model)
+         161         602 LOAD_FAST                6 (model)
          
-         156         592 LOAD_FAST                7 (model_tokens)
+         162         604 LOAD_FAST                7 (model_tokens)
          
-         153         594 LOAD_CONST              10 (('adapter', 'model', 'getters'))
-                     596 BUILD_CONST_KEY_MAP      3
+         159         606 LOAD_CONST              10 (('adapter', 'model', 'getters'))
+                     608 BUILD_CONST_KEY_MAP      3
          
-         157         598 LOAD_FAST                9 (kwargs)
+         163         610 LOAD_FAST                9 (kwargs)
          
-         153         600 DICT_MERGE               1
-                     602 CALL_FUNCTION_EX         1
-                     604 RETURN_VALUE
+         159         612 DICT_MERGE               1
+                     614 CALL_FUNCTION_EX         1
+                     616 RETURN_VALUE
          ExceptionTable:
            128 to 152 -> 156 [0]
            156 to 214 -> 216 [1] lasti
          consts
             None
             0
             "No adapter found with identifier '"
@@ -917,24 +930,25 @@
             '.'
             2
             'from_context'
             "Model and field name are required: 'mymodel.myfield' or 'from_context'"
             1
             ('adapter', 'model', 'getters')
             ()
-         names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'compile_filter', 'get_kwargs', 'required_kwargs', 'AdapterNode')
+         names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'compile_filter', 'get_kwargs', 'required_kwargs', 'absolute_tokens', 'AdapterNode')
          varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit'
-         firstlineno 122
+         firstlineno 123
          lnotab
             0x020328022a012a0202011e01120126ff08030a0104012a012a02260118
-            010c0102ff1004260350022c020e010201020102fd040402fc
+            010c0102ff1004260350020c01020102010c010cfc10070e010201020102
+            fd040402fc
       True
       ('takes_context',)
       'context'
       'adapter'
       'return'
       code
          argcount  : 2
@@ -945,59 +959,59 @@
             0x970069007d0264017c007600720b7c006401190000000000000000007d
             027c0064013d007c00a00000000000000000000000000000000000000000
             007c02a6010000ab01000000000000000001007c016a0100000000000000
             007c0064023c0000007c016a0200000000000000007c0064033c0000007c
             016a0300000000000000007c0064043c0000007c01a00400000000000000
             000000000000000000000000007c00a6010000ab01000000000000000053
             00
-         162           0 RESUME                   0
+         168           0 RESUME                   0
          
-         164           2 BUILD_MAP                0
+         170           2 BUILD_MAP                0
                        4 STORE_FAST               2 (parent_context)
          
-         166           6 LOAD_CONST               1 ('parent_context')
+         172           6 LOAD_CONST               1 ('parent_context')
                        8 LOAD_FAST                0 (context)
                       10 CONTAINS_OP              0
                       12 POP_JUMP_FORWARD_IF_FALSE    11 (to 36)
          
-         167          14 LOAD_FAST                0 (context)
+         173          14 LOAD_FAST                0 (context)
                       16 LOAD_CONST               1 ('parent_context')
                       18 BINARY_SUBSCR
                       28 STORE_FAST               2 (parent_context)
          
-         168          30 LOAD_FAST                0 (context)
+         174          30 LOAD_FAST                0 (context)
                       32 LOAD_CONST               1 ('parent_context')
                       34 DELETE_SUBSCR
          
-         170     >>   36 LOAD_FAST                0 (context)
+         176     >>   36 LOAD_FAST                0 (context)
                       38 LOAD_METHOD              0 (update)
                       60 LOAD_FAST                2 (parent_context)
                       62 PRECALL                  1
                       66 CALL                     1
                       76 POP_TOP
          
-         172          78 LOAD_FAST                1 (adapter)
+         178          78 LOAD_FAST                1 (adapter)
                       80 LOAD_ATTR                1 (field_name)
                       90 LOAD_FAST                0 (context)
                       92 LOAD_CONST               2 ('wagtail_fedit_field')
                       94 STORE_SUBSCR
          
-         173          98 LOAD_FAST                1 (adapter)
+         179          98 LOAD_FAST                1 (adapter)
                      100 LOAD_ATTR                2 (object)
                      110 LOAD_FAST                0 (context)
                      112 LOAD_CONST               3 ('wagtail_fedit_instance')
                      114 STORE_SUBSCR
          
-         174         118 LOAD_FAST                1 (adapter)
+         180         118 LOAD_FAST                1 (adapter)
                      120 LOAD_ATTR                3 (request)
                      130 LOAD_FAST                0 (context)
                      132 LOAD_CONST               4 ('request')
                      134 STORE_SUBSCR
          
-         176         138 LOAD_FAST                1 (adapter)
+         182         138 LOAD_FAST                1 (adapter)
                      140 LOAD_METHOD              4 (render_content)
                      162 LOAD_FAST                0 (context)
                      164 PRECALL                  1
                      168 CALL                     1
                      178 RETURN_VALUE
          consts
             None
@@ -1007,15 +1021,15 @@
             'request'
          names      ('update', 'field_name', 'object', 'request', 'render_content')
          varnames   ('context', 'adapter', 'parent_context')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_adapter'
-         firstlineno 162
+         firstlineno 168
          lnotab 0x020204020801100106022a02140114011402
       'wagtail_fedit/_hook_output.html'
       'fedit_scripts'
       ('name', 'takes_context')
       code
          argcount  : 2
          nlocals   : 7
@@ -1032,107 +1046,107 @@
             00530067007d04740f000000000000000000006a0800000000000000007c
             03a6010000ab01000000000000000044005d417d0502007c057c02a60100
             00ab0100000000000000007d067413000000000000000000007c06741400
             0000000000000000007416000000000000000000006602a6020000ab0200
             0000000000000073037c0667017d067c04a00c0000000000000000000000
             0000000000000000007c06a6010000ab01000000000000000001008c4264
             067c0469015300
-         179           0 RESUME                   0
+         185           0 RESUME                   0
          
-         181           2 LOAD_FAST                1 (css_or_js)
+         187           2 LOAD_FAST                1 (css_or_js)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               1 (css_or_js)
          
-         183          42 LOAD_FAST                1 (css_or_js)
+         189          42 LOAD_FAST                1 (css_or_js)
                       44 LOAD_CONST               1 (('css', 'js'))
                       46 CONTAINS_OP              1
                       48 POP_JUMP_FORWARD_IF_FALSE    15 (to 80)
          
-         184          50 LOAD_GLOBAL              3 (NULL + ValueError)
+         190          50 LOAD_GLOBAL              3 (NULL + ValueError)
                       62 LOAD_CONST               2 ("Invalid argument, must be 'css' or 'js'")
                       64 PRECALL                  1
                       68 CALL                     1
                       78 RAISE_VARARGS            1
          
-         186     >>   80 LOAD_FAST                0 (context)
+         192     >>   80 LOAD_FAST                0 (context)
                       82 LOAD_METHOD              2 (get)
                      104 LOAD_CONST               3 ('request')
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               2 (request)
          
-         188         122 LOAD_FAST                1 (css_or_js)
+         194         122 LOAD_FAST                1 (css_or_js)
                      124 LOAD_CONST               4 ('css')
                      126 COMPARE_OP               2 (==)
                      132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
          
-         189         134 LOAD_GLOBAL              6 (REGISTER_CSS)
+         195         134 LOAD_GLOBAL              6 (REGISTER_CSS)
                      146 STORE_FAST               3 (hook_name)
                      148 JUMP_FORWARD             7 (to 164)
          
-         191     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
+         197     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
                      162 STORE_FAST               3 (hook_name)
          
-         193     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
+         199     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
                      176 LOAD_FAST                2 (request)
                      178 LOAD_GLOBAL             12 (FEDIT_PREVIEW_VAR)
                      190 LOAD_CONST               5 (False)
                      192 PRECALL                  3
                      196 CALL                     3
                      206 POP_JUMP_FORWARD_IF_TRUE     2 (to 212)
          
-         194         208 BUILD_MAP                0
+         200         208 BUILD_MAP                0
                      210 RETURN_VALUE
          
-         196     >>  212 BUILD_LIST               0
+         202     >>  212 BUILD_LIST               0
                      214 STORE_FAST               4 (files)
          
-         197         216 LOAD_GLOBAL             15 (NULL + hooks)
+         203         216 LOAD_GLOBAL             15 (NULL + hooks)
                      228 LOAD_ATTR                8 (get_hooks)
                      238 LOAD_FAST                3 (hook_name)
                      240 PRECALL                  1
                      244 CALL                     1
                      254 GET_ITER
                  >>  256 FOR_ITER                65 (to 388)
                      258 STORE_FAST               5 (hook)
          
-         198         260 PUSH_NULL
+         204         260 PUSH_NULL
                      262 LOAD_FAST                5 (hook)
                      264 LOAD_FAST                2 (request)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 STORE_FAST               6 (ret)
          
-         200         282 LOAD_GLOBAL             19 (NULL + isinstance)
+         206         282 LOAD_GLOBAL             19 (NULL + isinstance)
                      294 LOAD_FAST                6 (ret)
                      296 LOAD_GLOBAL             20 (list)
                      308 LOAD_GLOBAL             22 (tuple)
                      320 BUILD_TUPLE              2
                      322 PRECALL                  2
                      326 CALL                     2
                      336 POP_JUMP_FORWARD_IF_TRUE     3 (to 344)
          
-         201         338 LOAD_FAST                6 (ret)
+         207         338 LOAD_FAST                6 (ret)
                      340 BUILD_LIST               1
                      342 STORE_FAST               6 (ret)
          
-         203     >>  344 LOAD_FAST                4 (files)
+         209     >>  344 LOAD_FAST                4 (files)
                      346 LOAD_METHOD             12 (extend)
                      368 LOAD_FAST                6 (ret)
                      370 PRECALL                  1
                      374 CALL                     1
                      384 POP_TOP
                      386 JUMP_BACKWARD           66 (to 256)
          
-         206     >>  388 LOAD_CONST               6 ('hook_output')
+         212     >>  388 LOAD_CONST               6 ('hook_output')
                      390 LOAD_FAST                4 (files)
          
-         205         392 BUILD_MAP                1
+         211         392 BUILD_MAP                1
                      394 RETURN_VALUE
          consts
             None
             ('css', 'js')
             "Invalid argument, must be 'css' or 'js'"
             'request'
             'css'
@@ -1140,174 +1154,268 @@
             'hook_output'
          names      ('lower', 'ValueError', 'get', 'REGISTER_CSS', 'REGISTER_JS', 'getattr', 'FEDIT_PREVIEW_VAR', 'hooks', 'get_hooks', 'isinstance', 'list', 'tuple', 'extend')
          varnames   ('context', 'css_or_js', 'request', 'hook_name', 'files', 'hook', 'ret')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'static_hook_output'
-         firstlineno 179
+         firstlineno 185
          lnotab
             0x0202280208011e022a020c0110020e022c01040204012c011602380106
             022c0304ff
       'tokens'
       'kwarg_list'
+      'absolute_tokens'
       code
-         argcount  : 3
-         nlocals   : 10
-         stacksize : 5
+         argcount  : 4
+         nlocals   : 12
+         stacksize : 6
          flags     : 3
          code
-            0x970064017d0369007d047c02730267007d027401000000000000000000
-            007c01a6010000ab01000000000000000044005d985c0200007d057d067c
-            06a00100000000000000000000000000000000000000006402a6010000ab
-            0100000000000000007d077405000000000000000000007c07a6010000ab
-            01000000000000000064036b020000000072437405000000000000000000
-            007c02a6010000ab0100000000000000007c056b040000000072307c0372
-            0f7407000000000000000000006404a6010000ab01000000000000000082
-            017c00a00400000000000000000000000000000000000000007c06a60100
-            00ab0100000000000000007c047c027c05190000000000000000003c0000
-            008c707c076405190000000000000000007d087c00a00400000000000000
-            000000000000000000000000007c07640319000000000000000000a60100
-            00ab0100000000000000007c047c083c00000064067d038c997c0244005d
-            187d097c097c0476017212740b0000000000000000000064077c099b009d
-            02a6010000ab01000000000000000082018c197c045300
-         210           0 RESUME                   0
+            0x970064017d0469007d057c02730267007d027c03730267007d03740100
+            0000000000000000007c01a6010000ab010000000000000000440090015d
+            125c0200007d067d077c07a0010000000000000000000000000000000000
+            0000006402a6010000ab0100000000000000007d08740500000000000000
+            0000007c08a6010000ab01000000000000000064036b0200000000725974
+            05000000000000000000007c02a6010000ab0100000000000000007c066b
+            040000000072467c086404190000000000000000007c037600720c64057c
+            057c086404190000000000000000003c0000008c577c04720f7407000000
+            000000000000006406a6010000ab01000000000000000082017c00a00400
+            000000000000000000000000000000000000007c07a6010000ab01000000
+            00000000007c057c027c06190000000000000000003c0000008c87740500
+            0000000000000000007c08a6010000ab01000000000000000064036b0200
+            00000072397c086404190000000000000000007c037600720c64057c057c
+            086404190000000000000000003c0000008cb07c08640419000000000000
+            0000007d097c00a00400000000000000000000000000000000000000007c
+            09a6010000ab0100000000000000007d0a7c0a7c057c093c0000008cd37c
+            086404190000000000000000007d097c097c037600721374070000000000
+            000000000064077c099b0064089d03a6010000ab01000000000000000082
+            017c00a00400000000000000000000000000000000000000007c08640319
+            000000000000000000a6010000ab0100000000000000007c057c093c0000
+            0064057d0490018c147c0244005d187d0b7c0b7c0576017212740b000000
+            0000000000000064097c0b9b009d02a6010000ab01000000000000000082
+            018c197c055300
+         216           0 RESUME                   0
          
-         211           2 LOAD_CONST               1 (False)
-                       4 STORE_FAST               3 (had_kwargs)
+         217           2 LOAD_CONST               1 (False)
+                       4 STORE_FAST               4 (had_kwargs)
          
-         212           6 BUILD_MAP                0
-                       8 STORE_FAST               4 (kwargs)
+         218           6 BUILD_MAP                0
+                       8 STORE_FAST               5 (kwargs)
          
-         214          10 LOAD_FAST                2 (kwarg_list)
+         220          10 LOAD_FAST                2 (kwarg_list)
                       12 POP_JUMP_FORWARD_IF_TRUE     2 (to 18)
          
-         215          14 BUILD_LIST               0
+         221          14 BUILD_LIST               0
                       16 STORE_FAST               2 (kwarg_list)
          
-         217     >>   18 LOAD_GLOBAL              1 (NULL + enumerate)
-                      30 LOAD_FAST                1 (tokens)
-                      32 PRECALL                  1
-                      36 CALL                     1
-                      46 GET_ITER
-                 >>   48 FOR_ITER               152 (to 354)
-                      50 UNPACK_SEQUENCE          2
-                      54 STORE_FAST               5 (i)
-                      56 STORE_FAST               6 (token)
-         
-         218          58 LOAD_FAST                6 (token)
-                      60 LOAD_METHOD              1 (split)
-                      82 LOAD_CONST               2 ('=')
-                      84 PRECALL                  1
-                      88 CALL                     1
-                      98 STORE_FAST               7 (split)
-         
-         219         100 LOAD_GLOBAL              5 (NULL + len)
-                     112 LOAD_FAST                7 (split)
-                     114 PRECALL                  1
-                     118 CALL                     1
-                     128 LOAD_CONST               3 (1)
-                     130 COMPARE_OP               2 (==)
-                     136 POP_JUMP_FORWARD_IF_FALSE    67 (to 272)
-                     138 LOAD_GLOBAL              5 (NULL + len)
-                     150 LOAD_FAST                2 (kwarg_list)
-                     152 PRECALL                  1
-                     156 CALL                     1
-                     166 LOAD_FAST                5 (i)
-                     168 COMPARE_OP               4 (>)
-                     174 POP_JUMP_FORWARD_IF_FALSE    48 (to 272)
-         
-         220         176 LOAD_FAST                3 (had_kwargs)
-                     178 POP_JUMP_FORWARD_IF_FALSE    15 (to 210)
-         
-         221         180 LOAD_GLOBAL              7 (NULL + ValueError)
-                     192 LOAD_CONST               4 ('Unexpected positional argument after keyword argument')
-                     194 PRECALL                  1
-                     198 CALL                     1
-                     208 RAISE_VARARGS            1
-         
-         223     >>  210 LOAD_FAST                0 (parser)
-                     212 LOAD_METHOD              4 (compile_filter)
-                     234 LOAD_FAST                6 (token)
-                     236 PRECALL                  1
-                     240 CALL                     1
-                     250 LOAD_FAST                4 (kwargs)
-                     252 LOAD_FAST                2 (kwarg_list)
-                     254 LOAD_FAST                5 (i)
-                     256 BINARY_SUBSCR
-                     266 STORE_SUBSCR
-                     270 JUMP_BACKWARD          112 (to 48)
-         
-         225     >>  272 LOAD_FAST                7 (split)
-                     274 LOAD_CONST               5 (0)
-                     276 BINARY_SUBSCR
-                     286 STORE_FAST               8 (key)
-         
-         229         288 LOAD_FAST                0 (parser)
-                     290 LOAD_METHOD              4 (compile_filter)
-                     312 LOAD_FAST                7 (split)
-                     314 LOAD_CONST               3 (1)
-                     316 BINARY_SUBSCR
-                     326 PRECALL                  1
-                     330 CALL                     1
-                     340 LOAD_FAST                4 (kwargs)
-                     342 LOAD_FAST                8 (key)
-                     344 STORE_SUBSCR
-         
-         230         348 LOAD_CONST               6 (True)
-                     350 STORE_FAST               3 (had_kwargs)
-                     352 JUMP_BACKWARD          153 (to 48)
-         
-         232     >>  354 LOAD_FAST                2 (kwarg_list)
-                     356 GET_ITER
-                 >>  358 FOR_ITER                24 (to 408)
-                     360 STORE_FAST               9 (kwarg)
-         
-         233         362 LOAD_FAST                9 (kwarg)
-                     364 LOAD_FAST                4 (kwargs)
-                     366 CONTAINS_OP              1
-                     368 POP_JUMP_FORWARD_IF_FALSE    18 (to 406)
-         
-         234         370 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
-                     382 LOAD_CONST               7 ('Missing required keyword argument ')
-                     384 LOAD_FAST                9 (kwarg)
-                     386 FORMAT_VALUE             0
-                     388 BUILD_STRING             2
-                     390 PRECALL                  1
-                     394 CALL                     1
-                     404 RAISE_VARARGS            1
+         223     >>   18 LOAD_FAST                3 (absolute_tokens)
+                      20 POP_JUMP_FORWARD_IF_TRUE     2 (to 26)
+         
+         224          22 BUILD_LIST               0
+                      24 STORE_FAST               3 (absolute_tokens)
          
-         233     >>  406 JUMP_BACKWARD           25 (to 358)
+         226     >>   26 LOAD_GLOBAL              1 (NULL + enumerate)
+                      38 LOAD_FAST                1 (tokens)
+                      40 PRECALL                  1
+                      44 CALL                     1
+                      54 GET_ITER
+                 >>   56 EXTENDED_ARG             1
+                      58 FOR_ITER               274 (to 608)
+                      60 UNPACK_SEQUENCE          2
+                      64 STORE_FAST               6 (i)
+                      66 STORE_FAST               7 (token)
+         
+         227          68 LOAD_FAST                7 (token)
+                      70 LOAD_METHOD              1 (split)
+                      92 LOAD_CONST               2 ('=')
+                      94 PRECALL                  1
+                      98 CALL                     1
+                     108 STORE_FAST               8 (split)
+         
+         228         110 LOAD_GLOBAL              5 (NULL + len)
+                     122 LOAD_FAST                8 (split)
+                     124 PRECALL                  1
+                     128 CALL                     1
+                     138 LOAD_CONST               3 (1)
+                     140 COMPARE_OP               2 (==)
+                     146 POP_JUMP_FORWARD_IF_FALSE    89 (to 326)
+                     148 LOAD_GLOBAL              5 (NULL + len)
+                     160 LOAD_FAST                2 (kwarg_list)
+                     162 PRECALL                  1
+                     166 CALL                     1
+                     176 LOAD_FAST                6 (i)
+                     178 COMPARE_OP               4 (>)
+                     184 POP_JUMP_FORWARD_IF_FALSE    70 (to 326)
+         
+         229         186 LOAD_FAST                8 (split)
+                     188 LOAD_CONST               4 (0)
+                     190 BINARY_SUBSCR
+                     200 LOAD_FAST                3 (absolute_tokens)
+                     202 CONTAINS_OP              0
+                     204 POP_JUMP_FORWARD_IF_FALSE    12 (to 230)
+         
+         230         206 LOAD_CONST               5 (True)
+                     208 LOAD_FAST                5 (kwargs)
+                     210 LOAD_FAST                8 (split)
+                     212 LOAD_CONST               4 (0)
+                     214 BINARY_SUBSCR
+                     224 STORE_SUBSCR
+         
+         231         228 JUMP_BACKWARD           87 (to 56)
+         
+         233     >>  230 LOAD_FAST                4 (had_kwargs)
+                     232 POP_JUMP_FORWARD_IF_FALSE    15 (to 264)
+         
+         234         234 LOAD_GLOBAL              7 (NULL + ValueError)
+                     246 LOAD_CONST               6 ('Unexpected positional argument after keyword argument')
+                     248 PRECALL                  1
+                     252 CALL                     1
+                     262 RAISE_VARARGS            1
+         
+         236     >>  264 LOAD_FAST                0 (parser)
+                     266 LOAD_METHOD              4 (compile_filter)
+                     288 LOAD_FAST                7 (token)
+                     290 PRECALL                  1
+                     294 CALL                     1
+                     304 LOAD_FAST                5 (kwargs)
+                     306 LOAD_FAST                2 (kwarg_list)
+                     308 LOAD_FAST                6 (i)
+                     310 BINARY_SUBSCR
+                     320 STORE_SUBSCR
+                     324 JUMP_BACKWARD          135 (to 56)
+         
+         237     >>  326 LOAD_GLOBAL              5 (NULL + len)
+                     338 LOAD_FAST                8 (split)
+                     340 PRECALL                  1
+                     344 CALL                     1
+                     354 LOAD_CONST               3 (1)
+                     356 COMPARE_OP               2 (==)
+                     362 POP_JUMP_FORWARD_IF_FALSE    57 (to 478)
+         
+         238         364 LOAD_FAST                8 (split)
+                     366 LOAD_CONST               4 (0)
+                     368 BINARY_SUBSCR
+                     378 LOAD_FAST                3 (absolute_tokens)
+                     380 CONTAINS_OP              0
+                     382 POP_JUMP_FORWARD_IF_FALSE    12 (to 408)
+         
+         239         384 LOAD_CONST               5 (True)
+                     386 LOAD_FAST                5 (kwargs)
+                     388 LOAD_FAST                8 (split)
+                     390 LOAD_CONST               4 (0)
+                     392 BINARY_SUBSCR
+                     402 STORE_SUBSCR
+         
+         240         406 JUMP_BACKWARD          176 (to 56)
+         
+         242     >>  408 LOAD_FAST                8 (split)
+                     410 LOAD_CONST               4 (0)
+                     412 BINARY_SUBSCR
+                     422 STORE_FAST               9 (key)
+         
+         243         424 LOAD_FAST                0 (parser)
+                     426 LOAD_METHOD              4 (compile_filter)
+                     448 LOAD_FAST                9 (key)
+                     450 PRECALL                  1
+                     454 CALL                     1
+                     464 STORE_FAST              10 (value)
+         
+         244         466 LOAD_FAST               10 (value)
+                     468 LOAD_FAST                5 (kwargs)
+                     470 LOAD_FAST                9 (key)
+                     472 STORE_SUBSCR
+                     476 JUMP_BACKWARD          211 (to 56)
+         
+         246     >>  478 LOAD_FAST                8 (split)
+                     480 LOAD_CONST               4 (0)
+                     482 BINARY_SUBSCR
+                     492 STORE_FAST               9 (key)
+         
+         249         494 LOAD_FAST                9 (key)
+                     496 LOAD_FAST                3 (absolute_tokens)
+                     498 CONTAINS_OP              0
+                     500 POP_JUMP_FORWARD_IF_FALSE    19 (to 540)
+         
+         250         502 LOAD_GLOBAL              7 (NULL + ValueError)
+                     514 LOAD_CONST               7 ('Keyword argument ')
+                     516 LOAD_FAST                9 (key)
+                     518 FORMAT_VALUE             0
+                     520 LOAD_CONST               8 (' cannot be resolved; it will not be parsed as a variable.')
+                     522 BUILD_STRING             3
+                     524 PRECALL                  1
+                     528 CALL                     1
+                     538 RAISE_VARARGS            1
+         
+         252     >>  540 LOAD_FAST                0 (parser)
+                     542 LOAD_METHOD              4 (compile_filter)
+                     564 LOAD_FAST                8 (split)
+                     566 LOAD_CONST               3 (1)
+                     568 BINARY_SUBSCR
+                     578 PRECALL                  1
+                     582 CALL                     1
+                     592 LOAD_FAST                5 (kwargs)
+                     594 LOAD_FAST                9 (key)
+                     596 STORE_SUBSCR
+         
+         253         600 LOAD_CONST               5 (True)
+                     602 STORE_FAST               4 (had_kwargs)
+                     604 EXTENDED_ARG             1
+                     606 JUMP_BACKWARD          276 (to 56)
+         
+         255     >>  608 LOAD_FAST                2 (kwarg_list)
+                     610 GET_ITER
+                 >>  612 FOR_ITER                24 (to 662)
+                     614 STORE_FAST              11 (kwarg)
+         
+         256         616 LOAD_FAST               11 (kwarg)
+                     618 LOAD_FAST                5 (kwargs)
+                     620 CONTAINS_OP              1
+                     622 POP_JUMP_FORWARD_IF_FALSE    18 (to 660)
+         
+         257         624 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
+                     636 LOAD_CONST               9 ('Missing required keyword argument ')
+                     638 LOAD_FAST               11 (kwarg)
+                     640 FORMAT_VALUE             0
+                     642 BUILD_STRING             2
+                     644 PRECALL                  1
+                     648 CALL                     1
+                     658 RAISE_VARARGS            1
          
-         236     >>  408 LOAD_FAST                4 (kwargs)
-                     410 RETURN_VALUE
+         256     >>  660 JUMP_BACKWARD           25 (to 612)
+         
+         259     >>  662 LOAD_FAST                5 (kwargs)
+                     664 RETURN_VALUE
          consts
             None
             False
             '='
             1
-            'Unexpected positional argument after keyword argument'
             0
             True
+            'Unexpected positional argument after keyword argument'
+            'Keyword argument '
+            ' cannot be resolved; it will not be parsed as a variable.'
             'Missing required keyword argument '
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError')
-         varnames   ('parser', 'tokens', 'kwarg_list', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'kwarg')
+         varnames   ('parser', 'tokens', 'kwarg_list', 'absolute_tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'value', 'kwarg')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 210
+         firstlineno 216
          lnotab
-            0x0201040104020401040228012a014c0104011e023e0210043c01060208
-            01080124ff0203
-      (None,)
-   names      ('typing', 'Type', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'str', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'list', 'get_kwargs')
+            0x02010401040204010402040104022a012a014c0114011601020204011e
+            023e01260114011601020210012a010c021003080126023c010802080108
+            0124ff0203
+      (None, None)
+   names      ('typing', 'Type', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'str', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'list', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c0114030c0314040c010c010c020c0208021806140510061e
-      03040104041c4d2a010eff0e0102272a0112ff0e0102102e010aff0e0102
+      0x00ff02010c0114030c0314040c010c010c020c0208021806180610061e
+      03040104041c4d2a010eff0e01022c2a0112ff0e0102102e010aff0e0102
       1e
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.2/wagtail_fedit/templatetags/fedit.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     BaseAdapter,
     AdapterError,
 )
 from ..utils import (
     wrap_adapter,
     _can_edit,
     FEDIT_PREVIEW_VAR,
+    TEMPLATE_TAG_NAME,
 )
 from ..hooks import (
     REGISTER_CSS,
     REGISTER_JS,
 )
 
 
@@ -115,15 +116,15 @@
         if not adapter.check_permissions()\
           or not _can_edit(request, obj):
             return adapter.render_content(context)
 
         return wrap_adapter(request, adapter, context)
 
 
-@register.tag(name="fedit")
+@register.tag(name=TEMPLATE_TAG_NAME)
 def do_render_fedit(parser: Parser, token: Token):
 
     tokens = token.split_contents()
 
     _ = tokens.pop(0)
     adapter_id = tokens.pop(0)
 
@@ -144,15 +145,20 @@
                 )
 
         if len(model_tokens) > 1:
             # mymodel.myfield
             # mymodel.related_field.myfield
             model = parser.compile_filter(model_tokens.pop(0))
 
-    kwargs = get_kwargs(parser, tokens, adapter.required_kwargs)
+    kwargs = get_kwargs(
+        parser,
+        tokens,
+        adapter.required_kwargs,
+        adapter.absolute_tokens,
+    )
 
     return AdapterNode(
         adapter=adapter,
         model=model,
         getters=model_tokens,
         **kwargs,
     )
@@ -203,32 +209,49 @@
         files.extend(ret)
         
     return {
         "hook_output": files,
     }
 
 
-def get_kwargs(parser: Parser, tokens: list[str], kwarg_list: list[str] = None) -> dict:
+def get_kwargs(parser: Parser, tokens: list[str], kwarg_list: list[str] = None, absolute_tokens: list[str] = None) -> dict:
     had_kwargs = False
     kwargs = {}
 
     if not kwarg_list:
         kwarg_list = []
 
+    if not absolute_tokens:
+        absolute_tokens = []
+
     for i, token in enumerate(tokens):
         split = token.split("=")
         if len(split) == 1 and len(kwarg_list) > i:
+            if split[0] in absolute_tokens:
+                kwargs[split[0]] = True
+                continue
+
             if had_kwargs:
                 raise ValueError("Unexpected positional argument after keyword argument")
             
             kwargs[kwarg_list[i]] = parser.compile_filter(token)
+        elif len(split) == 1:
+            if split[0] in absolute_tokens:
+                kwargs[split[0]] = True
+                continue
+            else:
+                key = split[0]
+                value = parser.compile_filter(key)
+                kwargs[key] = value
         else:
             key = split[0]
             # if key not in kwargs_names:
             #     raise ValueError(f"Unexpected keyword argument {key}")
+            if key in absolute_tokens:
+                raise ValueError(f"Keyword argument {key} cannot be resolved; it will not be parsed as a variable.")
             
             kwargs[key] = parser.compile_filter(split[1])
             had_kwargs = True
 
     for kwarg in kwarg_list:
         if kwarg not in kwargs:
             raise TemplateSyntaxError(f"Missing required keyword argument {kwarg}")
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.2/wagtail_fedit/test/core/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from django.db import models
 from django.http import HttpResponse
 from django.utils.text import slugify
 from wagtail.snippets.models import register_snippet
 from django.template import Template, Context
 from wagtail import blocks
+from wagtail.admin.panels import (
+    FieldPanel,
+)
 from wagtail.fields import (
     StreamField,
     StreamValue,
 )
 from wagtail.models import (
     Page,
     LockableMixin,
@@ -151,7 +154,19 @@
     
     def permissions_for_user(self, user):
         return FeditPermissionTester(
             self,
             user=user,
             policy=self.get_permissions_policy()
         )
+
+
+class EditablePageModel(Page):
+    body = models.TextField()
+    content: StreamValue = StreamField([
+        ("heading_component", HeadingComponent()),
+        ("flat_menu_component", FlatMenuComponent())
+    ], use_json_field=True)
+
+    content_panels = Page.content_panels + [
+        FieldPanel("content")
+    ]
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
 from django.db import models from django.http import HttpResponse from
 django.utils.text import slugify from wagtail.snippets.models import
 register_snippet from django.template import Template, Context from wagtail
-import blocks from wagtail.fields import ( StreamField, StreamValue, ) from
-wagtail.models import ( Page, LockableMixin, RevisionMixin, PreviewableMixin,
-WorkflowMixin, DraftStateMixin, ) from wagtail_fedit.models import
-( FEditableMixin, FeditPermissionTester, ModelPermissionPolicy, ) class
-HeadingComponent(blocks.StructBlock): heading = blocks.CharBlock(max_length=25)
-subheading = blocks.CharBlock(max_length=40) def render(self, value,
-context=None): template = Template("""
+import blocks from wagtail.admin.panels import ( FieldPanel, ) from
+wagtail.fields import ( StreamField, StreamValue, ) from wagtail.models import
+( Page, LockableMixin, RevisionMixin, PreviewableMixin, WorkflowMixin,
+DraftStateMixin, ) from wagtail_fedit.models import ( FEditableMixin,
+FeditPermissionTester, ModelPermissionPolicy, ) class HeadingComponent
+(blocks.StructBlock): heading = blocks.CharBlock(max_length=25) subheading =
+blocks.CharBlock(max_length=40) def render(self, value, context=None): template
+= Template("""
 ************ {{{{ hheeaaddiinngg }}}} ************
 ********** {{{{ ssuubbhheeaaddiinngg }}}} **********
 """) context = self.get_context(value, parent_context=context) return
 template.render(Context(context)) class LinkBlock(blocks.StructBlock): text =
 blocks.CharBlock(max_length=25) def render(self, value, context=None): template
 = Template(""" _{_{_ _t_e_x_t_ _}_} """) context = self.get_context(value,
 parent_context=context) return template.render(Context(context)) class
@@ -54,8 +55,12 @@
 (BaseEditableMixin, WorkflowMixin, DraftStateMixin, RevisionMixin,
 LockableMixin, models.Model): title = models.CharField(max_length=255) body =
 models.TextField() content: StreamValue = StreamField([ ("heading_component",
 HeadingComponent()), ("flat_menu_component", FlatMenuComponent()) ],
 use_json_field=True) def get_permissions_policy(self): return
 ModelPermissionPolicy(self.__class__) def permissions_for_user(self, user):
 return FeditPermissionTester( self, user=user,
-policy=self.get_permissions_policy() )
+policy=self.get_permissions_policy() ) class EditablePageModel(Page): body =
+models.TextField() content: StreamValue = StreamField([ ("heading_component",
+HeadingComponent()), ("flat_menu_component", FlatMenuComponent()) ],
+use_json_field=True) content_panels = Page.content_panels + [ FieldPanel
+("content") ]
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 from django.urls import reverse
 from django.test import RequestFactory
 from django.contrib.auth.models import (
     User,
     Permission,
     AnonymousUser,
 )
+from wagtail.models import (
+    Page,
+)
 from ..models import (
     BasicModel,
+    EditablePageModel,
     EditableFullModel,
     EditableDraftModel,
     EditableRevisionModel,
     EditablePreviewModel,
     EditableLockModel,
 )
 
@@ -115,15 +119,23 @@
     # Block ID for a sub-block present in test data.
     BLOCK_ID = "c757f54d-0df5-4b35-8a06-4174f180ec41"
     
     def setUp(self):
         super().setUp()
 
         self.request_factory = RequestFactory()
-
+        root_page: Page = Page.add_root(title="Root Page")
+        self.page_model = root_page.add_child(
+            instance=EditablePageModel(
+                title="Editable Page",
+                body="Editable Page Body",
+                content=TEST_BLOCK_DATA,
+                url_path="/home/editable-page/",
+            )
+        )
         self.full_model = EditableFullModel.objects.create(
             title="Full Model",
             body="Full Model Body",
             content=TEST_BLOCK_DATA,
         )
         self.draft_model = EditableDraftModel.objects.create(
             title="Draft Model",
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,24 +40,32 @@
 
 class TestContextAdapter(TestAdapter):
     identifier = "test_context"
 
     def render_content(self, parent_context: dict = None) -> str:
         return parent_context["testing"]
 
+class TestAbsoluteTokensAdapter(TestAdapter):
+    identifier = "test_absolute_tokens"
+    absolute_tokens = ["absolute"]
+
+    def render_content(self, parent_context: dict = None) -> str:
+        return str(self.kwargs.get("absolute", False))
+
 class TestBlockAdapter(BlockAdapter, TestAdapter):
     identifier = "test_block"
 
 class TestFieldAdapter(FieldAdapter, TestAdapter):
     identifier = "test_field"
 
 adapter_registry.register(TestAdapter)
 adapter_registry.register(TestBlockAdapter)
 adapter_registry.register(TestFieldAdapter)
 adapter_registry.register(TestContextAdapter)
+adapter_registry.register(TestAbsoluteTokensAdapter)
 
 
 class TestBaseAdapter(BaseFEditTest):
 
     def test_required_kwargs_ok(self):
         self.assertEqual(TestAdapter.required_kwargs, ["test"])
 
@@ -135,14 +143,64 @@
         )
 
         self.assertEqual(
             adapter.render_content(),
             f"TestAdapter: {self.basic_model.title}"
         )
 
+    def test_adapter_absolute_tokens(self):
+        tpl = Template(
+            "{% load fedit %}"
+            "{% fedit test_absolute_tokens object.title test='test' absolute id=4 %}"
+        )
+
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
+        request.user = self.admin_user
+
+        tpl = tpl.render(
+            Context({
+                "request": request,
+                "object": self.basic_model,
+            })
+        )
+
+        self.assertHTMLEqual(
+            tpl,
+            str(True),
+        )
+
+    def test_adapter_absolute_tokens_fail(self):
+        tpl = Template(
+            "{% load fedit %}"
+            "{% fedit test_absolute_tokens object.title test='test' id=4 %}"
+        )
+
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
+        request.user = self.admin_user
+
+        tpl = tpl.render(
+            Context({
+                "request": request,
+                "object": self.basic_model,
+            })
+        )
+
+        self.assertHTMLEqual(
+            tpl,
+            str(False),
+        )
+
     def test_adapter_editable(self):
         self.assertEqual(TestAdapter.required_kwargs, ["test"])
 
         tpl = Template(
             "{% load fedit %}"
             "{% fedit test object.title test='test' id=4 %}"
         )
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.2/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.2/wagtail_fedit/toolbar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from .adapters import BaseAdapter
 
 class FeditToolbarComponent:
     template_name = None
     permissions: list[str] = []
 
-    def __init__(self):
-        pass
+    def __init__(self, request):
+        self.request = request
 
-    def get_context_data(self, request):
+    def get_context_data(self):
         return {
             "self": self,
-            "request": request,
+            "request": self.request,
         }
     
-    def is_shown(self, request):
-        if not all([request, request.user.is_authenticated]):
+    def is_shown(self):
+        if not all([self.request, self.request.user.is_authenticated]):
             return False
         
         if not self.permissions:
             return True
         
-        return request.user.has_perms(self.permissions)
+        return self.request.user.has_perms(self.permissions)
     
-    def render(self, request):
-        if not self.is_shown(request):
+    def render(self):
+        if not self.is_shown():
             return ""
 
         return mark_safe(render_to_string(
             self.template_name,
-            self.get_context_data(request),
+            self.get_context_data(),
         ))
 
 
-class FeditBlockEditButton(FeditToolbarComponent):
+class FeditAdapterComponent(FeditToolbarComponent):
+    def __init__(self, request, adapter: "BaseAdapter"):
+        super().__init__(request)
+        self.adapter = adapter
+
+class FeditAdapterEditButton(FeditAdapterComponent):
     """
         Required button class for the edit modal to function.
         This button is handled by the script in `wagtail_fedit/js/frontend.js`
     """
-    template_name = "wagtail_fedit/content/buttons/edit_block.html"
+    template_name = "wagtail_fedit/content/buttons/edit_adapter.html"
     permissions = [
         "wagtailadmin.access_admin",
     ]
 
-
-class FeditFieldEditButton(FeditToolbarComponent):
+class FeditAdapterAdminLinkButton(FeditAdapterComponent):
     """
         Required button class for the edit modal to function.
         This button is handled by the script in `wagtail_fedit/js/frontend.js`
     """
-    template_name = "wagtail_fedit/content/buttons/edit_field.html"
+    template_name = "wagtail_fedit/content/buttons/admin_link.html"
     permissions = [
         "wagtailadmin.access_admin",
     ]
 
-class FeditAdapterEditButton(FeditToolbarComponent):
-    """
-        Required button class for the edit modal to function.
-        This button is handled by the script in `wagtail_fedit/js/frontend.js`
-    """
-    template_name = "wagtail_fedit/content/buttons/edit_adapter.html"
-    permissions = [
-        "wagtailadmin.access_admin",
-    ]
+    def get_context_data(self):
+        return super().get_context_data() | {
+            "admin_url": self.adapter.get_admin_url(),
+        }
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.2/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.2/wagtail_fedit/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,48 +2,52 @@
 from collections import namedtuple
 from urllib.parse import urlencode
 from django.db import models
 from django.http import HttpRequest
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from django.template.loader import render_to_string
-from django.template.base import FilterExpression
 from django.conf import settings
 from django.urls import reverse
 
-from wagtail import hooks
 from wagtail.models import (
     DraftStateMixin,
     WorkflowMixin,
     LockableMixin,
     PreviewableMixin
 )
 from wagtail.admin.admin_url_finder import AdminURLFinder
 from wagtail.blocks.stream_block import StreamValue
 from wagtail.blocks.list_block import ListValue
-from wagtail import blocks
+from wagtail import (
+    hooks,
+    blocks,
+    VERSION as WAGTAIL_VERSION,
+)
 
 from .toolbar import (
-    FeditToolbarComponent,
+    FeditAdapterComponent,
     FeditAdapterEditButton,
 )
 from .hooks import (
     EXCLUDE_FROM_RELATED_FORMS,
     REGISTER_TYPE_RENDERER,
     REGISTER_FIELD_RENDERER,
     CONSTRUCT_ADAPTER_TOOLBAR,
 )
 
 
 if TYPE_CHECKING:
     from .adapters.base import BaseAdapter
 
 
+TEMPLATE_TAG_NAME = "fedit"
 FEDIT_PREVIEW_VAR = "_wagtail_fedit_preview"
 USERBAR_MODEL_VAR = "_wagtail_fedit_userbar_model"
+LOG_ACTION_TEMPLATES_AVAILABLE = WAGTAIL_VERSION < (6, 1, 0)
 
 
 class FeditPermissionCheck:
     @staticmethod
     def has_perms(request: HttpRequest, model: Any) -> bool:
 
         user = request
@@ -447,48 +451,27 @@
     else:
         lock = None
         locked_for_user = False
 
     return _lock_info(lock, locked_for_user)
 
 
-def get_hooks(hook_name):
-    """
-        Return the hooks for a given hook name in the wagtail_fedit namespace.
-    """
-    for hook in hooks.get_hooks(f"wagtail_fedit.{hook_name}"):
-        yield hook
-
-    
-def _resolve_expressions(context, *expressions):
-    """
-        Resolve a list of possible templatetag filterexpressions.
-    """
-    def _map(expression):
-        if isinstance(expression, FilterExpression):
-            return expression.resolve(context)
-        return expression
-    
-    return tuple(map(_map, expressions))
-
-
-
 def wrap_adapter(request: HttpRequest, adapter: "BaseAdapter", context: dict, run_context_processors: bool = False) -> str:
     if not context:
         context = {}
 
-    items: list[FeditToolbarComponent] = [
-        FeditAdapterEditButton(),
+    items: list[FeditAdapterComponent] = [
         *adapter.get_toolbar_buttons(),
+        FeditAdapterEditButton(request, adapter),
     ]
 
     for hook in hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR):
         hook(items=items, adapter=adapter)
 
-    items = [item.render(request) for item in items]
+    items = [item.render() for item in items]
     items = list(filter(None, items))
 
     reverse_kwargs = {
         "adapter_id": adapter.identifier,
         "field_name": adapter.field_name,
         "app_label": adapter.object._meta.app_label,
         "model_name": adapter.object._meta.model_name,
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.2/wagtail_fedit/views/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,17 @@
         if not hasattr(self.instance, field_name):
             return HttpResponseBadRequest("Invalid field name for object")
 
 
         shared_context = request.GET.get("shared_context")
         if shared_context:
             self.shared_context = self.adapter_class.decode_shared_context(
+                request,
+                self.instance,
+                field_name,
                 shared_context,
             )
         else:
             self.shared_context = {}
 
         self.adapter = self.adapter_class(
             request=request,
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.2/wagtail_fedit/views/editable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any
 from django.db import models
 from django.conf import settings
+from django.contrib.contenttypes.models import ContentType
 from django.utils.translation import gettext_lazy as _
 from django.views.generic import TemplateView
 from django.shortcuts import redirect
 from django.urls import reverse
 from django.http import (
     HttpRequest,
     HttpResponseBadRequest,
@@ -30,14 +31,15 @@
     ModelLogEntry,
     Page,
 )
 from .. import forms as block_forms
 from ..utils import (
     FEDIT_PREVIEW_VAR,
     USERBAR_MODEL_VAR,
+    LOG_ACTION_TEMPLATES_AVAILABLE,
     FeditPermissionCheck,
     with_userbar_model,
     # user_can_publish,
     # user_can_unpublish,
     # user_can_submit_for_moderation,
     # lock_info,
 )
@@ -266,20 +268,22 @@
                 "wagtailadmin_pages:history",
                 args=[self.object.pk],
             )
                 
         elif issubclass(log_entry_model, ModelLogEntry):
             log_entries = log_entry_model.objects\
                 .filter(object_id=self.object.pk)\
+                .filter(content_type=ContentType.objects.get_for_model(self.object))\
                 .order_by("-timestamp")
                 
         else:
             log_entries = None
 
-        if log_entries:
+        has_existing_published = log_entries.filter(action="wagtail.publish").exists()
+        if log_entries and has_existing_published:
             log_entries = log_entries.filter(
                 timestamp__gt=models.Subquery(
                     log_entries.filter(action="wagtail.publish")\
                                .values("timestamp")\
                                .order_by("-timestamp")[:1]
                 )
             )
@@ -296,20 +300,23 @@
                 log_entries = log_entries.select_related("page")
             else:
                 log_entries = log_entries.select_related("content_type")
 
             log_entry_count = log_entries.count()
             log_entries = log_entries[:MAX_LOG_ENTRIES_DISPLAYED]
 
+
         context.update({
             "log_entries": log_entries,
             "has_more_entries": log_entry_count > MAX_LOG_ENTRIES_DISPLAYED,
             "log_entry_count": log_entry_count,
             "last_published_at": self.object.last_published_at,
             "is_page": isinstance(self.object, Page),
+            
+            "LOG_ACTION_TEMPLATES_AVAILABLE": LOG_ACTION_TEMPLATES_AVAILABLE,
         })
 
         return context
 
     def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
         if not policy.can_publish():
             raise ValueError("User does not have permission to publish")
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.2/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,70 +28,71 @@
 )
 
 class FeditableModelComponent(FeditToolbarComponent):
     template_name = "wagtail_fedit/userbar/publish/action_button.html"
     action_icon = None
     action_text = None
 
-    def __init__(self, instance):
+    def __init__(self, request, instance):
+        self.request = request
         self.instance = instance
 
-    def get_context_data(self, request):
-        return super().get_context_data(request) | {
+    def get_context_data(self):
+        return super().get_context_data() | {
             "hidden": not self.instance.has_unpublished_changes,
             "action_icon": self.action_icon,
             "action_text": self.action_text,
             "action_url": reverse(
                 self.action_url,
                 args=[self.instance.pk, self.instance._meta.app_label, self.instance._meta.model_name],
             ),
         }
 
 class UserBarActionPublishComponent(FeditableModelComponent):
     action_url = "wagtail_fedit:publish"
     action_icon = "fedit-eye-open"
     action_text = _("Publish")
     
-    def is_shown(self, request):
-        if not super().is_shown(request):
+    def is_shown(self):
+        if not super().is_shown():
             return False
         
-        return user_can_publish(self.instance, request.user, check_for_changes=False)\
+        return user_can_publish(self.instance, self.request.user, check_for_changes=False)\
                and self.instance.has_unpublished_changes
 
 class UserBarActionUnpublishComponent(FeditableModelComponent):
     action_url = "wagtail_fedit:unpublish"
     action_icon = "fedit-eye-closed"
     action_text = _("Unpublish")
         
-    def is_shown(self, request):
-        if not super().is_shown(request):
+    def is_shown(self):
+        if not super().is_shown():
             return False
         
-        return user_can_unpublish(self.instance, request.user)
+        return user_can_unpublish(self.instance, self.request.user)
 
 class UserBarActionSubmitComponent(FeditableModelComponent):
     action_url = "wagtail_fedit:submit"
     action_icon = "fedit-check-list"
     action_text = _("Submit for moderation")
 
-    def is_shown(self, request):
-        if not super().is_shown(request):
+    def is_shown(self):
+        if not super().is_shown():
             return False
         
-        return user_can_submit_for_moderation(self.instance, request.user, check_for_changes=False)\
+        return user_can_submit_for_moderation(self.instance, self.request.user, check_for_changes=False)\
                and self.instance.has_unpublished_changes
 
 class UserBarActionCancelComponent(FeditableModelComponent):
     action_url = "wagtail_fedit:cancel"
     action_icon = "fedit-stop-sign"
     action_text = _("Cancel Workflow")
 
-    def is_shown(self, request):
-        if not super().is_shown(request):
+    def is_shown(self):
+        if not super().is_shown():
             return False
         
         if not is_draft_capable(self.instance):
             return False
         
         if not isinstance(self.instance, WorkflowMixin):
             return False
@@ -169,23 +170,23 @@
             return ""
 
         return super().render(request)
 
     def get_context_data(self, request):
 
         buttons = [
-            UserBarActionPublishComponent(self.model),
-            UserBarActionSubmitComponent(self.model),
-            UserBarActionUnpublishComponent(self.model),
-            UserBarActionCancelComponent(self.model),
+            UserBarActionPublishComponent(request, self.model),
+            UserBarActionSubmitComponent(request, self.model),
+            UserBarActionUnpublishComponent(request, self.model),
+            UserBarActionCancelComponent(request, self.model),
         ]
 
         return super().get_context_data(request) | {
             "buttons": list(
-                filter(None, map(lambda x: x.render(request), buttons))
+                filter(None, map(lambda x: x.render(), buttons))
             ),
         }
 
 def retrieve_page_model(items):
     # Retrieve page from other items...
     # sad we are not just provided with the context or page too.
     for item in items:
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.1a3
+Version: 1.5.2
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -23,16 +23,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=5.2
 
 wagtail_fedit
 =============
 
 ![Wagtail FEdit Example](https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
@@ -42,22 +40,28 @@
 - [Getting Started](#getting-started)
 - [Getting Editing!](#getting-editing)
 - [Permissions](#permissions)
 - [Revisions](#revisions)
 - [Workflows](#workflows)
 - [Logs](#logs)
 - [Caveats](#caveats)
-- [Adapters Python](#adapters-python)
-- [Adapters Javascript](#adapters-javascript)
+- [Adapters](#adapters)
+  - [Adapters Python](#adapters-python)
+  - [Adapters Javascript](#adapters-javascript)
 - [Hooks](#hooks)
   - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
   - [Register Type Renderer](#wagtail_feditregister_type_renderer)
   - [Register Field Renderer](#wagtail_feditregister_field_renderer)
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
+  - [Register CSS](#wagtail_feditregister_css)
+  - [Register JS](#wagtail_feditregister_js)
+  - [Field Editor Size](#wagtail_feditfield_editor_size)
+- [Settings](#settings)
+  - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
 - [How your content is rendered](#how-your-content-is-rendered)
   - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
 
@@ -66,14 +70,15 @@
    ```
    INSTALLED_APPS = [
    ...,
    'wagtail_fedit',
    ]
    ```
 2. Run `py ./manage.py collectstatic`.
+3. Run `py ./manage.py adapter_help` to see all your options and their requirements.
 
 ## Getting Editing!
 
 1. Make sure the models you wish to edit inherit from PreviewableMixin.
 
    **This is a requirement.**
 2. Define a template for your model.
@@ -84,29 +89,31 @@
    {% load fedit static wagtailuserbar %} {# Load the required template tag libraries #}
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
-       <link rel="stylesheet" href="{% static 'wagtail_fedit/css/frontend.css' %}">
+       {# Load all registered CSS required for the adapters. Only included inside edit view! #}
+       {% fedit_scripts "css" %}
    </head>
    <body>
        {# Adress the model.field or model.my.related.field you wish to edit. #}
-       {# Editable fields get a special `inline` argument. #}
-       {# if True the button is not placed with an absolute CSS position. #}
-       <h1>{% fedit field self.title inline=True or False %}</h1>
+       {# For help on arguments for the adapters please run the adapter_help command. #}
+       {# Example: `python3 ./manage.py adapter_help` #}
+       <h1>{% fedit field self.title inline %}</h1>
 
        <main class="my-streamfield-content">
            {% fedit field self.content %}
        </main>
 
        {% wagtailuserbar %}
 
-       <script src="{% static 'wagtail_fedit/js/frontend.js' %}"></script>
+       {# Load all registered Javascript required for the adapters. Only included inside edit view! #}
+       {% fedit_scripts "js" %}
    </body>
    </html>
 
 
    ```
 3. If your needs some special form of rendering; we allow your model to define a custom render method.
    The format of the method name should be `render_fedit_{fieldname}`.
@@ -228,21 +235,179 @@
 ```django-html
 {% for item in self.items.bound_blocks %}
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
-## Adapters Python
+## Adapters
 
-* TBA
+Creating a custom adapter is relatively simple.  
+We highly recommend you to inherit from `BaseFieldFuncAdapter` or `BaseBlockFuncAdapter`.  
+These adapters are basically pre-setup to callback to a javascript function on successful form submission.  
+This will save you the most amount of work.
 
-## Adapters Javascript
+We will create an adapter to change the color of a text field.
 
-* TBA
+Our adapter will be called `colorizer`.
+
+1. Our model is defined as follows:
+
+```python
+from wagtail.models import Page
+from wagtail.admin.panels import FieldPanel
+from django.db import models
+
+class MyPage(Page):
+    COLOR_CHOICES = [
+        ("#000000", "Black"),
+        ("#FFFFFF", "White"),
+        ("#FF0000", "Red"),
+        ("#00FF00", "Green"),
+        ("#0000FF", "Blue"),
+    ]
+
+    color = models.CharField(max_length=7, default="#000000", choices=COLOR_CHOICES)
+
+    content_panels = Page.content_panels + [
+        FieldPanel("color"),
+    ]
+```
+
+2. We have the following HTML template:
+
+```django-html
+...
+
+{% load fedit %}
+{% fedit colorizer page.color target=".my-colorized-div" %}
+<div class="my-colorized-div" style="color: {{ page.color }}">
+    <h1>Colorized Text!</h1>
+</div>
+
+...
+```
+
+###  Adapters Python
+
+We will get started creating the adapter definition.  
+Adapters can be defined anywhere; we recommend a separate `adapters.py` file.
+
+Adapter instances also have access to the following variables:
+
+* `self.object` - The model instance.
+* `self.field_name` - The field name.
+* `self.meta_field` - The models.Field instance.
+* `self.field_value` - The field value (Retrieved with `self.meta_field.value_from_object(self.object)`)
+* `self.request` - The django HTTP request object.
+* `self.kwargs` - Any shared context / keyword arguments for this adapter.
+
+```python
+# myapp/adapters.py
+
+from wagtail_fedit.adapters import (
+    BaseFieldFuncAdapter,
+    VARIABLES,
+)
+
+class ColorizerAdapter(BaseFieldFuncAdapter):
+    # Required keyword arguments for the template tag are defined by the superclass.
+    # required_kwargs = [
+    #   "target",
+    #   "name", # the function name, override in __init__ method.
+    # ]
+
+    # Optional kwargs are used to inform inside of the adapter_help command.
+    # They are only for developer convenience.
+    # optional_kwargs = []
+
+    # How the adapter will be adressed inside of the template tag.
+    identifier = "colorizer"
+
+    # A simple description of what this adapter does.
+    usage_description = "Change the color of the text for the given target element."
+
+    # Optional explanation of keyword arguments
+    help_text_dict = {
+        "target": "The target element to apply the color to.",
+    }
+
+    def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
+        kwargs["name"] = "myColorizerJavascriptFunction"
+        super().__init__(object, field_name, request, **kwargs)
+
+    def render_content(self, parent_context=None):
+        # This is not required; we will replace a CSS variable; thus we are not returning any actual content.
+        return ""
+        
+    def get_response_data(self, parent_context=None):
+        """
+        Return the data to be sent to the frontend adapter.
+        """
+        data = super().get_response_data(parent_context)
+        return data | {
+            "color": self.field_value,
+        }
+
+    def get_form_attrs(self) -> dict:
+        """
+        Return form attributes for the form inside of the edit modal.
+        This can be used to control editor size.
+        """
+        attrs = super().get_form_attrs()
+        attrs[VARIABLES.FORM_SIZE_VAR] = "full" # Fullscreen, there is also `large`.
+        return attrs
+```
+
+We must then register the adapter to make sure it is available for templates.
+
+This should be done in a `wagtail_hooks.py` file.
+
+```python
+# myapp/wagtail_hooks.py
+
+from wagtail_fedit.adapters import adapter_registry
+from myapp.adapters import ColorizerAdapter
+
+adapter_registry.register(ColorizerAdapter)
+```
+
+###  Adapters Javascript
+
+We now need to create the javascript function to actually apply the color to the styles of the element.  
+This function will be called `myColorizerJavascriptFunction`, as defined in the adapter's `__init__` method.
+
+```javascript
+// myapp/static/myapp/js/custom.js
+function myColorizerJavascriptFunction(element, response) {
+    element.style.color = response.color;
+}
+```
+
+We must then register this javascript file to be included in the frontend editing interface.
+
+This should be done in a `wagtail_hooks.py` file.
+
+```python
+# myapp/wagtail_hooks.py
+
+from django.utils.html import format_html
+from django.templatetags.static import static
+from wagtail_fedit.hooks import REGISTER_JS
+from wagtail import hooks
+
+@hooks.register(REGISTER_JS)
+def register_js(request):
+    return [
+        format_html(
+            '<script src="{0}"></script>',
+            static('myapp/js/custom.js')
+        ),
+    ]
+```
 
 ## Hooks
 
 ### wagtail_fedit.construct_adapter_toolbar
 
 Construct the toolbar for the given adapter.
 This is used to display the edit icon for the given adapter.
@@ -271,14 +436,63 @@
     # It will render the Page model as a simple h2 tag.
     renderer_map[Page] = lambda request, context, instance, value: format_html(
         '<h2>{0}</h2>',
         value.title
     )
 ```
 
+### wagtail_fedit.register_css
+
+Register a custom CSS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
+
+Example of how this hook is used in wagtail_hooks.py:
+    
+```python
+@hooks.register(REGISTER_CSS)
+def register_css(request):
+    return [
+        format_html(
+            '<link rel="stylesheet" href="{0}">',
+            static('css/custom.css')
+        ),
+    ]
+```
+
+### wagtail_fedit.field_editor_size
+
+Control the size of the editor for the given model-field type.
+
+Example of how this hook is called:
+    
+```python
+for hook in hooks.get_hooks(FEDIT_FIELD_EDITOR_SIZE):
+    size = hook(model_instance, model_field)
+    if size:
+        return size
+```
+
+### wagtail_fedit.register_js
+
+Register a custom JS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
+
+This can be used to register custom adapter JS.
+
+Example of how this hook is used in wagtail_hooks.py:
+    
+    ```python
+    @hooks.register(REGISTER_JS)
+    def register_js(request):
+        return [
+            format_html(
+                '<script src="{0}"></script>',
+                static('js/custom.js')
+            ),
+        ]
+    ```
+
 ### wagtail_fedit.register_field_renderer
 
 Register a custom renderer for a field.
 
 Example of how this type of renderer is used in wagtail_hooks/renderers.py:
 
 ```python
@@ -325,14 +539,25 @@
 ```python
 for hook in hooks.get_hooks(ACTION_MENU_ITEM_IS_SHOWN):
     result = hook(context, instance)
     if result is not None:
         return result # <- bool
 ```
 
+## Settings
+
+### `WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT`
+
+Default: `True`
+
+Sign the shared context with a secret key.  
+This is useful to prevent tampering with the shared context.  
+It will also be compressed with zlib if available.  
+It might not be in your site's security model to need this.
+
 ## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
 ### Rendered editable output HTML
```

#### html2text {}

```diff
@@ -1,49 +1,57 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.1a3 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.2 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
 Dynamic Content Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: Django>=4.2 Requires-Dist: Wagtail>=5.2
-wagtail_fedit ============= ![Wagtail FEdit Example](https://github.com/
-Nigel2392/wagtail_fedit/blob/main/.github/images/
+License-File: LICENSE wagtail_fedit ============= ![Wagtail FEdit Example]
+(https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
-(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters Python]
-(#adapters-python) - [Adapters Javascript](#adapters-javascript) - [Hooks]
-(#hooks) - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
-- [Register Type Renderer](#wagtail_feditregister_type_renderer) - [Register
-Field Renderer](#wagtail_feditregister_field_renderer) - [Exclude Related
-Forms](#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
-(#wagtail_feditaction_menu_item_is_shown) - [How your content is rendered]
-(#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
-output-html) - [Implemented](#implemented) Getting Started --------------- 1.
-Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
+(#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters](#adapters) -
+[Adapters Python](#adapters-python) - [Adapters Javascript](#adapters-
+javascript) - [Hooks](#hooks) - [Construct Adapter Toolbar]
+(#wagtail_feditconstruct_adapter_toolbar) - [Register Type Renderer]
+(#wagtail_feditregister_type_renderer) - [Register Field Renderer]
+(#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
+(#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
+(#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
+(#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
+[Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
+[Sign Shared Context](#wagtail_fedit_sign_shared_context) - [How your content
+is rendered](#how-your-content-is-rendered) - [Rendered output HTML](#rendered-
+editable-output-html) - [Implemented](#implemented) Getting Started -----------
+---- 1. Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
 INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
-collectstatic`. ## Getting Editing! 1. Make sure the models you wish to edit
-inherit from PreviewableMixin. **This is a requirement.** 2. Define a template
-for your model. Example: ```django-html {% load fedit static wagtailuserbar %}
-{# Load the required template tag libraries #}
-{# Adress the model.field or model.my.related.field you wish to edit. #} {#
-Editable fields get a special `inline` argument. #} {# if True the button is
-not placed with an absolute CSS position. #}
-************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee==TTrruuee oorr FFaallssee %%}} ************
-{% fedit field self.content %} {% wagtailuserbar %}
+collectstatic`. 3. Run `py ./manage.py adapter_help` to see all your options
+and their requirements. ## Getting Editing! 1. Make sure the models you wish to
+edit inherit from PreviewableMixin. **This is a requirement.** 2. Define a
+template for your model. Example: ```django-html {% load fedit static
+wagtailuserbar %} {# Load the required template tag libraries #}
+{# Load all registered CSS required for the adapters. Only included inside edit
+view! #} {% fedit_scripts "css" %}
+{# Adress the model.field or model.my.related.field you wish to edit. #} {# For
+help on arguments for the adapters please run the adapter_help command. #} {#
+Example: `python3 ./manage.py adapter_help` #}
+************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee %%}} ************
+{% fedit field self.content %} {% wagtailuserbar %} {# Load all registered
+Javascript required for the adapters. Only included inside edit view! #} {%
+fedit_scripts "js" %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
 fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by {# fedit
@@ -100,48 +108,124 @@
 %} {% include_block item %} {# No access to ID! Cannot edit! #} {% endfor %}
 ``` To make this an editable block instead; we would slightly change the loop
 to make the block's `id` available. This is done by accessing the
 `bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for
 the toplevel block!)* Our new loop would then be: ```django-html {% for item in
 self.items.bound_blocks %} {# Field name and model are the same arguments as in
 the first example! #} {% fedit block my_model_instance_var.content_field
-block=item block_id=item.id %} {% endfor %} ``` ## Adapters Python * TBA ##
-Adapters Javascript * TBA ## Hooks ### wagtail_fedit.construct_adapter_toolbar
-Construct the toolbar for the given adapter. This is used to display the edit
-icon for the given adapter. How it is called: ```python items =
-[ FeditAdapterEditButton(), ] for hook in hooks.get_hooks
-(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter) ``` ###
-wagtail_fedit.register_type_renderer Register a custom renderer for a type.
-Example of how this type of renderer can be used: ```python @hooks.register
-(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): # This is a
-custom renderer for the Page model. # It will render the Page model as a simple
-h2 tag. renderer_map[Page] = lambda request, context, instance, value:
-format_html( '
+block=item block_id=item.id %} {% endfor %} ``` ## Adapters Creating a custom
+adapter is relatively simple. We highly recommend you to inherit from
+`BaseFieldFuncAdapter` or `BaseBlockFuncAdapter`. These adapters are basically
+pre-setup to callback to a javascript function on successful form submission.
+This will save you the most amount of work. We will create an adapter to change
+the color of a text field. Our adapter will be called `colorizer`. 1. Our model
+is defined as follows: ```python from wagtail.models import Page from
+wagtail.admin.panels import FieldPanel from django.db import models class
+MyPage(Page): COLOR_CHOICES = [ ("#000000", "Black"), ("#FFFFFF", "White"),
+("#FF0000", "Red"), ("#00FF00", "Green"), ("#0000FF", "Blue"), ] color =
+models.CharField(max_length=7, default="#000000", choices=COLOR_CHOICES)
+content_panels = Page.content_panels + [ FieldPanel("color"), ] ``` 2. We have
+the following HTML template: ```django-html ... {% load fedit %} {% fedit
+colorizer page.color target=".my-colorized-div" %}
+************ CCoolloorriizzeedd TTeexxtt!! ************
+... ``` ### Adapters Python We will get started creating the adapter
+definition. Adapters can be defined anywhere; we recommend a separate
+`adapters.py` file. Adapter instances also have access to the following
+variables: * `self.object` - The model instance. * `self.field_name` - The
+field name. * `self.meta_field` - The models.Field instance. *
+`self.field_value` - The field value (Retrieved with
+`self.meta_field.value_from_object(self.object)`) * `self.request` - The django
+HTTP request object. * `self.kwargs` - Any shared context / keyword arguments
+for this adapter. ```python # myapp/adapters.py from wagtail_fedit.adapters
+import ( BaseFieldFuncAdapter, VARIABLES, ) class ColorizerAdapter
+(BaseFieldFuncAdapter): # Required keyword arguments for the template tag are
+defined by the superclass. # required_kwargs = [ # "target", # "name", # the
+function name, override in __init__ method. # ] # Optional kwargs are used to
+inform inside of the adapter_help command. # They are only for developer
+convenience. # optional_kwargs = [] # How the adapter will be adressed inside
+of the template tag. identifier = "colorizer" # A simple description of what
+this adapter does. usage_description = "Change the color of the text for the
+given target element." # Optional explanation of keyword arguments
+help_text_dict = { "target": "The target element to apply the color to.", } def
+__init__(self, object, field_name: str, request: HttpRequest, **kwargs): kwargs
+["name"] = "myColorizerJavascriptFunction" super().__init__(object, field_name,
+request, **kwargs) def render_content(self, parent_context=None): # This is not
+required; we will replace a CSS variable; thus we are not returning any actual
+content. return "" def get_response_data(self, parent_context=None): """ Return
+the data to be sent to the frontend adapter. """ data = super
+().get_response_data(parent_context) return data | { "color": self.field_value,
+} def get_form_attrs(self) -> dict: """ Return form attributes for the form
+inside of the edit modal. This can be used to control editor size. """ attrs =
+super().get_form_attrs() attrs[VARIABLES.FORM_SIZE_VAR] = "full" # Fullscreen,
+there is also `large`. return attrs ``` We must then register the adapter to
+make sure it is available for templates. This should be done in a
+`wagtail_hooks.py` file. ```python # myapp/wagtail_hooks.py from
+wagtail_fedit.adapters import adapter_registry from myapp.adapters import
+ColorizerAdapter adapter_registry.register(ColorizerAdapter) ``` ### Adapters
+Javascript We now need to create the javascript function to actually apply the
+color to the styles of the element. This function will be called
+`myColorizerJavascriptFunction`, as defined in the adapter's `__init__` method.
+```javascript // myapp/static/myapp/js/custom.js function
+myColorizerJavascriptFunction(element, response) { element.style.color =
+response.color; } ``` We must then register this javascript file to be included
+in the frontend editing interface. This should be done in a `wagtail_hooks.py`
+file. ```python # myapp/wagtail_hooks.py from django.utils.html import
+format_html from django.templatetags.static import static from
+wagtail_fedit.hooks import REGISTER_JS from wagtail import hooks
+@hooks.register(REGISTER_JS) def register_js(request): return [ format_html( '
+', static('myapp/js/custom.js') ), ] ``` ## Hooks ###
+wagtail_fedit.construct_adapter_toolbar Construct the toolbar for the given
+adapter. This is used to display the edit icon for the given adapter. How it is
+called: ```python items = [ FeditAdapterEditButton(), ] for hook in
+hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter)
+``` ### wagtail_fedit.register_type_renderer Register a custom renderer for a
+type. Example of how this type of renderer can be used: ```python
+@hooks.register(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): #
+This is a custom renderer for the Page model. # It will render the Page model
+as a simple h2 tag. renderer_map[Page] = lambda request, context, instance,
+value: format_html( '
 ********** {{00}} **********
-', value.title ) ``` ### wagtail_fedit.register_field_renderer Register a
-custom renderer for a field. Example of how this type of renderer is used in
-wagtail_hooks/renderers.py: ```python @hooks.register(REGISTER_FIELD_RENDERER)
-def register_renderers(renderer_map): # This is a custom renderer for RichText
-fields. # It will render the RichText field as a RichText block. renderer_map
-[RichTextField] =\ lambda request, context, instance, value: richtext(value)
-``` ### wagtail_fedit.exclude_related_forms Exclude the given model type from
-the related forms. This is used internally to exclude the Page, Image, and
-Document models from the related forms. This way; the user will have the actual
-widget for the field instead of the related form. Example of how this hook is
-called and how it is used internally: ```python def use_related_form(field:
-models.Field) -> bool: for hook in hooks.get_hooks(EXCLUDE_FROM_RELATED_FORMS):
-if hook(field): return False return True @hooks.register
-(EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field): if
-field.related_model in [Page, Image, Document]: return True return False ```
+', value.title ) ``` ### wagtail_fedit.register_css Register a custom CSS file
+to be included when the utils.FEDIT_PREVIEW_VAR is set to True. Example of how
+this hook is used in wagtail_hooks.py: ```python @hooks.register(REGISTER_CSS)
+def register_css(request): return [ format_html( '
+', static('css/custom.css') ), ] ``` ### wagtail_fedit.field_editor_size
+Control the size of the editor for the given model-field type. Example of how
+this hook is called: ```python for hook in hooks.get_hooks
+(FEDIT_FIELD_EDITOR_SIZE): size = hook(model_instance, model_field) if size:
+return size ``` ### wagtail_fedit.register_js Register a custom JS file to be
+included when the utils.FEDIT_PREVIEW_VAR is set to True. This can be used to
+register custom adapter JS. Example of how this hook is used in
+wagtail_hooks.py: ```python @hooks.register(REGISTER_JS) def register_js
+(request): return [ format_html( '
+', static('js/custom.js') ), ] ``` ### wagtail_fedit.register_field_renderer
+Register a custom renderer for a field. Example of how this type of renderer is
+used in wagtail_hooks/renderers.py: ```python @hooks.register
+(REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
+custom renderer for RichText fields. # It will render the RichText field as a
+RichText block. renderer_map[RichTextField] =\ lambda request, context,
+instance, value: richtext(value) ``` ### wagtail_fedit.exclude_related_forms
+Exclude the given model type from the related forms. This is used internally to
+exclude the Page, Image, and Document models from the related forms. This way;
+the user will have the actual widget for the field instead of the related form.
+Example of how this hook is called and how it is used internally: ```python def
+use_related_form(field: models.Field) -> bool: for hook in hooks.get_hooks
+(EXCLUDE_FROM_RELATED_FORMS): if hook(field): return False return True
+@hooks.register(EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field):
+if field.related_model in [Page, Image, Document]: return True return False ```
 ### wagtail_fedit.action_menu_item_is_shown Decide if the action menu item
 should be shown for the given instance. Return None if you cannot decide, False
 if you want to hide the item, and True if you want to show the item. Example of
 how this hook is called: ```python for hook in hooks.get_hooks
 (ACTION_MENU_ITEM_IS_SHOWN): result = hook(context, instance) if result is not
-None: return result # <- bool ``` ## How your content is rendered
+None: return result # <- bool ``` ## Settings ###
+`WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT` Default: `True` Sign the shared context
+with a secret key. This is useful to prevent tampering with the shared context.
+It will also be compressed with zlib if available. It might not be in your
+site's security model to need this. ## How your content is rendered
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
 or even at all for most content - **if** you don't get hyperspecific with your
 CSS selectors and structure your templates well.) Your block and field are
 wrapped in a `div`, any CSS for your templates should keep this in mind. ###
 Rendered editable output HTML ```html
 % if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
 { edit_url }}">
```

### Comparing `wagtail_fedit-1.5.1a3/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.2/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 wagtail_fedit/__init__.py
 wagtail_fedit/apps.py
 wagtail_fedit/hooks.py
 wagtail_fedit/models.py
+wagtail_fedit/settings.py
 wagtail_fedit/toolbar.py
 wagtail_fedit/urls.py
 wagtail_fedit/utils.py
 wagtail_fedit.egg-info/PKG-INFO
 wagtail_fedit.egg-info/SOURCES.txt
 wagtail_fedit.egg-info/dependency_links.txt
 wagtail_fedit.egg-info/requires.txt
@@ -32,17 +33,16 @@
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/static/wagtail_fedit/css/frontend.css
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
 wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
 wagtail_fedit/templates/wagtail_fedit/_hook_output.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
-wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
-wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
@@ -60,17 +60,14 @@
 wagtail_fedit/test/__init__.py
 wagtail_fedit/test/manage.py
 wagtail_fedit/test/core/__init__.py
 wagtail_fedit/test/core/apps.py
 wagtail_fedit/test/core/context_processors.py
 wagtail_fedit/test/core/models.py
 wagtail_fedit/test/core/migrations/0001_initial.py
-wagtail_fedit/test/core/migrations/0002_basicmodel.py
-wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
-wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
 wagtail_fedit/test/core/migrations/__init__.py
 wagtail_fedit/test/core/tests/__init__.py
 wagtail_fedit/test/core/tests/base.py
 wagtail_fedit/test/core/tests/test_adapters.py
 wagtail_fedit/test/core/tests/test_block_edit.py
 wagtail_fedit/test/core/tests/test_blocks.py
 wagtail_fedit/test/core/tests/test_field_edit.py
```

