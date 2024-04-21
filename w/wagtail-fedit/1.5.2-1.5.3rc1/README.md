# Comparing `tmp/wagtail_fedit-1.5.2.tar.gz` & `tmp/wagtail_fedit-1.5.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.2.tar", last modified: Sat Apr 20 23:41:16 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.3rc1.tar", last modified: Sun Apr 21 00:35:01 2024, max compression
```

## Comparing `wagtail_fedit-1.5.2.tar` & `wagtail_fedit-1.5.3rc1.tar`

### file list

```diff
@@ -1,125 +1,127 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.873446 wagtail_fedit-1.5.2/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0    19504 2024-04-20 23:41:16.873446 wagtail_fedit-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    18306 2024-04-20 20:08:53.000000 wagtail_fedit-1.5.2/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-04-20 23:41:16.883842 wagtail_fedit-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.221848 wagtail_fedit-1.5.2/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.2/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.326428 wagtail_fedit-1.5.2/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0     9235 2024-04-20 14:51:04.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.2/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.2/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.350268 wagtail_fedit-1.5.2/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.2/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.2/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1765 2024-04-18 20:28:58.000000 wagtail_fedit-1.5.2/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4214 2024-04-16 18:40:39.000000 wagtail_fedit-1.5.2/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.143468 wagtail_fedit-1.5.2/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.144478 wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.360361 wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.361344 wagtail_fedit-1.5.2/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.2/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.362902 wagtail_fedit-1.5.2/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.2/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0      351 2024-04-19 19:34:54.000000 wagtail_fedit-1.5.2/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.146470 wagtail_fedit-1.5.2/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.146470 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.381574 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.411358 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.147469 wagtail_fedit-1.5.2/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.413871 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.423951 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.434737 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.466914 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      889 2024-04-18 15:45:49.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5980 2024-04-16 13:14:54.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.506469 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.516207 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.526812 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.540306 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.544828 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    10007 2024-04-19 19:46:13.000000 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     7503 2024-04-19 19:46:11.000000 wagtail_fedit-1.5.2/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.556205 wagtail_fedit-1.5.2/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.576661 wagtail_fedit-1.5.2/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.594087 wagtail_fedit-1.5.2/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.664638 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    11767 2024-04-20 20:40:55.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.752638 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.2/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.2/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.2/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.796489 wagtail_fedit-1.5.2/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.2/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6516 2024-04-19 19:15:42.000000 wagtail_fedit-1.5.2/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.2/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.2/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.871923 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     1881 2024-04-16 18:44:29.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-20 23:41:16.265798 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    19504 2024-04-20 23:41:16.000000 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3905 2024-04-20 23:41:16.000000 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 23:41:16.000000 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-20 23:41:16.000000 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-20 23:41:16.000000 wagtail_fedit-1.5.2/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:01.038780 wagtail_fedit-1.5.3rc1/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0    19867 2024-04-21 00:35:01.039779 wagtail_fedit-1.5.3rc1/PKG-INFO
+-rw-rw-rw-   0        0        0    18666 2024-04-21 00:33:38.000000 wagtail_fedit-1.5.3rc1/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-04-21 00:35:01.048322 wagtail_fedit-1.5.3rc1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.832688 wagtail_fedit-1.5.3rc1/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.884669 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    10014 2024-04-21 00:27:28.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.887666 wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1765 2024-04-18 20:28:58.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4214 2024-04-16 18:40:39.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.805985 wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.806517 wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.894218 wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.895220 wagtail_fedit-1.5.3rc1/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.896216 wagtail_fedit-1.5.3rc1/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0      667 2024-04-21 00:26:28.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.808707 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.809721 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.901215 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.923471 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.810719 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.927467 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.928469 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.931474 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.943521 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      566 2024-04-21 00:09:10.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.948522 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.959486 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.964566 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.966568 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.968566 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10007 2024-04-19 19:46:13.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7503 2024-04-19 19:46:11.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.971078 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.977609 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.987378 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:01.008568 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    11767 2024-04-20 20:40:55.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:01.017108 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:01.025113 wagtail_fedit-1.5.3rc1/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6551 2024-04-21 00:08:49.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:01.037786 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     1881 2024-04-16 18:44:29.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-21 00:35:00.864660 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    19867 2024-04-21 00:35:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4038 2024-04-21 00:35:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 00:35:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-21 00:35:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 00:35:00.000000 wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.2/LICENSE` & `wagtail_fedit-1.5.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/PKG-INFO` & `wagtail_fedit-1.5.3rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.2
+Version: 1.5.3rc1
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -54,14 +54,15 @@
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
+  - [Share With Sessions](#wagtail_fedit_share_with_sessions)
 - [How your content is rendered](#how-your-content-is-rendered)
   - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
 
@@ -237,17 +238,17 @@
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
 ## Adapters
 
-Creating a custom adapter is relatively simple.  
-We highly recommend you to inherit from `BaseFieldFuncAdapter` or `BaseBlockFuncAdapter`.  
-These adapters are basically pre-setup to callback to a javascript function on successful form submission.  
+Creating a custom adapter is relatively simple.
+We highly recommend you to inherit from `BaseFieldFuncAdapter` or `BaseBlockFuncAdapter`.
+These adapters are basically pre-setup to callback to a javascript function on successful form submission.
 This will save you the most amount of work.
 
 We will create an adapter to change the color of a text field.
 
 Our adapter will be called `colorizer`.
 
 1. Our model is defined as follows:
@@ -283,17 +284,17 @@
 <div class="my-colorized-div" style="color: {{ page.color }}">
     <h1>Colorized Text!</h1>
 </div>
 
 ...
 ```
 
-###  Adapters Python
+### Adapters Python
 
-We will get started creating the adapter definition.  
+We will get started creating the adapter definition.
 Adapters can be defined anywhere; we recommend a separate `adapters.py` file.
 
 Adapter instances also have access to the following variables:
 
 * `self.object` - The model instance.
 * `self.field_name` - The field name.
 * `self.meta_field` - The models.Field instance.
@@ -334,15 +335,15 @@
     def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
         kwargs["name"] = "myColorizerJavascriptFunction"
         super().__init__(object, field_name, request, **kwargs)
 
     def render_content(self, parent_context=None):
         # This is not required; we will replace a CSS variable; thus we are not returning any actual content.
         return ""
-        
+    
     def get_response_data(self, parent_context=None):
         """
         Return the data to be sent to the frontend adapter.
         """
         data = super().get_response_data(parent_context)
         return data | {
             "color": self.field_value,
@@ -367,17 +368,17 @@
 
 from wagtail_fedit.adapters import adapter_registry
 from myapp.adapters import ColorizerAdapter
 
 adapter_registry.register(ColorizerAdapter)
 ```
 
-###  Adapters Javascript
+### Adapters Javascript
 
-We now need to create the javascript function to actually apply the color to the styles of the element.  
+We now need to create the javascript function to actually apply the color to the styles of the element.
 This function will be called `myColorizerJavascriptFunction`, as defined in the adapter's `__init__` method.
 
 ```javascript
 // myapp/static/myapp/js/custom.js
 function myColorizerJavascriptFunction(element, response) {
     element.style.color = response.color;
 }
@@ -441,15 +442,15 @@
 ```
 
 ### wagtail_fedit.register_css
 
 Register a custom CSS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
 
 Example of how this hook is used in wagtail_hooks.py:
-    
+
 ```python
 @hooks.register(REGISTER_CSS)
 def register_css(request):
     return [
         format_html(
             '<link rel="stylesheet" href="{0}">',
             static('css/custom.css')
@@ -458,40 +459,31 @@
 ```
 
 ### wagtail_fedit.field_editor_size
 
 Control the size of the editor for the given model-field type.
 
 Example of how this hook is called:
-    
+
 ```python
 for hook in hooks.get_hooks(FEDIT_FIELD_EDITOR_SIZE):
     size = hook(model_instance, model_field)
     if size:
         return size
 ```
 
 ### wagtail_fedit.register_js
 
 Register a custom JS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
 
 This can be used to register custom adapter JS.
 
 Example of how this hook is used in wagtail_hooks.py:
-    
-    ```python
-    @hooks.register(REGISTER_JS)
-    def register_js(request):
-        return [
-            format_html(
-                '<script src="{0}"></script>',
-                static('js/custom.js')
-            ),
-        ]
-    ```
+
+    ``python     @hooks.register(REGISTER_JS)     def register_js(request):         return [             format_html(                 '<script src="{0}"></script>',                 static('js/custom.js')             ),         ]     ``
 
 ### wagtail_fedit.register_field_renderer
 
 Register a custom renderer for a field.
 
 Example of how this type of renderer is used in wagtail_hooks/renderers.py:
 
@@ -545,34 +537,43 @@
 
 ## Settings
 
 ### `WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT`
 
 Default: `True`
 
-Sign the shared context with a secret key.  
-This is useful to prevent tampering with the shared context.  
-It will also be compressed with zlib if available.  
+Sign the shared context with a secret key.
+This is useful to prevent tampering with the shared context.
+It will also be compressed with zlib if available.
 It might not be in your site's security model to need this.
 
+### `WAGTAIL_FEDIT_SHARE_WITH_SESSIONS`
+
+Default: `False`
+
+Share the context through the session data.
+This is useful if you are running into limits with the URL length.
+This will store the context in the session and pass the session
+key to the iFrame instead of the context.
+
 ## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
 ### Rendered editable output HTML
 
 ```html
-<div class="wagtail-fedit-adapter-wrapper{%if shared_context.inline%} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}"{% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
+{% load fedit %}<div id="{{ adapter.get_element_id }}" class="wagtail-fedit-adapter-wrapper{% if shared_context.inline or adapter.inline %} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}" data-fedit-constructor="{{ js_constructor }}" {% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
     <div class="wagtail-fedit-buttons">
         {% for button in buttons %}
-            {{ button }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
+            {{ button }}
         {% endfor %}
-    </div>{{ content|safe }}
+    </div>{% render_adapter adapter %}
 </div>
 ```
 
 ## Implemented
 
 * Revision Support
 * Locked Support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.2 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc1 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -25,18 +25,19 @@
 (#wagtail_feditconstruct_adapter_toolbar) - [Register Type Renderer]
 (#wagtail_feditregister_type_renderer) - [Register Field Renderer]
 (#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
-[Sign Shared Context](#wagtail_fedit_sign_shared_context) - [How your content
-is rendered](#how-your-content-is-rendered) - [Rendered output HTML](#rendered-
-editable-output-html) - [Implemented](#implemented) Getting Started -----------
----- 1. Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
+[Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
+Sessions](#wagtail_fedit_share_with_sessions) - [How your content is rendered]
+(#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
+output-html) - [Implemented](#implemented) Getting Started --------------- 1.
+Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
 INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
 collectstatic`. 3. Run `py ./manage.py adapter_help` to see all your options
 and their requirements. ## Getting Editing! 1. Make sure the models you wish to
 edit inherit from PreviewableMixin. **This is a requirement.** 2. Define a
 template for your model. Example: ```django-html {% load fedit static
 wagtailuserbar %} {# Load the required template tag libraries #}
 {# Load all registered CSS required for the adapters. Only included inside edit
@@ -191,17 +192,17 @@
 ', static('css/custom.css') ), ] ``` ### wagtail_fedit.field_editor_size
 Control the size of the editor for the given model-field type. Example of how
 this hook is called: ```python for hook in hooks.get_hooks
 (FEDIT_FIELD_EDITOR_SIZE): size = hook(model_instance, model_field) if size:
 return size ``` ### wagtail_fedit.register_js Register a custom JS file to be
 included when the utils.FEDIT_PREVIEW_VAR is set to True. This can be used to
 register custom adapter JS. Example of how this hook is used in
-wagtail_hooks.py: ```python @hooks.register(REGISTER_JS) def register_js
+wagtail_hooks.py: ``python @hooks.register(REGISTER_JS) def register_js
 (request): return [ format_html( '
-', static('js/custom.js') ), ] ``` ### wagtail_fedit.register_field_renderer
+', static('js/custom.js') ), ] `` ### wagtail_fedit.register_field_renderer
 Register a custom renderer for a field. Example of how this type of renderer is
 used in wagtail_hooks/renderers.py: ```python @hooks.register
 (REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
 custom renderer for RichText fields. # It will render the RichText field as a
 RichText block. renderer_map[RichTextField] =\ lambda request, context,
 instance, value: richtext(value) ``` ### wagtail_fedit.exclude_related_forms
 Exclude the given model type from the related forms. This is used internally to
@@ -217,21 +218,24 @@
 if you want to hide the item, and True if you want to show the item. Example of
 how this hook is called: ```python for hook in hooks.get_hooks
 (ACTION_MENU_ITEM_IS_SHOWN): result = hook(context, instance) if result is not
 None: return result # <- bool ``` ## Settings ###
 `WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT` Default: `True` Sign the shared context
 with a secret key. This is useful to prevent tampering with the shared context.
 It will also be compressed with zlib if available. It might not be in your
-site's security model to need this. ## How your content is rendered
-(**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
-or even at all for most content - **if** you don't get hyperspecific with your
-CSS selectors and structure your templates well.) Your block and field are
-wrapped in a `div`, any CSS for your templates should keep this in mind. ###
-Rendered editable output HTML ```html
+site's security model to need this. ### `WAGTAIL_FEDIT_SHARE_WITH_SESSIONS`
+Default: `False` Share the context through the session data. This is useful if
+you are running into limits with the URL length. This will store the context in
+the session and pass the session key to the iFrame instead of the context. ##
+How your content is rendered (**Maintainer's note:** In my experience this
+doesn't mess the CSS up too much, or even at all for most content - **if** you
+don't get hyperspecific with your CSS selectors and structure your templates
+well.) Your block and field are wrapped in a `div`, any CSS for your templates
+should keep this in mind. ### Rendered editable output HTML ```html {% load
+fedit %}
 % if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
 { edit_url }}">
-{% for button in buttons %} {{ button }} {# Edit button; more buttons MIGHT
-possibly be added in the future. #} {% endfor %}
-{{ content|safe }}
+{% for button in buttons %} {{ button }} {% endfor %}
+{% render_adapter adapter %}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.5.2/README.md` & `wagtail_fedit-1.5.3rc1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
+  - [Share With Sessions](#wagtail_fedit_share_with_sessions)
 - [How your content is rendered](#how-your-content-is-rendered)
   - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
 
@@ -207,17 +208,17 @@
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
 ## Adapters
 
-Creating a custom adapter is relatively simple.  
-We highly recommend you to inherit from `BaseFieldFuncAdapter` or `BaseBlockFuncAdapter`.  
-These adapters are basically pre-setup to callback to a javascript function on successful form submission.  
+Creating a custom adapter is relatively simple.
+We highly recommend you to inherit from `BaseFieldFuncAdapter` or `BaseBlockFuncAdapter`.
+These adapters are basically pre-setup to callback to a javascript function on successful form submission.
 This will save you the most amount of work.
 
 We will create an adapter to change the color of a text field.
 
 Our adapter will be called `colorizer`.
 
 1. Our model is defined as follows:
@@ -253,17 +254,17 @@
 <div class="my-colorized-div" style="color: {{ page.color }}">
     <h1>Colorized Text!</h1>
 </div>
 
 ...
 ```
 
-###  Adapters Python
+### Adapters Python
 
-We will get started creating the adapter definition.  
+We will get started creating the adapter definition.
 Adapters can be defined anywhere; we recommend a separate `adapters.py` file.
 
 Adapter instances also have access to the following variables:
 
 * `self.object` - The model instance.
 * `self.field_name` - The field name.
 * `self.meta_field` - The models.Field instance.
@@ -304,15 +305,15 @@
     def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
         kwargs["name"] = "myColorizerJavascriptFunction"
         super().__init__(object, field_name, request, **kwargs)
 
     def render_content(self, parent_context=None):
         # This is not required; we will replace a CSS variable; thus we are not returning any actual content.
         return ""
-        
+    
     def get_response_data(self, parent_context=None):
         """
         Return the data to be sent to the frontend adapter.
         """
         data = super().get_response_data(parent_context)
         return data | {
             "color": self.field_value,
@@ -337,17 +338,17 @@
 
 from wagtail_fedit.adapters import adapter_registry
 from myapp.adapters import ColorizerAdapter
 
 adapter_registry.register(ColorizerAdapter)
 ```
 
-###  Adapters Javascript
+### Adapters Javascript
 
-We now need to create the javascript function to actually apply the color to the styles of the element.  
+We now need to create the javascript function to actually apply the color to the styles of the element.
 This function will be called `myColorizerJavascriptFunction`, as defined in the adapter's `__init__` method.
 
 ```javascript
 // myapp/static/myapp/js/custom.js
 function myColorizerJavascriptFunction(element, response) {
     element.style.color = response.color;
 }
@@ -411,15 +412,15 @@
 ```
 
 ### wagtail_fedit.register_css
 
 Register a custom CSS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
 
 Example of how this hook is used in wagtail_hooks.py:
-    
+
 ```python
 @hooks.register(REGISTER_CSS)
 def register_css(request):
     return [
         format_html(
             '<link rel="stylesheet" href="{0}">',
             static('css/custom.css')
@@ -428,40 +429,31 @@
 ```
 
 ### wagtail_fedit.field_editor_size
 
 Control the size of the editor for the given model-field type.
 
 Example of how this hook is called:
-    
+
 ```python
 for hook in hooks.get_hooks(FEDIT_FIELD_EDITOR_SIZE):
     size = hook(model_instance, model_field)
     if size:
         return size
 ```
 
 ### wagtail_fedit.register_js
 
 Register a custom JS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
 
 This can be used to register custom adapter JS.
 
 Example of how this hook is used in wagtail_hooks.py:
-    
-    ```python
-    @hooks.register(REGISTER_JS)
-    def register_js(request):
-        return [
-            format_html(
-                '<script src="{0}"></script>',
-                static('js/custom.js')
-            ),
-        ]
-    ```
+
+    ``python     @hooks.register(REGISTER_JS)     def register_js(request):         return [             format_html(                 '<script src="{0}"></script>',                 static('js/custom.js')             ),         ]     ``
 
 ### wagtail_fedit.register_field_renderer
 
 Register a custom renderer for a field.
 
 Example of how this type of renderer is used in wagtail_hooks/renderers.py:
 
@@ -515,34 +507,43 @@
 
 ## Settings
 
 ### `WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT`
 
 Default: `True`
 
-Sign the shared context with a secret key.  
-This is useful to prevent tampering with the shared context.  
-It will also be compressed with zlib if available.  
+Sign the shared context with a secret key.
+This is useful to prevent tampering with the shared context.
+It will also be compressed with zlib if available.
 It might not be in your site's security model to need this.
 
+### `WAGTAIL_FEDIT_SHARE_WITH_SESSIONS`
+
+Default: `False`
+
+Share the context through the session data.
+This is useful if you are running into limits with the URL length.
+This will store the context in the session and pass the session
+key to the iFrame instead of the context.
+
 ## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
 ### Rendered editable output HTML
 
 ```html
-<div class="wagtail-fedit-adapter-wrapper{%if shared_context.inline%} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}"{% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
+{% load fedit %}<div id="{{ adapter.get_element_id }}" class="wagtail-fedit-adapter-wrapper{% if shared_context.inline or adapter.inline %} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}" data-fedit-constructor="{{ js_constructor }}" {% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
     <div class="wagtail-fedit-buttons">
         {% for button in buttons %}
-            {{ button }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
+            {{ button }}
         {% endfor %}
-    </div>{{ content|safe }}
+    </div>{% render_adapter adapter %}
 </div>
 ```
 
 ## Implemented
 
 * Revision Support
 * Locked Support
```

#### html2text {}

```diff
@@ -10,18 +10,19 @@
 (#wagtail_feditconstruct_adapter_toolbar) - [Register Type Renderer]
 (#wagtail_feditregister_type_renderer) - [Register Field Renderer]
 (#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
-[Sign Shared Context](#wagtail_fedit_sign_shared_context) - [How your content
-is rendered](#how-your-content-is-rendered) - [Rendered output HTML](#rendered-
-editable-output-html) - [Implemented](#implemented) Getting Started -----------
----- 1. Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
+[Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
+Sessions](#wagtail_fedit_share_with_sessions) - [How your content is rendered]
+(#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
+output-html) - [Implemented](#implemented) Getting Started --------------- 1.
+Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
 INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
 collectstatic`. 3. Run `py ./manage.py adapter_help` to see all your options
 and their requirements. ## Getting Editing! 1. Make sure the models you wish to
 edit inherit from PreviewableMixin. **This is a requirement.** 2. Define a
 template for your model. Example: ```django-html {% load fedit static
 wagtailuserbar %} {# Load the required template tag libraries #}
 {# Load all registered CSS required for the adapters. Only included inside edit
@@ -176,17 +177,17 @@
 ', static('css/custom.css') ), ] ``` ### wagtail_fedit.field_editor_size
 Control the size of the editor for the given model-field type. Example of how
 this hook is called: ```python for hook in hooks.get_hooks
 (FEDIT_FIELD_EDITOR_SIZE): size = hook(model_instance, model_field) if size:
 return size ``` ### wagtail_fedit.register_js Register a custom JS file to be
 included when the utils.FEDIT_PREVIEW_VAR is set to True. This can be used to
 register custom adapter JS. Example of how this hook is used in
-wagtail_hooks.py: ```python @hooks.register(REGISTER_JS) def register_js
+wagtail_hooks.py: ``python @hooks.register(REGISTER_JS) def register_js
 (request): return [ format_html( '
-', static('js/custom.js') ), ] ``` ### wagtail_fedit.register_field_renderer
+', static('js/custom.js') ), ] `` ### wagtail_fedit.register_field_renderer
 Register a custom renderer for a field. Example of how this type of renderer is
 used in wagtail_hooks/renderers.py: ```python @hooks.register
 (REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
 custom renderer for RichText fields. # It will render the RichText field as a
 RichText block. renderer_map[RichTextField] =\ lambda request, context,
 instance, value: richtext(value) ``` ### wagtail_fedit.exclude_related_forms
 Exclude the given model type from the related forms. This is used internally to
@@ -202,21 +203,24 @@
 if you want to hide the item, and True if you want to show the item. Example of
 how this hook is called: ```python for hook in hooks.get_hooks
 (ACTION_MENU_ITEM_IS_SHOWN): result = hook(context, instance) if result is not
 None: return result # <- bool ``` ## Settings ###
 `WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT` Default: `True` Sign the shared context
 with a secret key. This is useful to prevent tampering with the shared context.
 It will also be compressed with zlib if available. It might not be in your
-site's security model to need this. ## How your content is rendered
-(**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
-or even at all for most content - **if** you don't get hyperspecific with your
-CSS selectors and structure your templates well.) Your block and field are
-wrapped in a `div`, any CSS for your templates should keep this in mind. ###
-Rendered editable output HTML ```html
+site's security model to need this. ### `WAGTAIL_FEDIT_SHARE_WITH_SESSIONS`
+Default: `False` Share the context through the session data. This is useful if
+you are running into limits with the URL length. This will store the context in
+the session and pass the session key to the iFrame instead of the context. ##
+How your content is rendered (**Maintainer's note:** In my experience this
+doesn't mess the CSS up too much, or even at all for most content - **if** you
+don't get hyperspecific with your CSS selectors and structure your templates
+well.) Your block and field are wrapped in a `div`, any CSS for your templates
+should keep this in mind. ### Rendered editable output HTML ```html {% load
+fedit %}
 % if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
 { edit_url }}">
-{% for button in buttons %} {{ button }} {# Edit button; more buttons MIGHT
-possibly be added in the future. #} {% endfor %}
-{{ content|safe }}
+{% for button in buttons %} {{ button }} {% endfor %}
+{% render_adapter adapter %}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.5.2/setup.cfg` & `wagtail_fedit-1.5.3rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
-00000040: 2046 726f 6e74 656e 6420 6564 6974 696e   Frontend editin
-00000050: 6720 666f 7220 796f 7572 2057 6167 7461  g for your Wagta
-00000060: 696c 2073 6974 650d 0a6c 6f6e 675f 6465  il site..long_de
-00000070: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
-00000080: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
-00000090: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
-000000a0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-000000b0: 742f 6d61 726b 646f 776e 0d0a 6175 7468  t/markdown..auth
-000000c0: 6f72 203d 204e 6967 656c 0d0a 6175 7468  or = Nigel..auth
-000000d0: 6f72 5f65 6d61 696c 203d 206e 6967 656c  or_email = nigel
-000000e0: 4067 6f6f 6461 6476 6963 652e 6974 0d0a  @goodadvice.it..
-000000f0: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000100: 7468 7562 2e63 6f6d 2f4e 6967 656c 3233  thub.com/Nigel23
-00000110: 3932 2f77 6167 7461 696c 5f66 6564 6974  92/wagtail_fedit
-00000120: 0d0a 6c69 6365 6e73 6520 3d20 4750 4c2d  ..license = GPL-
-00000130: 322e 302d 6f6e 6c79 0d0a 636c 6173 7369  2.0-only..classi
-00000140: 6669 6572 7320 3d20 0d0a 0945 6e76 6972  fiers = ...Envir
-00000150: 6f6e 6d65 6e74 203a 3a20 5765 6220 456e  onment :: Web En
-00000160: 7669 726f 6e6d 656e 740d 0a09 4672 616d  vironment...Fram
-00000170: 6577 6f72 6b20 3a3a 2044 6a61 6e67 6f0d  ework :: Django.
-00000180: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
-00000190: 6a61 6e67 6f20 3a3a 2034 2e32 0d0a 0946  jango :: 4.2...F
-000001a0: 7261 6d65 776f 726b 203a 3a20 5761 6774  ramework :: Wagt
-000001b0: 6169 6c0d 0a09 4672 616d 6577 6f72 6b20  ail...Framework 
-000001c0: 3a3a 2057 6167 7461 696c 203a 3a20 350d  :: Wagtail :: 5.
-000001d0: 0a09 4672 616d 6577 6f72 6b20 3a3a 2057  ..Framework :: W
-000001e0: 6167 7461 696c 203a 3a20 360d 0a09 496e  agtail :: 6...In
-000001f0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-00000200: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
-00000210: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000220: 7070 726f 7665 6420 3a3a 2047 4e55 2047  pproved :: GNU G
-00000230: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
-00000240: 6365 6e73 6520 7632 206f 7220 6c61 7465  cense v2 or late
-00000250: 7220 2847 504c 7632 2b29 0d0a 094f 7065  r (GPLv2+)...Ope
-00000260: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000270: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-00000280: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000290: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002a0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000002b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002c0: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
-000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002e0: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
-000002f0: 4f6e 6c79 0d0a 0950 726f 6772 616d 6d69  Only...Programmi
-00000300: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000310: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
-00000320: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000330: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000340: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
-00000350: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000360: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
-00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000380: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000390: 3a20 332e 3131 0d0a 0954 6f70 6963 203a  : 3.11...Topic :
-000003a0: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
-000003b0: 572f 4854 5450 0d0a 0954 6f70 6963 203a  W/HTTP...Topic :
-000003c0: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
-000003d0: 572f 4854 5450 203a 3a20 4479 6e61 6d69  W/HTTP :: Dynami
-000003e0: 6320 436f 6e74 656e 740d 0a0d 0a5b 6f70  c Content....[op
-000003f0: 7469 6f6e 735d 0d0a 696e 636c 7564 655f  tions]..include_
-00000400: 7061 636b 6167 655f 6461 7461 203d 2074  package_data = t
-00000410: 7275 650d 0a70 6163 6b61 6765 7320 3d20  rue..packages = 
-00000420: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-00000430: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
-00000440: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000450: 203d 200d 0a09 446a 616e 676f 203e 3d20   = ...Django >= 
-00000460: 342e 320d 0a09 5761 6774 6169 6c20 3e3d  4.2...Wagtail >=
-00000470: 2035 2e32 0d0a 0d0a 5b65 6767 5f69 6e66   5.2....[egg_inf
-00000480: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000490: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000004a0: 0d0a                                     ..
+00000030: 3372 6331 0d0a 6465 7363 7269 7074 696f  3rc1..descriptio
+00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
+00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
+00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
+00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000b0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
+000000c0: 7574 686f 7220 3d20 4e69 6765 6c0d 0a61  uthor = Nigel..a
+000000d0: 7574 686f 725f 656d 6169 6c20 3d20 6e69  uthor_email = ni
+000000e0: 6765 6c40 676f 6f64 6164 7669 6365 2e69  gel@goodadvice.i
+000000f0: 740d 0a75 726c 203d 2068 7474 7073 3a2f  t..url = https:/
+00000100: 2f67 6974 6875 622e 636f 6d2f 4e69 6765  /github.com/Nige
+00000110: 6c32 3339 322f 7761 6774 6169 6c5f 6665  l2392/wagtail_fe
+00000120: 6469 740d 0a6c 6963 656e 7365 203d 2047  dit..license = G
+00000130: 504c 2d32 2e30 2d6f 6e6c 790d 0a63 6c61  PL-2.0-only..cla
+00000140: 7373 6966 6965 7273 203d 200d 0a09 456e  ssifiers = ...En
+00000150: 7669 726f 6e6d 656e 7420 3a3a 2057 6562  vironment :: Web
+00000160: 2045 6e76 6972 6f6e 6d65 6e74 0d0a 0946   Environment...F
+00000170: 7261 6d65 776f 726b 203a 3a20 446a 616e  ramework :: Djan
+00000180: 676f 0d0a 0946 7261 6d65 776f 726b 203a  go...Framework :
+00000190: 3a20 446a 616e 676f 203a 3a20 342e 320d  : Django :: 4.2.
+000001a0: 0a09 4672 616d 6577 6f72 6b20 3a3a 2057  ..Framework :: W
+000001b0: 6167 7461 696c 0d0a 0946 7261 6d65 776f  agtail...Framewo
+000001c0: 726b 203a 3a20 5761 6774 6169 6c20 3a3a  rk :: Wagtail ::
+000001d0: 2035 0d0a 0946 7261 6d65 776f 726b 203a   5...Framework :
+000001e0: 3a20 5761 6774 6169 6c20 3a3a 2036 0d0a  : Wagtail :: 6..
+000001f0: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+00000200: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+00000210: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
+00000220: 4920 4170 7072 6f76 6564 203a 3a20 474e  I Approved :: GN
+00000230: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+00000240: 204c 6963 656e 7365 2076 3220 6f72 206c   License v2 or l
+00000250: 6174 6572 2028 4750 4c76 322b 290d 0a09  ater (GPLv2+)...
+00000260: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000270: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+00000280: 6e74 0d0a 0950 726f 6772 616d 6d69 6e67  nt...Programming
+00000290: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002a0: 686f 6e0d 0a09 5072 6f67 7261 6d6d 696e  hon...Programmin
+000002b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002c0: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
+000002d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002e0: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+000002f0: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
+00000300: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000310: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
+00000320: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000330: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000340: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
+00000350: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000360: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000370: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000380: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000390: 6e20 3a3a 2033 2e31 310d 0a09 546f 7069  n :: 3.11...Topi
+000003a0: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
+000003b0: 2057 5757 2f48 5454 500d 0a09 546f 7069   WWW/HTTP...Topi
+000003c0: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
+000003d0: 2057 5757 2f48 5454 5020 3a3a 2044 796e   WWW/HTTP :: Dyn
+000003e0: 616d 6963 2043 6f6e 7465 6e74 0d0a 0d0a  amic Content....
+000003f0: 5b6f 7074 696f 6e73 5d0d 0a69 6e63 6c75  [options]..inclu
+00000400: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000410: 3d20 7472 7565 0d0a 7061 636b 6167 6573  = true..packages
+00000420: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
+00000430: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+00000440: 380d 0a69 6e73 7461 6c6c 5f72 6571 7569  8..install_requi
+00000450: 7265 7320 3d20 0d0a 0944 6a61 6e67 6f20  res = ...Django 
+00000460: 3e3d 2034 2e32 0d0a 0957 6167 7461 696c  >= 4.2...Wagtail
+00000470: 203e 3d20 352e 320d 0a0d 0a5b 6567 675f   >= 5.2....[egg_
+00000480: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000490: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+000004a0: 300d 0a0d 0a                             0....
```

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Signer,
 )
 from django.http import (
     HttpRequest,
 )
 from ..settings import (
     SIGN_SHARED_CONTEXT,
+    SHARE_WITH_SESSIONS,
 )
 from ..utils import (
     FeditIFrameMixin,
     wrap_adapter,
 )
 
 if TYPE_CHECKING:
@@ -59,14 +60,18 @@
     return base64.b85encode(json.dumps(obj).encode("utf-8")).decode("utf-8")
 
 def Base85_json_loads(data):
     return json.loads(base64.b85decode(data).decode("utf-8"))
 
 class BaseAdapter(FeditIFrameMixin):
     identifier              = None
+
+    # The template used to render the form.
+    template_name           = "wagtail_fedit/editor/adapter_iframe.html"
+
     signer: Signer          = Signer()
     # Required keyword arguments for the adapter
     required_kwargs         = []
     # Optional keyword arguments for the adapter, these are only used to print the help example.
     optional_kwargs         = []
     # Tokens which should be resolved absolutely (no parser.compile_filter)
     # These are NOT required.
@@ -136,14 +141,20 @@
         """
         if "inline" in cls.absolute_tokens:
             return {
                 "inline": "if passed; the adapter will be rendered with inline styles.",
                 **cls.help_text_dict,
             }
         return cls.help_text_dict
+    
+    def get_template_names(self) -> list[str]:
+        """
+        Return the template names for the adapter.
+        """
+        return [self.template_name]
 
     @property
     def field_value(self):
         """
         Call the value_from_object method on
         the meta field to get the value from the instance.
         """
@@ -205,15 +216,20 @@
         """
         return []
 
     def get_element_id(self) -> str:
         """
         Return a unique identifier for the elements on the frontend.
         """
-        raise NotImplementedError
+        return content_id_from_parts(
+            self.model._meta.app_label,
+            self.model._meta.model_name,
+            self.object.pk,
+            self.field_name,
+        )
     
     def get_form_attrs(self) -> dict:
         """
         Extra possible form attributes rendered in the iFrame.
         """
         return {}
     
@@ -256,27 +272,36 @@
         """
         Encode a dictionary to a string.
         This will be passed as a GET parameter to the iFrame.
         Make sure the data is not too large.
         """
         if not self.kwargs:
             return ""
+        if SHARE_WITH_SESSIONS:
+            id = self.get_element_id()
+            self.request.session[id] = self.kwargs
+            self.request.session.modified = True
+            return id
         # return self.signer.sign_object(self.kwargs)# , serializer=PickleBlockSerializer)
         if SIGN_SHARED_CONTEXT:
             return self.signer.sign_object(self.kwargs, compress=True)
         
         return Base85_json_dumps(self.kwargs)
 
+
     @classmethod
     def decode_shared_context(cls, request: HttpRequest, object: models.Model, field: str, context: str) -> dict:
         """
         Decode an encoded contex string back to a dictionary.
         """
-        if not context:
-            return {}
+        if SHARE_WITH_SESSIONS:
+            if not context:
+                return {}
+            return request.session.get(context, {})
+        
         if SIGN_SHARED_CONTEXT:
             return cls.signer.unsign_object(context)# , serializer=PickleBlockSerializer)
         try:
             return Base85_json_loads(context)
         except json.JSONDecodeError:
             pass
         return {}
```

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/block.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/models.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-{% extends "./base_iframe.html" %}
-
 {% load i18n wagtailadmin_tags %}
-
-{% block content %}
-    <div class="wagtail-fedit-form-wrapper{% if form.block.block.meta.fedit_full %} fedit-full{% endif %}">
-
-        {{ block.super }}
-
-        <form id="wagtail-fedit-form" data-edit-form action="{{ edit_url }}" method="post" {% for k, v in form_attrs.items %}{{ k }}="{{ v|safe }}" {% endfor %}>
-            {% csrf_token %}
-            {% block form %}
-                {% panel id="wagtail-fedit-editor" icon="draft" heading=meta_field.verbose_name %}
-                    <div class="wagtail-fedit-form">
-                        {% for field in form %}
-                            {% include "./field.html" %}
-                        {% endfor %}
-                    </div>
-                {% endpanel %}
-            {% endblock %}
-        </form>
-    </div>
-{% endblock %}
+<form id="wagtail-fedit-form" data-edit-form action="{{ edit_url }}" method="post" {% for k, v in form_attrs.items %}{{ k }}="{{ v|safe }}" {% endfor %}>
+    {% csrf_token %}
+    {% block form %}
+        {% panel id="wagtail-fedit-editor" icon="draft" heading=meta_field.verbose_name %}
+            <div class="wagtail-fedit-form">
+                {% for field in form %}
+                    {% include "./field.html" %}
+                {% endfor %}
+            </div>
+        {% endpanel %}
+    {% endblock %}
+</form>
```

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files 10% similar despite different names*

```diff
@@ -67,28 +67,17 @@
                     {% help_block status="info" %}
                         <p>{% translate "This object is locked and cannot be edited." %}</p>
                     {% endhelp_block %}
                 {% endpanel %}
             {% else %}
             
                 {% block content %}
-                    {% block errors %}
-                        {% if form.errors %}
-                            <div class="error-message">
-                                <h2>{{ view.get_error_title }}</h2>
-                                <ul>
-                                    {% for field in form %}
-                                        {% for error in field.errors %}
-                                            <li class="error">{{ field.label }}: {{ error }}</li>
-                                        {% endfor %}
-                                    {% endfor %}
-                                </ul>
-                            </div>
-                        {% endif %}
-                    {% endblock %}
+
+                    
+
                 {% endblock %}
                 
             {% endif %}
         </div>
     </main>
     {% block sidebar_root %}
         <aside>
```

#### html2text {}

```diff
@@ -25,21 +25,16 @@
 status="info" %}
 {% translate "This object is locked" %}
 {% translate "You are still able to edit this object." %}
 {% endhelp_block %} {% endpanel %} {% endif %} {% if locked_for_user %} {%
 panel id="wagtail-fedit-lock-text" icon="help" heading=locked_heading %} {%
 help_block status="info" %}
 {% translate "This object is locked and cannot be edited." %}
-{% endhelp_block %} {% endpanel %} {% else %} {% block content %} {% block
-errors %} {% if form.errors %}
-********** {{{{ vviieeww..ggeett__eerrrroorr__ttiittllee }}}} **********
-    * {% for field in form %} {% for error in field.errors %}
-    * {{ field.label }}: {{ error }}
-    * {% endfor %} {% endfor %}
-{% endif %} {% endblock %} {% endblock %} {% endif %}
+{% endhelp_block %} {% endpanel %} {% else %} {% block content %} {% endblock
+%} {% endif %}
 {% block sidebar_root %}
 {% block sidebar_logo %}{% endblock %}
 {% block sidebar %} {% if admin_edit_url %}
 }" target="_blank"> {% icon name="link-external" %}
 {% endif %}
 }">
 }" viewBox="0 0 16 16">
```

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/views/adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     FeditIFrameMixin,
     FEDIT_PREVIEW_VAR,
     lock_info,
 )
 
 @method_decorator(xframe_options_sameorigin, name="dispatch")
 class BaseAdapterView(FeditIFrameMixin, FeditPermissionCheck, WagtailAdminTemplateMixin, View):
-    template_name = "wagtail_fedit/editor/adapter_iframe.html"
     ERROR_TITLE = _("Validation Errors")
 
     def dispatch(self, 
             request:    HttpRequest,
             adapter_id: str = None,
             field_name: str = None,
             app_label:  str = None,
@@ -103,15 +102,18 @@
             True,
         )
 
         return super().dispatch(
             request, adapter_id, field_name, app_label, model_name, model_id,
         )
     
-
+    @property
+    def template_name(self):
+        return self.adapter.get_template_names()
+    
     def render_to_response(self, context: dict[str, Any], success: bool = True, extra: dict = None, **response_kwargs: Any) -> HttpResponse:
         if not extra:
             extra = {}
 
         extra.update({
             "success": success,
         })
```

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.3rc1/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.2
+Version: 1.5.3rc1
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -54,14 +54,15 @@
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
+  - [Share With Sessions](#wagtail_fedit_share_with_sessions)
 - [How your content is rendered](#how-your-content-is-rendered)
   - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
 
@@ -237,17 +238,17 @@
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
 ## Adapters
 
-Creating a custom adapter is relatively simple.  
-We highly recommend you to inherit from `BaseFieldFuncAdapter` or `BaseBlockFuncAdapter`.  
-These adapters are basically pre-setup to callback to a javascript function on successful form submission.  
+Creating a custom adapter is relatively simple.
+We highly recommend you to inherit from `BaseFieldFuncAdapter` or `BaseBlockFuncAdapter`.
+These adapters are basically pre-setup to callback to a javascript function on successful form submission.
 This will save you the most amount of work.
 
 We will create an adapter to change the color of a text field.
 
 Our adapter will be called `colorizer`.
 
 1. Our model is defined as follows:
@@ -283,17 +284,17 @@
 <div class="my-colorized-div" style="color: {{ page.color }}">
     <h1>Colorized Text!</h1>
 </div>
 
 ...
 ```
 
-###  Adapters Python
+### Adapters Python
 
-We will get started creating the adapter definition.  
+We will get started creating the adapter definition.
 Adapters can be defined anywhere; we recommend a separate `adapters.py` file.
 
 Adapter instances also have access to the following variables:
 
 * `self.object` - The model instance.
 * `self.field_name` - The field name.
 * `self.meta_field` - The models.Field instance.
@@ -334,15 +335,15 @@
     def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
         kwargs["name"] = "myColorizerJavascriptFunction"
         super().__init__(object, field_name, request, **kwargs)
 
     def render_content(self, parent_context=None):
         # This is not required; we will replace a CSS variable; thus we are not returning any actual content.
         return ""
-        
+    
     def get_response_data(self, parent_context=None):
         """
         Return the data to be sent to the frontend adapter.
         """
         data = super().get_response_data(parent_context)
         return data | {
             "color": self.field_value,
@@ -367,17 +368,17 @@
 
 from wagtail_fedit.adapters import adapter_registry
 from myapp.adapters import ColorizerAdapter
 
 adapter_registry.register(ColorizerAdapter)
 ```
 
-###  Adapters Javascript
+### Adapters Javascript
 
-We now need to create the javascript function to actually apply the color to the styles of the element.  
+We now need to create the javascript function to actually apply the color to the styles of the element.
 This function will be called `myColorizerJavascriptFunction`, as defined in the adapter's `__init__` method.
 
 ```javascript
 // myapp/static/myapp/js/custom.js
 function myColorizerJavascriptFunction(element, response) {
     element.style.color = response.color;
 }
@@ -441,15 +442,15 @@
 ```
 
 ### wagtail_fedit.register_css
 
 Register a custom CSS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
 
 Example of how this hook is used in wagtail_hooks.py:
-    
+
 ```python
 @hooks.register(REGISTER_CSS)
 def register_css(request):
     return [
         format_html(
             '<link rel="stylesheet" href="{0}">',
             static('css/custom.css')
@@ -458,40 +459,31 @@
 ```
 
 ### wagtail_fedit.field_editor_size
 
 Control the size of the editor for the given model-field type.
 
 Example of how this hook is called:
-    
+
 ```python
 for hook in hooks.get_hooks(FEDIT_FIELD_EDITOR_SIZE):
     size = hook(model_instance, model_field)
     if size:
         return size
 ```
 
 ### wagtail_fedit.register_js
 
 Register a custom JS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
 
 This can be used to register custom adapter JS.
 
 Example of how this hook is used in wagtail_hooks.py:
-    
-    ```python
-    @hooks.register(REGISTER_JS)
-    def register_js(request):
-        return [
-            format_html(
-                '<script src="{0}"></script>',
-                static('js/custom.js')
-            ),
-        ]
-    ```
+
+    ``python     @hooks.register(REGISTER_JS)     def register_js(request):         return [             format_html(                 '<script src="{0}"></script>',                 static('js/custom.js')             ),         ]     ``
 
 ### wagtail_fedit.register_field_renderer
 
 Register a custom renderer for a field.
 
 Example of how this type of renderer is used in wagtail_hooks/renderers.py:
 
@@ -545,34 +537,43 @@
 
 ## Settings
 
 ### `WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT`
 
 Default: `True`
 
-Sign the shared context with a secret key.  
-This is useful to prevent tampering with the shared context.  
-It will also be compressed with zlib if available.  
+Sign the shared context with a secret key.
+This is useful to prevent tampering with the shared context.
+It will also be compressed with zlib if available.
 It might not be in your site's security model to need this.
 
+### `WAGTAIL_FEDIT_SHARE_WITH_SESSIONS`
+
+Default: `False`
+
+Share the context through the session data.
+This is useful if you are running into limits with the URL length.
+This will store the context in the session and pass the session
+key to the iFrame instead of the context.
+
 ## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
 ### Rendered editable output HTML
 
 ```html
-<div class="wagtail-fedit-adapter-wrapper{%if shared_context.inline%} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}"{% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
+{% load fedit %}<div id="{{ adapter.get_element_id }}" class="wagtail-fedit-adapter-wrapper{% if shared_context.inline or adapter.inline %} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}" data-fedit-constructor="{{ js_constructor }}" {% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
     <div class="wagtail-fedit-buttons">
         {% for button in buttons %}
-            {{ button }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
+            {{ button }}
         {% endfor %}
-    </div>{{ content|safe }}
+    </div>{% render_adapter adapter %}
 </div>
 ```
 
 ## Implemented
 
 * Revision Support
 * Locked Support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.2 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.3rc1 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -25,18 +25,19 @@
 (#wagtail_feditconstruct_adapter_toolbar) - [Register Type Renderer]
 (#wagtail_feditregister_type_renderer) - [Register Field Renderer]
 (#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
-[Sign Shared Context](#wagtail_fedit_sign_shared_context) - [How your content
-is rendered](#how-your-content-is-rendered) - [Rendered output HTML](#rendered-
-editable-output-html) - [Implemented](#implemented) Getting Started -----------
----- 1. Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
+[Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
+Sessions](#wagtail_fedit_share_with_sessions) - [How your content is rendered]
+(#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
+output-html) - [Implemented](#implemented) Getting Started --------------- 1.
+Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
 INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
 collectstatic`. 3. Run `py ./manage.py adapter_help` to see all your options
 and their requirements. ## Getting Editing! 1. Make sure the models you wish to
 edit inherit from PreviewableMixin. **This is a requirement.** 2. Define a
 template for your model. Example: ```django-html {% load fedit static
 wagtailuserbar %} {# Load the required template tag libraries #}
 {# Load all registered CSS required for the adapters. Only included inside edit
@@ -191,17 +192,17 @@
 ', static('css/custom.css') ), ] ``` ### wagtail_fedit.field_editor_size
 Control the size of the editor for the given model-field type. Example of how
 this hook is called: ```python for hook in hooks.get_hooks
 (FEDIT_FIELD_EDITOR_SIZE): size = hook(model_instance, model_field) if size:
 return size ``` ### wagtail_fedit.register_js Register a custom JS file to be
 included when the utils.FEDIT_PREVIEW_VAR is set to True. This can be used to
 register custom adapter JS. Example of how this hook is used in
-wagtail_hooks.py: ```python @hooks.register(REGISTER_JS) def register_js
+wagtail_hooks.py: ``python @hooks.register(REGISTER_JS) def register_js
 (request): return [ format_html( '
-', static('js/custom.js') ), ] ``` ### wagtail_fedit.register_field_renderer
+', static('js/custom.js') ), ] `` ### wagtail_fedit.register_field_renderer
 Register a custom renderer for a field. Example of how this type of renderer is
 used in wagtail_hooks/renderers.py: ```python @hooks.register
 (REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
 custom renderer for RichText fields. # It will render the RichText field as a
 RichText block. renderer_map[RichTextField] =\ lambda request, context,
 instance, value: richtext(value) ``` ### wagtail_fedit.exclude_related_forms
 Exclude the given model type from the related forms. This is used internally to
@@ -217,21 +218,24 @@
 if you want to hide the item, and True if you want to show the item. Example of
 how this hook is called: ```python for hook in hooks.get_hooks
 (ACTION_MENU_ITEM_IS_SHOWN): result = hook(context, instance) if result is not
 None: return result # <- bool ``` ## Settings ###
 `WAGTAIL_FEDIT_SIGN_SHARED_CONTEXT` Default: `True` Sign the shared context
 with a secret key. This is useful to prevent tampering with the shared context.
 It will also be compressed with zlib if available. It might not be in your
-site's security model to need this. ## How your content is rendered
-(**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
-or even at all for most content - **if** you don't get hyperspecific with your
-CSS selectors and structure your templates well.) Your block and field are
-wrapped in a `div`, any CSS for your templates should keep this in mind. ###
-Rendered editable output HTML ```html
+site's security model to need this. ### `WAGTAIL_FEDIT_SHARE_WITH_SESSIONS`
+Default: `False` Share the context through the session data. This is useful if
+you are running into limits with the URL length. This will store the context in
+the session and pass the session key to the iFrame instead of the context. ##
+How your content is rendered (**Maintainer's note:** In my experience this
+doesn't mess the CSS up too much, or even at all for most content - **if** you
+don't get hyperspecific with your CSS selectors and structure your templates
+well.) Your block and field are wrapped in a `div`, any CSS for your templates
+should keep this in mind. ### Rendered editable output HTML ```html {% load
+fedit %}
 % if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
 { edit_url }}">
-{% for button in buttons %} {{ button }} {# Edit button; more buttons MIGHT
-possibly be added in the future. #} {% endfor %}
-{{ content|safe }}
+{% for button in buttons %} {{ button }} {% endfor %}
+{% render_adapter adapter %}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.5.2/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.3rc1/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
 wagtail_fedit/templates/wagtail_fedit/_hook_output.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
```

