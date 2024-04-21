# Comparing `tmp/wagtail_fedit-1.5.3rc2.tar.gz` & `tmp/wagtail_fedit-1.5.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.3rc2.tar", last modified: Sun Apr 21 00:49:07 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.3rc3.tar", last modified: Sun Apr 21 01:28:58 2024, max compression
```

## Comparing `wagtail_fedit-1.5.3rc2.tar` & `wagtail_fedit-1.5.3rc3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.036119 wagtail_fedit-1.5.3rc2/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/MANIFEST.in
--rw-rw-rw-   0        0        0    20237 2024-04-21 00:49:07.036119 wagtail_fedit-1.5.3rc2/PKG-INFO
--rw-rw-rw-   0        0        0    19036 2024-04-21 00:47:52.000000 wagtail_fedit-1.5.3rc2/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-04-21 00:49:07.046811 wagtail_fedit-1.5.3rc2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.910995 wagtail_fedit-1.5.3rc2/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.956471 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    10268 2024-04-21 00:45:14.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.960469 wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1765 2024-04-18 20:28:58.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4214 2024-04-16 18:40:39.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.872802 wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.873816 wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.962469 wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.962974 wagtail_fedit-1.5.3rc2/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.963980 wagtail_fedit-1.5.3rc2/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0      973 2024-04-21 00:46:27.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.875808 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.875808 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.967983 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.969982 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.876923 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.970984 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.973497 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.976506 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.983582 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      566 2024-04-21 00:09:10.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.990587 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.992589 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.994830 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.995989 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.998997 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    10007 2024-04-19 19:46:13.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     7503 2024-04-19 19:46:11.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.000993 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.006656 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.008654 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.016883 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    11767 2024-04-20 20:40:55.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.023541 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.026536 wagtail_fedit-1.5.3rc2/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6551 2024-04-21 00:08:49.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.035119 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     1881 2024-04-16 18:44:29.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.936844 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    20237 2024-04-21 00:49:06.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4038 2024-04-21 00:49:06.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 00:49:06.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-21 00:49:06.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 00:49:06.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:58.021902 wagtail_fedit-1.5.3rc3/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/MANIFEST.in
+-rw-rw-rw-   0        0        0    20306 2024-04-21 01:28:58.022904 wagtail_fedit-1.5.3rc3/PKG-INFO
+-rw-rw-rw-   0        0        0    19105 2024-04-21 00:53:02.000000 wagtail_fedit-1.5.3rc3/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-04-21 01:28:58.033742 wagtail_fedit-1.5.3rc3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.766415 wagtail_fedit-1.5.3rc3/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.816008 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    10463 2024-04-21 01:05:15.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.820552 wagtail_fedit-1.5.3rc3/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1765 2024-04-18 20:28:58.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4214 2024-04-16 18:40:39.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.729587 wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.729587 wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.840387 wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.841397 wagtail_fedit-1.5.3rc3/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.842399 wagtail_fedit-1.5.3rc3/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0      973 2024-04-21 00:46:27.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.731907 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.732905 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.856705 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.881773 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.733905 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.883247 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.885260 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.898057 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.927661 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      566 2024-04-21 00:09:10.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.934177 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.952436 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.975595 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.977591 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.980594 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10817 2024-04-21 01:26:50.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7961 2024-04-21 01:25:52.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.982839 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.988845 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.991367 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:58.000366 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    12859 2024-04-21 01:26:42.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:58.005731 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:58.010730 wagtail_fedit-1.5.3rc3/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6551 2024-04-21 00:08:49.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:58.021902 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     1881 2024-04-16 18:44:29.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.804778 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    20306 2024-04-21 01:28:57.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4038 2024-04-21 01:28:57.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 01:28:57.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-21 01:28:57.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 01:28:57.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.3rc2/LICENSE` & `wagtail_fedit-1.5.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/PKG-INFO` & `wagtail_fedit-1.5.3rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.3rc2
+Version: 1.5.3rc3
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -55,14 +55,15 @@
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
   - [Share With Sessions](#wagtail_fedit_share_with_sessions)
+  - [Use Adapter Session ID](#wagtail_fedit_use_adapter_session_id)
 - [How your content is rendered](#how-your-content-is-rendered)
   - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc2 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc3 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -26,24 +26,25 @@
 (#wagtail_feditregister_type_renderer) - [Register Field Renderer]
 (#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
 [Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
-Sessions](#wagtail_fedit_share_with_sessions) - [How your content is rendered]
-(#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
-output-html) - [Implemented](#implemented) Getting Started --------------- 1.
-Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
-INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
-collectstatic`. 3. Run `py ./manage.py adapter_help` to see all your options
-and their requirements. ## Getting Editing! 1. Make sure the models you wish to
-edit inherit from PreviewableMixin. **This is a requirement.** 2. Define a
-template for your model. Example: ```django-html {% load fedit static
-wagtailuserbar %} {# Load the required template tag libraries #}
+Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
+(#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
+your-content-is-rendered) - [Rendered output HTML](#rendered-editable-output-
+html) - [Implemented](#implemented) Getting Started --------------- 1. Add
+'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
+[ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. 3. Run `py
+./manage.py adapter_help` to see all your options and their requirements. ##
+Getting Editing! 1. Make sure the models you wish to edit inherit from
+PreviewableMixin. **This is a requirement.** 2. Define a template for your
+model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
+the required template tag libraries #}
 {# Load all registered CSS required for the adapters. Only included inside edit
 view! #} {% fedit_scripts "css" %}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {# For
 help on arguments for the adapters please run the adapter_help command. #} {#
 Example: `python3 ./manage.py adapter_help` #}
 ************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee %%}} ************
 {% fedit field self.content %} {% wagtailuserbar %} {# Load all registered
```

### Comparing `wagtail_fedit-1.5.3rc2/README.md` & `wagtail_fedit-1.5.3rc3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
   - [Share With Sessions](#wagtail_fedit_share_with_sessions)
+  - [Use Adapter Session ID](#wagtail_fedit_use_adapter_session_id)
 - [How your content is rendered](#how-your-content-is-rendered)
   - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
```

#### html2text {}

```diff
@@ -11,24 +11,25 @@
 (#wagtail_feditregister_type_renderer) - [Register Field Renderer]
 (#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
 [Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
-Sessions](#wagtail_fedit_share_with_sessions) - [How your content is rendered]
-(#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
-output-html) - [Implemented](#implemented) Getting Started --------------- 1.
-Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
-INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
-collectstatic`. 3. Run `py ./manage.py adapter_help` to see all your options
-and their requirements. ## Getting Editing! 1. Make sure the models you wish to
-edit inherit from PreviewableMixin. **This is a requirement.** 2. Define a
-template for your model. Example: ```django-html {% load fedit static
-wagtailuserbar %} {# Load the required template tag libraries #}
+Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
+(#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
+your-content-is-rendered) - [Rendered output HTML](#rendered-editable-output-
+html) - [Implemented](#implemented) Getting Started --------------- 1. Add
+'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
+[ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. 3. Run `py
+./manage.py adapter_help` to see all your options and their requirements. ##
+Getting Editing! 1. Make sure the models you wish to edit inherit from
+PreviewableMixin. **This is a requirement.** 2. Define a template for your
+model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
+the required template tag libraries #}
 {# Load all registered CSS required for the adapters. Only included inside edit
 view! #} {% fedit_scripts "css" %}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {# For
 help on arguments for the adapters please run the adapter_help command. #} {#
 Example: `python3 ./manage.py adapter_help` #}
 ************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee %%}} ************
 {% fedit field self.content %} {% wagtailuserbar %} {# Load all registered
```

### Comparing `wagtail_fedit-1.5.3rc2/setup.cfg` & `wagtail_fedit-1.5.3rc3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3372 6332 0d0a 6465 7363 7269 7074 696f  3rc2..descriptio
+00000030: 3372 6333 0d0a 6465 7363 7269 7074 696f  3rc3..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -275,26 +275,31 @@
         """
         Encode a dictionary to a string.
         This will be passed as a GET parameter to the iFrame.
         Make sure the data is not too large.
         """
         if not self.kwargs:
             return ""
+        
         if SHARE_WITH_SESSIONS:
             if USE_ADAPTER_SESSION_ID:
+                # This ID should be uniquely generated for each adapter instance.
+                # But this is not always possible - hence why we allow UUID's.
                 id = self.get_element_id()
             else:
+                # Set in kwargs, try not to clutter session data too much.
                 id = self.kwargs.setdefault(
                     "wagtail_fedit_uuid",
                     str(uuid.uuid4())
                 )
+                
             self.request.session[id] = self.kwargs
             self.request.session.modified = True
             return id
-        # return self.signer.sign_object(self.kwargs)# , serializer=PickleBlockSerializer)
+        
         if SIGN_SHARED_CONTEXT:
             return self.signer.sign_object(self.kwargs, compress=True)
         
         return Base85_json_dumps(self.kwargs)
 
 
     @classmethod
@@ -305,14 +310,15 @@
         if SHARE_WITH_SESSIONS:
             if not context:
                 return {}
             return request.session.get(context, {})
         
         if SIGN_SHARED_CONTEXT:
             return cls.signer.unsign_object(context)# , serializer=PickleBlockSerializer)
+        
         try:
             return Base85_json_loads(context)
         except json.JSONDecodeError:
             pass
         return {}
     
 class BlockFieldReplacementAdapter(BaseAdapter):
```

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/block.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/models.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,35 +1,35 @@
 magic:    0xa70d0d0a
-moddate:  0x03ca2266 (Fri Apr 19 19:46:11 2024 UTC)
-files sz: 7503
+moddate:  0x206b2466 (Sun Apr 21 01:25:52 2024 UTC)
+files sz: 7961
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
       055a050100640064036c066d075a070100640064046c086d095a096d0a5a
       0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f01
       00640064076c106d115a110100640064086c126d135a130100640064096c
       145a14640a640b6c156d165a166d175a176d185a186d195a190100640a64
       0c6c1a6d1b5a1b6d1c5a1c6d1d5a1d6d1e5a1e0100640a640d6c136d1f5a
       1f6d205a200100020065036a210000000000000000a6000000ab00000000
-      00000000005a22640e5a23640f5a24020047006410840064116504a60300
-      00ab0300000000000000005a256522a02600000000000000000000000000
-      00000000000000651eac12a6010000ab0100000000000000006413650964
-      14650a660464158404a6000000ab0000000000000000005a276522a02800
-      000000000000000000000000000000000000006416ac17a6010000ab0100
-      000000000000006418650764196518641a65296606641b8404a6000000ab
-      0000000000000000005a2a6522a02b000000000000000000000000000000
-      0000000000641c641d6416ac1ea6030000ab030000000000000000641a65
-      2c6602641f8404a6000000ab0000000000000000005a2d64246413650964
-      20652e6529190000000000000000006421652e6529190000000000000000
-      006422652e652919000000000000000000641a652c660a642384055a2f64
-      095300
+      00000000005a22640e5a23640f5a24641065256411650764126525641365
+      256608641484045a26020047006415840064166504a6030000ab03000000
+      00000000005a276522a02800000000000000000000000000000000000000
+      00651eac17a6010000ab010000000000000000641865096419650a660464
+      1a8404a6000000ab0000000000000000005a296522a02a00000000000000
+      00000000000000000000000000641bac1ca6010000ab0100000000000000
+      0064116507641d6518641365256606641e8404a6000000ab000000000000
+      0000005a2b6522a02c000000000000000000000000000000000000000064
+      1f6420641bac21a6030000ab0300000000000000006413652d6602642284
+      04a6000000ab0000000000000000005a2e6427641865096423652f652519
+      0000000000000000006424652f6525190000000000000000006425652f65
+      25190000000000000000006413652d660a642684055a3064095300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Type',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Type)
                 10 STORE_NAME               1 (Type)
@@ -141,109 +141,122 @@
    
     41         216 LOAD_CONST              14 ('Field name is not available in the context for %(object)s.')
                218 STORE_NAME              35 (WARNING_FIELD_NAME_NOT_AVAILABLE)
    
     42         220 LOAD_CONST              15 ('Model instance is not available in the context for %(object)s.')
                222 STORE_NAME              36 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
    
-    46         224 PUSH_NULL
-               226 LOAD_BUILD_CLASS
-               228 LOAD_CONST              16 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 46>)
-               230 MAKE_FUNCTION            0
-               232 LOAD_CONST              17 ('AdapterNode')
-               234 LOAD_NAME                4 (Node)
-               236 PRECALL                  3
-               240 CALL                     3
-               250 STORE_NAME              37 (AdapterNode)
-   
-   123         252 LOAD_NAME               34 (register)
-               254 LOAD_METHOD             38 (tag)
-               276 LOAD_NAME               30 (TEMPLATE_TAG_NAME)
-               278 KW_NAMES                18
-               280 PRECALL                  1
-               284 CALL                     1
-   
-   124         294 LOAD_CONST              19 ('parser')
-               296 LOAD_NAME                9 (Parser)
-               298 LOAD_CONST              20 ('token')
-               300 LOAD_NAME               10 (Token)
-               302 BUILD_TUPLE              4
-               304 LOAD_CONST              21 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 123>)
-               306 MAKE_FUNCTION            4 (annotations)
-   
-   123         308 PRECALL                  0
-               312 CALL                     0
-   
-   124         322 STORE_NAME              39 (do_render_fedit)
-   
-   168         324 LOAD_NAME               34 (register)
-               326 LOAD_METHOD             40 (simple_tag)
-               348 LOAD_CONST              22 (True)
-               350 KW_NAMES                23
-               352 PRECALL                  1
-               356 CALL                     1
-   
-   169         366 LOAD_CONST              24 ('context')
-               368 LOAD_NAME                7 (Context)
-               370 LOAD_CONST              25 ('adapter')
-               372 LOAD_NAME               24 (BaseAdapter)
-               374 LOAD_CONST              26 ('return')
-               376 LOAD_NAME               41 (str)
-               378 BUILD_TUPLE              6
-               380 LOAD_CONST              27 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 168>)
-               382 MAKE_FUNCTION            4 (annotations)
-   
-   168         384 PRECALL                  0
-               388 CALL                     0
-   
-   169         398 STORE_NAME              42 (render_adapter)
-   
-   185         400 LOAD_NAME               34 (register)
-               402 LOAD_METHOD             43 (inclusion_tag)
-               424 LOAD_CONST              28 ('wagtail_fedit/_hook_output.html')
-               426 LOAD_CONST              29 ('fedit_scripts')
-               428 LOAD_CONST              22 (True)
-               430 KW_NAMES                30
-               432 PRECALL                  3
-               436 CALL                     3
-   
-   186         446 LOAD_CONST              26 ('return')
-               448 LOAD_NAME               44 (dict)
-               450 BUILD_TUPLE              2
-               452 LOAD_CONST              31 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 185>)
-               454 MAKE_FUNCTION            4 (annotations)
-   
-   185         456 PRECALL                  0
-               460 CALL                     0
-   
-   186         470 STORE_NAME              45 (static_hook_output)
-   
-   216         472 LOAD_CONST              36 ((None, None))
-               474 LOAD_CONST              19 ('parser')
-               476 LOAD_NAME                9 (Parser)
-               478 LOAD_CONST              32 ('tokens')
-               480 LOAD_NAME               46 (list)
-               482 LOAD_NAME               41 (str)
-               484 BINARY_SUBSCR
-               494 LOAD_CONST              33 ('kwarg_list')
-               496 LOAD_NAME               46 (list)
-               498 LOAD_NAME               41 (str)
-               500 BINARY_SUBSCR
-               510 LOAD_CONST              34 ('absolute_tokens')
-               512 LOAD_NAME               46 (list)
-               514 LOAD_NAME               41 (str)
-               516 BINARY_SUBSCR
-               526 LOAD_CONST              26 ('return')
-               528 LOAD_NAME               44 (dict)
-               530 BUILD_TUPLE             10
-               532 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 216>)
-               534 MAKE_FUNCTION            5 (defaults, annotations)
-               536 STORE_NAME              47 (get_kwargs)
-               538 LOAD_CONST               9 (None)
-               540 RETURN_VALUE
+    45         224 LOAD_CONST              16 ('var')
+               226 LOAD_NAME               37 (str)
+               228 LOAD_CONST              17 ('context')
+               230 LOAD_NAME                7 (Context)
+               232 LOAD_CONST              18 ('value')
+               234 LOAD_NAME               37 (str)
+               236 LOAD_CONST              19 ('return')
+               238 LOAD_NAME               37 (str)
+               240 BUILD_TUPLE              8
+               242 LOAD_CONST              20 (<code object as_var, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 45>)
+               244 MAKE_FUNCTION            4 (annotations)
+               246 STORE_NAME              38 (as_var)
+   
+    52         248 PUSH_NULL
+               250 LOAD_BUILD_CLASS
+               252 LOAD_CONST              21 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 52>)
+               254 MAKE_FUNCTION            0
+               256 LOAD_CONST              22 ('AdapterNode')
+               258 LOAD_NAME                4 (Node)
+               260 PRECALL                  3
+               264 CALL                     3
+               274 STORE_NAME              39 (AdapterNode)
+   
+   130         276 LOAD_NAME               34 (register)
+               278 LOAD_METHOD             40 (tag)
+               300 LOAD_NAME               30 (TEMPLATE_TAG_NAME)
+               302 KW_NAMES                23
+               304 PRECALL                  1
+               308 CALL                     1
+   
+   131         318 LOAD_CONST              24 ('parser')
+               320 LOAD_NAME                9 (Parser)
+               322 LOAD_CONST              25 ('token')
+               324 LOAD_NAME               10 (Token)
+               326 BUILD_TUPLE              4
+               328 LOAD_CONST              26 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 130>)
+               330 MAKE_FUNCTION            4 (annotations)
+   
+   130         332 PRECALL                  0
+               336 CALL                     0
+   
+   131         346 STORE_NAME              41 (do_render_fedit)
+   
+   182         348 LOAD_NAME               34 (register)
+               350 LOAD_METHOD             42 (simple_tag)
+               372 LOAD_CONST              27 (True)
+               374 KW_NAMES                28
+               376 PRECALL                  1
+               380 CALL                     1
+   
+   183         390 LOAD_CONST              17 ('context')
+               392 LOAD_NAME                7 (Context)
+               394 LOAD_CONST              29 ('adapter')
+               396 LOAD_NAME               24 (BaseAdapter)
+               398 LOAD_CONST              19 ('return')
+               400 LOAD_NAME               37 (str)
+               402 BUILD_TUPLE              6
+               404 LOAD_CONST              30 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 182>)
+               406 MAKE_FUNCTION            4 (annotations)
+   
+   182         408 PRECALL                  0
+               412 CALL                     0
+   
+   183         422 STORE_NAME              43 (render_adapter)
+   
+   199         424 LOAD_NAME               34 (register)
+               426 LOAD_METHOD             44 (inclusion_tag)
+               448 LOAD_CONST              31 ('wagtail_fedit/_hook_output.html')
+               450 LOAD_CONST              32 ('fedit_scripts')
+               452 LOAD_CONST              27 (True)
+               454 KW_NAMES                33
+               456 PRECALL                  3
+               460 CALL                     3
+   
+   200         470 LOAD_CONST              19 ('return')
+               472 LOAD_NAME               45 (dict)
+               474 BUILD_TUPLE              2
+               476 LOAD_CONST              34 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 199>)
+               478 MAKE_FUNCTION            4 (annotations)
+   
+   199         480 PRECALL                  0
+               484 CALL                     0
+   
+   200         494 STORE_NAME              46 (static_hook_output)
+   
+   230         496 LOAD_CONST              39 ((None, None))
+               498 LOAD_CONST              24 ('parser')
+               500 LOAD_NAME                9 (Parser)
+               502 LOAD_CONST              35 ('tokens')
+               504 LOAD_NAME               47 (list)
+               506 LOAD_NAME               37 (str)
+               508 BINARY_SUBSCR
+               518 LOAD_CONST              36 ('kwarg_list')
+               520 LOAD_NAME               47 (list)
+               522 LOAD_NAME               37 (str)
+               524 BINARY_SUBSCR
+               534 LOAD_CONST              37 ('absolute_tokens')
+               536 LOAD_NAME               47 (list)
+               538 LOAD_NAME               37 (str)
+               540 BINARY_SUBSCR
+               550 LOAD_CONST              19 ('return')
+               552 LOAD_NAME               45 (dict)
+               554 BUILD_TUPLE             10
+               556 LOAD_CONST              38 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 230>)
+               558 MAKE_FUNCTION            5 (defaults, annotations)
+               560 STORE_NAME              48 (get_kwargs)
+               562 LOAD_CONST               9 (None)
+               564 RETURN_VALUE
    consts
       0
       ('Type',)
       ('library', 'Node', 'TemplateSyntaxError')
       ('Context',)
       ('Parser', 'Token', 'FilterExpression')
       ('HttpRequest',)
@@ -253,504 +266,571 @@
       None
       2
       ('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError')
       ('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME')
       ('REGISTER_CSS', 'REGISTER_JS')
       'Field name is not available in the context for %(object)s.'
       'Model instance is not available in the context for %(object)s.'
+      'var'
+      'context'
+      'value'
+      'return'
+      code
+         argcount  : 3
+         nlocals   : 3
+         stacksize : 3
+         flags     : 3
+         code 0x97007c0073027c0253007c027c017c003c00000064015300
+          45           0 RESUME                   0
+         
+          46           2 LOAD_FAST                0 (var)
+                       4 POP_JUMP_FORWARD_IF_TRUE     2 (to 10)
+         
+          47           6 LOAD_FAST                2 (value)
+                       8 RETURN_VALUE
+         
+          49     >>   10 LOAD_FAST                2 (value)
+                      12 LOAD_FAST                1 (context)
+                      14 LOAD_FAST                0 (var)
+                      16 STORE_SUBSCR
+         
+          50          20 LOAD_CONST               1 ('')
+                      22 RETURN_VALUE
+         consts
+            None
+            ''
+         names      ()
+         varnames   ('var', 'context', 'value')
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         name       'as_var'
+         firstlineno 45
+         lnotab 0x0201040104020a01
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 7
+         stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a02020065036a040000000000000000a6000000ab
-            0000000000000000005a0564016506650719000000000000000000640265
-            0864036509650a190000000000000000006606640484045a0b640584005a
-            0c640684005a0d64075300
-          46           0 RESUME                   0
+            0000000000000000005a0564096402650665071900000000000000000064
+            03650864046509650a190000000000000000006405650a6608640684055a
+            0b640784005a0c640884005a0d64015300
+          52           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdapterNode')
                        8 STORE_NAME               2 (__qualname__)
          
-          47          10 PUSH_NULL
+          53          10 PUSH_NULL
                       12 LOAD_NAME                3 (signing)
                       14 LOAD_ATTR                4 (TimestampSigner)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_NAME               5 (signer)
          
-          49          40 LOAD_CONST               1 ('adapter')
-                      42 LOAD_NAME                6 (Type)
-                      44 LOAD_NAME                7 (BaseAdapter)
-                      46 BINARY_SUBSCR
-                      56 LOAD_CONST               2 ('model')
-                      58 LOAD_NAME                8 (FilterExpression)
-                      60 LOAD_CONST               3 ('getters')
-                      62 LOAD_NAME                9 (list)
-                      64 LOAD_NAME               10 (str)
-                      66 BINARY_SUBSCR
-                      76 BUILD_TUPLE              6
-                      78 LOAD_CONST               4 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 49>)
-                      80 MAKE_FUNCTION            4 (annotations)
-                      82 STORE_NAME              11 (__init__)
-         
-          55          84 LOAD_CONST               5 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 55>)
-                      86 MAKE_FUNCTION            0
-                      88 STORE_NAME              12 (_resolve_expressions)
+          55          40 LOAD_CONST               9 ((None,))
+                      42 LOAD_CONST               2 ('adapter')
+                      44 LOAD_NAME                6 (Type)
+                      46 LOAD_NAME                7 (BaseAdapter)
+                      48 BINARY_SUBSCR
+                      58 LOAD_CONST               3 ('model')
+                      60 LOAD_NAME                8 (FilterExpression)
+                      62 LOAD_CONST               4 ('getters')
+                      64 LOAD_NAME                9 (list)
+                      66 LOAD_NAME               10 (str)
+                      68 BINARY_SUBSCR
+                      78 LOAD_CONST               5 ('as_var')
+                      80 LOAD_NAME               10 (str)
+                      82 BUILD_TUPLE              8
+                      84 LOAD_CONST               6 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 55>)
+                      86 MAKE_FUNCTION            5 (defaults, annotations)
+                      88 STORE_NAME              11 (__init__)
          
-          65          90 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 65>)
+          62          90 LOAD_CONST               7 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 62>)
                       92 MAKE_FUNCTION            0
-                      94 STORE_NAME              13 (render)
-                      96 LOAD_CONST               7 (None)
-                      98 RETURN_VALUE
+                      94 STORE_NAME              12 (_resolve_expressions)
+         
+          72          96 LOAD_CONST               8 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 72>)
+                      98 MAKE_FUNCTION            0
+                     100 STORE_NAME              13 (render)
+                     102 LOAD_CONST               1 (None)
+                     104 RETURN_VALUE
          consts
             'AdapterNode'
+            None
             'adapter'
             'model'
             'getters'
+            'as_var'
             code
-               argcount  : 4
-               nlocals   : 5
+               argcount  : 5
+               nlocals   : 6
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
-                  007c037c005f0200000000000000007c047c005f03000000000000000064
-                  005300
-                49           0 RESUME                   0
+                  007c037c005f0200000000000000007c057c005f0300000000000000007c
+                  047c005f04000000000000000064005300
+                55           0 RESUME                   0
                
-                50           2 LOAD_FAST                1 (adapter)
+                56           2 LOAD_FAST                1 (adapter)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (adapter)
                
-                51          16 LOAD_FAST                2 (model)
+                57          16 LOAD_FAST                2 (model)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (model)
                
-                52          30 LOAD_FAST                3 (getters)
+                58          30 LOAD_FAST                3 (getters)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (getters)
                
-                53          44 LOAD_FAST                4 (kwargs)
+                59          44 LOAD_FAST                5 (kwargs)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (kwargs)
-                            58 LOAD_CONST               0 (None)
-                            60 RETURN_VALUE
+               
+                60          58 LOAD_FAST                4 (as_var)
+                            60 LOAD_FAST                0 (self)
+                            62 STORE_ATTR               4 (as_var)
+                            72 LOAD_CONST               0 (None)
+                            74 RETURN_VALUE
                consts
                   None
-               names      ('adapter', 'model', 'getters', 'kwargs')
-               varnames   ('self', 'adapter', 'model', 'getters', 'kwargs')
+               names      ('adapter', 'model', 'getters', 'kwargs', 'as_var')
+               varnames   ('self', 'adapter', 'model', 'getters', 'as_var', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 49
-               lnotab 0x02010e010e010e01
+               firstlineno 55
+               lnotab 0x02010e010e010e010e01
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
                flags     : 11
                code
                   0x97007c03a0000000000000000000000000000000000000000000a60000
                   00ab00000000000000000044005d325c0200007d047d0574030000000000
                   00000000007c05740400000000000000000000a6020000ab020000000000
                   00000072187c05a00300000000000000000000000000000000000000007c
                   01a6010000ab0100000000000000007c037c043c0000008c337403000000
                   000000000000007c02740400000000000000000000a6020000ab02000000
                   000000000072157c02a00300000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d027c027c0366025300
-                55           0 RESUME                   0
+                62           0 RESUME                   0
                
-                56           2 LOAD_FAST                3 (kwargs)
+                63           2 LOAD_FAST                3 (kwargs)
                              4 LOAD_METHOD              0 (items)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 GET_ITER
                        >>   42 FOR_ITER                50 (to 144)
                             44 UNPACK_SEQUENCE          2
                             48 STORE_FAST               4 (k)
                             50 STORE_FAST               5 (v)
                
-                57          52 LOAD_GLOBAL              3 (NULL + isinstance)
+                64          52 LOAD_GLOBAL              3 (NULL + isinstance)
                             64 LOAD_FAST                5 (v)
                             66 LOAD_GLOBAL              4 (FilterExpression)
                             78 PRECALL                  2
                             82 CALL                     2
                             92 POP_JUMP_FORWARD_IF_FALSE    24 (to 142)
                
-                58          94 LOAD_FAST                5 (v)
+                65          94 LOAD_FAST                5 (v)
                             96 LOAD_METHOD              3 (resolve)
                            118 LOAD_FAST                1 (context)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 LOAD_FAST                3 (kwargs)
                            136 LOAD_FAST                4 (k)
                            138 STORE_SUBSCR
                        >>  142 JUMP_BACKWARD           51 (to 42)
                
-                60     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
+                67     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
                            156 LOAD_FAST                2 (model)
                            158 LOAD_GLOBAL              4 (FilterExpression)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 POP_JUMP_FORWARD_IF_FALSE    21 (to 228)
                
-                61         186 LOAD_FAST                2 (model)
+                68         186 LOAD_FAST                2 (model)
                            188 LOAD_METHOD              3 (resolve)
                            210 LOAD_FAST                1 (context)
                            212 PRECALL                  1
                            216 CALL                     1
                            226 STORE_FAST               2 (model)
                
-                63     >>  228 LOAD_FAST                2 (model)
+                70     >>  228 LOAD_FAST                2 (model)
                            230 LOAD_FAST                3 (kwargs)
                            232 BUILD_TUPLE              2
                            234 RETURN_VALUE
                consts
                   None
                names      ('items', 'isinstance', 'FilterExpression', 'resolve')
                varnames   ('self', 'context', 'model', 'kwargs', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '_resolve_expressions'
-               firstlineno 55
+               firstlineno 62
                lnotab 0x020132012a0132022a012a02
             code
                argcount  : 2
                nlocals   : 12
-               stacksize : 8
+               stacksize : 9
                flags     : 3
                code
                   0x97007c006a0000000000000000007d027c006a0100000000000000007d
                   0302007c006a0200000000000000007c017c02660269007c006a03000000
                   0000000000a4018e015c0200007d027d0464017c017600721864027c0176
                   0072147c0273127c016401190000000000000000007d057c016402190000
-                  000000000000007d0690016e087c0273847409000000000000000000006a
+                  000000000000007d0690016e1c7c0273987409000000000000000000006a
                   050000000000000000740c0000000000000000000064037c006a07000000
                   00000000006a08000000000000000069017a060000741200000000000000
                   000000a6020000ab02000000000000000001007c01a00a00000000000000
                   00000000000000000000000000a6000000ab0000000000000000007d0109
-                  0002007c006a0700000000000000006a0b00000000000000007c01660169
-                  007c04a4018e0153002300741800000000000000000000240072217d0774
-                  1b00000000000000000000741d000000000000000000007c07a6010000ab
-                  010000000000000000a6010000ab010000000000000000820164007d077e
-                  07770177007803590077017c03741f000000000000000000007c03a60100
-                  00ab01000000000000000064047a0a0000190000000000000000007d057c
-                  027d06742100000000000000000000741f000000000000000000007c03a6
-                  010000ab01000000000000000064047a0a0000a6010000ab010000000000
-                  00000044005d487d087c037c08190000000000000000007d090900742300
-                  0000000000000000007c067c09a6020000ab0200000000000000007d068c
-                  1c2300742400000000000000000000240072200100742500000000000000
-                  00000064057c026a1300000000000000006a0800000000000000009b0064
-                  067c099b009d04a6010000ab010000000000000000820177007803590077
-                  017c01a01400000000000000000000000000000000000000006407a60100
-                  00ab0100000000000000007d0a02007c006a07000000000000000064097c
-                  067c057c0a64089c037c04a4018e017d0b7c0ba015000000000000000000
-                  0000000000000000000000a6000000ab0000000000000000007210742d00
-                  0000000000000000007c0a7c06a6020000ab02000000000000000073157c
-                  0ba01700000000000000000000000000000000000000007c01a6010000ab
-                  01000000000000000053007431000000000000000000007c0a7c0b7c01a6
+                  007417000000000000000000007c006a0b00000000000000007c0102007c
+                  006a0700000000000000006a0c00000000000000007c01660169007c04a4
+                  018e01a6030000ab03000000000000000053002300741a00000000000000
+                  000000240072217d07741d00000000000000000000741f00000000000000
+                  0000007c07a6010000ab010000000000000000a6010000ab010000000000
+                  000000820164007d077e07770177007803590077017c0374210000000000
+                  00000000007c03a6010000ab01000000000000000064047a0a0000190000
+                  000000000000007d057c027d067423000000000000000000007421000000
+                  000000000000007c03a6010000ab01000000000000000064047a0a0000a6
+                  010000ab01000000000000000044005d487d087c037c0819000000000000
+                  0000007d0909007425000000000000000000007c067c09a6020000ab0200
+                  000000000000007d068c1c23007426000000000000000000002400722001
+                  0074270000000000000000000064057c026a1400000000000000006a0800
+                  000000000000009b0064067c099b009d04a6010000ab0100000000000000
+                  00820177007803590077017c01a015000000000000000000000000000000
+                  00000000006407a6010000ab0100000000000000007d0a02007c006a0700
+                  0000000000000064097c067c057c0a64089c037c04a4018e017d0b7c0ba0
+                  160000000000000000000000000000000000000000a6000000ab00000000
+                  00000000007210742f000000000000000000007c0a7c06a6020000ab0200
+                  0000000000000073297417000000000000000000007c006a0b0000000000
+                  0000007c017c0ba01800000000000000000000000000000000000000007c
+                  01a6010000ab010000000000000000a6030000ab03000000000000000053
+                  007417000000000000000000007c006a0b00000000000000007c01743300
+                  0000000000000000007c0a7c0b7c01a6030000ab030000000000000000a6
                   030000ab0300000000000000005300
-                65           0 RESUME                   0
+                72           0 RESUME                   0
                
-                66           2 LOAD_FAST                0 (self)
+                73           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (model)
                             14 STORE_FAST               2 (model)
                
-                67          16 LOAD_FAST                0 (self)
+                74          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (getters)
                             28 STORE_FAST               3 (getters)
                
-                69          30 PUSH_NULL
+                76          30 PUSH_NULL
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                2 (_resolve_expressions)
                
-                70          44 LOAD_FAST                1 (context)
+                77          44 LOAD_FAST                1 (context)
                             46 LOAD_FAST                2 (model)
                
-                69          48 BUILD_TUPLE              2
+                76          48 BUILD_TUPLE              2
                             50 BUILD_MAP                0
                
-                70          52 LOAD_FAST                0 (self)
+                77          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (kwargs)
                
-                69          64 DICT_MERGE               1
+                76          64 DICT_MERGE               1
                             66 CALL_FUNCTION_EX         1
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               2 (model)
                             74 STORE_FAST               4 (kwargs)
                
-                73          76 LOAD_CONST               1 ('wagtail_fedit_field')
+                80          76 LOAD_CONST               1 ('wagtail_fedit_field')
                             78 LOAD_FAST                1 (context)
                             80 CONTAINS_OP              0
                             82 POP_JUMP_FORWARD_IF_FALSE    24 (to 132)
                
-                74          84 LOAD_CONST               2 ('wagtail_fedit_instance')
+                81          84 LOAD_CONST               2 ('wagtail_fedit_instance')
                             86 LOAD_FAST                1 (context)
                             88 CONTAINS_OP              0
                             90 POP_JUMP_FORWARD_IF_FALSE    20 (to 132)
                
-                75          92 LOAD_FAST                2 (model)
+                82          92 LOAD_FAST                2 (model)
                
-                74          94 POP_JUMP_FORWARD_IF_TRUE    18 (to 132)
+                81          94 POP_JUMP_FORWARD_IF_TRUE    18 (to 132)
                
-                77          96 LOAD_FAST                1 (context)
+                84          96 LOAD_FAST                1 (context)
                             98 LOAD_CONST               1 ('wagtail_fedit_field')
                            100 BINARY_SUBSCR
                            110 STORE_FAST               5 (field_name)
                
-                78         112 LOAD_FAST                1 (context)
+                85         112 LOAD_FAST                1 (context)
                            114 LOAD_CONST               2 ('wagtail_fedit_instance')
                            116 BINARY_SUBSCR
                            126 STORE_FAST               6 (obj)
                            128 EXTENDED_ARG             1
-                           130 JUMP_FORWARD           264 (to 660)
+                           130 JUMP_FORWARD           284 (to 700)
                
-                82     >>  132 LOAD_FAST                2 (model)
-                           134 POP_JUMP_FORWARD_IF_TRUE   132 (to 400)
+                89     >>  132 LOAD_FAST                2 (model)
+                           134 POP_JUMP_FORWARD_IF_TRUE   152 (to 440)
                
-                83         136 LOAD_GLOBAL              9 (NULL + warnings)
+                90         136 LOAD_GLOBAL              9 (NULL + warnings)
                            148 LOAD_ATTR                5 (warn)
                
-                84         158 LOAD_GLOBAL             12 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+                91         158 LOAD_GLOBAL             12 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
                
-                85         170 LOAD_CONST               3 ('object')
+                92         170 LOAD_CONST               3 ('object')
                            172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                7 (adapter)
                            184 LOAD_ATTR                8 (__name__)
                
-                84         194 BUILD_MAP                1
+                91         194 BUILD_MAP                1
                            196 BINARY_OP                6 (%)
                
-                87         200 LOAD_GLOBAL             18 (RuntimeWarning)
+                94         200 LOAD_GLOBAL             18 (RuntimeWarning)
                
-                83         212 PRECALL                  2
+                90         212 PRECALL                  2
                            216 CALL                     2
                            226 POP_TOP
                
-                90         228 LOAD_FAST                1 (context)
+                97         228 LOAD_FAST                1 (context)
                            230 LOAD_METHOD             10 (flatten)
                            252 PRECALL                  0
                            256 CALL                     0
                            266 STORE_FAST               1 (context)
                
-                92         268 NOP
+                99         268 NOP
                
-                93         270 PUSH_NULL
-                           272 LOAD_FAST                0 (self)
-                           274 LOAD_ATTR                7 (adapter)
-                           284 LOAD_ATTR               11 (render_from_kwargs)
-               
-                94         294 LOAD_FAST                1 (context)
-               
-                93         296 BUILD_TUPLE              1
-                           298 BUILD_MAP                0
-               
-                94         300 LOAD_FAST                4 (kwargs)
-               
-                93         302 DICT_MERGE               1
-                           304 CALL_FUNCTION_EX         1
-                           306 RETURN_VALUE
-                       >>  308 PUSH_EXC_INFO
-               
-                96         310 LOAD_GLOBAL             24 (AdapterError)
-                           322 CHECK_EXC_MATCH
-                           324 POP_JUMP_FORWARD_IF_FALSE    33 (to 392)
-                           326 STORE_FAST               7 (e)
-               
-                97         328 LOAD_GLOBAL             27 (NULL + TemplateSyntaxError)
-                           340 LOAD_GLOBAL             29 (NULL + str)
-                           352 LOAD_FAST                7 (e)
-                           354 PRECALL                  1
-                           358 CALL                     1
-                           368 PRECALL                  1
-                           372 CALL                     1
-                           382 RAISE_VARARGS            1
-                       >>  384 LOAD_CONST               0 (None)
-                           386 STORE_FAST               7 (e)
-                           388 DELETE_FAST              7 (e)
-                           390 RERAISE                  1
-               
-                96     >>  392 RERAISE                  0
-                       >>  394 COPY                     3
-                           396 POP_EXCEPT
-                           398 RERAISE                  1
-               
-                99     >>  400 LOAD_FAST                3 (getters)
-                           402 LOAD_GLOBAL             31 (NULL + len)
-                           414 LOAD_FAST                3 (getters)
-                           416 PRECALL                  1
-                           420 CALL                     1
-                           430 LOAD_CONST               4 (1)
-                           432 BINARY_OP               10 (-)
-                           436 BINARY_SUBSCR
-                           446 STORE_FAST               5 (field_name)
-               
-               100         448 LOAD_FAST                2 (model)
-                           450 STORE_FAST               6 (obj)
-               
-               101         452 LOAD_GLOBAL             33 (NULL + range)
-                           464 LOAD_GLOBAL             31 (NULL + len)
-                           476 LOAD_FAST                3 (getters)
-                           478 PRECALL                  1
-                           482 CALL                     1
-                           492 LOAD_CONST               4 (1)
-                           494 BINARY_OP               10 (-)
-                           498 PRECALL                  1
-                           502 CALL                     1
-                           512 GET_ITER
-                       >>  514 FOR_ITER                72 (to 660)
-                           516 STORE_FAST               8 (i)
-               
-               102         518 LOAD_FAST                3 (getters)
-                           520 LOAD_FAST                8 (i)
-                           522 BINARY_SUBSCR
-                           532 STORE_FAST               9 (getter)
-               
-               103         534 NOP
-               
-               104         536 LOAD_GLOBAL             35 (NULL + getattr)
-                           548 LOAD_FAST                6 (obj)
-                           550 LOAD_FAST                9 (getter)
-                           552 PRECALL                  2
-                           556 CALL                     2
-                           566 STORE_FAST               6 (obj)
-                           568 JUMP_BACKWARD           28 (to 514)
-                       >>  570 PUSH_EXC_INFO
-               
-               105         572 LOAD_GLOBAL             36 (AttributeError)
-                           584 CHECK_EXC_MATCH
-                           586 POP_JUMP_FORWARD_IF_FALSE    32 (to 652)
-                           588 POP_TOP
-               
-               106         590 LOAD_GLOBAL             37 (NULL + AttributeError)
-                           602 LOAD_CONST               5 ('Object ')
-                           604 LOAD_FAST                2 (model)
-                           606 LOAD_ATTR               19 (__class__)
-                           616 LOAD_ATTR                8 (__name__)
-                           626 FORMAT_VALUE             0
-                           628 LOAD_CONST               6 (' does not have attribute ')
-                           630 LOAD_FAST                9 (getter)
-                           632 FORMAT_VALUE             0
-                           634 BUILD_STRING             4
-                           636 PRECALL                  1
-                           640 CALL                     1
-                           650 RAISE_VARARGS            1
-               
-               105     >>  652 RERAISE                  0
-                       >>  654 COPY                     3
-                           656 POP_EXCEPT
-                           658 RERAISE                  1
-               
-               108     >>  660 LOAD_FAST                1 (context)
-                           662 LOAD_METHOD             20 (get)
-                           684 LOAD_CONST               7 ('request')
-                           686 PRECALL                  1
-                           690 CALL                     1
-                           700 STORE_FAST              10 (request)
-               
-               109         702 PUSH_NULL
-                           704 LOAD_FAST                0 (self)
-                           706 LOAD_ATTR                7 (adapter)
-                           716 LOAD_CONST               9 (())
-               
-               110         718 LOAD_FAST                6 (obj)
-               
-               111         720 LOAD_FAST                5 (field_name)
-               
-               112         722 LOAD_FAST               10 (request)
-               
-               109         724 LOAD_CONST               8 (('object', 'field_name', 'request'))
-                           726 BUILD_CONST_KEY_MAP      3
-               
-               113         728 LOAD_FAST                4 (kwargs)
-               
-               109         730 DICT_MERGE               1
-                           732 CALL_FUNCTION_EX         1
-                           734 STORE_FAST              11 (adapter)
-               
-               116         736 LOAD_FAST               11 (adapter)
-                           738 LOAD_METHOD             21 (check_permissions)
-                           760 PRECALL                  0
-                           764 CALL                     0
-                           774 POP_JUMP_FORWARD_IF_FALSE    16 (to 808)
-               
-               117         776 LOAD_GLOBAL             45 (NULL + _can_edit)
-                           788 LOAD_FAST               10 (request)
-                           790 LOAD_FAST                6 (obj)
-                           792 PRECALL                  2
-                           796 CALL                     2
-               
-               116         806 POP_JUMP_FORWARD_IF_TRUE    21 (to 850)
-               
-               118     >>  808 LOAD_FAST               11 (adapter)
-                           810 LOAD_METHOD             23 (render_content)
-                           832 LOAD_FAST                1 (context)
-                           834 PRECALL                  1
-                           838 CALL                     1
-                           848 RETURN_VALUE
-               
-               120     >>  850 LOAD_GLOBAL             49 (NULL + wrap_adapter)
-                           862 LOAD_FAST               10 (request)
-                           864 LOAD_FAST               11 (adapter)
-                           866 LOAD_FAST                1 (context)
-                           868 PRECALL                  3
-                           872 CALL                     3
-                           882 RETURN_VALUE
+               100         270 LOAD_GLOBAL             23 (NULL + as_var)
+                           282 LOAD_FAST                0 (self)
+                           284 LOAD_ATTR               11 (as_var)
+                           294 LOAD_FAST                1 (context)
+                           296 PUSH_NULL
+                           298 LOAD_FAST                0 (self)
+                           300 LOAD_ATTR                7 (adapter)
+                           310 LOAD_ATTR               12 (render_from_kwargs)
+               
+               101         320 LOAD_FAST                1 (context)
+               
+               100         322 BUILD_TUPLE              1
+                           324 BUILD_MAP                0
+               
+               101         326 LOAD_FAST                4 (kwargs)
+               
+               100         328 DICT_MERGE               1
+                           330 CALL_FUNCTION_EX         1
+                           332 PRECALL                  3
+                           336 CALL                     3
+                           346 RETURN_VALUE
+                       >>  348 PUSH_EXC_INFO
+               
+               103         350 LOAD_GLOBAL             26 (AdapterError)
+                           362 CHECK_EXC_MATCH
+                           364 POP_JUMP_FORWARD_IF_FALSE    33 (to 432)
+                           366 STORE_FAST               7 (e)
+               
+               104         368 LOAD_GLOBAL             29 (NULL + TemplateSyntaxError)
+                           380 LOAD_GLOBAL             31 (NULL + str)
+                           392 LOAD_FAST                7 (e)
+                           394 PRECALL                  1
+                           398 CALL                     1
+                           408 PRECALL                  1
+                           412 CALL                     1
+                           422 RAISE_VARARGS            1
+                       >>  424 LOAD_CONST               0 (None)
+                           426 STORE_FAST               7 (e)
+                           428 DELETE_FAST              7 (e)
+                           430 RERAISE                  1
+               
+               103     >>  432 RERAISE                  0
+                       >>  434 COPY                     3
+                           436 POP_EXCEPT
+                           438 RERAISE                  1
+               
+               106     >>  440 LOAD_FAST                3 (getters)
+                           442 LOAD_GLOBAL             33 (NULL + len)
+                           454 LOAD_FAST                3 (getters)
+                           456 PRECALL                  1
+                           460 CALL                     1
+                           470 LOAD_CONST               4 (1)
+                           472 BINARY_OP               10 (-)
+                           476 BINARY_SUBSCR
+                           486 STORE_FAST               5 (field_name)
+               
+               107         488 LOAD_FAST                2 (model)
+                           490 STORE_FAST               6 (obj)
+               
+               108         492 LOAD_GLOBAL             35 (NULL + range)
+                           504 LOAD_GLOBAL             33 (NULL + len)
+                           516 LOAD_FAST                3 (getters)
+                           518 PRECALL                  1
+                           522 CALL                     1
+                           532 LOAD_CONST               4 (1)
+                           534 BINARY_OP               10 (-)
+                           538 PRECALL                  1
+                           542 CALL                     1
+                           552 GET_ITER
+                       >>  554 FOR_ITER                72 (to 700)
+                           556 STORE_FAST               8 (i)
+               
+               109         558 LOAD_FAST                3 (getters)
+                           560 LOAD_FAST                8 (i)
+                           562 BINARY_SUBSCR
+                           572 STORE_FAST               9 (getter)
+               
+               110         574 NOP
+               
+               111         576 LOAD_GLOBAL             37 (NULL + getattr)
+                           588 LOAD_FAST                6 (obj)
+                           590 LOAD_FAST                9 (getter)
+                           592 PRECALL                  2
+                           596 CALL                     2
+                           606 STORE_FAST               6 (obj)
+                           608 JUMP_BACKWARD           28 (to 554)
+                       >>  610 PUSH_EXC_INFO
+               
+               112         612 LOAD_GLOBAL             38 (AttributeError)
+                           624 CHECK_EXC_MATCH
+                           626 POP_JUMP_FORWARD_IF_FALSE    32 (to 692)
+                           628 POP_TOP
+               
+               113         630 LOAD_GLOBAL             39 (NULL + AttributeError)
+                           642 LOAD_CONST               5 ('Object ')
+                           644 LOAD_FAST                2 (model)
+                           646 LOAD_ATTR               20 (__class__)
+                           656 LOAD_ATTR                8 (__name__)
+                           666 FORMAT_VALUE             0
+                           668 LOAD_CONST               6 (' does not have attribute ')
+                           670 LOAD_FAST                9 (getter)
+                           672 FORMAT_VALUE             0
+                           674 BUILD_STRING             4
+                           676 PRECALL                  1
+                           680 CALL                     1
+                           690 RAISE_VARARGS            1
+               
+               112     >>  692 RERAISE                  0
+                       >>  694 COPY                     3
+                           696 POP_EXCEPT
+                           698 RERAISE                  1
+               
+               115     >>  700 LOAD_FAST                1 (context)
+                           702 LOAD_METHOD             21 (get)
+                           724 LOAD_CONST               7 ('request')
+                           726 PRECALL                  1
+                           730 CALL                     1
+                           740 STORE_FAST              10 (request)
+               
+               116         742 PUSH_NULL
+                           744 LOAD_FAST                0 (self)
+                           746 LOAD_ATTR                7 (adapter)
+                           756 LOAD_CONST               9 (())
+               
+               117         758 LOAD_FAST                6 (obj)
+               
+               118         760 LOAD_FAST                5 (field_name)
+               
+               119         762 LOAD_FAST               10 (request)
+               
+               116         764 LOAD_CONST               8 (('object', 'field_name', 'request'))
+                           766 BUILD_CONST_KEY_MAP      3
+               
+               120         768 LOAD_FAST                4 (kwargs)
+               
+               116         770 DICT_MERGE               1
+                           772 CALL_FUNCTION_EX         1
+                           774 STORE_FAST              11 (adapter)
+               
+               123         776 LOAD_FAST               11 (adapter)
+                           778 LOAD_METHOD             22 (check_permissions)
+                           800 PRECALL                  0
+                           804 CALL                     0
+                           814 POP_JUMP_FORWARD_IF_FALSE    16 (to 848)
+               
+               124         816 LOAD_GLOBAL             47 (NULL + _can_edit)
+                           828 LOAD_FAST               10 (request)
+                           830 LOAD_FAST                6 (obj)
+                           832 PRECALL                  2
+                           836 CALL                     2
+               
+               123         846 POP_JUMP_FORWARD_IF_TRUE    41 (to 930)
+               
+               125     >>  848 LOAD_GLOBAL             23 (NULL + as_var)
+                           860 LOAD_FAST                0 (self)
+                           862 LOAD_ATTR               11 (as_var)
+                           872 LOAD_FAST                1 (context)
+                           874 LOAD_FAST               11 (adapter)
+                           876 LOAD_METHOD             24 (render_content)
+                           898 LOAD_FAST                1 (context)
+                           900 PRECALL                  1
+                           904 CALL                     1
+                           914 PRECALL                  3
+                           918 CALL                     3
+                           928 RETURN_VALUE
+               
+               127     >>  930 LOAD_GLOBAL             23 (NULL + as_var)
+                           942 LOAD_FAST                0 (self)
+                           944 LOAD_ATTR               11 (as_var)
+                           954 LOAD_FAST                1 (context)
+                           956 LOAD_GLOBAL             51 (NULL + wrap_adapter)
+                           968 LOAD_FAST               10 (request)
+                           970 LOAD_FAST               11 (adapter)
+                           972 LOAD_FAST                1 (context)
+                           974 PRECALL                  3
+                           978 CALL                     3
+                           988 PRECALL                  3
+                           992 CALL                     3
+                          1002 RETURN_VALUE
                ExceptionTable:
-                 270 to 304 -> 308 [0]
-                 308 to 326 -> 394 [1] lasti
-                 328 to 382 -> 384 [1] lasti
-                 384 to 392 -> 394 [1] lasti
-                 536 to 566 -> 570 [1]
-                 570 to 652 -> 654 [2] lasti
+                 270 to 344 -> 348 [0]
+                 348 to 366 -> 434 [1] lasti
+                 368 to 422 -> 424 [1] lasti
+                 424 to 432 -> 434 [1] lasti
+                 576 to 606 -> 610 [1]
+                 610 to 692 -> 694 [2] lasti
                consts
                   None
                   'wagtail_fedit_field'
                   'wagtail_fedit_instance'
                   'object'
                   1
                   'Object '
                   ' does not have attribute '
                   'request'
                   ('object', 'field_name', 'request')
                   ()
-               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'adapter', '__name__', 'RuntimeWarning', 'flatten', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'render_content', 'wrap_adapter')
+               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'adapter', '__name__', 'RuntimeWarning', 'flatten', 'as_var', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'render_content', 'wrap_adapter')
                varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 65
+               firstlineno 72
                lnotab
                   0x02010e010e020e0104ff04010cff0c040801080102ff02031001140404
-                  0116010c0118ff06030cfc100728020201180102ff040102ff0803120140
+                  0116010c0118ff06030cfc100728020201320102ff040102ff1603120140
                   ff080330010401420110010201240112013eff08032a0110010201020102
-                  fd040402fc060728011eff02022a02
-            None
+                  fd040402fc060728011eff02025202
+            (None,)
          names      ('__name__', '__module__', '__qualname__', 'signing', 'TimestampSigner', 'signer', 'Type', 'BaseAdapter', 'FilterExpression', 'list', 'str', '__init__', '_resolve_expressions', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'AdapterNode'
-         firstlineno 46
-         lnotab 0x0a011e022c06060a
+         firstlineno 52
+         lnotab 0x0a011e023207060a
       'AdapterNode'
       ('name',)
       'parser'
       'token'
       code
          argcount  : 2
-         nlocals   : 10
-         stacksize : 7
+         nlocals   : 11
+         stacksize : 8
          flags     : 3
          code
             0x97007c01a0000000000000000000000000000000000000000000a60000
             00ab0000000000000000007d027c02a00100000000000000000000000000
             000000000000006401a6010000ab0100000000000000007d037c02a00100
             000000000000000000000000000000000000006401a6010000ab01000000
             00000000007d0409007404000000000000000000007c0419000000000000
@@ -762,256 +842,305 @@
             0000006405a6010000ab0100000000000000007d07740d00000000000000
             0000007c07a6010000ab01000000000000000064066b0000000000721b7c
             0764011900000000000000000064076b0300000000720f74090000000000
             00000000006408a6010000ab0100000000000000008201740d0000000000
             00000000007c07a6010000ab01000000000000000064096b040000000072
             287c00a00700000000000000000000000000000000000000007c07a00100
             000000000000000000000000000000000000006401a6010000ab01000000
-            0000000000a6010000ab0100000000000000007d06741100000000000000
-            0000007c007c027c056a0900000000000000007c056a0a00000000000000
-            00a6040000ab0400000000000000007d0974170000000000000000000064
-            0b7c057c067c07640a9c037c09a4018e015300
-         123           0 RESUME                   0
+            0000000000a6010000ab0100000000000000007d0664007d097c0272667c
+            02740d000000000000000000007c02a6010000ab01000000000000000064
+            067a0a000019000000000000000000640a6b0200000000724a7c02a00100
+            00000000000000000000000000000000000000740d000000000000000000
+            007c02a6010000ab01000000000000000064097a0a0000a6010000ab0100
+            000000000000007d097c02a0010000000000000000000000000000000000
+            000000740d000000000000000000007c02a6010000ab0100000000000000
+            0064097a0a0000a6010000ab010000000000000000010074110000000000
+            00000000007c007c027c056a0900000000000000007c056a0a0000000000
+            000000a6040000ab0400000000000000007d0a7417000000000000000000
+            00640c7c057c067c077c09640b9c047c0aa4018e015300
+         130           0 RESUME                   0
          
-         126           2 LOAD_FAST                1 (token)
+         133           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         128          42 LOAD_FAST                2 (tokens)
+         135          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         129          84 LOAD_FAST                2 (tokens)
+         136          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (adapter_id)
          
-         131         126 NOP
+         138         126 NOP
          
-         132         128 LOAD_GLOBAL              4 (adapter_registry)
+         139         128 LOAD_GLOBAL              4 (adapter_registry)
                      140 LOAD_FAST                4 (adapter_id)
                      142 BINARY_SUBSCR
                      152 STORE_FAST               5 (adapter)
                      154 JUMP_FORWARD            33 (to 222)
                  >>  156 PUSH_EXC_INFO
          
-         133         158 LOAD_GLOBAL              6 (RegistryLookUpError)
+         140         158 LOAD_GLOBAL              6 (RegistryLookUpError)
                      170 CHECK_EXC_MATCH
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
                      174 POP_TOP
          
-         134         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         141         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
                      188 LOAD_CONST               2 ("No adapter found with identifier '")
                      190 LOAD_FAST                4 (adapter_id)
                      192 FORMAT_VALUE             0
                      194 LOAD_CONST               3 ("'")
                      196 BUILD_STRING             3
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         133     >>  214 RERAISE                  0
+         140     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         136     >>  222 LOAD_CONST               4 ((None, None))
+         143     >>  222 LOAD_CONST               4 ((None, None))
                      224 UNPACK_SEQUENCE          2
                      228 STORE_FAST               6 (model)
                      230 STORE_FAST               7 (model_tokens)
          
-         137         232 LOAD_FAST                2 (tokens)
+         144         232 LOAD_FAST                2 (tokens)
                      234 POP_JUMP_FORWARD_IF_FALSE   147 (to 530)
          
-         138         236 LOAD_FAST                2 (tokens)
+         145         236 LOAD_FAST                2 (tokens)
                      238 LOAD_METHOD              1 (pop)
                      260 LOAD_CONST               1 (0)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST               8 (model__field)
          
-         139         278 LOAD_FAST                8 (model__field)
+         146         278 LOAD_FAST                8 (model__field)
                      280 LOAD_METHOD              5 (split)
                      302 LOAD_CONST               5 ('.')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               7 (model_tokens)
          
-         141         320 LOAD_GLOBAL             13 (NULL + len)
+         148         320 LOAD_GLOBAL             13 (NULL + len)
                      332 LOAD_FAST                7 (model_tokens)
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_CONST               6 (2)
                      350 COMPARE_OP               0 (<)
                      356 POP_JUMP_FORWARD_IF_FALSE    27 (to 412)
          
-         142         358 LOAD_FAST                7 (model_tokens)
+         149         358 LOAD_FAST                7 (model_tokens)
                      360 LOAD_CONST               1 (0)
                      362 BINARY_SUBSCR
                      372 LOAD_CONST               7 ('from_context')
                      374 COMPARE_OP               3 (!=)
                      380 POP_JUMP_FORWARD_IF_FALSE    15 (to 412)
          
-         143         382 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         150         382 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
          
-         144         394 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
+         151         394 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
          
-         143         396 PRECALL                  1
+         150         396 PRECALL                  1
                      400 CALL                     1
                      410 RAISE_VARARGS            1
          
-         147     >>  412 LOAD_GLOBAL             13 (NULL + len)
+         154     >>  412 LOAD_GLOBAL             13 (NULL + len)
                      424 LOAD_FAST                7 (model_tokens)
                      426 PRECALL                  1
                      430 CALL                     1
                      440 LOAD_CONST               9 (1)
                      442 COMPARE_OP               4 (>)
                      448 POP_JUMP_FORWARD_IF_FALSE    40 (to 530)
          
-         150         450 LOAD_FAST                0 (parser)
+         157         450 LOAD_FAST                0 (parser)
                      452 LOAD_METHOD              7 (compile_filter)
                      474 LOAD_FAST                7 (model_tokens)
                      476 LOAD_METHOD              1 (pop)
                      498 LOAD_CONST               1 (0)
                      500 PRECALL                  1
                      504 CALL                     1
                      514 PRECALL                  1
                      518 CALL                     1
                      528 STORE_FAST               6 (model)
          
-         152     >>  530 LOAD_GLOBAL             17 (NULL + get_kwargs)
-         
-         153         542 LOAD_FAST                0 (parser)
-         
-         154         544 LOAD_FAST                2 (tokens)
-         
-         155         546 LOAD_FAST                5 (adapter)
-                     548 LOAD_ATTR                9 (required_kwargs)
-         
-         156         558 LOAD_FAST                5 (adapter)
-                     560 LOAD_ATTR               10 (absolute_tokens)
+         159     >>  530 LOAD_CONST               0 (None)
+                     532 STORE_FAST               9 (as_var)
          
-         152         570 PRECALL                  4
-                     574 CALL                     4
-                     584 STORE_FAST               9 (kwargs)
-         
-         159         586 LOAD_GLOBAL             23 (NULL + AdapterNode)
-                     598 LOAD_CONST              11 (())
-         
-         160         600 LOAD_FAST                5 (adapter)
-         
-         161         602 LOAD_FAST                6 (model)
-         
-         162         604 LOAD_FAST                7 (model_tokens)
-         
-         159         606 LOAD_CONST              10 (('adapter', 'model', 'getters'))
-                     608 BUILD_CONST_KEY_MAP      3
-         
-         163         610 LOAD_FAST                9 (kwargs)
-         
-         159         612 DICT_MERGE               1
-                     614 CALL_FUNCTION_EX         1
-                     616 RETURN_VALUE
+         160         534 LOAD_FAST                2 (tokens)
+                     536 POP_JUMP_FORWARD_IF_FALSE   102 (to 742)
+                     538 LOAD_FAST                2 (tokens)
+                     540 LOAD_GLOBAL             13 (NULL + len)
+                     552 LOAD_FAST                2 (tokens)
+                     554 PRECALL                  1
+                     558 CALL                     1
+                     568 LOAD_CONST               6 (2)
+                     570 BINARY_OP               10 (-)
+                     574 BINARY_SUBSCR
+                     584 LOAD_CONST              10 ('as')
+                     586 COMPARE_OP               2 (==)
+                     592 POP_JUMP_FORWARD_IF_FALSE    74 (to 742)
+         
+         161         594 LOAD_FAST                2 (tokens)
+                     596 LOAD_METHOD              1 (pop)
+                     618 LOAD_GLOBAL             13 (NULL + len)
+                     630 LOAD_FAST                2 (tokens)
+                     632 PRECALL                  1
+                     636 CALL                     1
+                     646 LOAD_CONST               9 (1)
+                     648 BINARY_OP               10 (-)
+                     652 PRECALL                  1
+                     656 CALL                     1
+                     666 STORE_FAST               9 (as_var)
+         
+         162         668 LOAD_FAST                2 (tokens)
+                     670 LOAD_METHOD              1 (pop)
+                     692 LOAD_GLOBAL             13 (NULL + len)
+                     704 LOAD_FAST                2 (tokens)
+                     706 PRECALL                  1
+                     710 CALL                     1
+                     720 LOAD_CONST               9 (1)
+                     722 BINARY_OP               10 (-)
+                     726 PRECALL                  1
+                     730 CALL                     1
+                     740 POP_TOP
+         
+         165     >>  742 LOAD_GLOBAL             17 (NULL + get_kwargs)
+         
+         166         754 LOAD_FAST                0 (parser)
+         
+         167         756 LOAD_FAST                2 (tokens)
+         
+         168         758 LOAD_FAST                5 (adapter)
+                     760 LOAD_ATTR                9 (required_kwargs)
+         
+         169         770 LOAD_FAST                5 (adapter)
+                     772 LOAD_ATTR               10 (absolute_tokens)
+         
+         165         782 PRECALL                  4
+                     786 CALL                     4
+                     796 STORE_FAST              10 (kwargs)
+         
+         172         798 LOAD_GLOBAL             23 (NULL + AdapterNode)
+                     810 LOAD_CONST              12 (())
+         
+         173         812 LOAD_FAST                5 (adapter)
+         
+         174         814 LOAD_FAST                6 (model)
+         
+         175         816 LOAD_FAST                7 (model_tokens)
+         
+         176         818 LOAD_FAST                9 (as_var)
+         
+         172         820 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
+                     822 BUILD_CONST_KEY_MAP      4
+         
+         177         824 LOAD_FAST               10 (kwargs)
+         
+         172         826 DICT_MERGE               1
+                     828 CALL_FUNCTION_EX         1
+                     830 RETURN_VALUE
          ExceptionTable:
            128 to 152 -> 156 [0]
            156 to 214 -> 216 [1] lasti
          consts
             None
             0
             "No adapter found with identifier '"
             "'"
             (None, None)
             '.'
             2
             'from_context'
             "Model and field name are required: 'mymodel.myfield' or 'from_context'"
             1
-            ('adapter', 'model', 'getters')
+            'as'
+            ('adapter', 'model', 'getters', 'as_var')
             ()
          names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'compile_filter', 'get_kwargs', 'required_kwargs', 'absolute_tokens', 'AdapterNode')
-         varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'kwargs')
+         varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'as_var', 'kwargs')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit'
-         firstlineno 123
+         firstlineno 130
          lnotab
             0x020328022a012a0202011e01120126ff08030a0104012a012a02260118
-            010c0102ff1004260350020c01020102010c010cfc10070e010201020102
-            fd040402fc
+            010c0102ff10042603500204013c014a014a030c01020102010c010cfc10
+            070e0102010201020102fc040502fb
       True
       ('takes_context',)
-      'context'
       'adapter'
-      'return'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code
             0x970069007d0264017c007600720b7c006401190000000000000000007d
             027c0064013d007c00a00000000000000000000000000000000000000000
             007c02a6010000ab01000000000000000001007c016a0100000000000000
             007c0064023c0000007c016a0200000000000000007c0064033c0000007c
             016a0300000000000000007c0064043c0000007c01a00400000000000000
             000000000000000000000000007c00a6010000ab01000000000000000053
             00
-         168           0 RESUME                   0
+         182           0 RESUME                   0
          
-         170           2 BUILD_MAP                0
+         184           2 BUILD_MAP                0
                        4 STORE_FAST               2 (parent_context)
          
-         172           6 LOAD_CONST               1 ('parent_context')
+         186           6 LOAD_CONST               1 ('parent_context')
                        8 LOAD_FAST                0 (context)
                       10 CONTAINS_OP              0
                       12 POP_JUMP_FORWARD_IF_FALSE    11 (to 36)
          
-         173          14 LOAD_FAST                0 (context)
+         187          14 LOAD_FAST                0 (context)
                       16 LOAD_CONST               1 ('parent_context')
                       18 BINARY_SUBSCR
                       28 STORE_FAST               2 (parent_context)
          
-         174          30 LOAD_FAST                0 (context)
+         188          30 LOAD_FAST                0 (context)
                       32 LOAD_CONST               1 ('parent_context')
                       34 DELETE_SUBSCR
          
-         176     >>   36 LOAD_FAST                0 (context)
+         190     >>   36 LOAD_FAST                0 (context)
                       38 LOAD_METHOD              0 (update)
                       60 LOAD_FAST                2 (parent_context)
                       62 PRECALL                  1
                       66 CALL                     1
                       76 POP_TOP
          
-         178          78 LOAD_FAST                1 (adapter)
+         192          78 LOAD_FAST                1 (adapter)
                       80 LOAD_ATTR                1 (field_name)
                       90 LOAD_FAST                0 (context)
                       92 LOAD_CONST               2 ('wagtail_fedit_field')
                       94 STORE_SUBSCR
          
-         179          98 LOAD_FAST                1 (adapter)
+         193          98 LOAD_FAST                1 (adapter)
                      100 LOAD_ATTR                2 (object)
                      110 LOAD_FAST                0 (context)
                      112 LOAD_CONST               3 ('wagtail_fedit_instance')
                      114 STORE_SUBSCR
          
-         180         118 LOAD_FAST                1 (adapter)
+         194         118 LOAD_FAST                1 (adapter)
                      120 LOAD_ATTR                3 (request)
                      130 LOAD_FAST                0 (context)
                      132 LOAD_CONST               4 ('request')
                      134 STORE_SUBSCR
          
-         182         138 LOAD_FAST                1 (adapter)
+         196         138 LOAD_FAST                1 (adapter)
                      140 LOAD_METHOD              4 (render_content)
                      162 LOAD_FAST                0 (context)
                      164 PRECALL                  1
                      168 CALL                     1
                      178 RETURN_VALUE
          consts
             None
@@ -1019,17 +1148,17 @@
             'wagtail_fedit_field'
             'wagtail_fedit_instance'
             'request'
          names      ('update', 'field_name', 'object', 'request', 'render_content')
          varnames   ('context', 'adapter', 'parent_context')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_adapter'
-         firstlineno 168
+         firstlineno 182
          lnotab 0x020204020801100106022a02140114011402
       'wagtail_fedit/_hook_output.html'
       'fedit_scripts'
       ('name', 'takes_context')
       code
          argcount  : 2
          nlocals   : 7
@@ -1046,123 +1175,123 @@
             00530067007d04740f000000000000000000006a0800000000000000007c
             03a6010000ab01000000000000000044005d417d0502007c057c02a60100
             00ab0100000000000000007d067413000000000000000000007c06741400
             0000000000000000007416000000000000000000006602a6020000ab0200
             0000000000000073037c0667017d067c04a00c0000000000000000000000
             0000000000000000007c06a6010000ab01000000000000000001008c4264
             067c0469015300
-         185           0 RESUME                   0
+         199           0 RESUME                   0
          
-         187           2 LOAD_FAST                1 (css_or_js)
+         201           2 LOAD_FAST                1 (css_or_js)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               1 (css_or_js)
          
-         189          42 LOAD_FAST                1 (css_or_js)
+         203          42 LOAD_FAST                1 (css_or_js)
                       44 LOAD_CONST               1 (('css', 'js'))
                       46 CONTAINS_OP              1
                       48 POP_JUMP_FORWARD_IF_FALSE    15 (to 80)
          
-         190          50 LOAD_GLOBAL              3 (NULL + ValueError)
+         204          50 LOAD_GLOBAL              3 (NULL + ValueError)
                       62 LOAD_CONST               2 ("Invalid argument, must be 'css' or 'js'")
                       64 PRECALL                  1
                       68 CALL                     1
                       78 RAISE_VARARGS            1
          
-         192     >>   80 LOAD_FAST                0 (context)
+         206     >>   80 LOAD_FAST                0 (context)
                       82 LOAD_METHOD              2 (get)
                      104 LOAD_CONST               3 ('request')
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               2 (request)
          
-         194         122 LOAD_FAST                1 (css_or_js)
+         208         122 LOAD_FAST                1 (css_or_js)
                      124 LOAD_CONST               4 ('css')
                      126 COMPARE_OP               2 (==)
                      132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
          
-         195         134 LOAD_GLOBAL              6 (REGISTER_CSS)
+         209         134 LOAD_GLOBAL              6 (REGISTER_CSS)
                      146 STORE_FAST               3 (hook_name)
                      148 JUMP_FORWARD             7 (to 164)
          
-         197     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
+         211     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
                      162 STORE_FAST               3 (hook_name)
          
-         199     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
+         213     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
                      176 LOAD_FAST                2 (request)
                      178 LOAD_GLOBAL             12 (FEDIT_PREVIEW_VAR)
                      190 LOAD_CONST               5 (False)
                      192 PRECALL                  3
                      196 CALL                     3
                      206 POP_JUMP_FORWARD_IF_TRUE     2 (to 212)
          
-         200         208 BUILD_MAP                0
+         214         208 BUILD_MAP                0
                      210 RETURN_VALUE
          
-         202     >>  212 BUILD_LIST               0
+         216     >>  212 BUILD_LIST               0
                      214 STORE_FAST               4 (files)
          
-         203         216 LOAD_GLOBAL             15 (NULL + hooks)
+         217         216 LOAD_GLOBAL             15 (NULL + hooks)
                      228 LOAD_ATTR                8 (get_hooks)
                      238 LOAD_FAST                3 (hook_name)
                      240 PRECALL                  1
                      244 CALL                     1
                      254 GET_ITER
                  >>  256 FOR_ITER                65 (to 388)
                      258 STORE_FAST               5 (hook)
          
-         204         260 PUSH_NULL
+         218         260 PUSH_NULL
                      262 LOAD_FAST                5 (hook)
                      264 LOAD_FAST                2 (request)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 STORE_FAST               6 (ret)
          
-         206         282 LOAD_GLOBAL             19 (NULL + isinstance)
+         220         282 LOAD_GLOBAL             19 (NULL + isinstance)
                      294 LOAD_FAST                6 (ret)
                      296 LOAD_GLOBAL             20 (list)
                      308 LOAD_GLOBAL             22 (tuple)
                      320 BUILD_TUPLE              2
                      322 PRECALL                  2
                      326 CALL                     2
                      336 POP_JUMP_FORWARD_IF_TRUE     3 (to 344)
          
-         207         338 LOAD_FAST                6 (ret)
+         221         338 LOAD_FAST                6 (ret)
                      340 BUILD_LIST               1
                      342 STORE_FAST               6 (ret)
          
-         209     >>  344 LOAD_FAST                4 (files)
+         223     >>  344 LOAD_FAST                4 (files)
                      346 LOAD_METHOD             12 (extend)
                      368 LOAD_FAST                6 (ret)
                      370 PRECALL                  1
                      374 CALL                     1
                      384 POP_TOP
                      386 JUMP_BACKWARD           66 (to 256)
          
-         212     >>  388 LOAD_CONST               6 ('hook_output')
+         226     >>  388 LOAD_CONST               6 ('hook_output')
                      390 LOAD_FAST                4 (files)
          
-         211         392 BUILD_MAP                1
+         225         392 BUILD_MAP                1
                      394 RETURN_VALUE
          consts
             None
             ('css', 'js')
             "Invalid argument, must be 'css' or 'js'"
             'request'
             'css'
             False
             'hook_output'
          names      ('lower', 'ValueError', 'get', 'REGISTER_CSS', 'REGISTER_JS', 'getattr', 'FEDIT_PREVIEW_VAR', 'hooks', 'get_hooks', 'isinstance', 'list', 'tuple', 'extend')
          varnames   ('context', 'css_or_js', 'request', 'hook_name', 'files', 'hook', 'ret')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'static_hook_output'
-         firstlineno 185
+         firstlineno 199
          lnotab
             0x0202280208011e022a020c0110020e022c01040204012c011602380106
             022c0304ff
       'tokens'
       'kwarg_list'
       'absolute_tokens'
       code
@@ -1190,204 +1319,204 @@
             086404190000000000000000007d097c097c037600721374070000000000
             000000000064077c099b0064089d03a6010000ab01000000000000000082
             017c00a00400000000000000000000000000000000000000007c08640319
             000000000000000000a6010000ab0100000000000000007c057c093c0000
             0064057d0490018c147c0244005d187d0b7c0b7c0576017212740b000000
             0000000000000064097c0b9b009d02a6010000ab01000000000000000082
             018c197c055300
-         216           0 RESUME                   0
+         230           0 RESUME                   0
          
-         217           2 LOAD_CONST               1 (False)
+         231           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               4 (had_kwargs)
          
-         218           6 BUILD_MAP                0
+         232           6 BUILD_MAP                0
                        8 STORE_FAST               5 (kwargs)
          
-         220          10 LOAD_FAST                2 (kwarg_list)
+         234          10 LOAD_FAST                2 (kwarg_list)
                       12 POP_JUMP_FORWARD_IF_TRUE     2 (to 18)
          
-         221          14 BUILD_LIST               0
+         235          14 BUILD_LIST               0
                       16 STORE_FAST               2 (kwarg_list)
          
-         223     >>   18 LOAD_FAST                3 (absolute_tokens)
+         237     >>   18 LOAD_FAST                3 (absolute_tokens)
                       20 POP_JUMP_FORWARD_IF_TRUE     2 (to 26)
          
-         224          22 BUILD_LIST               0
+         238          22 BUILD_LIST               0
                       24 STORE_FAST               3 (absolute_tokens)
          
-         226     >>   26 LOAD_GLOBAL              1 (NULL + enumerate)
+         240     >>   26 LOAD_GLOBAL              1 (NULL + enumerate)
                       38 LOAD_FAST                1 (tokens)
                       40 PRECALL                  1
                       44 CALL                     1
                       54 GET_ITER
                  >>   56 EXTENDED_ARG             1
                       58 FOR_ITER               274 (to 608)
                       60 UNPACK_SEQUENCE          2
                       64 STORE_FAST               6 (i)
                       66 STORE_FAST               7 (token)
          
-         227          68 LOAD_FAST                7 (token)
+         241          68 LOAD_FAST                7 (token)
                       70 LOAD_METHOD              1 (split)
                       92 LOAD_CONST               2 ('=')
                       94 PRECALL                  1
                       98 CALL                     1
                      108 STORE_FAST               8 (split)
          
-         228         110 LOAD_GLOBAL              5 (NULL + len)
+         242         110 LOAD_GLOBAL              5 (NULL + len)
                      122 LOAD_FAST                8 (split)
                      124 PRECALL                  1
                      128 CALL                     1
                      138 LOAD_CONST               3 (1)
                      140 COMPARE_OP               2 (==)
                      146 POP_JUMP_FORWARD_IF_FALSE    89 (to 326)
                      148 LOAD_GLOBAL              5 (NULL + len)
                      160 LOAD_FAST                2 (kwarg_list)
                      162 PRECALL                  1
                      166 CALL                     1
                      176 LOAD_FAST                6 (i)
                      178 COMPARE_OP               4 (>)
                      184 POP_JUMP_FORWARD_IF_FALSE    70 (to 326)
          
-         229         186 LOAD_FAST                8 (split)
+         243         186 LOAD_FAST                8 (split)
                      188 LOAD_CONST               4 (0)
                      190 BINARY_SUBSCR
                      200 LOAD_FAST                3 (absolute_tokens)
                      202 CONTAINS_OP              0
                      204 POP_JUMP_FORWARD_IF_FALSE    12 (to 230)
          
-         230         206 LOAD_CONST               5 (True)
+         244         206 LOAD_CONST               5 (True)
                      208 LOAD_FAST                5 (kwargs)
                      210 LOAD_FAST                8 (split)
                      212 LOAD_CONST               4 (0)
                      214 BINARY_SUBSCR
                      224 STORE_SUBSCR
          
-         231         228 JUMP_BACKWARD           87 (to 56)
+         245         228 JUMP_BACKWARD           87 (to 56)
          
-         233     >>  230 LOAD_FAST                4 (had_kwargs)
+         247     >>  230 LOAD_FAST                4 (had_kwargs)
                      232 POP_JUMP_FORWARD_IF_FALSE    15 (to 264)
          
-         234         234 LOAD_GLOBAL              7 (NULL + ValueError)
+         248         234 LOAD_GLOBAL              7 (NULL + ValueError)
                      246 LOAD_CONST               6 ('Unexpected positional argument after keyword argument')
                      248 PRECALL                  1
                      252 CALL                     1
                      262 RAISE_VARARGS            1
          
-         236     >>  264 LOAD_FAST                0 (parser)
+         250     >>  264 LOAD_FAST                0 (parser)
                      266 LOAD_METHOD              4 (compile_filter)
                      288 LOAD_FAST                7 (token)
                      290 PRECALL                  1
                      294 CALL                     1
                      304 LOAD_FAST                5 (kwargs)
                      306 LOAD_FAST                2 (kwarg_list)
                      308 LOAD_FAST                6 (i)
                      310 BINARY_SUBSCR
                      320 STORE_SUBSCR
                      324 JUMP_BACKWARD          135 (to 56)
          
-         237     >>  326 LOAD_GLOBAL              5 (NULL + len)
+         251     >>  326 LOAD_GLOBAL              5 (NULL + len)
                      338 LOAD_FAST                8 (split)
                      340 PRECALL                  1
                      344 CALL                     1
                      354 LOAD_CONST               3 (1)
                      356 COMPARE_OP               2 (==)
                      362 POP_JUMP_FORWARD_IF_FALSE    57 (to 478)
          
-         238         364 LOAD_FAST                8 (split)
+         252         364 LOAD_FAST                8 (split)
                      366 LOAD_CONST               4 (0)
                      368 BINARY_SUBSCR
                      378 LOAD_FAST                3 (absolute_tokens)
                      380 CONTAINS_OP              0
                      382 POP_JUMP_FORWARD_IF_FALSE    12 (to 408)
          
-         239         384 LOAD_CONST               5 (True)
+         253         384 LOAD_CONST               5 (True)
                      386 LOAD_FAST                5 (kwargs)
                      388 LOAD_FAST                8 (split)
                      390 LOAD_CONST               4 (0)
                      392 BINARY_SUBSCR
                      402 STORE_SUBSCR
          
-         240         406 JUMP_BACKWARD          176 (to 56)
+         254         406 JUMP_BACKWARD          176 (to 56)
          
-         242     >>  408 LOAD_FAST                8 (split)
+         256     >>  408 LOAD_FAST                8 (split)
                      410 LOAD_CONST               4 (0)
                      412 BINARY_SUBSCR
                      422 STORE_FAST               9 (key)
          
-         243         424 LOAD_FAST                0 (parser)
+         257         424 LOAD_FAST                0 (parser)
                      426 LOAD_METHOD              4 (compile_filter)
                      448 LOAD_FAST                9 (key)
                      450 PRECALL                  1
                      454 CALL                     1
                      464 STORE_FAST              10 (value)
          
-         244         466 LOAD_FAST               10 (value)
+         258         466 LOAD_FAST               10 (value)
                      468 LOAD_FAST                5 (kwargs)
                      470 LOAD_FAST                9 (key)
                      472 STORE_SUBSCR
                      476 JUMP_BACKWARD          211 (to 56)
          
-         246     >>  478 LOAD_FAST                8 (split)
+         260     >>  478 LOAD_FAST                8 (split)
                      480 LOAD_CONST               4 (0)
                      482 BINARY_SUBSCR
                      492 STORE_FAST               9 (key)
          
-         249         494 LOAD_FAST                9 (key)
+         263         494 LOAD_FAST                9 (key)
                      496 LOAD_FAST                3 (absolute_tokens)
                      498 CONTAINS_OP              0
                      500 POP_JUMP_FORWARD_IF_FALSE    19 (to 540)
          
-         250         502 LOAD_GLOBAL              7 (NULL + ValueError)
+         264         502 LOAD_GLOBAL              7 (NULL + ValueError)
                      514 LOAD_CONST               7 ('Keyword argument ')
                      516 LOAD_FAST                9 (key)
                      518 FORMAT_VALUE             0
                      520 LOAD_CONST               8 (' cannot be resolved; it will not be parsed as a variable.')
                      522 BUILD_STRING             3
                      524 PRECALL                  1
                      528 CALL                     1
                      538 RAISE_VARARGS            1
          
-         252     >>  540 LOAD_FAST                0 (parser)
+         266     >>  540 LOAD_FAST                0 (parser)
                      542 LOAD_METHOD              4 (compile_filter)
                      564 LOAD_FAST                8 (split)
                      566 LOAD_CONST               3 (1)
                      568 BINARY_SUBSCR
                      578 PRECALL                  1
                      582 CALL                     1
                      592 LOAD_FAST                5 (kwargs)
                      594 LOAD_FAST                9 (key)
                      596 STORE_SUBSCR
          
-         253         600 LOAD_CONST               5 (True)
+         267         600 LOAD_CONST               5 (True)
                      602 STORE_FAST               4 (had_kwargs)
                      604 EXTENDED_ARG             1
                      606 JUMP_BACKWARD          276 (to 56)
          
-         255     >>  608 LOAD_FAST                2 (kwarg_list)
+         269     >>  608 LOAD_FAST                2 (kwarg_list)
                      610 GET_ITER
                  >>  612 FOR_ITER                24 (to 662)
                      614 STORE_FAST              11 (kwarg)
          
-         256         616 LOAD_FAST               11 (kwarg)
+         270         616 LOAD_FAST               11 (kwarg)
                      618 LOAD_FAST                5 (kwargs)
                      620 CONTAINS_OP              1
                      622 POP_JUMP_FORWARD_IF_FALSE    18 (to 660)
          
-         257         624 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
+         271         624 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
                      636 LOAD_CONST               9 ('Missing required keyword argument ')
                      638 LOAD_FAST               11 (kwarg)
                      640 FORMAT_VALUE             0
                      642 BUILD_STRING             2
                      644 PRECALL                  1
                      648 CALL                     1
                      658 RAISE_VARARGS            1
          
-         256     >>  660 JUMP_BACKWARD           25 (to 612)
+         270     >>  660 JUMP_BACKWARD           25 (to 612)
          
-         259     >>  662 LOAD_FAST                5 (kwargs)
+         273     >>  662 LOAD_FAST                5 (kwargs)
                      664 RETURN_VALUE
          consts
             None
             False
             '='
             1
             0
@@ -1396,26 +1525,26 @@
             'Keyword argument '
             ' cannot be resolved; it will not be parsed as a variable.'
             'Missing required keyword argument '
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError')
          varnames   ('parser', 'tokens', 'kwarg_list', 'absolute_tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'value', 'kwarg')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 216
+         firstlineno 230
          lnotab
             0x02010401040204010402040104022a012a014c0114011601020204011e
             023e01260114011601020210012a010c021003080126023c010802080108
             0124ff0203
       (None, None)
-   names      ('typing', 'Type', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'str', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'list', 'get_kwargs')
+   names      ('typing', 'Type', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'list', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c0114030c0314040c010c010c020c0208021806180610061e
-      03040104041c4d2a010eff0e01022c2a0112ff0e0102102e010aff0e0102
-      1e
+      030401040318071c4e2a010eff0e0102332a0112ff0e0102102e010aff0e
+      01021e
```

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/fedit.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,23 +38,30 @@
 register = library.Library()
 
 
 WARNING_FIELD_NAME_NOT_AVAILABLE = "Field name is not available in the context for %(object)s."
 WARNING_MODEL_INSTANCE_NOT_AVAILABLE = "Model instance is not available in the context for %(object)s."
 
 
+def as_var(var: str, context: Context, value: str) -> str:
+    if not var:
+        return value
+
+    context[var] = value
+    return ""
 
 class AdapterNode(Node):
     signer = signing.TimestampSigner()
 
-    def __init__(self, adapter: Type[BaseAdapter], model: FilterExpression, getters: list[str], **kwargs):
+    def __init__(self, adapter: Type[BaseAdapter], model: FilterExpression, getters: list[str], as_var: str = None, **kwargs):
         self.adapter = adapter
         self.model = model
         self.getters = getters
         self.kwargs = kwargs
+        self.as_var = as_var
 
     def _resolve_expressions(self, context, model, **kwargs):
         for k, v in kwargs.items():
             if isinstance(v, FilterExpression):
                 kwargs[k] = v.resolve(context)
         
         if isinstance(model, FilterExpression):
@@ -86,17 +93,17 @@
                     },
                     RuntimeWarning,
                 )
 
                 context = context.flatten()
 
                 try:
-                    return self.adapter.render_from_kwargs(
+                    return as_var(self.as_var, context, self.adapter.render_from_kwargs(
                         context, **kwargs,
-                    )
+                    ))
                 except AdapterError as e:
                     raise TemplateSyntaxError(str(e))
 
             field_name = getters[len(getters)-1]
             obj = model
             for i in range(len(getters) - 1):
                 getter = getters[i]
@@ -111,17 +118,17 @@
             field_name=field_name,
             request=request,
             **kwargs,
         )
 
         if not adapter.check_permissions()\
           or not _can_edit(request, obj):
-            return adapter.render_content(context)
+            return as_var(self.as_var, context, adapter.render_content(context))
 
-        return wrap_adapter(request, adapter, context)
+        return as_var(self.as_var, context, wrap_adapter(request, adapter, context))
 
 
 @register.tag(name=TEMPLATE_TAG_NAME)
 def do_render_fedit(parser: Parser, token: Token):
 
     tokens = token.split_contents()
 
@@ -145,25 +152,32 @@
                 )
 
         if len(model_tokens) > 1:
             # mymodel.myfield
             # mymodel.related_field.myfield
             model = parser.compile_filter(model_tokens.pop(0))
 
+    as_var = None
+    if tokens and tokens[len(tokens)-2] == "as":
+        as_var = tokens.pop(len(tokens)-1)
+        tokens.pop(len(tokens)-1)
+
+
     kwargs = get_kwargs(
         parser,
         tokens,
         adapter.required_kwargs,
         adapter.absolute_tokens,
     )
 
     return AdapterNode(
         adapter=adapter,
         model=model,
         getters=model_tokens,
+        as_var=as_var,
         **kwargs,
     )
 
 
 
 @register.simple_tag(takes_context=True)
 def render_adapter(context: Context, adapter: BaseAdapter) -> str:
```

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,14 +296,51 @@
         tpl = template.render(Context(context))
 
         self.assertHTMLEqual(
             tpl,
             wrap_adapter(request, adapters[5], {})
         )
 
+    def test_render_as_var(self):
+        streamfield = self.basic_model.content
+        block = find_block(self.BLOCK_ID, streamfield)
+        
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
+        
+        request.user = self.admin_user
+        setattr(
+            request,
+            FEDIT_PREVIEW_VAR,
+            True,
+        )
+        block_value, _ = block
+        template = Template(
+            "{% load fedit %}"
+            "{% fedit test_block object.content block=block block_id=block_id id=6 as test %}"
+            "{{ test }}"
+        )
+
+        context = {
+            "object": self.basic_model,
+            "request": request,
+            "block": block_value,
+            "block_id": self.BLOCK_ID,
+        }
+
+        tpl = template.render(Context(context))
+
+        self.assertHTMLEqual(
+            tpl,
+            wrap_adapter(request, adapters[6], {})
+        )
+
     def test_render_from_context(self):
         streamfield = self.basic_model.content
         block = find_block(self.BLOCK_ID, streamfield)
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
```

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/views/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.3rc2
+Version: 1.5.3rc3
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -55,14 +55,15 @@
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
   - [Share With Sessions](#wagtail_fedit_share_with_sessions)
+  - [Use Adapter Session ID](#wagtail_fedit_use_adapter_session_id)
 - [How your content is rendered](#how-your-content-is-rendered)
   - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.3rc2 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.3rc3 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -26,24 +26,25 @@
 (#wagtail_feditregister_type_renderer) - [Register Field Renderer]
 (#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
 [Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
-Sessions](#wagtail_fedit_share_with_sessions) - [How your content is rendered]
-(#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
-output-html) - [Implemented](#implemented) Getting Started --------------- 1.
-Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
-INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
-collectstatic`. 3. Run `py ./manage.py adapter_help` to see all your options
-and their requirements. ## Getting Editing! 1. Make sure the models you wish to
-edit inherit from PreviewableMixin. **This is a requirement.** 2. Define a
-template for your model. Example: ```django-html {% load fedit static
-wagtailuserbar %} {# Load the required template tag libraries #}
+Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
+(#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
+your-content-is-rendered) - [Rendered output HTML](#rendered-editable-output-
+html) - [Implemented](#implemented) Getting Started --------------- 1. Add
+'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
+[ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. 3. Run `py
+./manage.py adapter_help` to see all your options and their requirements. ##
+Getting Editing! 1. Make sure the models you wish to edit inherit from
+PreviewableMixin. **This is a requirement.** 2. Define a template for your
+model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
+the required template tag libraries #}
 {# Load all registered CSS required for the adapters. Only included inside edit
 view! #} {% fedit_scripts "css" %}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {# For
 help on arguments for the adapters please run the adapter_help command. #} {#
 Example: `python3 ./manage.py adapter_help` #}
 ************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee %%}} ************
 {% fedit field self.content %} {% wagtailuserbar %} {# Load all registered
```

### Comparing `wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

