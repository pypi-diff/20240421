# Comparing `tmp/wagtail_fedit-1.5.3rc1.tar.gz` & `tmp/wagtail_fedit-1.5.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.3rc1.tar", last modified: Sun Apr 21 00:35:01 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.3rc2.tar", last modified: Sun Apr 21 00:49:07 2024, max compression
```

## Comparing `wagtail_fedit-1.5.3rc1.tar` & `wagtail_fedit-1.5.3rc2.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:01.038780 wagtail_fedit-1.5.3rc1/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/MANIFEST.in
--rw-rw-rw-   0        0        0    19867 2024-04-21 00:35:01.039779 wagtail_fedit-1.5.3rc1/PKG-INFO
--rw-rw-rw-   0        0        0    18666 2024-04-21 00:33:38.000000 wagtail_fedit-1.5.3rc1/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-04-21 00:35:01.048322 wagtail_fedit-1.5.3rc1/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.832688 wagtail_fedit-1.5.3rc1/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.884669 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    10014 2024-04-21 00:27:28.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.887666 wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1765 2024-04-18 20:28:58.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4214 2024-04-16 18:40:39.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.805985 wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.806517 wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.894218 wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.895220 wagtail_fedit-1.5.3rc1/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.896216 wagtail_fedit-1.5.3rc1/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0      667 2024-04-21 00:26:28.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.808707 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.809721 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.901215 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.923471 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.810719 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.927467 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.928469 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.931474 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.943521 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      566 2024-04-21 00:09:10.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.948522 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.959486 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.964566 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.966568 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.968566 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    10007 2024-04-19 19:46:13.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     7503 2024-04-19 19:46:11.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.971078 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.977609 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.987378 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:01.008568 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    11767 2024-04-20 20:40:55.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:01.017108 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:01.025113 wagtail_fedit-1.5.3rc1/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6551 2024-04-21 00:08:49.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:01.037786 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     1881 2024-04-16 18:44:29.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.864660 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    19867 2024-04-21 00:35:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4038 2024-04-21 00:35:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 00:35:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-21 00:35:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 00:35:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.036119 wagtail_fedit-1.5.3rc2/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/MANIFEST.in
+-rw-rw-rw-   0        0        0    20237 2024-04-21 00:49:07.036119 wagtail_fedit-1.5.3rc2/PKG-INFO
+-rw-rw-rw-   0        0        0    19036 2024-04-21 00:47:52.000000 wagtail_fedit-1.5.3rc2/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-04-21 00:49:07.046811 wagtail_fedit-1.5.3rc2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.910995 wagtail_fedit-1.5.3rc2/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.956471 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    10268 2024-04-21 00:45:14.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.960469 wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1765 2024-04-18 20:28:58.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4214 2024-04-16 18:40:39.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.872802 wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.873816 wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.962469 wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.962974 wagtail_fedit-1.5.3rc2/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.963980 wagtail_fedit-1.5.3rc2/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0      973 2024-04-21 00:46:27.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.875808 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.875808 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.967983 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.969982 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.876923 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.970984 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.973497 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.976506 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.983582 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      566 2024-04-21 00:09:10.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.990587 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.992589 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.994830 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.995989 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.998997 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10007 2024-04-19 19:46:13.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7503 2024-04-19 19:46:11.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.000993 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.006656 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.008654 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.016883 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    11767 2024-04-20 20:40:55.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.023541 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.026536 wagtail_fedit-1.5.3rc2/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6551 2024-04-21 00:08:49.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:07.035119 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     1881 2024-04-16 18:44:29.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:49:06.936844 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    20237 2024-04-21 00:49:06.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4038 2024-04-21 00:49:06.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 00:49:06.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-21 00:49:06.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 00:49:06.000000 wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.3rc1/LICENSE` & `wagtail_fedit-1.5.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/PKG-INFO` & `wagtail_fedit-1.5.3rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.3rc1
+Version: 1.5.3rc2
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -551,14 +551,23 @@
 Default: `False`
 
 Share the context through the session data.
 This is useful if you are running into limits with the URL length.
 This will store the context in the session and pass the session
 key to the iFrame instead of the context.
 
