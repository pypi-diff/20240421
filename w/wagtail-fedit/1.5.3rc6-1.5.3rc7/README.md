# Comparing `tmp/wagtail_fedit-1.5.3rc6.tar.gz` & `tmp/wagtail_fedit-1.5.3rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.3rc6.tar", last modified: Sun Apr 21 02:17:38 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.3rc7.tar", last modified: Sun Apr 21 02:27:45 2024, max compression
```

## Comparing `wagtail_fedit-1.5.3rc6.tar` & `wagtail_fedit-1.5.3rc7.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.433426 wagtail_fedit-1.5.3rc6/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc6/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc6/MANIFEST.in
--rw-rw-rw-   0        0        0    20306 2024-04-21 02:17:38.434943 wagtail_fedit-1.5.3rc6/PKG-INFO
--rw-rw-rw-   0        0        0    19105 2024-04-21 00:53:02.000000 wagtail_fedit-1.5.3rc6/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc6/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-04-21 02:17:38.453937 wagtail_fedit-1.5.3rc6/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.154449 wagtail_fedit-1.5.3rc6/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.197237 wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    10463 2024-04-21 01:05:15.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.202815 wagtail_fedit-1.5.3rc6/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3071 2024-04-21 02:15:33.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.043096 wagtail_fedit-1.5.3rc6/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.044090 wagtail_fedit-1.5.3rc6/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.202815 wagtail_fedit-1.5.3rc6/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.211075 wagtail_fedit-1.5.3rc6/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.214718 wagtail_fedit-1.5.3rc6/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0      973 2024-04-21 00:46:27.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.047464 wagtail_fedit-1.5.3rc6/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.047464 wagtail_fedit-1.5.3rc6/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.222331 wagtail_fedit-1.5.3rc6/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.224331 wagtail_fedit-1.5.3rc6/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.110838 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.226485 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.229489 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.234316 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.250892 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      566 2024-04-21 00:09:10.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.264800 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.268375 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.268375 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.275416 wagtail_fedit-1.5.3rc6/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.281403 wagtail_fedit-1.5.3rc6/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    10817 2024-04-21 01:26:50.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     7961 2024-04-21 01:25:52.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.285297 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.296108 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.301418 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.321329 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    14761 2024-04-21 01:30:53.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.333988 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.343082 wagtail_fedit-1.5.3rc6/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6551 2024-04-21 00:08:49.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.420733 wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2378 2024-04-21 02:17:05.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-21 02:17:38.182001 wagtail_fedit-1.5.3rc6/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    20306 2024-04-21 02:17:37.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4038 2024-04-21 02:17:38.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 02:17:37.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-21 02:17:37.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 02:17:37.000000 wagtail_fedit-1.5.3rc6/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.761746 wagtail_fedit-1.5.3rc7/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc7/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc7/MANIFEST.in
+-rw-rw-rw-   0        0        0    20684 2024-04-21 02:27:45.763753 wagtail_fedit-1.5.3rc7/PKG-INFO
+-rw-rw-rw-   0        0        0    19483 2024-04-21 02:27:07.000000 wagtail_fedit-1.5.3rc7/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc7/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-04-21 02:27:45.786445 wagtail_fedit-1.5.3rc7/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.423756 wagtail_fedit-1.5.3rc7/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.503600 wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    10463 2024-04-21 01:05:15.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1810 2024-04-18 15:38:03.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.512413 wagtail_fedit-1.5.3rc7/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3110 2024-04-21 02:24:44.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.355947 wagtail_fedit-1.5.3rc7/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.356950 wagtail_fedit-1.5.3rc7/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.518991 wagtail_fedit-1.5.3rc7/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.525525 wagtail_fedit-1.5.3rc7/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.527953 wagtail_fedit-1.5.3rc7/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0      973 2024-04-21 00:46:27.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.363463 wagtail_fedit-1.5.3rc7/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.364477 wagtail_fedit-1.5.3rc7/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.537582 wagtail_fedit-1.5.3rc7/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.541584 wagtail_fedit-1.5.3rc7/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.366477 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.545106 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.548118 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.555168 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.578855 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      566 2024-04-21 00:09:10.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.594963 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.602597 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.608087 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.614631 wagtail_fedit-1.5.3rc7/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.620649 wagtail_fedit-1.5.3rc7/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10817 2024-04-21 01:26:50.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7961 2024-04-21 01:25:52.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.626860 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.639457 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.645988 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.677782 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    14761 2024-04-21 01:30:53.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.697770 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.718413 wagtail_fedit-1.5.3rc7/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6551 2024-04-21 00:08:49.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.757760 wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2378 2024-04-21 02:17:05.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-21 02:27:45.479470 wagtail_fedit-1.5.3rc7/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    20684 2024-04-21 02:27:45.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4038 2024-04-21 02:27:45.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 02:27:45.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-21 02:27:45.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 02:27:45.000000 wagtail_fedit-1.5.3rc7/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.3rc6/LICENSE` & `wagtail_fedit-1.5.3rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/PKG-INFO` & `wagtail_fedit-1.5.3rc7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.3rc6
+Version: 1.5.3rc7
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -47,14 +47,15 @@
 - [Adapters](#adapters)
   - [Adapters Python](#adapters-python)
   - [Adapters Javascript](#adapters-javascript)
 - [Hooks](#hooks)
   - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
   - [Register Type Renderer](#wagtail_feditregister_type_renderer)
   - [Register Field Renderer](#wagtail_feditregister_field_renderer)
+  - [Register Field Widgets](#wagtail_feditregister_field_widgets)
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
@@ -494,14 +495,26 @@
 
     # This is a custom renderer for RichText fields.
     # It will render the RichText field as a RichText block.
     renderer_map[RichTextField] =\
         lambda request, context, instance, value: richtext(value)
 ```
 
+### wagtail_fedit.register_field_widgets
+Register a custom widget for a field.
+
+Example of how this hook is used in wagtail_hooks.py:
+    
+```python
+@hooks.register(REGISTER_FIELD_WIDGETS)
+def register_field_widgets(widgets):
+    widgets[RichTextField] = AdminRichTextField
+    return widgets
+```
+
 ### wagtail_fedit.exclude_related_forms
 
 Exclude the given model type from the related forms.
 This is used internally to exclude the Page, Image, and Document models from the related forms.
 This way; the user will have the actual widget for the field instead of the related form.
 
 Example of how this hook is called and how it is used internally:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc6 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc7 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -20,15 +20,16 @@
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
 (#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters](#adapters) -
 [Adapters Python](#adapters-python) - [Adapters Javascript](#adapters-
 javascript) - [Hooks](#hooks) - [Construct Adapter Toolbar]
 (#wagtail_feditconstruct_adapter_toolbar) - [Register Type Renderer]
 (#wagtail_feditregister_type_renderer) - [Register Field Renderer]
-(#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
+(#wagtail_feditregister_field_renderer) - [Register Field Widgets]
+(#wagtail_feditregister_field_widgets) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
 [Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
 Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
 (#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
@@ -201,19 +202,23 @@
 (request): return [ format_html( '
 ', static('js/custom.js') ), ] `` ### wagtail_fedit.register_field_renderer
 Register a custom renderer for a field. Example of how this type of renderer is
 used in wagtail_hooks/renderers.py: ```python @hooks.register
 (REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
 custom renderer for RichText fields. # It will render the RichText field as a
 RichText block. renderer_map[RichTextField] =\ lambda request, context,
-instance, value: richtext(value) ``` ### wagtail_fedit.exclude_related_forms
-Exclude the given model type from the related forms. This is used internally to
-exclude the Page, Image, and Document models from the related forms. This way;
-the user will have the actual widget for the field instead of the related form.
-Example of how this hook is called and how it is used internally: ```python def
+instance, value: richtext(value) ``` ### wagtail_fedit.register_field_widgets
+Register a custom widget for a field. Example of how this hook is used in
+wagtail_hooks.py: ```python @hooks.register(REGISTER_FIELD_WIDGETS) def
+register_field_widgets(widgets): widgets[RichTextField] = AdminRichTextField
+return widgets ``` ### wagtail_fedit.exclude_related_forms Exclude the given
+model type from the related forms. This is used internally to exclude the Page,
+Image, and Document models from the related forms. This way; the user will have
+the actual widget for the field instead of the related form. Example of how
+this hook is called and how it is used internally: ```python def
 use_related_form(field: models.Field) -> bool: for hook in hooks.get_hooks
 (EXCLUDE_FROM_RELATED_FORMS): if hook(field): return False return True
 @hooks.register(EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field):
 if field.related_model in [Page, Image, Document]: return True return False ```
 ### wagtail_fedit.action_menu_item_is_shown Decide if the action menu item
 should be shown for the given instance. Return None if you cannot decide, False
 if you want to hide the item, and True if you want to show the item. Example of
```

### Comparing `wagtail_fedit-1.5.3rc6/README.md` & `wagtail_fedit-1.5.3rc7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 - [Adapters](#adapters)
   - [Adapters Python](#adapters-python)
   - [Adapters Javascript](#adapters-javascript)
 - [Hooks](#hooks)
   - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
   - [Register Type Renderer](#wagtail_feditregister_type_renderer)
   - [Register Field Renderer](#wagtail_feditregister_field_renderer)
+  - [Register Field Widgets](#wagtail_feditregister_field_widgets)
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
@@ -464,14 +465,26 @@
 
     # This is a custom renderer for RichText fields.
     # It will render the RichText field as a RichText block.
     renderer_map[RichTextField] =\
         lambda request, context, instance, value: richtext(value)
 ```
 
+### wagtail_fedit.register_field_widgets
+Register a custom widget for a field.
+
+Example of how this hook is used in wagtail_hooks.py:
+    
+```python
+@hooks.register(REGISTER_FIELD_WIDGETS)
+def register_field_widgets(widgets):
+    widgets[RichTextField] = AdminRichTextField
+    return widgets
+```
+
 ### wagtail_fedit.exclude_related_forms
 
 Exclude the given model type from the related forms.
 This is used internally to exclude the Page, Image, and Document models from the related forms.
 This way; the user will have the actual widget for the field instead of the related form.
 
 Example of how this hook is called and how it is used internally:
```

#### html2text {}

```diff
@@ -5,15 +5,16 @@
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
 (#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters](#adapters) -
 [Adapters Python](#adapters-python) - [Adapters Javascript](#adapters-
 javascript) - [Hooks](#hooks) - [Construct Adapter Toolbar]
 (#wagtail_feditconstruct_adapter_toolbar) - [Register Type Renderer]
 (#wagtail_feditregister_type_renderer) - [Register Field Renderer]
-(#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
+(#wagtail_feditregister_field_renderer) - [Register Field Widgets]
+(#wagtail_feditregister_field_widgets) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
 [Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
 Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
 (#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
@@ -186,19 +187,23 @@
 (request): return [ format_html( '
 ', static('js/custom.js') ), ] `` ### wagtail_fedit.register_field_renderer
 Register a custom renderer for a field. Example of how this type of renderer is
 used in wagtail_hooks/renderers.py: ```python @hooks.register
 (REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
 custom renderer for RichText fields. # It will render the RichText field as a
 RichText block. renderer_map[RichTextField] =\ lambda request, context,
-instance, value: richtext(value) ``` ### wagtail_fedit.exclude_related_forms
-Exclude the given model type from the related forms. This is used internally to
-exclude the Page, Image, and Document models from the related forms. This way;
-the user will have the actual widget for the field instead of the related form.
-Example of how this hook is called and how it is used internally: ```python def
+instance, value: richtext(value) ``` ### wagtail_fedit.register_field_widgets
+Register a custom widget for a field. Example of how this hook is used in
+wagtail_hooks.py: ```python @hooks.register(REGISTER_FIELD_WIDGETS) def
+register_field_widgets(widgets): widgets[RichTextField] = AdminRichTextField
+return widgets ``` ### wagtail_fedit.exclude_related_forms Exclude the given
+model type from the related forms. This is used internally to exclude the Page,
+Image, and Document models from the related forms. This way; the user will have
+the actual widget for the field instead of the related form. Example of how
+this hook is called and how it is used internally: ```python def
 use_related_form(field: models.Field) -> bool: for hook in hooks.get_hooks
 (EXCLUDE_FROM_RELATED_FORMS): if hook(field): return False return True
 @hooks.register(EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field):
 if field.related_model in [Page, Image, Document]: return True return False ```
 ### wagtail_fedit.action_menu_item_is_shown Decide if the action menu item
 should be shown for the given instance. Return None if you cannot decide, False
 if you want to hide the item, and True if you want to show the item. Example of
```

### Comparing `wagtail_fedit-1.5.3rc6/setup.cfg` & `wagtail_fedit-1.5.3rc7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3372 6336 0d0a 6465 7363 7269 7074 696f  3rc6..descriptio
+00000030: 3372 6337 0d0a 6465 7363 7269 7074 696f  3rc7..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/block.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/forms/fields.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,32 +44,23 @@
 
     if widget is None:
         pass
 
     return widget
 
 
-class PossiblePreviewForm(WagtailAdminModelForm):
+class PossibleRevisionForm(WagtailAdminModelForm):
     """
     A form that can save a revision if the model is a RevisionMixin.
     Otherwise resorts to the default save method; this saves the (live) instance.
     """
     def __init__(self, *args, request = None, **kwargs):
         self.request = request
         super().__init__(*args, **kwargs)
 
-        for key, field in self.fields.items():
-            meta_field = self._meta.model._meta.get_field(key)
-            widget = get_widget_for_field(meta_field)
-            if widget:
-                if not isinstance(field.widget, widget):
-                    field.widget = widget()
-                else:
-                    field.widget = widget
-
     def save(self, commit=True):
         instance = super().save(commit=False)
         if commit:
             instance = save_possible_revision(instance, self.request)
         return instance
 
 def save_possible_revision(instance: models.Model, request: HttpRequest, **kwargs) -> models.Model:
@@ -83,25 +74,34 @@
         )
         instance = instance.as_object()
     else:
         instance.save()
 
     return instance
 
-def get_form_class_for_fields(form_model: models.Model, form_fields: list[str]) -> Type[PossiblePreviewForm]:
+def get_form_class_for_fields(form_model: models.Model, form_fields: list[str]) -> Type[PossibleRevisionForm]:
     """
     Return a form class for a model with specific fields.
-    This is similar to django's modelform_factory.
+    This is similar to django's modelform_factory, but with the added benefit of using the custom widgets.
+    It also keeps the revision functionality in mind.
     """
 
     if hasattr(form_model, "get_fedit_form"):
         return form_model.get_fedit_form(form_fields)
     
-    # if form_fields == "__all__" or form_fields == ["__all__"]:
-    #     form_fields = [f.name for f in form_model._meta.fields]
+    if form_fields == "__all__" or tuple(form_fields) == ("__all__", ):
+        form_fields = [f.name for f in form_model._meta.fields]
     
-    class Form(PossiblePreviewForm):
+    form_widgets = {}
+    for field_name in form_fields:
+        field = form_model._meta.get_field(field_name)
+        widget = get_widget_for_field(field)
+        if widget:
+            form_widgets[field_name] = widget
+
+    class RevisionForm(PossibleRevisionForm):
         class Meta:
             model = form_model
             fields = form_fields
+            widgets = form_widgets
 
-    return Form
+    return RevisionForm
```

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/models.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/views/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.3rc7/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.3rc7/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.3rc6
+Version: 1.5.3rc7
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -47,14 +47,15 @@
 - [Adapters](#adapters)
   - [Adapters Python](#adapters-python)
   - [Adapters Javascript](#adapters-javascript)
 - [Hooks](#hooks)
   - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
   - [Register Type Renderer](#wagtail_feditregister_type_renderer)
   - [Register Field Renderer](#wagtail_feditregister_field_renderer)
+  - [Register Field Widgets](#wagtail_feditregister_field_widgets)
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
@@ -494,14 +495,26 @@
 
     # This is a custom renderer for RichText fields.
     # It will render the RichText field as a RichText block.
     renderer_map[RichTextField] =\
         lambda request, context, instance, value: richtext(value)
 ```
 
+### wagtail_fedit.register_field_widgets
+Register a custom widget for a field.
+
+Example of how this hook is used in wagtail_hooks.py:
+    
+```python
+@hooks.register(REGISTER_FIELD_WIDGETS)
+def register_field_widgets(widgets):
+    widgets[RichTextField] = AdminRichTextField
+    return widgets
+```
+
 ### wagtail_fedit.exclude_related_forms
 
 Exclude the given model type from the related forms.
 This is used internally to exclude the Page, Image, and Document models from the related forms.
 This way; the user will have the actual widget for the field instead of the related form.
 
 Example of how this hook is called and how it is used internally:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.3rc6 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.3rc7 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -20,15 +20,16 @@
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
 (#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters](#adapters) -
 [Adapters Python](#adapters-python) - [Adapters Javascript](#adapters-
 javascript) - [Hooks](#hooks) - [Construct Adapter Toolbar]
 (#wagtail_feditconstruct_adapter_toolbar) - [Register Type Renderer]
 (#wagtail_feditregister_type_renderer) - [Register Field Renderer]
-(#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
+(#wagtail_feditregister_field_renderer) - [Register Field Widgets]
+(#wagtail_feditregister_field_widgets) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
 [Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
 Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
 (#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
@@ -201,19 +202,23 @@
 (request): return [ format_html( '
 ', static('js/custom.js') ), ] `` ### wagtail_fedit.register_field_renderer
 Register a custom renderer for a field. Example of how this type of renderer is
 used in wagtail_hooks/renderers.py: ```python @hooks.register
 (REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
 custom renderer for RichText fields. # It will render the RichText field as a
 RichText block. renderer_map[RichTextField] =\ lambda request, context,
-instance, value: richtext(value) ``` ### wagtail_fedit.exclude_related_forms
-Exclude the given model type from the related forms. This is used internally to
-exclude the Page, Image, and Document models from the related forms. This way;
-the user will have the actual widget for the field instead of the related form.
-Example of how this hook is called and how it is used internally: ```python def
+instance, value: richtext(value) ``` ### wagtail_fedit.register_field_widgets
+Register a custom widget for a field. Example of how this hook is used in
+wagtail_hooks.py: ```python @hooks.register(REGISTER_FIELD_WIDGETS) def
+register_field_widgets(widgets): widgets[RichTextField] = AdminRichTextField
+return widgets ``` ### wagtail_fedit.exclude_related_forms Exclude the given
+model type from the related forms. This is used internally to exclude the Page,
+Image, and Document models from the related forms. This way; the user will have
+the actual widget for the field instead of the related form. Example of how
+this hook is called and how it is used internally: ```python def
 use_related_form(field: models.Field) -> bool: for hook in hooks.get_hooks
 (EXCLUDE_FROM_RELATED_FORMS): if hook(field): return False return True
 @hooks.register(EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field):
 if field.related_model in [Page, Image, Document]: return True return False ```
 ### wagtail_fedit.action_menu_item_is_shown Decide if the action menu item
 should be shown for the given instance. Return None if you cannot decide, False
 if you want to hide the item, and True if you want to show the item. Example of
```

### Comparing `wagtail_fedit-1.5.3rc6/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.3rc7/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

