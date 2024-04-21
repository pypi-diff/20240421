# Comparing `tmp/wagtail_fedit-1.5.3rc3.tar.gz` & `tmp/wagtail_fedit-1.5.3rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.3rc3.tar", last modified: Sun Apr 21 01:28:58 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.3rc4.tar", last modified: Sun Apr 21 02:15:13 2024, max compression
```

## Comparing `wagtail_fedit-1.5.3rc3.tar` & `wagtail_fedit-1.5.3rc4.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:58.021902 wagtail_fedit-1.5.3rc3/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/MANIFEST.in
--rw-rw-rw-   0        0        0    20306 2024-04-21 01:28:58.022904 wagtail_fedit-1.5.3rc3/PKG-INFO
--rw-rw-rw-   0        0        0    19105 2024-04-21 00:53:02.000000 wagtail_fedit-1.5.3rc3/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-04-21 01:28:58.033742 wagtail_fedit-1.5.3rc3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.766415 wagtail_fedit-1.5.3rc3/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.816008 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    10463 2024-04-21 01:05:15.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.820552 wagtail_fedit-1.5.3rc3/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1765 2024-04-18 20:28:58.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4214 2024-04-16 18:40:39.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.729587 wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.729587 wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.840387 wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.841397 wagtail_fedit-1.5.3rc3/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.842399 wagtail_fedit-1.5.3rc3/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0      973 2024-04-21 00:46:27.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.731907 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.732905 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.856705 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.881773 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.733905 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.883247 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.885260 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.898057 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.927661 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      566 2024-04-21 00:09:10.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.934177 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.952436 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.975595 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.977591 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.980594 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    10817 2024-04-21 01:26:50.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     7961 2024-04-21 01:25:52.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.982839 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.988845 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.991367 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:58.000366 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    12859 2024-04-21 01:26:42.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:58.005731 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:58.010730 wagtail_fedit-1.5.3rc3/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6551 2024-04-21 00:08:49.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:58.021902 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     1881 2024-04-16 18:44:29.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-21 01:28:57.804778 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    20306 2024-04-21 01:28:57.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4038 2024-04-21 01:28:57.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 01:28:57.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-21 01:28:57.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 01:28:57.000000 wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.983002 wagtail_fedit-1.5.3rc4/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc4/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc4/MANIFEST.in
+-rw-rw-rw-   0        0        0    20306 2024-04-21 02:15:12.984001 wagtail_fedit-1.5.3rc4/PKG-INFO
+-rw-rw-rw-   0        0        0    19105 2024-04-21 00:53:02.000000 wagtail_fedit-1.5.3rc4/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc4/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-04-21 02:15:12.995564 wagtail_fedit-1.5.3rc4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.836743 wagtail_fedit-1.5.3rc4/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.878781 wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    10463 2024-04-21 01:05:15.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.884782 wagtail_fedit-1.5.3rc4/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3082 2024-04-21 02:10:32.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.798068 wagtail_fedit-1.5.3rc4/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.798068 wagtail_fedit-1.5.3rc4/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.888783 wagtail_fedit-1.5.3rc4/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.889783 wagtail_fedit-1.5.3rc4/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.891290 wagtail_fedit-1.5.3rc4/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0      973 2024-04-21 00:46:27.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.800067 wagtail_fedit-1.5.3rc4/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.800067 wagtail_fedit-1.5.3rc4/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.895298 wagtail_fedit-1.5.3rc4/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.897301 wagtail_fedit-1.5.3rc4/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.801069 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.898299 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.899300 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.902298 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.913298 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      566 2024-04-21 00:09:10.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.921304 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.924299 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.927298 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.930377 wagtail_fedit-1.5.3rc4/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.934388 wagtail_fedit-1.5.3rc4/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10817 2024-04-21 01:26:50.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7961 2024-04-21 01:25:52.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.937386 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.942385 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.945386 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.955898 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    14761 2024-04-21 01:30:53.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.961990 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.967990 wagtail_fedit-1.5.3rc4/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6551 2024-04-21 00:08:49.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.983002 wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2277 2024-04-21 02:11:31.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:15:12.865780 wagtail_fedit-1.5.3rc4/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    20306 2024-04-21 02:15:12.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4038 2024-04-21 02:15:12.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 02:15:12.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-21 02:15:12.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 02:15:12.000000 wagtail_fedit-1.5.3rc4/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.3rc3/LICENSE` & `wagtail_fedit-1.5.3rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/PKG-INFO` & `wagtail_fedit-1.5.3rc4/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail_fedit
-Version: 1.5.3rc3
+Name: wagtail-fedit
+Version: 1.5.3rc4
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc3 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.3rc4 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.3rc3/README.md` & `wagtail_fedit-1.5.3rc4/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/setup.cfg` & `wagtail_fedit-1.5.3rc4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3372 6333 0d0a 6465 7363 7269 7074 696f  3rc3..descriptio
+00000030: 3372 6334 0d0a 6465 7363 7269 7074 696f  3rc4..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/block.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/hooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,14 +88,29 @@
     # This is a custom renderer for RichText fields.
     # It will render the RichText field as a RichText block.
     renderer_map[RichTextField] =\
         lambda request, context, instance, value: richtext(value)
 ```
 """
 
+REGISTER_FIELD_WIDGETS = prefix("register_field_widgets")
+"""
+### wagtail_fedit.register_field_widgets
+Register a custom widget for a field.
+
+Example of how this hook is used in wagtail_hooks.py:
+    
+    ```python
+    @hooks.register(REGISTER_FIELD_WIDGETS)
+    def register_field_widgets(widgets):
+        widgets[RichTextField] = AdminRichTextField
+        return widgets
+    ```
+"""
+
 
 FIELD_EDITOR_SIZE = prefix("field_editor_size")
 """
 ### wagtail_fedit.field_editor_size
 Control the size of the editor for the given model-field type.
 
 Example of how this hook is called:
```