+### `WAGTAIL_FEDIT_USE_ADAPTER_SESSION_ID`
+
+Default: `True`
+
+Use the get_element_id method of the adapter to generate a session ID.
+*This could __maybe__ interfere with other editable- block's session data, but is highly unlikely!*
+This is useful to not clutter session data too much.
+If `False`, the session ID will be generated each time the page is loaded.
+
 ## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
 ### Rendered editable output HTML
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc1 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc2 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -221,21 +221,25 @@
 None: return result # <- bool ``` ## Settings ###
 `WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT` Default: `True` Sign the shared context
 with a secret key. This is useful to prevent tampering with the shared context.
 It will also be compressed with zlib if available. It might not be in your
 site's security model to need this. ### `WAGTAIL_FEDIT_SHARE_WITH_SESSIONS`
 Default: `False` Share the context through the session data. This is useful if
 you are running into limits with the URL length. This will store the context in
-the session and pass the session key to the iFrame instead of the context. ##
-How your content is rendered (**Maintainer's note:** In my experience this
-doesn't mess the CSS up too much, or even at all for most content - **if** you
-don't get hyperspecific with your CSS selectors and structure your templates
-well.) Your block and field are wrapped in a `div`, any CSS for your templates
-should keep this in mind. ### Rendered editable output HTML ```html {% load
-fedit %}
+the session and pass the session key to the iFrame instead of the context. ###
+`WAGTAIL_FEDIT_USE_ADAPTER_SESSION_ID` Default: `True` Use the get_element_id
+method of the adapter to generate a session ID. *This could __maybe__ interfere
+with other editable- block's session data, but is highly unlikely!* This is
+useful to not clutter session data too much. If `False`, the session ID will be
+generated each time the page is loaded. ## How your content is rendered
+(**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
+or even at all for most content - **if** you don't get hyperspecific with your
+CSS selectors and structure your templates well.) Your block and field are
+wrapped in a `div`, any CSS for your templates should keep this in mind. ###
+Rendered editable output HTML ```html {% load fedit %}
 % if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
 { edit_url }}">
 {% for button in buttons %} {{ button }} {% endfor %}
 {% render_adapter adapter %}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.5.3rc1/README.md` & `wagtail_fedit-1.5.3rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -521,14 +521,23 @@
 Default: `False`
 
 Share the context through the session data.
 This is useful if you are running into limits with the URL length.
 This will store the context in the session and pass the session
 key to the iFrame instead of the context.
 
+### `WAGTAIL_FEDIT_USE_ADAPTER_SESSION_ID`
+
+Default: `True`
+
+Use the get_element_id method of the adapter to generate a session ID.
+*This could __maybe__ interfere with other editable- block's session data, but is highly unlikely!*
+This is useful to not clutter session data too much.
+If `False`, the session ID will be generated each time the page is loaded.
+
 ## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
 ### Rendered editable output HTML
```

#### html2text {}

```diff
@@ -206,21 +206,25 @@
 None: return result # <- bool ``` ## Settings ###
 `WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT` Default: `True` Sign the shared context
 with a secret key. This is useful to prevent tampering with the shared context.
 It will also be compressed with zlib if available. It might not be in your
 site's security model to need this. ### `WAGTAIL_FEDIT_SHARE_WITH_SESSIONS`
 Default: `False` Share the context through the session data. This is useful if
 you are running into limits with the URL length. This will store the context in