#### html2text {}

```diff
@@ -23,29 +23,33 @@
 ', static('js/custom.js') ), ] ``` """ REGISTER_FIELD_RENDERER = prefix
 ("register_field_renderer") """ ### wagtail_fedit.register_field_renderer
 Register a custom renderer for a field. Example of how this type of renderer is
 used in wagtail_hooks/renderers.py: ```python @hooks.register
 (REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
 custom renderer for RichText fields. # It will render the RichText field as a
 RichText block. renderer_map[RichTextField] =\ lambda request, context,
-instance, value: richtext(value) ``` """ FIELD_EDITOR_SIZE = prefix
-("field_editor_size") """ ### wagtail_fedit.field_editor_size Control the size
-of the editor for the given model-field type. Example of how this hook is
-called: ```python for hook in hooks.get_hooks(FEDIT_FIELD_EDITOR_SIZE): size =
-hook(model_instance, model_field) if size: return size ``` """
-EXCLUDE_FROM_RELATED_FORMS = prefix("exclude_related_forms") """ ###
-wagtail_fedit.exclude_related_forms Exclude the given model type from the
-related forms. This is used internally to exclude the Page, Image, and Document
-models from the related forms. This way; the user will have the actual widget
-for the field instead of the related form. Example of how this hook is called
-and how it is used internally: ```python def use_related_form(field:
-models.Field) -> bool: for hook in hooks.get_hooks(EXCLUDE_FROM_RELATED_FORMS):
-if hook(field): return False return True @hooks.register
-(EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field): if
-field.related_model in [Page, Image, Document]: return True return False ```
+instance, value: richtext(value) ``` """ REGISTER_FIELD_WIDGETS = prefix
+("register_field_widgets") """ ### wagtail_fedit.register_field_widgets
+Register a custom widget for a field. Example of how this hook is used in
+wagtail_hooks.py: ```python @hooks.register(REGISTER_FIELD_WIDGETS) def
+register_field_widgets(widgets): widgets[RichTextField] = AdminRichTextField
+return widgets ``` """ FIELD_EDITOR_SIZE = prefix("field_editor_size") """ ###
+wagtail_fedit.field_editor_size Control the size of the editor for the given
+model-field type. Example of how this hook is called: ```python for hook in
+hooks.get_hooks(FEDIT_FIELD_EDITOR_SIZE): size = hook(model_instance,
+model_field) if size: return size ``` """ EXCLUDE_FROM_RELATED_FORMS = prefix
+("exclude_related_forms") """ ### wagtail_fedit.exclude_related_forms Exclude
+the given model type from the related forms. This is used internally to exclude
+the Page, Image, and Document models from the related forms. This way; the user
+will have the actual widget for the field instead of the related form. Example
+of how this hook is called and how it is used internally: ```python def
+use_related_form(field: models.Field) -> bool: for hook in hooks.get_hooks
+(EXCLUDE_FROM_RELATED_FORMS): if hook(field): return False return True
+@hooks.register(EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field):
+if field.related_model in [Page, Image, Document]: return True return False ```
 """ ACTION_MENU_ITEM_IS_SHOWN = prefix("action_menu_item_is_shown") """ ###
 wagtail_fedit.action_menu_item_is_shown Decide if the action menu item should
 be shown for the given instance. Return None if you cannot decide, False if you
 want to hide the item, and True if you want to show the item. Example of how
 this hook is called: ```python for hook in hooks.get_hooks
 (ACTION_MENU_ITEM_IS_SHOWN): result = hook(context, instance) if result is not
 None: return result # <- bool ``` """
```

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/models.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files 8% similar despite different names*

```diff
@@ -226,14 +226,48 @@
         )
 
         self.assertHTMLEqual(
             tpl,
             wrap_adapter(request, adapters[4], {})
         )
 
+    def test_adapter_editable_as_var(self):
+        self.assertEqual(TestAdapter.required_kwargs, ["test"])
+
+        tpl = Template(
+            "{% load fedit %}"
+            "{% fedit test object.title test='test' id=5 as test_adapter_as_variable_name %}"
+            "{{ test_adapter_as_variable_name }}"
+        )
+
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
+        request.user = self.admin_user
+
+        setattr(
+            request,
+            FEDIT_PREVIEW_VAR,
+            True,
+        )
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
+            wrap_adapter(request, adapters[5], {})
+        )
+
     def test_context_processors_run(self):
         tpl = Template(
             "{% load fedit %}"
             "{% fedit test_context object.title test='test' id=5 %}"
         )
 
         request = self.request_factory.get(
@@ -299,21 +333,21 @@
             tpl,
             wrap_adapter(request, adapters[5], {})
         )
 
     def test_render_as_var(self):
         streamfield = self.basic_model.content
         block = find_block(self.BLOCK_ID, streamfield)
-        
+
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
         )
-        
+
         request.user = self.admin_user
         setattr(
             request,
             FEDIT_PREVIEW_VAR,
             True,
         )
         block_value, _ = block
@@ -430,8 +464,38 @@
     
             tpl = template.render(Context(context))
     
             self.assertHTMLEqual(
                 tpl,
                 wrap_adapter(request, adapters[7], {})
             )
+
+        def test_render_as_var(self):
+            request = self.request_factory.get(
+                self.get_editable_url(
+                    self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+                )
+            )
+            request.user = self.admin_user
+            setattr(
+                request,
+                FEDIT_PREVIEW_VAR,
+                True,
+            )
+            template = Template(
+                "{% load fedit %}"
+                "{% fedit test_field object.title test=True id=8 as test %}"
+                "{{ test }}"
+            )
+    
+            context = {
+                "object": self.basic_model,
+                "request": request,
+            }
+    
+            tpl = template.render(Context(context))
+    
+            self.assertHTMLEqual(
+                tpl,
+                wrap_adapter(request, adapters[8], {})
+            )
```

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/views/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,39 +5,50 @@
 from wagtail.fields import (
     RichTextField,
     StreamField,
 )
 from wagtail.templatetags.wagtailcore_tags import (
     richtext,
 )
-from wagtail.images.models import (
-    Image,
+from wagtail.images import (
+    get_image_model,
 )
-from wagtail.documents.models import Document
+from wagtail.images.widgets import AdminImageChooser
+from wagtail.documents import get_document_model
+from wagtail.documents.widgets import AdminDocumentChooser
 from ..hooks import (
     EXCLUDE_FROM_RELATED_FORMS,
     REGISTER_FIELD_RENDERER,
+    REGISTER_FIELD_WIDGETS,
     FIELD_EDITOR_SIZE,
     REGISTER_CSS,
     REGISTER_JS,
 )
 
+Image = get_image_model()
+Document = get_document_model()
+
 @hooks.register(EXCLUDE_FROM_RELATED_FORMS)
 def exclude_related_forms(field):
     if field.related_model in [Page, Image, Document]:
         return True
     return False
 
 
 @hooks.register(REGISTER_FIELD_RENDERER)
 def register_renderers(renderer_map):
     # This is a custom renderer for RichText fields.
     # It will render the RichText field as a RichText block.
     renderer_map[RichTextField] = lambda request, context, instance, value: richtext(value)
 
+@hooks.register(REGISTER_FIELD_WIDGETS)
+def register_field_widgets(widgets):
+    widgets[Image] = AdminImageChooser
+    widgets[Document] = AdminDocumentChooser
+    return widgets
 
 @hooks.register(FIELD_EDITOR_SIZE)
 def field_editor_size(model_instance, model_field):
     if isinstance(model_field, RichTextField):
         return "large"
     
     if isinstance(model_field, StreamField):
```