-the session and pass the session key to the iFrame instead of the context. ##
-How your content is rendered (**Maintainer's note:** In my experience this
-doesn't mess the CSS up too much, or even at all for most content - **if** you
-don't get hyperspecific with your CSS selectors and structure your templates
-well.) Your block and field are wrapped in a `div`, any CSS for your templates
-should keep this in mind. ### Rendered editable output HTML ```html {% load
-fedit %}
+the session and pass the session key to the iFrame instead of the context. ###
+`WAGTAIL_FEDIT_USE_ADAPTER_SESSION_ID` Default: `True` Use the get_element_id
+method of the adapter to generate a session ID. *This could __maybe__ interfere
+with other editable- block's session data, but is highly unlikely!* This is
+useful to not clutter session data too much. If `False`, the session ID will be
+generated each time the page is loaded. ## How your content is rendered
+(**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
+or even at all for most content - **if** you don't get hyperspecific with your
+CSS selectors and structure your templates well.) Your block and field are
+wrapped in a `div`, any CSS for your templates should keep this in mind. ###
+Rendered editable output HTML ```html {% load fedit %}
 % if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
 { edit_url }}">
 {% for button in buttons %} {{ button }} {% endfor %}
 {% render_adapter adapter %}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.5.3rc1/setup.cfg` & `wagtail_fedit-1.5.3rc2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3372 6331 0d0a 6465 7363 7269 7074 696f  3rc1..descriptio
+00000030: 3372 6332 0d0a 6465 7363 7269 7074 696f  3rc2..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,23 @@
 )
 from django.http import (
     HttpRequest,
 )
 from ..settings import (
     SIGN_SHARED_CONTEXT,
     SHARE_WITH_SESSIONS,
+    USE_ADAPTER_SESSION_ID,
 )
 from ..utils import (
     FeditIFrameMixin,
     wrap_adapter,
 )
 
+import uuid
+
 if TYPE_CHECKING:
     from ..toolbar import (
         FeditToolbarComponent,
     )
 
 class AdapterError(Exception):
     pass
@@ -273,15 +276,21 @@
         Encode a dictionary to a string.
         This will be passed as a GET parameter to the iFrame.
         Make sure the data is not too large.
         """
         if not self.kwargs:
             return ""
         if SHARE_WITH_SESSIONS:
-            id = self.get_element_id()
+            if USE_ADAPTER_SESSION_ID:
+                id = self.get_element_id()
+            else:
+                id = self.kwargs.setdefault(
+                    "wagtail_fedit_uuid",
+                    str(uuid.uuid4())
+                )
             self.request.session[id] = self.kwargs
             self.request.session.modified = True
             return id
         # return self.signer.sign_object(self.kwargs)# , serializer=PickleBlockSerializer)
         if SIGN_SHARED_CONTEXT:
             return self.signer.sign_object(self.kwargs, compress=True)
```

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/block.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/models.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,7 +15,15 @@
 """
 Share the context with the session.
 This is useful if you are running into limits with the URL length.
 This will store the context in the session and pass the session
 key to the iFrame instead of the context.
 """
 
+USE_ADAPTER_SESSION_ID = getattr(settings, "WAGTAIL_FEDIT_USE_ADAPTER_SESSION_ID", True)
+"""
+Use the get_element_id method of the adapter to generate a session ID.
+This is useful to not clutter session data too much.
+If `False`, the session ID will be generated each time the page is loaded.
+"""
+
+
```

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/views/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.3rc2/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.3rc1
+Version: 1.5.3rc2
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -551,14 +551,23 @@
 Default: `False`
 
 Share the context through the session data.
 This is useful if you are running into limits with the URL length.
 This will store the context in the session and pass the session
 key to the iFrame instead of the context.
 
+### `WAGTAIL_FEDIT_USE_ADAPTER_SESSION_ID`
+
+Default: `True`
+
+Use the get_element_id method of the adapter to generate a session ID.
+*This could __maybe__ interfere with other editable- block's session data, but is highly unlikely!*
+This is useful to not clutter session data too much.
+If `False`, the session ID will be generated each time the page is loaded.
+
 ## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
 ### Rendered editable output HTML
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.3rc1 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.3rc2 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -221,21 +221,25 @@
 None: return result # <- bool ``` ## Settings ###
 `WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT` Default: `True` Sign the shared context
 with a secret key. This is useful to prevent tampering with the shared context.
 It will also be compressed with zlib if available. It might not be in your
 site's security model to need this. ### `WAGTAIL_FEDIT_SHARE_WITH_SESSIONS`
 Default: `False` Share the context through the session data. This is useful if
 you are running into limits with the URL length. This will store the context in
-the session and pass the session key to the iFrame instead of the context. ##
-How your content is rendered (**Maintainer's note:** In my experience this
-doesn't mess the CSS up too much, or even at all for most content - **if** you
-don't get hyperspecific with your CSS selectors and structure your templates
-well.) Your block and field are wrapped in a `div`, any CSS for your templates
-should keep this in mind. ### Rendered editable output HTML ```html {% load
-fedit %}
+the session and pass the session key to the iFrame instead of the context. ###
+`WAGTAIL_FEDIT_USE_ADAPTER_SESSION_ID` Default: `True` Use the get_element_id
+method of the adapter to generate a session ID. *This could __maybe__ interfere
+with other editable- block's session data, but is highly unlikely!* This is
+useful to not clutter session data too much. If `False`, the session ID will be
+generated each time the page is loaded. ## How your content is rendered
+(**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
+or even at all for most content - **if** you don't get hyperspecific with your
+CSS selectors and structure your templates well.) Your block and field are
+wrapped in a `div`, any CSS for your templates should keep this in mind. ###
+Rendered editable output HTML ```html {% load fedit %}
 % if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
 { edit_url }}">
 {% for button in buttons %} {{ button }} {% endfor %}
 {% render_adapter adapter %}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.3rc2/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