#### html2text {}

```diff
@@ -1,22 +1,27 @@
 from django.utils.html import format_html from django.templatetags.static
 import static from wagtail import hooks from wagtail.models import Page from
 wagtail.fields import ( RichTextField, StreamField, ) from
-wagtail.templatetags.wagtailcore_tags import ( richtext, ) from
-wagtail.images.models import ( Image, ) from wagtail.documents.models import
-Document from ..hooks import ( EXCLUDE_FROM_RELATED_FORMS,
-REGISTER_FIELD_RENDERER, FIELD_EDITOR_SIZE, REGISTER_CSS, REGISTER_JS, )
-@hooks.register(EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field):
-if field.related_model in [Page, Image, Document]: return True return False
-@hooks.register(REGISTER_FIELD_RENDERER) def register_renderers(renderer_map):
-# This is a custom renderer for RichText fields. # It will render the RichText
-field as a RichText block. renderer_map[RichTextField] = lambda request,
-context, instance, value: richtext(value) @hooks.register(FIELD_EDITOR_SIZE)
-def field_editor_size(model_instance, model_field): if isinstance(model_field,
-RichTextField): return "large" if isinstance(model_field, StreamField): return
-"full" return None #
+wagtail.templatetags.wagtailcore_tags import ( richtext, ) from wagtail.images
+import ( get_image_model, ) from wagtail.images.widgets import
+AdminImageChooser from wagtail.documents import get_document_model from
+wagtail.documents.widgets import AdminDocumentChooser from ..hooks import
+( EXCLUDE_FROM_RELATED_FORMS, REGISTER_FIELD_RENDERER, REGISTER_FIELD_WIDGETS,
+FIELD_EDITOR_SIZE, REGISTER_CSS, REGISTER_JS, ) Image = get_image_model()
+Document = get_document_model() @hooks.register(EXCLUDE_FROM_RELATED_FORMS) def
+exclude_related_forms(field): if field.related_model in [Page, Image,
+Document]: return True return False @hooks.register(REGISTER_FIELD_RENDERER)
+def register_renderers(renderer_map): # This is a custom renderer for RichText
+fields. # It will render the RichText field as a RichText block. renderer_map
+[RichTextField] = lambda request, context, instance, value: richtext(value)
+@hooks.register(REGISTER_FIELD_WIDGETS) def register_field_widgets(widgets):
+widgets[Image] = AdminImageChooser widgets[Document] = AdminDocumentChooser
+return widgets @hooks.register(FIELD_EDITOR_SIZE) def field_editor_size
+(model_instance, model_field): if isinstance(model_field, RichTextField):
+return "large" if isinstance(model_field, StreamField): return "full" return
+None #
 #
 @hooks.register(REGISTER_CSS, order=-1) def register_css(request): return
 [ format_html( '
 ', static('wagtail_fedit/css/frontend.css') ), ] @hooks.register(REGISTER_JS,
 order=-1) def register_js(request): return [ format_html( '
 ', static('wagtail_fedit/js/frontend.js') ), ]
```

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.3rc4/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.3rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail-fedit
-Version: 1.5.3rc3
+Name: wagtail_fedit
+Version: 1.5.3rc4
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.3rc3 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc4 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.3rc3/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.3rc4/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

