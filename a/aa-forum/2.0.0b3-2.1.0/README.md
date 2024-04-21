# Comparing `tmp/aa_forum-2.0.0b3.tar.gz` & `tmp/aa_forum-2.1.0.tar.gz`

## Comparing `aa_forum-2.0.0b3.tar` & `aa_forum-2.1.0.tar`

### file list

```diff
@@ -1,195 +1,204 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/__init__.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/admin.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/app_settings.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/apps.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/auth_hooks.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/constants.py
--rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/forms.py
--rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/managers.py
--rw-r--r--   0        0        0    30320 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/models.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/signals.py
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/urls.py
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/helper/discord_messages.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/helper/eve_images.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/helper/forms.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/helper/pagination.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/helper/text.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/helper/user.py
--rw-r--r--   0        0        0    38210 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/django.pot
--rw-r--r--   0        0        0    28064 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    50493 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43600 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    38543 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    38389 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    38261 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    38950 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    34195 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    56613 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39141 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    38534 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0001_initial.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0002_default_settings.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0003_board_discord_webhook.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0004_board_use_webhook_for_replies.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0005_announcement_boards.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0006_reset_default_settings.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0007_change_settings_to_singleton.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0008_populate_default_settings.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0009_add_related_names.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0010_better_setting_names.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0011_userprofile.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0012_personal_messages.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0014_userprofile_discord_dm_on_new_personal_message.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0016_fix_quotation_marks.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/migrations/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/scripts/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/scripts/drop_tables.sql
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/scripts/fake_messages.py
--rw-r--r--   0        0        0    13044 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/css/aa-forum.css
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/css/aa-forum.min.css
--rw-r--r--   0        0        0    15567 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/css/aa-forum.min.css.map
--rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-admin.js
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js.map
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md
--rw-r--r--   0        0        0    18931 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css
--rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css
--rw-r--r--   0        0        0   167106 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js
--rw-r--r--   0        0        0    76775 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js
--rw-r--r--   0        0        0   156955 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js
--rw-r--r--   0        0        0    73170 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE
--rw-r--r--   0        0        0    34395 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css
--rw-r--r--   0        0        0    29738 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css
--rw-r--r--   0        0        0    38867 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map
--rw-r--r--   0        0        0    34280 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js
--rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
--rw-r--r--   0        0        0     9711 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/base.html
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/aa-forum-admin-js.html
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/aa-forum-ckeditor-js.html
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/aa-forum-css.html
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/aa-forum-dashboard-widgets-js.html
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/aa-forum-oembed-js.html
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/aa-forum-personal-messages-js.html
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/ckeditor-js.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/ckeditor5-css.html
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/ckeditor5-js.html
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/select2-css.html
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/select2-js.html
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/sumoselect-css.html
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/sumoselect-js.html
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/administration/delete-board.html
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/administration/delete-category.html
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/breadcrumb.html
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/menu.html
--rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/administration/board-loop.html
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/administration/categories.html
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/administration/category-loop.html
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/administration/new-category.html
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/administration/settings-form.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/form/required-field-hint.html
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/forum-index.html
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/board/board-index.html
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/board/board.html
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/board/no-access.html
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/board/pagination.html
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/board/topic.html
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/message.html
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/reply.html
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/menu/menu-admin.html
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/menu/menu-user.html
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/profile/form.html
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/search/pagination.html
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/search/search-form.html
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/search/search-result.html
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/widgets/unread-topics.html
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/administration/forum-settings.html
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/board.html
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/index.html
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/modify-message.html
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/modify-topic.html
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/new-topic.html
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/topic.html
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/unread-topics.html
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/personal-messages/inbox.html
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/personal-messages/new-message.html
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/profile/index.html
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/search/results.html
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templatetags/__init__.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/templatetags/aa_forum.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/test_app_settings.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/test_auth_hooks.py
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/test_helpers.py
--rw-r--r--   0        0        0    70535 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/test_integration.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/test_managers.py
--rw-r--r--   0        0        0    36507 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/test_models.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/test_signals.py
--rw-r--r--   0        0        0    29381 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/test_templatetags.py
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/test_views_admin.py
--rw-r--r--   0        0        0    51417 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/test_views_forum.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/tests/utils.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/views/__init__.py
--rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/views/admin.py
--rw-r--r--   0        0        0    43825 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/views/forum.py
--rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/views/personal_messages.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/views/profile.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/views/search.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/aa_forum/views/widgets.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/LICENSE
--rw-r--r--   0        0        0    20328 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/README.md
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/pyproject.toml
--rw-r--r--   0        0        0    63024 2020-02-02 00:00:00.000000 aa_forum-2.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/__init__.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/admin.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/app_settings.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/apps.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/auth_hooks.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/constants.py
+-rw-r--r--   0        0        0    19631 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/forms.py
+-rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/managers.py
+-rw-r--r--   0        0        0    30320 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/models.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/signals.py
+-rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/urls.py
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/discord_messages.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/eve_images.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/forms.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/pagination.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/text.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/helper/user.py
+-rw-r--r--   0        0        0    39481 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/django.pot
+-rw-r--r--   0        0        0    39556 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    28897 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    52203 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    44946 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40664 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39660 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39532 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41205 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    39473 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39830 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    58050 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    39551 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40498 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39849 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0002_default_settings.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0003_board_discord_webhook.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0004_board_use_webhook_for_replies.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0005_announcement_boards.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0006_reset_default_settings.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0007_change_settings_to_singleton.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0008_populate_default_settings.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0009_add_related_names.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0010_better_setting_names.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0011_userprofile.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0012_personal_messages.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0014_userprofile_discord_dm_on_new_personal_message.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0016_fix_quotation_marks.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/migrations/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/scripts/__init__.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/scripts/drop_tables.sql
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/scripts/fake_messages.py
+-rw-r--r--   0        0        0    13044 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.css
+-rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.min.css
+-rw-r--r--   0        0        0    15567 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.min.css.map
+-rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.js
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.js
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js.map
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js.map
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md
+-rw-r--r--   0        0        0    18931 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css
+-rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css
+-rw-r--r--   0        0        0   167106 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js
+-rw-r--r--   0        0        0    76775 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js
+-rw-r--r--   0        0        0   156955 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js
+-rw-r--r--   0        0        0    73170 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE
+-rw-r--r--   0        0        0    34395 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css
+-rw-r--r--   0        0        0    29738 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0        0        0    38867 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map
+-rw-r--r--   0        0        0    34280 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js
+-rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
+-rw-r--r--   0        0        0     9711 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/base.html
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-admin-js.html
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-bootstrap-js.html
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-ckeditor-js.html
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-css.html
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-dashboard-widgets-js.html
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-oembed-js.html
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/aa-forum-personal-messages-js.html
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/ckeditor-js.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/ckeditor5-css.html
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/ckeditor5-js.html
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/select2-css.html
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/select2-js.html
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/sumoselect-css.html
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/sumoselect-js.html
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/administration/delete-board.html
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/administration/delete-category.html
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/breadcrumb.html
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/menu.html
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/board-loop.html
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/categories.html
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/category-loop.html
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/new-category.html
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/settings-form.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/form/required-field-hint.html
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/forum-index.html
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/board-index.html
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/board.html
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/no-access.html
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/pagination.html
+-rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/topic.html
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/message.html
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/reply.html
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/menu/menu-admin.html
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/menu/menu-user.html
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/profile/form.html
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/search/pagination.html
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/search/search-form.html
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/search/search-result.html
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/widgets/unread-topics.html
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/administration/forum-settings.html
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/board.html
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/index.html
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/modify-message.html
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/modify-topic.html
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/new-topic.html
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/topic.html
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/unread-topics.html
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/inbox.html
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/new-message.html
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/profile/index.html
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/search/results.html
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templatetags/__init__.py
+-rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/templatetags/aa_forum.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_app_settings.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_helpers.py
+-rw-r--r--   0        0        0    74867 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_integration.py
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_managers.py
+-rw-r--r--   0        0        0    36507 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_models.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_signals.py
+-rw-r--r--   0        0        0    29431 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_templatetags.py
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_views_admin.py
+-rw-r--r--   0        0        0    51417 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/test_views_forum.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/tests/utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/__init__.py
+-rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/admin.py
+-rw-r--r--   0        0        0    44779 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/forum.py
+-rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/personal_messages.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/profile.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/search.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_forum-2.1.0/aa_forum/views/widgets.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_forum-2.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_forum-2.1.0/LICENSE
+-rw-r--r--   0        0        0    20310 2020-02-02 00:00:00.000000 aa_forum-2.1.0/README.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 aa_forum-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    63005 2020-02-02 00:00:00.000000 aa_forum-2.1.0/PKG-INFO
```

### Comparing `aa_forum-2.0.0b3/aa_forum/admin.py` & `aa_forum-2.1.0/aa_forum/admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/app_settings.py` & `aa_forum-2.1.0/aa_forum/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/apps.py` & `aa_forum-2.1.0/aa_forum/apps.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/auth_hooks.py` & `aa_forum-2.1.0/aa_forum/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/constants.py` & `aa_forum-2.1.0/aa_forum/constants.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/forms.py` & `aa_forum-2.1.0/aa_forum/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,14 +353,30 @@
 
 
 class EditMessageForm(ModelForm):
     """
     Edit message form
     """
 
+    close_topic = forms.BooleanField(
+        required=False,
+        label=_("Close topic"),
+        help_text=_(
+            "If checked, this topic will be closed after posting this message."
+        ),
+    )
+
+    reopen_topic = forms.BooleanField(
+        required=False,
+        label=_("Reopen topic"),
+        help_text=_(
+            "If checked, this topic will be reopened after posting this message."
+        ),
+    )
+
     def __init__(self, *args, **kwargs):
         """
         When form is initialized
 
         :param args:
         :type args:
         :param kwargs:
@@ -374,15 +390,15 @@
 
     class Meta:  # pylint: disable=too-few-public-methods
         """
         Meta definitions
         """
 
         model = Message
-        fields = ["message"]
+        fields = ["message", "close_topic", "reopen_topic"]
         widgets = {
             "message": CKEditor5Widget(
                 config_name="extends",
                 attrs={
                     "class": "aa-forum-ckeditor django_ckeditor_5",
                     "rows": 10,
                     "cols": 20,
```

### Comparing `aa_forum-2.0.0b3/aa_forum/managers.py` & `aa_forum-2.1.0/aa_forum/managers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/models.py` & `aa_forum-2.1.0/aa_forum/models.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/signals.py` & `aa_forum-2.1.0/aa_forum/signals.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/urls.py` & `aa_forum-2.1.0/aa_forum/urls.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/helper/discord_messages.py` & `aa_forum-2.1.0/aa_forum/helper/discord_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/helper/eve_images.py` & `aa_forum-2.1.0/aa_forum/helper/eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/helper/forms.py` & `aa_forum-2.1.0/aa_forum/helper/forms.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/helper/pagination.py` & `aa_forum-2.1.0/aa_forum/helper/pagination.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/helper/text.py` & `aa_forum-2.1.0/aa_forum/helper/text.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/helper/user.py` & `aa_forum-2.1.0/aa_forum/helper/user.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/django.pot` & `aa_forum-2.1.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,588 +1,630 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
-#, fuzzy
+# Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 18:29+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"PO-Revision-Date: 2024-04-01 09:51+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/pl/>\n"
+"Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=INTEGER; plural=EXPRESSION;\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 5.4.3\n"
 
-#: aa_forum/__init__.py:12 aa_forum/templates/aa_forum/base.html:5
-#: aa_forum/templates/aa_forum/partials/menu.html:14
+#: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
+#: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
-#: aa_forum/templates/aa_forum/view/forum/board.html:5
-#: aa_forum/templates/aa_forum/view/forum/index.html:6
+#: aa_forum/templates/aa_forum/view/forum/board.html:6
+#: aa_forum/templates/aa_forum/view/forum/index.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:8
-#: aa_forum/templates/aa_forum/view/forum/topic.html:5
+#: aa_forum/templates/aa_forum/view/forum/topic.html:6
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:7
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:9
-#: aa_forum/templates/aa_forum/view/profile/index.html:9
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
 msgstr ""
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr ""
 
-#: aa_forum/forms.py:40
+#: aa_forum/forms.py:42
 msgid "This field is mandatory"
-msgstr ""
+msgstr "To pole jest wymagane"
 
-#: aa_forum/forms.py:91 aa_forum/forms.py:93 aa_forum/forms.py:124
-#: aa_forum/forms.py:126 aa_forum/forms.py:502
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:26
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:26
+#: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
+#: aa_forum/forms.py:171 aa_forum/forms.py:616
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr ""
 
-#: aa_forum/forms.py:102 aa_forum/forms.py:321 aa_forum/forms.py:512
-#: aa_forum/forms.py:558
-msgid "Message"
+#: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
+#: aa_forum/forms.py:730
+msgid "You have forgotten the message!"
 msgstr ""
 
-#: aa_forum/forms.py:145 aa_forum/forms.py:183 aa_forum/forms.py:204
+#: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
 msgstr ""
 
-#: aa_forum/forms.py:147 aa_forum/forms.py:185
+#: aa_forum/forms.py:192 aa_forum/forms.py:230
 msgid "Category name"
 msgstr ""
 
-#: aa_forum/forms.py:151 aa_forum/forms.py:162
+#: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
 msgstr ""
 
-#: aa_forum/forms.py:153
+#: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
 
-#: aa_forum/forms.py:206
+#: aa_forum/forms.py:251
 msgid "Board name"
 msgstr ""
 
-#: aa_forum/forms.py:210
+#: aa_forum/forms.py:255
 msgid "Description"
 msgstr ""
 
-#: aa_forum/forms.py:216
+#: aa_forum/forms.py:261
 msgid "Board description (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:222
+#: aa_forum/forms.py:267
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_forum/forms.py:224
+#: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:232
+#: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:234
+#: aa_forum/forms.py:279
 msgid ""
 "Discord webhook URL for the channel to post about new topics in this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:247
+#: aa_forum/forms.py:292
 msgid "Use this Discord webhook for replies as well?"
 msgstr ""
 
-#: aa_forum/forms.py:249
+#: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
 msgstr ""
 
-#: aa_forum/forms.py:257
+#: aa_forum/forms.py:302
 msgid "Mark board as \"Announcement Board\""
 msgstr ""
 
-#: aa_forum/forms.py:259
+#: aa_forum/forms.py:304
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. This setting will "
 "not be inherited to child boards. (Default: NO)"
 msgstr ""
 
-#: aa_forum/forms.py:267
+#: aa_forum/forms.py:312
 msgid "Start topic restrictions for \"Announcement Boards\""
 msgstr ""
 
-#: aa_forum/forms.py:269
+#: aa_forum/forms.py:314
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
 msgstr ""
 
-#: aa_forum/forms.py:354
-msgid "Signature"
+#: aa_forum/forms.py:362
+msgid "Close topic"
 msgstr ""
 
-#: aa_forum/forms.py:355
-msgid "Your signature will appear below your posts."
+#: aa_forum/forms.py:364
+msgid "If checked, this topic will be closed after posting this message."
+msgstr ""
+
+#: aa_forum/forms.py:370
+msgid "Reopen topic"
+msgstr ""
+
+#: aa_forum/forms.py:372
+msgid "If checked, this topic will be reopened after posting this message."
 msgstr ""
 
-#: aa_forum/forms.py:359
+#: aa_forum/forms.py:409 aa_forum/forms.py:652 aa_forum/forms.py:717
+msgid "Message"
+msgstr ""
+
+#: aa_forum/forms.py:446
 msgid "Website title"
 msgstr ""
 
-#: aa_forum/forms.py:361
+#: aa_forum/forms.py:448
 msgid "e.g.: My Homepage"
 msgstr ""
 
-#: aa_forum/forms.py:362
+#: aa_forum/forms.py:449
 msgid "Your website's title."
 msgstr ""
 
-#: aa_forum/forms.py:366
+#: aa_forum/forms.py:453
 msgid "Website URL"
 msgstr ""
 
-#: aa_forum/forms.py:370
+#: aa_forum/forms.py:457
 msgid ""
 "Your website's URL. (Don't forget to also set a title for your website, "
 "otherwise this field will be ignored.)"
 msgstr ""
 
-#: aa_forum/forms.py:376
+#: aa_forum/forms.py:463
 msgid "PM me on Discord when I get a new personal message"
 msgstr ""
 
-#: aa_forum/forms.py:378
+#: aa_forum/forms.py:466
 msgid ""
 "Information: There is currently no module installed that can handle Discord "
 "direct messages. Have a chat with your IT guys to remedy this."
 msgstr ""
 
-#: aa_forum/forms.py:419
+#: aa_forum/forms.py:475
+msgid "Show unread topics as widget on the dashboard"
+msgstr ""
+
+#: aa_forum/forms.py:478
+msgid ""
+"Activating this setting will ad a widget to your dashboard that shows unread "
+"topics in the forum."
+msgstr ""
+
+#: aa_forum/forms.py:507
+msgid "Signature"
+msgstr ""
+
+#: aa_forum/forms.py:508
+msgid "Your signature will appear below your posts."
+msgstr ""
+
+#: aa_forum/forms.py:532
 msgid ""
 "Ensure your signature has at most {max_signature_length} characters. "
 "(Currently: {len(signature)})"
 msgstr ""
 
-#: aa_forum/forms.py:440
+#: aa_forum/forms.py:554
 msgid "This is not a valid URL"
 msgstr ""
 
-#: aa_forum/forms.py:456
+#: aa_forum/forms.py:570
 msgid ""
 "How many messages per page should be displayed in a forum topic? (Default: "
 "15)"
 msgstr ""
 
-#: aa_forum/forms.py:466
+#: aa_forum/forms.py:580
 msgid ""
 "How many topics per page should be displayed in a forum category? (Default: "
 "10)"
 msgstr ""
 
-#: aa_forum/forms.py:476
+#: aa_forum/forms.py:590
 msgid ""
 "How long (Number of characters) is a user's signature allowed to be? "
 "(Default: 750)"
 msgstr ""
 
-#: aa_forum/forms.py:498
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:22
+#: aa_forum/forms.py:612
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:21
 msgid "Recipient"
 msgstr ""
 
-#: aa_forum/forms.py:504
+#: aa_forum/forms.py:618
 msgid "Hello there …"
 msgstr ""
 
-#: aa_forum/models.py:127
+#: aa_forum/models.py:139
 msgid "AA-Forum"
 msgstr ""
 
-#: aa_forum/models.py:131
+#: aa_forum/models.py:143
 msgid "Can access the AA-Forum module"
 msgstr ""
 
-#: aa_forum/models.py:134
+#: aa_forum/models.py:146
 msgid "Can manage the AA-Forum module (Category, topics and messages)"
 msgstr ""
 
-#: aa_forum/models.py:177
+#: aa_forum/models.py:193
 msgid "category"
 msgstr ""
 
-#: aa_forum/models.py:178
+#: aa_forum/models.py:194
 msgid "categories"
 msgstr ""
 
-#: aa_forum/models.py:222
+#: aa_forum/models.py:248
 msgid ""
 "Use this Discord webhook for replies as well? When activated every reply to "
 "any topic in this board will be posted to the defined Discord channel. "
 "(Child boards are excluded) Chose wisely! (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:240
+#: aa_forum/models.py:266
 msgid ""
 "User in at least one of these groups have access to this board. If no groups "
 "are selected, everyone with access to the forum has also access to this "
 "board."
 msgstr ""
 
-#: aa_forum/models.py:248
+#: aa_forum/models.py:274
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:259
+#: aa_forum/models.py:285
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so."
 msgstr ""
 
-#: aa_forum/models.py:295
+#: aa_forum/models.py:321
 msgid "board"
 msgstr ""
 
-#: aa_forum/models.py:296
+#: aa_forum/models.py:322
 msgid "boards"
 msgstr ""
 
-#: aa_forum/models.py:367
+#: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:578
+#: aa_forum/models.py:625
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:579
+#: aa_forum/models.py:626
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:736
+#: aa_forum/models.py:805
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:737
+#: aa_forum/models.py:806
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:872
+#: aa_forum/models.py:948
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:873
+#: aa_forum/models.py:949
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:920
+#: aa_forum/models.py:1003
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:921
+#: aa_forum/models.py:1004
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:922
+#: aa_forum/models.py:1005
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:927
+#: aa_forum/models.py:1010
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:932
+#: aa_forum/models.py:1015
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:937
+#: aa_forum/models.py:1020
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:1031
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:1032
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:952
+#: aa_forum/models.py:1042
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:16
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:978
+#: aa_forum/models.py:1069
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:979
+#: aa_forum/models.py:1070
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:982
+#: aa_forum/models.py:1080
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:30
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:7
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:38
+#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:8
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:56
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:73
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:59
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:75
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:69
 msgid "Delete message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:13
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:8
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:23
 msgid "Delete board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
+msgid "Close"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:22
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:22
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:21
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:21
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:21
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:20
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:20
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:20
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:19
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:19
 msgid "This action cannot be undone!"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:29
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:29
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:28
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:28
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:28
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:27
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:27
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:34
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:34
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:33
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:33
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:33
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
-msgstr ""
+msgstr "Usuń"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:15
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:16
 msgid "Are you sure you want to delete this category?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:17
 msgid "This will also remove all boards, topics and messages in this category."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:13
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:39
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:84
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
 msgid "Unlock/re-open topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:16
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:42
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:88
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
 msgid "Lock/close topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
 msgid "Are you sure you want to lock/close this topic?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:3
 msgid "Change sticky state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:13
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:9
 msgid "Remove \"sticky\" state from topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:16
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:12
 msgid "Set \"sticky\" state for topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:22
 msgid "Are you sure you want to remove the sticky state from this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
 msgid ""
 "Are you sure you want to make this topic sticky, so it always shows up on "
 "top of the topic list?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:39
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:37
 msgid "Unset sticky"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:42
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:97
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
 msgid "Delete topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:19
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:17
 msgid "This will also remove all messages in this topic."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:17
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:17
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:15
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:15
 msgid "Are you sure you want to delete this message?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:16
 msgid ""
 "If this message is the original post, then the entire topic will be removed "
 "as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:16
 msgid ""
 "If this message is the beginning of a conversation, all related messages "
 "will be removed as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:9
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:11
 msgid "Edit board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:22
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:36
 msgid ""
 "Changing the name of this board does not change its URL part. This will "
 "remain the same to not break any possible links into this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:58
 msgid "Change board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:56
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:70
 msgid "New child board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:63
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:62
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:77
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:84
 msgid ""
 "New boards will be added at the bottom of the board list for this category. "
 "You can move them via drag and drop to a position of your liking."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:79
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:75
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:93
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:97
 msgid "Create board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/categories.html:6
+#: aa_forum/templates/aa_forum/partials/administration/categories.html:5
 msgid ""
 "Here you can create, modify and delete categories and boards. You also can "
 "change their order via drag and drop."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:11
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:13
 msgid "Edit category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:19
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:35
 msgid "Expand/collapse category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:31
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:53
 msgid ""
 "Changing the name of this category does not change its URL part. This will "
 "remain the same to not break any possible links into this category."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:66
 msgid "Change category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:55
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:77
 msgid "New board"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:7
 msgid "Create new category"
 msgstr ""
 
@@ -597,24 +639,25 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:35
 msgid "Create category"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:21
-#: aa_forum/templates/aa_forum/partials/profile/form.html:21
+#: aa_forum/templates/aa_forum/partials/profile/form.html:22
 msgid "Submit"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:6
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:7
 msgid "Forum index"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:27
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:49
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:51
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:6
 msgid "Modify message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:34
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:7
@@ -630,72 +673,74 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
+"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
+"tłumaczenia?"
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr ""
+msgstr "Dołącz do naszego zespołu tłumaczy!"
 
-#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:9
+#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr ""
+msgstr "Pola z gwiazdką (*) są wymagane"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:34
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:51
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
 msgid "New"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
 msgid "Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:66
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:65
 msgid "Unread"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:82
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:88
 msgid "Last post:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:86
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:25
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:96
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:26
 msgid "Re:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:103
 msgid "posted by:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:94
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:104
 msgid "posted at:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:7
+#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:8
 msgid "New topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/no-access.html:6
 msgid ""
 "You either don't have access to this board, or this board doesn't exist."
 msgstr ""
@@ -761,58 +806,58 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
 msgid "Last post"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:38
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:39
 msgid "Copy message link to clipboard"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:81
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:87
 msgid "Last modified:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:14
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:27
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:21
@@ -820,68 +865,65 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:6
 msgid "Modify topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:20
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:21
 msgid "Warning: this topic is locked! Only admins can reply."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:33
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:44
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
 msgid "Clear form"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:7
 msgid "Show all unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:7
 msgid "Administration"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:12
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:13
 msgid "Categories and boards"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:6
-#: aa_forum/templates/aa_forum/view/profile/index.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:13
+#: aa_forum/templates/aa_forum/view/profile/index.html:7
 msgid "Profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:11
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:19
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:9
 msgid "Messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:23
 msgid "Inbox"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:18
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:18
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:17
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:17
 msgid "Date"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:22
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:21
 msgid "Sender"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:62
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:63
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:57
 msgid "Read message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:87
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:93
 msgid "No personal messages"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:8
 msgid "New personal message"
 msgstr ""
 
@@ -889,326 +931,322 @@
 msgid "Send message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:8
 msgid "Reply to:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:24
+#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:23
 msgid "Send reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:30
 msgid "Sent messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:56
-msgid "Read Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:67
-msgid "Delete Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:81
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:87
 msgid "No personal messages sent"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:17
 msgid "New message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/profile/form.html:7
 msgid "User profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/search/search-form.html:7
+#: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+msgid "Forum: Unread topics"
+msgstr ""
+
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:6
 msgid "Administration (Forum settings)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:26
+#: aa_forum/templates/aa_forum/view/forum/index.html:27
 msgid "New posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:35
+#: aa_forum/templates/aa_forum/view/forum/index.html:36
 msgid "No new posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:22
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:21
 msgid "Start new topic in"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:38
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
 msgid "Start topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/topic.html:23
+#: aa_forum/templates/aa_forum/view/forum/topic.html:24
 msgid "Modify topic subject"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:6
 msgid "Unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:16
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:15
 msgid "Unread Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:31
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:30
 msgid "You have no unread topics …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:7
 msgid "Personal messages (Inbox)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:7
 msgid "Personal messages (New message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:39
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:35
 msgid "Enter the recipients name"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:7
 msgid "Personal messages (Reply to message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:7
 msgid "Personal messages (Sent messages)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:6
 msgid "Search results"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:22
+#: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:32
+#: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
-#: aa_forum/templatetags/aa_forum_datetime.py:57
+#: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
 msgstr ""
 
-#: aa_forum/views/admin.py:165
+#: aa_forum/views/admin.py:169
 msgid "<h4>Success!</h4><p>Category created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:205
+#: aa_forum/views/admin.py:212
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Category name changed from \"{category_name_old}\" to "
 "\"{category.name}\".</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:245
+#: aa_forum/views/admin.py:255
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Category \"{category_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:298 aa_forum/views/admin.py:354
+#: aa_forum/views/admin.py:311 aa_forum/views/admin.py:371
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{new_board.name}\" created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:409
+#: aa_forum/views/admin.py:430
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board.name}\" changed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:450
+#: aa_forum/views/admin.py:475
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:556
+#: aa_forum/views/admin.py:587
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:566 aa_forum/views/personal_messages.py:116
-#: aa_forum/views/personal_messages.py:237 aa_forum/views/profile.py:68
+#: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
+#: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:225
+#: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:282
+#: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:309
+#: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:329
+#: aa_forum/views/forum.py:340
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in is an announcement "
 "board and you don't have the permissions to start a topic there.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:386
+#: aa_forum/views/forum.py:399
 msgid ""
 "<h4>Error!</h4><p>Either subject or message is missing. Please make sure you "
 "enter both fields, as both fields are mandatory.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:442 aa_forum/views/forum.py:672
+#: aa_forum/views/forum.py:461 aa_forum/views/forum.py:706
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to view does not exist or you do "
 "not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:539
+#: aa_forum/views/forum.py:563
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to modify does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:561
+#: aa_forum/views/forum.py:585
 msgid "<h4>Error!</h4><p>You are not allowed to modify this topic!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:593
+#: aa_forum/views/forum.py:617
 msgid "<h4>Success!</h4><p>The topic subject has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:791
+#: aa_forum/views/forum.py:845
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to reply does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:847
+#: aa_forum/views/forum.py:922
 msgid "<h4>Error!</h4><p>Message field is mandatory and cannot be empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:856
+#: aa_forum/views/forum.py:931
 msgid "<h4>Error!</h4><p>Something went wrong, please try again.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:894
+#: aa_forum/views/forum.py:972
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been unlocked/re-opened.</"
 "p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:908
+#: aa_forum/views/forum.py:986
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been locked/closed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:949
+#: aa_forum/views/forum.py:1030
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{curent_topic}\" is no longer \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:963
+#: aa_forum/views/forum.py:1044
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{curent_topic}\" is now \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:998
+#: aa_forum/views/forum.py:1082
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{topic__subject}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1034
+#: aa_forum/views/forum.py:1124
 msgid "<h4>Error!</h4><p>The message doesn't exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1078
+#: aa_forum/views/forum.py:1174
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to modify does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1101
+#: aa_forum/views/forum.py:1197
 msgid "<h4>Error!</h4><p>You are not allowed to modify this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1128
+#: aa_forum/views/forum.py:1224
 msgid "<h4>Success!</h4><p>The message has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1151
+#: aa_forum/views/forum.py:1247
 msgid "<h4>Error!</h4><p>Mandatory form field is empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1241
+#: aa_forum/views/forum.py:1345
 msgid "<h4>Error!</h4><p>You are not allowed to delete this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1271
+#: aa_forum/views/forum.py:1375
 msgid "<h4>Success!</h4><p>The message has been deleted.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1296
+#: aa_forum/views/forum.py:1400
 msgid ""
 "<h4>Success!</h4><p>The message has been deleted.</p><p>This was the topics "
 "opening post, so the topic has been deleted as well.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:104
+#: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:190
+#: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:226
+#: aa_forum/views/personal_messages.py:238
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Reply to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:282
-#: aa_forum/views/personal_messages.py:319
+#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:335
 msgid ""
 "<h4>Error!</h4><p>The message you tried to remove does either not exist or "
 "is not yours to remove.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:314
 msgid "<h4>Success!</h4><p>Message removed from your inbox.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:337
+#: aa_forum/views/personal_messages.py:353
 msgid ""
 "<h4>Success!</h4><p>Message has been removed from your sent messages.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:352
+#: aa_forum/views/personal_messages.py:368
 msgid "<h4>Error!</h4><p>Something went wrong.</p>"
 msgstr ""
 
-#: aa_forum/views/profile.py:58
+#: aa_forum/views/profile.py:60
 msgid "<h4>Success!</h4><p>Profile saved.</p>"
 msgstr ""
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/de/LC_MESSAGES/django.mo` & `aa_forum-2.1.0/aa_forum/locale/de/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-forum/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.4.3\n"
 
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] "%(counter)s Resultat"
 msgstr[1] "%(counter)s Resultate"
 
 msgid ""
@@ -217,14 +217,21 @@
 
 msgid "AA Forum v{__version__}"
 msgstr "AA Forum v{__version__}"
 
 msgid "AA-Forum"
 msgstr "AA-Forum"
 
+msgid ""
+"Activating this setting will ad a widget to your dashboard that shows unread "
+"topics in the forum."
+msgstr ""
+"Wenn diese Einstellung aktiviert ist, wird dem Dashboard ein Widget "
+"hinzugefügt, das ungelesene Themen im Forum anzeigt."
+
 msgid "Administration"
 msgstr "Verwaltung"
 
 msgid "Administration (Categories and boards)"
 msgstr "Verwaltung (Kategorien und Boards)"
 
 msgid "Administration (Forum settings)"
@@ -323,14 +330,20 @@
 
 msgid "Child boards:"
 msgstr "Untergeordnete Boards:"
 
 msgid "Clear form"
 msgstr "Formular löschen"
 
+msgid "Close"
+msgstr "Schließen"
+
+msgid "Close topic"
+msgstr "Thema schließen"
+
 msgid "Copy message link to clipboard"
 msgstr "Beitragslink in die Zwischenablage kopieren"
 
 msgid "Create board"
 msgstr "Board erstellen"
 
 msgid "Create category"
@@ -341,17 +354,14 @@
 
 msgid "Date"
 msgstr "Datum"
 
 msgid "Delete"
 msgstr "Löschen"
 
-msgid "Delete Message"
-msgstr "Beitrag löschen"
-
 msgid "Delete board"
 msgstr "Board löschen"
 
 msgid "Delete category"
 msgstr "Kategorie löschen"
 
 msgid "Delete message"
@@ -413,14 +423,17 @@
 
 msgid "Forum settings"
 msgstr "Forumeinstellungen"
 
 msgid "Forum user profile"
 msgstr "Benutzerprofil"
 
+msgid "Forum: Unread topics"
+msgstr "Forum: Ungelesene Themen"
+
 msgid "Go to last message"
 msgstr "Gehe zum letzten Beitrag"
 
 msgid "Group restrictions"
 msgstr "Gruppenbeschränkungen"
 
 msgid "Hello there …"
@@ -450,14 +463,24 @@
 msgid ""
 "How many topics per page should be displayed in a forum category? (Default: "
 "10)"
 msgstr ""
 "Wie viele Themen pro Seite sollen in einer Forenkategorie angezeigt werden? "
 "(Standard: 10)"
 
+msgid "If checked, this topic will be closed after posting this message."
+msgstr ""
+"Wenn diese Option aktiviert ist, wird dieses Thema nach dem Posten dieser "
+"Nachricht geschlossen."
+
+msgid "If checked, this topic will be reopened after posting this message."
+msgstr ""
+"Wenn diese Option aktiviert ist, wird dieses Thema nach dem Posten dieser "
+"Nachricht erneut geöffnet."
+
 msgid ""
 "If this message is the beginning of a conversation, all related messages "
 "will be removed as well."
 msgstr ""
 "Wenn diese Nachricht der Beginn einer Konversation ist, werden alle "
 "zugehörigen Nachrichten ebenfalls entfernt."
 
@@ -651,26 +674,26 @@
 
 msgid "Profile"
 msgstr "Profil"
 
 msgid "Re:"
 msgstr "Betreffend:"
 
-msgid "Read Message"
-msgstr "Nachricht lesen"
-
 msgid "Read message"
 msgstr "Nachricht lesen"
 
 msgid "Recipient"
 msgstr "Empfänger"
 
 msgid "Remove \"sticky\" state from topic"
 msgstr "Entferne den „Sticky“-Status von diesem Thema"
 
+msgid "Reopen topic"
+msgstr "Thema erneut öffnen"
+
 msgid "Replies"
 msgstr "Antworten"
 
 msgid "Reply"
 msgstr "Antwort"
 
 msgid "Reply to:"
@@ -702,14 +725,17 @@
 
 msgid "Set \"sticky\" state for topic"
 msgstr "Setze den „Sticky“-Status für dieses Thema"
 
 msgid "Show all unread topics"
 msgstr "Alle ungelesenen Themen anzeigen"
 
+msgid "Show unread topics as widget on the dashboard"
+msgstr "Zeige ungelesene Themen als Widget im Dashboard"
+
 msgid "Signature"
 msgstr "Signatur"
 
 msgid "Start new topic"
 msgstr "Neues Thema beginnen"
 
 msgid "Start new topic in"
@@ -765,17 +791,14 @@
 "beschränkt. Wenn keine Gruppen ausgewählt sind, kann jeder, der auf das "
 "Forum zugreifen kann, auch auf dieses Board zugreifen. (Diese Einstellung "
 "ist optional)"
 
 msgid "Timezone conversion"
 msgstr "Zeitzonenübersicht"
 
-msgid "Toggle navigation"
-msgstr "Navigation umschalten"
-
 msgid "Topic is always on top"
 msgstr "Das Thema steht immer oben"
 
 msgid "Topic is locked"
 msgstr "Thema ist gesperrt"
 
 msgid "Topics"
@@ -871,14 +894,17 @@
 
 msgid ""
 "You either don't have access to this board, or this board doesn't exist."
 msgstr ""
 "Du hast entweder keinen Zugriff auf dieses Board oder dieses Board existiert "
 "nicht."
 
+msgid "You have forgotten the message!"
+msgstr "Du hast die Nachricht vergessen!"
+
 msgid "You have no unread topics …"
 msgstr "Du hast keine ungelesenen Themen …"
 
 msgid "Your signature will appear below your posts."
 msgstr "Deine Signatur wird unter Deinem Beiträgen angezeigt."
 
 msgid ""
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/de/LC_MESSAGES/django.po` & `aa_forum-2.1.0/aa_forum/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,665 +1,712 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 #
 # Translators:
 # Peter Pfeufer, 2022
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 18:29+0200\n"
-"PO-Revision-Date: 2023-10-02 09:34+0000\n"
+"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"PO-Revision-Date: 2024-04-04 07:56+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-forum/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.4.3\n"
 
-#: aa_forum/__init__.py:12 aa_forum/templates/aa_forum/base.html:5
-#: aa_forum/templates/aa_forum/partials/menu.html:14
+#: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
+#: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
-#: aa_forum/templates/aa_forum/view/forum/board.html:5
-#: aa_forum/templates/aa_forum/view/forum/index.html:6
+#: aa_forum/templates/aa_forum/view/forum/board.html:6
+#: aa_forum/templates/aa_forum/view/forum/index.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:8
-#: aa_forum/templates/aa_forum/view/forum/topic.html:5
+#: aa_forum/templates/aa_forum/view/forum/topic.html:6
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:7
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:9
-#: aa_forum/templates/aa_forum/view/profile/index.html:9
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
 msgstr "Forum"
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr "AA Forum v{__version__}"
 
-#: aa_forum/forms.py:40
+#: aa_forum/forms.py:42
 msgid "This field is mandatory"
 msgstr "Dies ist ein Pflichtfeld"
 
-#: aa_forum/forms.py:91 aa_forum/forms.py:93 aa_forum/forms.py:124
-#: aa_forum/forms.py:126 aa_forum/forms.py:502
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:26
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:26
+#: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
+#: aa_forum/forms.py:171 aa_forum/forms.py:616
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr "Thema"
 
-#: aa_forum/forms.py:102 aa_forum/forms.py:321 aa_forum/forms.py:512
-#: aa_forum/forms.py:558
-msgid "Message"
-msgstr "Beitrag"
+#: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
+#: aa_forum/forms.py:730
+msgid "You have forgotten the message!"
+msgstr "Du hast die Nachricht vergessen!"
 
-#: aa_forum/forms.py:145 aa_forum/forms.py:183 aa_forum/forms.py:204
+#: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
 msgstr "Name"
 
-#: aa_forum/forms.py:147 aa_forum/forms.py:185
+#: aa_forum/forms.py:192 aa_forum/forms.py:230
 msgid "Category name"
 msgstr "Kategoriename"
 
-#: aa_forum/forms.py:151 aa_forum/forms.py:162
+#: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
 msgstr "Boards"
 
-#: aa_forum/forms.py:153
+#: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
 "Mit dieser Kategorie zu erstellende Boards (ein Board pro Zeile). Für diese "
 "Boards gelten keine Gruppenbeschränkungen, sodass diese später bei Bedarf "
 "hinzufügt werden müssen."
 
-#: aa_forum/forms.py:206
+#: aa_forum/forms.py:251
 msgid "Board name"
 msgstr "Boardname"
 
-#: aa_forum/forms.py:210
+#: aa_forum/forms.py:255
 msgid "Description"
 msgstr "Beschreibung"
 
-#: aa_forum/forms.py:216
+#: aa_forum/forms.py:261
 msgid "Board description (optional)"
 msgstr "Boardbeschreibung (Optional)"
 
-#: aa_forum/forms.py:222
+#: aa_forum/forms.py:267
 msgid "Group restrictions"
 msgstr "Gruppenbeschränkungen"
 
-#: aa_forum/forms.py:224
+#: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
 "Dadurch wird der Zugriff auf dieses Board auf die ausgewählten Gruppen "
 "beschränkt. Wenn keine Gruppen ausgewählt sind, kann jeder, der auf das "
 "Forum zugreifen kann, auch auf dieses Board zugreifen. (Diese Einstellung "
 "ist optional)"
 
-#: aa_forum/forms.py:232
+#: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
 msgstr "Discord-Webhook (Optional)"
 
-#: aa_forum/forms.py:234
+#: aa_forum/forms.py:279
 msgid ""
 "Discord webhook URL for the channel to post about new topics in this board. "
 "(This setting is optional)"
 msgstr ""
 "Discord-Webhook URL für den Kanal, um über neue Themen in diesem Board zu "
 "posten. (Diese Einstellung ist optional)"
 
-#: aa_forum/forms.py:247
+#: aa_forum/forms.py:292
 msgid "Use this Discord webhook for replies as well?"
 msgstr "Diesen Discord-Webhook auch für Antworten nutzen?"
 
-#: aa_forum/forms.py:249
+#: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
 msgstr ""
 "Wenn aktiviert, wird jede Antwort auf ein beliebiges Thema in diesem Board "
 "im definierten Discord-Kanal gepostet. (Child-Boards sind ausgeschlossen) "
 "Wähle mit Bedacht! (Standard: NEIN)"
 
-#: aa_forum/forms.py:257
+#: aa_forum/forms.py:302
 msgid "Mark board as \"Announcement Board\""
 msgstr "Board als „Ankündigungs-Board“ markieren"
 
-#: aa_forum/forms.py:259
+#: aa_forum/forms.py:304
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. This setting will "
 "not be inherited to child boards. (Default: NO)"
 msgstr ""
 "Markiere dieses Board als „Ankündigungs-Board“, was bedeutet, dass nur "
 "bestimmte ausgewählte Gruppen neue Themen starten können. Alle anderen, die "
 "Zugriff auf dieses Board haben, können jedoch weiterhin in den Themen "
 "diskutieren. Diese Einstellung wird nicht an untergeordnete Boards vererbt. "
 "(Standard: NEIN)"
 
-#: aa_forum/forms.py:267
+#: aa_forum/forms.py:312
 msgid "Start topic restrictions for \"Announcement Boards\""
 msgstr "„Starte Thema“ Einschränkungen für „Ankündigungs-Board“"
 
-#: aa_forum/forms.py:269
+#: aa_forum/forms.py:314
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
 msgstr ""
 "Benutzer in mindestens einer der ausgewählten Gruppen können Themen in "
 "„Ankündigungs-Boards“ beginnen. Wenn keine Gruppe ausgewählt ist, können "
 "dies nur Forenadministratoren tun. Diese Einstellung wird nicht an "
 "untergeordnete Boards vererbt. (Hinweis: Diese Einschränkungen wirken sich "
 "nur aus, wenn ein Board als „Ankündigungs-Board“ markiert ist, siehe "
 "Checkbox oben.)"
 
-#: aa_forum/forms.py:354
-msgid "Signature"
-msgstr "Signatur"
+#: aa_forum/forms.py:362
+msgid "Close topic"
+msgstr "Thema schließen"
 
-#: aa_forum/forms.py:355
-msgid "Your signature will appear below your posts."
-msgstr "Deine Signatur wird unter Deinem Beiträgen angezeigt."
+#: aa_forum/forms.py:364
+msgid "If checked, this topic will be closed after posting this message."
+msgstr ""
+"Wenn diese Option aktiviert ist, wird dieses Thema nach dem Posten dieser "
+"Nachricht geschlossen."
 
-#: aa_forum/forms.py:359
+#: aa_forum/forms.py:370
+msgid "Reopen topic"
+msgstr "Thema erneut öffnen"
+
+#: aa_forum/forms.py:372
+msgid "If checked, this topic will be reopened after posting this message."
+msgstr ""
+"Wenn diese Option aktiviert ist, wird dieses Thema nach dem Posten dieser "
+"Nachricht erneut geöffnet."
+
+#: aa_forum/forms.py:409 aa_forum/forms.py:652 aa_forum/forms.py:717
+msgid "Message"
+msgstr "Beitrag"
+
+#: aa_forum/forms.py:446
 msgid "Website title"
 msgstr "Webseitentitel"
 
-#: aa_forum/forms.py:361
+#: aa_forum/forms.py:448
 msgid "e.g.: My Homepage"
 msgstr "z.B.: Meine Homepage"
 
-#: aa_forum/forms.py:362
+#: aa_forum/forms.py:449
 msgid "Your website's title."
 msgstr "Der Titel Deiner Website."
 
-#: aa_forum/forms.py:366
+#: aa_forum/forms.py:453
 msgid "Website URL"
 msgstr "Webadresse"
 
-#: aa_forum/forms.py:370
+#: aa_forum/forms.py:457
 msgid ""
 "Your website's URL. (Don't forget to also set a title for your website, "
 "otherwise this field will be ignored.)"
 msgstr ""
 "Die URL Deiner Website. (Vergiss nicht, auch einen Titel für Deine Website "
 "festzulegen, da dieses Feld sonst ignoriert wird.)"
 
-#: aa_forum/forms.py:376
+#: aa_forum/forms.py:463
 msgid "PM me on Discord when I get a new personal message"
 msgstr ""
 "PM an mich auf Discord, wenn ich eine neue persönliche Nachricht erhalte"
 
-#: aa_forum/forms.py:378
+#: aa_forum/forms.py:466
 msgid ""
 "Information: There is currently no module installed that can handle Discord "
 "direct messages. Have a chat with your IT guys to remedy this."
 msgstr ""
 "Information: Derzeit ist kein Modul installiert, das Discord-"
 "Direktnachrichten verarbeiten kann. Sprich mit Deinen IT-Leuten, um Abhilfe "
 "zu schaffen."
 
-#: aa_forum/forms.py:419
+#: aa_forum/forms.py:475
+msgid "Show unread topics as widget on the dashboard"
+msgstr "Zeige ungelesene Themen als Widget im Dashboard"
+
+#: aa_forum/forms.py:478
+msgid ""
+"Activating this setting will ad a widget to your dashboard that shows unread "
+"topics in the forum."
+msgstr ""
+"Wenn diese Einstellung aktiviert ist, wird dem Dashboard ein Widget "
+"hinzugefügt, das ungelesene Themen im Forum anzeigt."
+
+#: aa_forum/forms.py:507
+msgid "Signature"
+msgstr "Signatur"
+
+#: aa_forum/forms.py:508
+msgid "Your signature will appear below your posts."
+msgstr "Deine Signatur wird unter Deinem Beiträgen angezeigt."
+
+#: aa_forum/forms.py:532
 msgid ""
 "Ensure your signature has at most {max_signature_length} characters. "
 "(Currently: {len(signature)})"
 msgstr ""
 "Stelle sicher, dass Deine Signatur höchstens {max_signature_length} Zeichen "
 "hat. (Aktuell: {len(signature)})"
 
-#: aa_forum/forms.py:440
+#: aa_forum/forms.py:554
 msgid "This is not a valid URL"
 msgstr "Dies ist keine gültige URL"
 
-#: aa_forum/forms.py:456
+#: aa_forum/forms.py:570
 msgid ""
 "How many messages per page should be displayed in a forum topic? (Default: "
 "15)"
 msgstr ""
 "Wie viele Beiträge pro Seite sollen in einem Forenthema angezeigt werden? "
 "(Standard: 15)"
 
-#: aa_forum/forms.py:466
+#: aa_forum/forms.py:580
 msgid ""
 "How many topics per page should be displayed in a forum category? (Default: "
 "10)"
 msgstr ""
 "Wie viele Themen pro Seite sollen in einer Forenkategorie angezeigt werden? "
 "(Standard: 10)"
 
-#: aa_forum/forms.py:476
+#: aa_forum/forms.py:590
 msgid ""
 "How long (Number of characters) is a user's signature allowed to be? "
 "(Default: 750)"
 msgstr ""
 "Wie lang (Anzahl Zeichen) darf die Signatur eines Benutzers sein? (Standard: "
 "750)"
 
-#: aa_forum/forms.py:498
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:22
+#: aa_forum/forms.py:612
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:21
 msgid "Recipient"
 msgstr "Empfänger"
 
-#: aa_forum/forms.py:504
+#: aa_forum/forms.py:618
 msgid "Hello there …"
 msgstr "Hallo …"
 
-#: aa_forum/models.py:127
+#: aa_forum/models.py:139
 msgid "AA-Forum"
 msgstr "AA-Forum"
 
-#: aa_forum/models.py:131
+#: aa_forum/models.py:143
 msgid "Can access the AA-Forum module"
 msgstr "Kann auf das AA-Forum-Modul zugreifen"
 
-#: aa_forum/models.py:134
+#: aa_forum/models.py:146
 msgid "Can manage the AA-Forum module (Category, topics and messages)"
 msgstr "Kann das AA-Forum-Modul verwalten (Kategorie, Themen und Nachrichten)"
 
-#: aa_forum/models.py:177
+#: aa_forum/models.py:193
 msgid "category"
 msgstr "Kategorie"
 
-#: aa_forum/models.py:178
+#: aa_forum/models.py:194
 msgid "categories"
 msgstr "Kategorien"
 
-#: aa_forum/models.py:222
+#: aa_forum/models.py:248
 msgid ""
 "Use this Discord webhook for replies as well? When activated every reply to "
 "any topic in this board will be posted to the defined Discord channel. "
 "(Child boards are excluded) Chose wisely! (Default: NO)"
 msgstr ""
 "Diesen Discord-Webhook auch für Antworten nutzen? Wenn aktiviert, wird jede "
 "Antwort zu einem beliebigen Thema in diesem Forum im definierten Discord-"
 "Kanal gepostet. (Untergeordnete Boards sind ausgeschlossen) Wähle mit "
 "Bedacht! (Standard: NEIN)"
 
-#: aa_forum/models.py:240
+#: aa_forum/models.py:266
 msgid ""
 "User in at least one of these groups have access to this board. If no groups "
 "are selected, everyone with access to the forum has also access to this "
 "board."
 msgstr ""
 "Benutzer in mindestens einer dieser Gruppen haben Zugriff auf dieses Board. "
 "Wenn keine Gruppen ausgewählt sind, hat jeder, der Zugriff auf das Forum "
 "hat, auch Zugriff auf dieses Board."
 
-#: aa_forum/models.py:248
+#: aa_forum/models.py:274
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. (Default: NO)"
 msgstr ""
 "Markiere dieses Board als „Ankündigungs-Board“, was bedeutet, dass nur "
 "bestimmte ausgewählte Gruppen neue Themen starten können. Alle anderen, die "
 "Zugriff auf dieses Board haben, können jedoch weiterhin in den Themen "
 "diskutieren. (Standard: NEIN)"
 
-#: aa_forum/models.py:259
+#: aa_forum/models.py:285
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so."
 msgstr ""
 "Benutzer in mindestens einer der ausgewählten Gruppen können Themen in "
 "„Ankündigungs-Boards“ starten. Wenn keine Gruppe ausgewählt ist, können dies "
 "nur Forumadministratoren tun."
 
-#: aa_forum/models.py:295
+#: aa_forum/models.py:321
 msgid "board"
 msgstr "Board"
 
-#: aa_forum/models.py:296
+#: aa_forum/models.py:322
 msgid "boards"
 msgstr "Boards"
 
-#: aa_forum/models.py:367
+#: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 "<h4>Warnung!</h4><p>Es gibt bereits ein Thema mit genau demselben Namen in "
 "diesem Board.</p><p>Siehe hier: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 
-#: aa_forum/models.py:578
+#: aa_forum/models.py:625
 msgid "topic"
 msgstr "Thema"
 
-#: aa_forum/models.py:579
+#: aa_forum/models.py:626
 msgid "topics"
 msgstr "Themen"
 
-#: aa_forum/models.py:736
+#: aa_forum/models.py:805
 msgid "message"
 msgstr "Beitrag"
 
-#: aa_forum/models.py:737
+#: aa_forum/models.py:806
 msgid "messages"
 msgstr "Beträge"
 
-#: aa_forum/models.py:872
+#: aa_forum/models.py:948
 msgid "personal message"
 msgstr "Persönliche Nachricht"
 
-#: aa_forum/models.py:873
+#: aa_forum/models.py:949
 msgid "personal messages"
 msgstr "Persönliche Nachrichten"
 
-#: aa_forum/models.py:920
+#: aa_forum/models.py:1003
 msgid "Messages per page"
 msgstr "Beiträge pro Seite"
 
-#: aa_forum/models.py:921
+#: aa_forum/models.py:1004
 msgid "Topics per page"
 msgstr "Themen pro Seite"
 
-#: aa_forum/models.py:922
+#: aa_forum/models.py:1005
 msgid "User signature length"
 msgstr "Länge der Benutzersignatur"
 
-#: aa_forum/models.py:927
+#: aa_forum/models.py:1010
 msgid "Maximum number of messages per page in the topic view"
 msgstr "Maximale Anzahl von Beiträgen pro Seite in der Themenansicht"
 
-#: aa_forum/models.py:932
+#: aa_forum/models.py:1015
 msgid "Maximum number of topics per page in the board view"
 msgstr "Maximale Anzahl von Themen pro Seite in der Board-Ansicht"
 
-#: aa_forum/models.py:937
+#: aa_forum/models.py:1020
 msgid "Maximum length of a users signature"
 msgstr "Maximale Länge einer Benutzersignatur"
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:1031
 msgid "setting"
 msgstr "Einstellung"
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:1032
 msgid "settings"
 msgstr "Einstellungen"
 
-#: aa_forum/models.py:952
+#: aa_forum/models.py:1042
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:16
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr "Forumeinstellungen"
 
-#: aa_forum/models.py:978
+#: aa_forum/models.py:1069
 msgid "user profile"
 msgstr "Benutzerprofil"
 
-#: aa_forum/models.py:979
+#: aa_forum/models.py:1070
 msgid "user profiles"
 msgstr "Benutzerprofile"
 
-#: aa_forum/models.py:982
+#: aa_forum/models.py:1080
 msgid "Forum user profile"
 msgstr "Benutzerprofil"
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:30
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr "geschrieben:"
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:7
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr "Antwort"
 
-#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:38
+#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:8
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:56
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:73
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:59
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:75
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:69
 msgid "Delete message"
 msgstr "Beitrag löschen"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:13
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:8
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:23
 msgid "Delete board"
 msgstr "Board löschen"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
+msgid "Close"
+msgstr "Schließen"
+
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr "Möchtest Du dieses Board wirklich löschen?"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
 msgstr "Dadurch werden auch alle Themen und Beiträge in diesem Board entfernt."
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:22
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:22
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:21
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:21
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:21
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:20
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:20
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:20
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:19
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:19
 msgid "This action cannot be undone!"
 msgstr "Diese Aktion kann nicht rückgängig gemacht werden!"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:29
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:29
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:28
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:28
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:28
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:27
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:27
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
 msgstr "Abbrechen"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:34
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:34
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:33
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:33
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:33
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
 msgstr "Löschen"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:15
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr "Kategorie löschen"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:16
 msgid "Are you sure you want to delete this category?"
 msgstr "Möchtest Du diese Kategorie wirklich löschen?"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:17
 msgid "This will also remove all boards, topics and messages in this category."
 msgstr ""
 "Dadurch werden auch alle Foren, Themen und Beiträge in dieser Kategorie "
 "entfernt."
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr "Sperrstatus des Themas ändern"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:13
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:39
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:84
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
 msgid "Unlock/re-open topic"
 msgstr "Thema entsperren/erneut öffnen"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:16
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:42
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:88
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
 msgid "Lock/close topic"
 msgstr "Thema sperren/schließen"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr "Möchtest Du dieses Thema wirklich entsperren/erneut öffnen?"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
 msgid "Are you sure you want to lock/close this topic?"
 msgstr "Möchtest Du dieses Thema wirklich sperren/schließen?"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:3
 msgid "Change sticky state of topic"
 msgstr "Sticky-Status des Themas ändern"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:13
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:9
 msgid "Remove \"sticky\" state from topic"
 msgstr "Entferne den „Sticky“-Status von diesem Thema"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:16
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:12
 msgid "Set \"sticky\" state for topic"
 msgstr "Setze den „Sticky“-Status für dieses Thema"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:22
 msgid "Are you sure you want to remove the sticky state from this topic?"
 msgstr ""
 "Bist Du sicher, dass Du den Sticky-Status von diesem Thema entfernen "
 "möchtest?"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
 msgid ""
 "Are you sure you want to make this topic sticky, so it always shows up on "
 "top of the topic list?"
 msgstr ""
 "Möchtest Du dieses Thema wirklich fixieren, sodass es immer ganz oben in der "
 "Themenliste angezeigt wird?"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:39
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:37
 msgid "Unset sticky"
 msgstr "Sticky aufheben"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:42
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr "Sticky setzen"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:97
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
 msgid "Delete topic"
 msgstr "Thema löschen"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr "Möchtest Du dieses Thema wirklich löschen?"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:19
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:17
 msgid "This will also remove all messages in this topic."
 msgstr ""
 "Dadurch werden auch alle Themen und Nachrichten in diesem Thema entfernt."
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:17
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:17
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:15
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:15
 msgid "Are you sure you want to delete this message?"
 msgstr "Möchtest Du diesen Beitrag wirklich löschen?"
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:16
 msgid ""
 "If this message is the original post, then the entire topic will be removed "
 "as well."
 msgstr ""
 "Wenn es sich bei diesem Beitrag um den ursprünglichen Beitrag handelt, wird "
 "auch das gesamte Thema entfernt."
 
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:16
 msgid ""
 "If this message is the beginning of a conversation, all related messages "
 "will be removed as well."
 msgstr ""
 "Wenn diese Nachricht der Beginn einer Konversation ist, werden alle "
 "zugehörigen Nachrichten ebenfalls entfernt."
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:9
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:11
 msgid "Edit board"
 msgstr "Board bearbeiten"
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:22
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:36
 msgid ""
 "Changing the name of this board does not change its URL part. This will "
 "remain the same to not break any possible links into this board."
 msgstr ""
 "Das Ändern des Namens dieses Boards ändert nicht seinen URL-Teil. Dies "
 "bleibt gleich, um keine möglichen Links in dieses Board zu unterbrechen."
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:58
 msgid "Change board"
 msgstr "Board ändern"
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:56
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:70
 msgid "New child board"
 msgstr "Neues Unterboard"
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:63
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:62
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:77
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:84
 msgid ""
 "New boards will be added at the bottom of the board list for this category. "
 "You can move them via drag and drop to a position of your liking."
 msgstr ""
 "Neue Boards werden am Ende der Boardliste für diese Kategorie hinzugefügt. "
 "Du kannst diese per Drag and Drop an eine Position Deiner Wahl verschieben."
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:79
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:75
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:93
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:97
 msgid "Create board"
 msgstr "Board erstellen"
 
-#: aa_forum/templates/aa_forum/partials/administration/categories.html:6
+#: aa_forum/templates/aa_forum/partials/administration/categories.html:5
 msgid ""
 "Here you can create, modify and delete categories and boards. You also can "
 "change their order via drag and drop."
 msgstr ""
 "Hier kannst Du Kategorien und Boards erstellen, ändern und löschen. Du "
 "kannst ihre Reihenfolge auch per Drag & Drop ändern."
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:11
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:13
 msgid "Edit category"
 msgstr "Kategorie bearbeiten"
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:19
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:35
 msgid "Expand/collapse category"
 msgstr "Kategorie erweitern/reduzieren"
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:31
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:53
 msgid ""
 "Changing the name of this category does not change its URL part. This will "
 "remain the same to not break any possible links into this category."
 msgstr ""
 "Das Ändern des Namens dieser Kategorie ändert nicht ihren URL-Teil. Dies "
 "bleibt gleich, um keine möglichen Links in diese Kategorie einzuteilen."
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:66
 msgid "Change category"
 msgstr "Kategorie ändern"
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:55
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:77
 msgid "New board"
 msgstr "Neues Board"
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:7
 msgid "Create new category"
 msgstr "Neue Kategorie erstellen"
 
@@ -676,24 +723,25 @@
 "per Drag and Drop an eine Position Deiner Wahl verschieben."
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:35
 msgid "Create category"
 msgstr "Kategorie erstellen"
 
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:21
-#: aa_forum/templates/aa_forum/partials/profile/form.html:21
+#: aa_forum/templates/aa_forum/partials/profile/form.html:22
 msgid "Submit"
 msgstr "Absenden"
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:6
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:7
 msgid "Forum index"
 msgstr "Forumindex"
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:27
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:49
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:51
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:6
 msgid "Modify message"
 msgstr "Beitrag bearbeiten"
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:34
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:7
@@ -716,67 +764,67 @@
 "Du möchtest helfen diese App in Deine Sprache zu übersetzen oder die "
 "bestehende Übersetzung verbessern?"
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Tritt unserm Team von Übersetzern bei!"
 
-#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:9
+#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr "Mit einem Sternchen (*) gekennzeichnete Felder sind Pflichtfelder"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr "In diesem Board wurden keine Themen begonnen …"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:34
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] "Dieses Board ist auf die folgende Gruppe beschränkt:"
 msgstr[1] "Dieses Board ist auf die folgenden Gruppen beschränkt:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr "Untergeordnete Boards:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:51
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
 msgid "New"
 msgstr "Neu"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr "Beiträge"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
 msgid "Topics"
 msgstr "Themen"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:66
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:65
 msgid "Unread"
 msgstr "Ungelesen"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:82
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:88
 msgid "Last post:"
 msgstr "Letzter Beitrag:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:86
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:25
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:96
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:26
 msgid "Re:"
 msgstr "Betreffend:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:103
 msgid "posted by:"
 msgstr "von:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:94
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:104
 msgid "posted at:"
 msgstr "geschrieben:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:7
+#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:8
 msgid "New topic"
 msgstr "Neues Thema"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/no-access.html:6
 msgid ""
 "You either don't have access to this board, or this board doesn't exist."
 msgstr ""
@@ -844,58 +892,58 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr "Letzter"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
 msgid "Topic is always on top"
 msgstr "Das Thema steht immer oben"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
 msgid "Topic is locked"
 msgstr "Thema ist gesperrt"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
 msgid "Started by"
 msgstr "Begonnen bei"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
 msgid "Replies"
 msgstr "Antworten"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
 msgid "Last post"
 msgstr "Letzter Beitrag"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
 msgid "Go to last message"
 msgstr "Gehe zum letzten Beitrag"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
 msgid "Change topics sticky state"
 msgstr "Sticky-Status vom Thema ändern"
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr "Alle Themen als gelesen markieren"
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:38
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:39
 msgid "Copy message link to clipboard"
 msgstr "Beitragslink in die Zwischenablage kopieren"
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:81
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:87
 msgid "Last modified:"
 msgstr "Zuletzt geändert:"
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:14
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
 msgstr ""
 "Hinweis: Du befindest Dich nicht auf der letzten Seite dieses Themas und "
 "verpasst möglicherweise die neuesten Antworten."
 
@@ -905,69 +953,66 @@
 msgstr "Ändern"
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:6
 msgid "Modify topic"
 msgstr "Thema ändern"
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:20
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:21
 msgid "Warning: this topic is locked! Only admins can reply."
 msgstr ""
 "Achtung: Dieses Thema ist gesperrt! Nur Administratoren können antworten."
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:33
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:44
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
 msgid "Clear form"
 msgstr "Formular löschen"
 
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:7
 msgid "Show all unread topics"
 msgstr "Alle ungelesenen Themen anzeigen"
 
-#: aa_forum/templates/aa_forum/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr "Navigation umschalten"
-
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:7
 msgid "Administration"
 msgstr "Verwaltung"
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:12
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:13
 msgid "Categories and boards"
 msgstr "Kategorien und Boards"
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:6
-#: aa_forum/templates/aa_forum/view/profile/index.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:13
+#: aa_forum/templates/aa_forum/view/profile/index.html:7
 msgid "Profile"
 msgstr "Profil"
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:11
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:19
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:9
 msgid "Messages"
 msgstr "Nachrichten"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:23
 msgid "Inbox"
 msgstr "Posteingang"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:18
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:18
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:17
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:17
 msgid "Date"
 msgstr "Datum"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:22
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:21
 msgid "Sender"
 msgstr "Absender"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:62
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:63
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:57
 msgid "Read message"
 msgstr "Nachricht lesen"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:87
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:93
 msgid "No personal messages"
 msgstr "Keine persönlichen Nachrichten"
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:8
 msgid "New personal message"
 msgstr "Keine persönlichen Nachrichten"
 
@@ -975,361 +1020,357 @@
 msgid "Send message"
 msgstr "Nachricht senden"
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:8
 msgid "Reply to:"
 msgstr "Antwort an:"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:24
+#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:23
 msgid "Send reply"
 msgstr "Antwort senden"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:30
 msgid "Sent messages"
 msgstr "Gesendete Nachrichten"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:56
-msgid "Read Message"
-msgstr "Nachricht lesen"
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:67
-msgid "Delete Message"
-msgstr "Beitrag löschen"
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:81
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:87
 msgid "No personal messages sent"
 msgstr "Keine gesendeten Nachrichten"
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:17
 msgid "New message"
 msgstr "Neue Nachricht"
 
 #: aa_forum/templates/aa_forum/partials/profile/form.html:7
 msgid "User profile"
 msgstr "Benutzerprofil"
 
-#: aa_forum/templates/aa_forum/partials/search/search-form.html:7
+#: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr "Suche …"
 
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+msgid "Forum: Unread topics"
+msgstr "Forum: Ungelesene Themen"
+
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr "Verwaltung (Kategorien und Boards)"
 
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:6
 msgid "Administration (Forum settings)"
 msgstr "Verwaltung (Forum-Einstellungen)"
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:26
+#: aa_forum/templates/aa_forum/view/forum/index.html:27
 msgid "New posts"
 msgstr "Neue Beiträge"
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:35
+#: aa_forum/templates/aa_forum/view/forum/index.html:36
 msgid "No new posts"
 msgstr "Keine neuen Beiträge"
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:22
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:21
 msgid "Start new topic in"
 msgstr "Neues Thema beginnen in"
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:38
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
 msgid "Start topic"
 msgstr "Thema beginnen"
 
-#: aa_forum/templates/aa_forum/view/forum/topic.html:23
+#: aa_forum/templates/aa_forum/view/forum/topic.html:24
 msgid "Modify topic subject"
 msgstr "Themenbetreff ändern"
 
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:6
 msgid "Unread topics"
 msgstr "Ungelesene Themen"
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:16
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:15
 msgid "Unread Topics"
 msgstr "Ungelesene Themen"
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:31
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:30
 msgid "You have no unread topics …"
 msgstr "Du hast keine ungelesenen Themen …"
 
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:7
 msgid "Personal messages (Inbox)"
 msgstr "Persönliche Nachrichten (Posteingang)"
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:7
 msgid "Personal messages (New message)"
 msgstr "Persönliche Nachrichten (Neue Nachricht)"
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:39
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:35
 msgid "Enter the recipients name"
 msgstr "Gib den Namen des Empfängers ein"
 
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:7
 msgid "Personal messages (Reply to message)"
 msgstr "Persönliche Nachrichten (Auf Nachricht antworten)"
 
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:7
 msgid "Personal messages (Sent messages)"
 msgstr "Persönliche Nachrichten (Gesendete Nachrichten)"
 
 #: aa_forum/templates/aa_forum/view/search/results.html:6
 msgid "Search results"
 msgstr "Suchergebnisse"
 
-#: aa_forum/templates/aa_forum/view/search/results.html:22
+#: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] "%(counter)s Resultat"
 msgstr[1] "%(counter)s Resultate"
 
-#: aa_forum/templates/aa_forum/view/search/results.html:32
+#: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr "Nichts gefunden …"
 
-#: aa_forum/templatetags/aa_forum_datetime.py:57
+#: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
 msgstr "Zeitzonenübersicht"
 
-#: aa_forum/views/admin.py:165
+#: aa_forum/views/admin.py:169
 msgid "<h4>Success!</h4><p>Category created.</p>"
 msgstr "<h4>Erfolg!</h4><p>Kategorie erstellt.</p>"
 
-#: aa_forum/views/admin.py:205
+#: aa_forum/views/admin.py:212
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Category name changed from \"{category_name_old}\" to "
 "\"{category.name}\".</p>"
 msgstr ""
 "<h4>Erfolg!</h4><p>Der Kategoriename wurde von „{category_name_old}“ in "
 "„{category.name}“geändert.</p>"
 
-#: aa_forum/views/admin.py:245
+#: aa_forum/views/admin.py:255
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Category \"{category_name}\" removed.</p>"
 msgstr "<h4>Erfolg!</h4><p>Kategorie „{category_name}“ entfernt.</p>"
 
-#: aa_forum/views/admin.py:298 aa_forum/views/admin.py:354
+#: aa_forum/views/admin.py:311 aa_forum/views/admin.py:371
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{new_board.name}\" created.</p>"
 msgstr "<h4>Erfolg!</h4><p>Board„{new_board.name}“ erstellt.</p>"
 
-#: aa_forum/views/admin.py:409
+#: aa_forum/views/admin.py:430
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board.name}\" changed.</p>"
 msgstr "<h4>Erfolg!</h4><p>Board „{board.name}“ geändert.</p>"
 
-#: aa_forum/views/admin.py:450
+#: aa_forum/views/admin.py:475
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board_name}\" removed.</p>"
 msgstr "<h4>Erfolg!</h4><p>Board „{board_name}“ entfernt.</p>"
 
-#: aa_forum/views/admin.py:556
+#: aa_forum/views/admin.py:587
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr "<h4>Erfolg!</h4><p>Einstellungen aktualisiert.</p>"
 
-#: aa_forum/views/admin.py:566 aa_forum/views/personal_messages.py:116
-#: aa_forum/views/personal_messages.py:237 aa_forum/views/profile.py:68
+#: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
+#: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr ""
-"<h4>Fehler!</h4><p>Etwas ist schief gelaufen, bitte überprüfe Deine "
-"Eingabe.</p>"
+"<h4>Fehler!</h4><p>Etwas ist schief gelaufen, bitte überprüfe Deine Eingabe."
+"</p>"
 
-#: aa_forum/views/forum.py:225
+#: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Das Board, das Du aufrufen willst, existiert entweder "
 "nicht oder Du hast keinen Zugriff darauf.</p>"
 
-#: aa_forum/views/forum.py:282
+#: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
-"<h4>Fehler!</h4><p>Die Kategorie, in der Du posten willst, existiert "
-"nicht.</p>"
+"<h4>Fehler!</h4><p>Die Kategorie, in der Du posten willst, existiert nicht.</"
+"p>"
 
-#: aa_forum/views/forum.py:309
+#: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Das Board, in dem Du posten willst, existiert entweder "
 "nicht oder Du hast keinen Zugriff darauf.</p>"
 
-#: aa_forum/views/forum.py:329
+#: aa_forum/views/forum.py:340
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in is an announcement "
 "board and you don't have the permissions to start a topic there.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Das Board in dem Du posten willst, ist ein „Ankündigungs-"
 "Board“ und Du hast nicht die Berechtigung, dort ein Thema zu eröffnen.</p>"
 
-#: aa_forum/views/forum.py:386
+#: aa_forum/views/forum.py:399
 msgid ""
 "<h4>Error!</h4><p>Either subject or message is missing. Please make sure you "
 "enter both fields, as both fields are mandatory.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Theme oder Beitrag fehlt. Bitte stelle sicher, dass Du "
 "beide Felder ausfüllst, da beide Felder Pflichtfelder sind.</p>"
 
-#: aa_forum/views/forum.py:442 aa_forum/views/forum.py:672
+#: aa_forum/views/forum.py:461 aa_forum/views/forum.py:706
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to view does not exist or you do "
 "not have access to it.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Das Thema, das Du öffnen wollten, existiert nicht oder Du "
 "hast keinen Zugriff darauf.</p>"
 
-#: aa_forum/views/forum.py:539
+#: aa_forum/views/forum.py:563
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to modify does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Das Thema, das Du bearbeiten willst, existiert nicht oder "
 "Du hast keinen Zugriff darauf.</p>"
 
-#: aa_forum/views/forum.py:561
+#: aa_forum/views/forum.py:585
 msgid "<h4>Error!</h4><p>You are not allowed to modify this topic!</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Du bist nicht berechtigt, dieses Thema zu ändern!</p>"
 
-#: aa_forum/views/forum.py:593
+#: aa_forum/views/forum.py:617
 msgid "<h4>Success!</h4><p>The topic subject has been updated.</p>"
 msgstr "<h4>Erfolg!</h4><p>Das Thema wurde aktualisiert.</p>"
 
-#: aa_forum/views/forum.py:791
+#: aa_forum/views/forum.py:845
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to reply does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Das Thema, auf das Du antworten willst, existiert nicht "
 "oder Du hast keinen Zugriff darauf.</p>"
 
-#: aa_forum/views/forum.py:847
+#: aa_forum/views/forum.py:922
 msgid "<h4>Error!</h4><p>Message field is mandatory and cannot be empty.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Das Beitragsfeld ist ein Pflichtfeld und darf nicht leer "
 "sein.</p>"
 
-#: aa_forum/views/forum.py:856
+#: aa_forum/views/forum.py:931
 msgid "<h4>Error!</h4><p>Something went wrong, please try again.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Etwas ist schief gelaufen, bitte versuche es erneut.</p>"
 
-#: aa_forum/views/forum.py:894
+#: aa_forum/views/forum.py:972
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been unlocked/re-opened.</"
 "p>"
 msgstr "<h4>Erfolg!</h4><p>Topic „{current_topic}“ wieder eröffnet.</p>"
 
-#: aa_forum/views/forum.py:908
+#: aa_forum/views/forum.py:986
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been locked/closed.</p>"
 msgstr ""
 "<h4>Erfolg!</h4><p>Thema „{current_topic}“ wurde gesperrt/geschlossen.</p>"
 
-#: aa_forum/views/forum.py:949
+#: aa_forum/views/forum.py:1030
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{curent_topic}\" is no longer \"sticky\".</p>"
 msgstr "<h4>Erfolg!</h4><p>Thema „{curent_topic}“ ist nicht mehr „Sticky“.</p>"
 
-#: aa_forum/views/forum.py:963
+#: aa_forum/views/forum.py:1044
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{curent_topic}\" is now \"sticky\".</p>"
 msgstr "<h4>Erfolg!</h4><p>Thema „{curent_topic}“ ist jetzt „Sticky“.</p>"
 
-#: aa_forum/views/forum.py:998
+#: aa_forum/views/forum.py:1082
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{topic__subject}\" removed.</p>"
 msgstr "<h4>Erfolg!</h4><p>Thema „{topic__subject}“ entfernt.</p>"
 
-#: aa_forum/views/forum.py:1034
+#: aa_forum/views/forum.py:1124
 msgid "<h4>Error!</h4><p>The message doesn't exist.</p>"
 msgstr "<h4>Fehler!</h4><p>Der Beitrag existiert nicht.</p>"
 
-#: aa_forum/views/forum.py:1078
+#: aa_forum/views/forum.py:1174
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to modify does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Der Beitrag, den Du ändern wilsst, existiert entweder "
 "nicht oder Du hast keinen Zugriff darauf.</p>"
 
-#: aa_forum/views/forum.py:1101
+#: aa_forum/views/forum.py:1197
 msgid "<h4>Error!</h4><p>You are not allowed to modify this message!</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Du bistnicht berechtigt, diesen Beitrag zu ändern!</p>"
 
-#: aa_forum/views/forum.py:1128
+#: aa_forum/views/forum.py:1224
 msgid "<h4>Success!</h4><p>The message has been updated.</p>"
 msgstr "<h4>Erfolg!</h4><p>Der Beitrag wurde aktualisiert.</p>"
 
-#: aa_forum/views/forum.py:1151
+#: aa_forum/views/forum.py:1247
 msgid "<h4>Error!</h4><p>Mandatory form field is empty.</p>"
 msgstr "<h4>Fehler!</h4><p>Pflichtfeld ist leer.</p>"
 
-#: aa_forum/views/forum.py:1241
+#: aa_forum/views/forum.py:1345
 msgid "<h4>Error!</h4><p>You are not allowed to delete this message!</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Du bist nicht berechtigt, diesen Beitrag zu löschen!</p>"
 
-#: aa_forum/views/forum.py:1271
+#: aa_forum/views/forum.py:1375
 msgid "<h4>Success!</h4><p>The message has been deleted.</p>"
 msgstr "<h4>Erfolg!</h4><p>Der Beitrag wurde gelöscht.</p>"
 
-#: aa_forum/views/forum.py:1296
+#: aa_forum/views/forum.py:1400
 msgid ""
 "<h4>Success!</h4><p>The message has been deleted.</p><p>This was the topics "
 "opening post, so the topic has been deleted as well.</p>"
 msgstr ""
 "<h4>Erfolg!</h4><p>Der Beitrag wurde gelöscht.</p><p>Dies war der "
 "Eröffnungsbeitrag des Themas, daher wurde das Thema ebenfalls gelöscht.</p>"
 
-#: aa_forum/views/personal_messages.py:104
+#: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr "<h4>Erfolg!</h4><p>Nachricht an {recipient_main_char} gesendet.</p>"
 
-#: aa_forum/views/personal_messages.py:190
+#: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Die Nachricht, auf die Du antworten willst, existiert "
 "entweder nicht oder Du bist nicht der Empfänger.</p>"
 
-#: aa_forum/views/personal_messages.py:226
+#: aa_forum/views/personal_messages.py:238
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Reply to {recipient_main_char} sent.</p>"
 msgstr "<h4>Erfolg!</h4><p>Antwort an {recipient_main_char} gesendet.</p>"
 
-#: aa_forum/views/personal_messages.py:282
-#: aa_forum/views/personal_messages.py:319
+#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:335
 msgid ""
 "<h4>Error!</h4><p>The message you tried to remove does either not exist or "
 "is not yours to remove.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Die Nachricht, die Du entfernen willst, existiert "
 "entweder nicht oder Du bist nicht berechtigt sie nicht entfernen.</p>"
 
-#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:314
 msgid "<h4>Success!</h4><p>Message removed from your inbox.</p>"
 msgstr "<h4>Erfolg!</h4><p>Nachricht aus Deinem Posteingang entfernt.</p>"
 
-#: aa_forum/views/personal_messages.py:337
+#: aa_forum/views/personal_messages.py:353
 msgid ""
 "<h4>Success!</h4><p>Message has been removed from your sent messages.</p>"
 msgstr "<h4>Erfolg!</h4><p>Nachricht aus Ihrem Postausgang entfernt.</p>"
 
-#: aa_forum/views/personal_messages.py:352
+#: aa_forum/views/personal_messages.py:368
 msgid "<h4>Error!</h4><p>Something went wrong.</p>"
 msgstr "<h4>Fehler!</h4><p>Etwas ist schief gelaufen.</p>"
 
-#: aa_forum/views/profile.py:58
+#: aa_forum/views/profile.py:60
 msgid "<h4>Success!</h4><p>Profile saved.</p>"
 msgstr "<h4>Erfolg!</h4><p>Profil gespeichert.</p>"
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/es/LC_MESSAGES/django.mo` & `aa_forum-2.1.0/aa_forum/locale/es/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-forum/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.4.3\n"
 
 msgid "Boards"
 msgstr "Tableros"
 
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
@@ -26,14 +26,17 @@
 
 msgid "Delete"
 msgstr "Borrar"
 
 msgid "Description"
 msgstr "Descripción"
 
+msgid "Discord webhook (optional)"
+msgstr "Discord Webhook (Opcional)"
+
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 "¿Quieres ayudar a traducir esta aplicación a tu idioma o mejorar la "
 "traducción existente?"
 
@@ -72,17 +75,14 @@
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
 "Esto restringirá el acceso a este tablero a los grupos seleccionados. Si no "
 "se selecciona ningún grupo, todos los que puedan acceder al foro también "
 "podrán acceder a este foro. (Esta configuración es opcional)"
 
-msgid "Toggle navigation"
-msgstr "Alternar la navegación"
-
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
 msgstr ""
 "Cuando se active, cada respuesta a cualquier tema en este foro se publicará "
 "en el canal de Discord definido. (los sub-tablones están excluidos) ¡Elija "
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/es/LC_MESSAGES/django.po` & `aa_forum-2.1.0/aa_forum/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,155 +1,155 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
 # Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023.
+# Mak3rco <depormanuf1@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 18:29+0200\n"
-"PO-Revision-Date: 2023-10-25 07:04+0000\n"
-"Last-Translator: Geovanny David Morales De la cruz <moralesgeovanny1996@gmail"
-".com>\n"
+"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"PO-Revision-Date: 2024-04-08 17:13+0000\n"
+"Last-Translator: Mak3rco <depormanuf1@gmail.com>\n"
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-forum/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.4.3\n"
 
-#: aa_forum/__init__.py:12 aa_forum/templates/aa_forum/base.html:5
-#: aa_forum/templates/aa_forum/partials/menu.html:14
+#: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
+#: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
-#: aa_forum/templates/aa_forum/view/forum/board.html:5
-#: aa_forum/templates/aa_forum/view/forum/index.html:6
+#: aa_forum/templates/aa_forum/view/forum/board.html:6
+#: aa_forum/templates/aa_forum/view/forum/index.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:8
-#: aa_forum/templates/aa_forum/view/forum/topic.html:5
+#: aa_forum/templates/aa_forum/view/forum/topic.html:6
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:7
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:9
-#: aa_forum/templates/aa_forum/view/profile/index.html:9
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
 msgstr "Foro"
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr ""
 
-#: aa_forum/forms.py:40
+#: aa_forum/forms.py:42
 msgid "This field is mandatory"
 msgstr "Este campo es obligatorio"
 
-#: aa_forum/forms.py:91 aa_forum/forms.py:93 aa_forum/forms.py:124
-#: aa_forum/forms.py:126 aa_forum/forms.py:502
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:26
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:26
+#: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
+#: aa_forum/forms.py:171 aa_forum/forms.py:616
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr "Asunto"
 
-#: aa_forum/forms.py:102 aa_forum/forms.py:321 aa_forum/forms.py:512
-#: aa_forum/forms.py:558
-msgid "Message"
-msgstr "Mensaje"
+#: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
+#: aa_forum/forms.py:730
+msgid "You have forgotten the message!"
+msgstr ""
 
-#: aa_forum/forms.py:145 aa_forum/forms.py:183 aa_forum/forms.py:204
+#: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
 msgstr "Nombre"
 
-#: aa_forum/forms.py:147 aa_forum/forms.py:185
+#: aa_forum/forms.py:192 aa_forum/forms.py:230
 #, fuzzy
 #| msgid "Category Name"
 msgid "Category name"
 msgstr "Nombre de la Categoría"
 
-#: aa_forum/forms.py:151 aa_forum/forms.py:162
+#: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
 msgstr "Tableros"
 
-#: aa_forum/forms.py:153
+#: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
 "Tableros a crear con esta categoría (Un tablero por línea). Estos tableros "
 "no tendrán restricciones de grupo, por lo que debe agregarlos más adelante "
 "cuando sea necesario."
 
-#: aa_forum/forms.py:206
+#: aa_forum/forms.py:251
 #, fuzzy
 #| msgid "Board Name"
 msgid "Board name"
 msgstr "Nombre del Tablón"
 
-#: aa_forum/forms.py:210
+#: aa_forum/forms.py:255
 msgid "Description"
 msgstr "Descripción"
 
-#: aa_forum/forms.py:216
+#: aa_forum/forms.py:261
 #, fuzzy
 #| msgid "Board Description (Optional)"
 msgid "Board description (optional)"
 msgstr "Descripción del Tablero (opcional)"
 
-#: aa_forum/forms.py:222
+#: aa_forum/forms.py:267
 msgid "Group restrictions"
 msgstr "Restricciones de grupo"
 
-#: aa_forum/forms.py:224
+#: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
 "Esto restringirá el acceso a este tablero a los grupos seleccionados. Si no "
 "se selecciona ningún grupo, todos los que puedan acceder al foro también "
 "podrán acceder a este foro. (Esta configuración es opcional)"
 
-#: aa_forum/forms.py:232
+#: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
-msgstr ""
+msgstr "Discord Webhook (Opcional)"
 
-#: aa_forum/forms.py:234
+#: aa_forum/forms.py:279
 msgid ""
 "Discord webhook URL for the channel to post about new topics in this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:247
+#: aa_forum/forms.py:292
 msgid "Use this Discord webhook for replies as well?"
 msgstr ""
 
-#: aa_forum/forms.py:249
+#: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
 msgstr ""
 "Cuando se active, cada respuesta a cualquier tema en este foro se publicará "
 "en el canal de Discord definido. (los sub-tablones están excluidos) ¡Elija "
 "sabiamente! (Predeterminado: NO)"
 
-#: aa_forum/forms.py:257
+#: aa_forum/forms.py:302
 #, fuzzy
 #| msgid "Mark Board as 'Announcement Board'"
 msgid "Mark board as \"Announcement Board\""
 msgstr "Marcar tablero como «Tablero de anuncios»"
 
-#: aa_forum/forms.py:259
+#: aa_forum/forms.py:304
 #, fuzzy
 #| msgid ""
 #| "Mark this board as an 'Announcement Board', meaning that only certain "
 #| "selected groups can start new topics. All others who have access to this "
 #| "board will still be able to discuss in the topics though. This setting "
 #| "will not be inherited to child boards. (Default: NO)"
 msgid ""
@@ -160,21 +160,21 @@
 msgstr ""
 "Marque este foro como «Tablero de anuncios», lo que significa que solo "
 "ciertos grupos seleccionados pueden iniciar nuevos temas. Sin embargo, todos "
 "los demás que tengan acceso a este foro aún podrán discutir los temas. Esta "
 "configuración no se heredará en los tableros secundarios. (Predeterminado: "
 "NO)"
 
-#: aa_forum/forms.py:267
+#: aa_forum/forms.py:312
 #, fuzzy
 #| msgid "Start Topic Restrictions for 'Announcement Boards'"
 msgid "Start topic restrictions for \"Announcement Boards\""
 msgstr "Restricciones del tema inicial para los «tablón de anuncios»"
 
-#: aa_forum/forms.py:269
+#: aa_forum/forms.py:314
 #, fuzzy
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
@@ -182,144 +182,178 @@
 "Los usuarios de al menos uno de los grupos seleccionados podrán iniciar "
 "temas en los «Tableros de anuncios». Si no se selecciona ningún grupo, sólo "
 "los administradores del foro podrán hacerlo. Esta configuración no se "
 "heredará en los tableros secundarios. (Sugerencia: estas restricciones solo "
 "entran en vigor cuando un tablero está marcado como «Tablero de anuncios», "
 "consulte la casilla de verificación arriba.)"
 
-#: aa_forum/forms.py:354
-msgid "Signature"
-msgstr "Firma"
+#: aa_forum/forms.py:362
+#, fuzzy
+#| msgid "Delete"
+msgid "Close topic"
+msgstr "Borrar"
 
-#: aa_forum/forms.py:355
-msgid "Your signature will appear below your posts."
-msgstr "Tu firma aparecerá debajo de tus publicaciones."
+#: aa_forum/forms.py:364
+msgid "If checked, this topic will be closed after posting this message."
+msgstr ""
 
-#: aa_forum/forms.py:359
+#: aa_forum/forms.py:370
+#, fuzzy
+#| msgid "Delete"
+msgid "Reopen topic"
+msgstr "Borrar"
+
+#: aa_forum/forms.py:372
+msgid "If checked, this topic will be reopened after posting this message."
+msgstr ""
+
+#: aa_forum/forms.py:409 aa_forum/forms.py:652 aa_forum/forms.py:717
+msgid "Message"
+msgstr "Mensaje"
+
+#: aa_forum/forms.py:446
 #, fuzzy
 #| msgid "Website Title"
 msgid "Website title"
 msgstr "Título de la página"
 
-#: aa_forum/forms.py:361
+#: aa_forum/forms.py:448
 msgid "e.g.: My Homepage"
 msgstr ""
 
-#: aa_forum/forms.py:362
+#: aa_forum/forms.py:449
 msgid "Your website's title."
 msgstr ""
 
-#: aa_forum/forms.py:366
+#: aa_forum/forms.py:453
 msgid "Website URL"
 msgstr ""
 
-#: aa_forum/forms.py:370
+#: aa_forum/forms.py:457
 msgid ""
 "Your website's URL. (Don't forget to also set a title for your website, "
 "otherwise this field will be ignored.)"
 msgstr ""
 
-#: aa_forum/forms.py:376
+#: aa_forum/forms.py:463
 msgid "PM me on Discord when I get a new personal message"
 msgstr ""
 
-#: aa_forum/forms.py:378
+#: aa_forum/forms.py:466
 msgid ""
 "Information: There is currently no module installed that can handle Discord "
 "direct messages. Have a chat with your IT guys to remedy this."
 msgstr ""
 
-#: aa_forum/forms.py:419
+#: aa_forum/forms.py:475
+msgid "Show unread topics as widget on the dashboard"
+msgstr ""
+
+#: aa_forum/forms.py:478
+msgid ""
+"Activating this setting will ad a widget to your dashboard that shows unread "
+"topics in the forum."
+msgstr ""
+
+#: aa_forum/forms.py:507
+msgid "Signature"
+msgstr "Firma"
+
+#: aa_forum/forms.py:508
+msgid "Your signature will appear below your posts."
+msgstr "Tu firma aparecerá debajo de tus publicaciones."
+
+#: aa_forum/forms.py:532
 msgid ""
 "Ensure your signature has at most {max_signature_length} characters. "
 "(Currently: {len(signature)})"
 msgstr ""
 
-#: aa_forum/forms.py:440
+#: aa_forum/forms.py:554
 msgid "This is not a valid URL"
 msgstr ""
 
-#: aa_forum/forms.py:456
+#: aa_forum/forms.py:570
 msgid ""
 "How many messages per page should be displayed in a forum topic? (Default: "
 "15)"
 msgstr ""
 
-#: aa_forum/forms.py:466
+#: aa_forum/forms.py:580
 msgid ""
 "How many topics per page should be displayed in a forum category? (Default: "
 "10)"
 msgstr ""
 
-#: aa_forum/forms.py:476
+#: aa_forum/forms.py:590
 msgid ""
 "How long (Number of characters) is a user's signature allowed to be? "
 "(Default: 750)"
 msgstr ""
 
-#: aa_forum/forms.py:498
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:22
+#: aa_forum/forms.py:612
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:21
 msgid "Recipient"
 msgstr ""
 
-#: aa_forum/forms.py:504
+#: aa_forum/forms.py:618
 msgid "Hello there …"
 msgstr ""
 
-#: aa_forum/models.py:127
+#: aa_forum/models.py:139
 msgid "AA-Forum"
 msgstr ""
 
-#: aa_forum/models.py:131
+#: aa_forum/models.py:143
 msgid "Can access the AA-Forum module"
 msgstr ""
 
-#: aa_forum/models.py:134
+#: aa_forum/models.py:146
 msgid "Can manage the AA-Forum module (Category, topics and messages)"
 msgstr ""
 
-#: aa_forum/models.py:177
+#: aa_forum/models.py:193
 msgid "category"
 msgstr ""
 
-#: aa_forum/models.py:178
+#: aa_forum/models.py:194
 msgid "categories"
 msgstr ""
 
-#: aa_forum/models.py:222
+#: aa_forum/models.py:248
 #, fuzzy
 #| msgid ""
 #| "When activated every reply to any topic in this board will be posted to "
 #| "the defined Discord channel. (Child boards are excluded) Chose wisely! "
 #| "(Default: NO)"
 msgid ""
 "Use this Discord webhook for replies as well? When activated every reply to "
 "any topic in this board will be posted to the defined Discord channel. "
 "(Child boards are excluded) Chose wisely! (Default: NO)"
 msgstr ""
 "Cuando se active, cada respuesta a cualquier tema en este foro se publicará "
 "en el canal de Discord definido. (los sub-tablones están excluidos) ¡Elija "
 "sabiamente! (Predeterminado: NO)"
 
-#: aa_forum/models.py:240
+#: aa_forum/models.py:266
 #, fuzzy
 #| msgid ""
 #| "This will restrict access to this board to the selected groups. If no "
 #| "groups are selected, everyone who can access the forum can also access "
 #| "this board. (This setting is optional)"
 msgid ""
 "User in at least one of these groups have access to this board. If no groups "
 "are selected, everyone with access to the forum has also access to this "
 "board."
 msgstr ""
 "Esto restringirá el acceso a este tablero a los grupos seleccionados. Si no "
 "se selecciona ningún grupo, todos los que puedan acceder al foro también "
 "podrán acceder a este foro. (Esta configuración es opcional)"
 
-#: aa_forum/models.py:248
+#: aa_forum/models.py:274
 #, fuzzy
 #| msgid ""
 #| "Mark this board as an 'Announcement Board', meaning that only certain "
 #| "selected groups can start new topics. All others who have access to this "
 #| "board will still be able to discuss in the topics though. This setting "
 #| "will not be inherited to child boards. (Default: NO)"
 msgid ""
@@ -329,15 +363,15 @@
 msgstr ""
 "Marque este foro como «Tablero de anuncios», lo que significa que solo "
 "ciertos grupos seleccionados pueden iniciar nuevos temas. Sin embargo, todos "
 "los demás que tengan acceso a este foro aún podrán discutir los temas. Esta "
 "configuración no se heredará en los tableros secundarios. (Predeterminado: "
 "NO)"
 
-#: aa_forum/models.py:259
+#: aa_forum/models.py:285
 #, fuzzy
 #| msgid ""
 #| "User in at least one of the selected groups will be able to start topics "
 #| "in 'Announcement Boards'. If no group is selected, only forum admins can "
 #| "do so. This setting will not be inherited to child boards. (Hint: These "
 #| "restrictions only take effect when a board is marked as 'Announcement "
 #| "Board', see checkbox above.)"
@@ -349,330 +383,341 @@
 "Los usuarios de al menos uno de los grupos seleccionados podrán iniciar "
 "temas en los «Tableros de anuncios». Si no se selecciona ningún grupo, sólo "
 "los administradores del foro podrán hacerlo. Esta configuración no se "
 "heredará en los tableros secundarios. (Sugerencia: estas restricciones solo "
 "entran en vigor cuando un tablero está marcado como «Tablero de anuncios», "
 "consulte la casilla de verificación arriba.)"
 
-#: aa_forum/models.py:295
+#: aa_forum/models.py:321
 msgid "board"
 msgstr ""
 
-#: aa_forum/models.py:296
+#: aa_forum/models.py:322
 msgid "boards"
 msgstr ""
 
-#: aa_forum/models.py:367
+#: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:578
+#: aa_forum/models.py:625
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:579
+#: aa_forum/models.py:626
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:736
+#: aa_forum/models.py:805
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:737
+#: aa_forum/models.py:806
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:872
+#: aa_forum/models.py:948
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:873
+#: aa_forum/models.py:949
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:920
+#: aa_forum/models.py:1003
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:921
+#: aa_forum/models.py:1004
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:922
+#: aa_forum/models.py:1005
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:927
+#: aa_forum/models.py:1010
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:932
+#: aa_forum/models.py:1015
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:937
+#: aa_forum/models.py:1020
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:1031
 msgid "setting"
 msgstr "ajuste"
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:1032
 msgid "settings"
 msgstr "ajustes"
 
-#: aa_forum/models.py:952
+#: aa_forum/models.py:1042
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:16
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 #, fuzzy
 #| msgid "settings"
 msgid "Forum settings"
 msgstr "ajustes"
 
-#: aa_forum/models.py:978
+#: aa_forum/models.py:1069
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:979
+#: aa_forum/models.py:1070
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:982
+#: aa_forum/models.py:1080
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:30
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:7
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:38
+#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:8
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:56
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:73
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:59
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:75
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:69
 #, fuzzy
 #| msgid "Delete"
 msgid "Delete message"
 msgstr "Borrar"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:13
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:8
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:23
 #, fuzzy
 #| msgid "Delete"
 msgid "Delete board"
 msgstr "Borrar"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
+msgid "Close"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:22
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:22
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:21
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:21
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:21
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:20
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:20
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:20
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:19
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:19
 msgid "This action cannot be undone!"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:29
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:29
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:28
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:28
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:28
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:27
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:27
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:34
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:34
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:33
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:33
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:33
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
 msgstr "Borrar"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:15
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:16
 msgid "Are you sure you want to delete this category?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:17
 msgid "This will also remove all boards, topics and messages in this category."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:13
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:39
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:84
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
 msgid "Unlock/re-open topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:16
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:42
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:88
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
 msgid "Lock/close topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
 msgid "Are you sure you want to lock/close this topic?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:3
 msgid "Change sticky state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:13
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:9
 msgid "Remove \"sticky\" state from topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:16
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:12
 msgid "Set \"sticky\" state for topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:22
 msgid "Are you sure you want to remove the sticky state from this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
 msgid ""
 "Are you sure you want to make this topic sticky, so it always shows up on "
 "top of the topic list?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:39
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:37
 msgid "Unset sticky"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:42
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:97
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
 #, fuzzy
 #| msgid "Delete"
 msgid "Delete topic"
 msgstr "Borrar"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:19
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:17
 msgid "This will also remove all messages in this topic."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:17
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:17
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:15
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:15
 msgid "Are you sure you want to delete this message?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:16
 msgid ""
 "If this message is the original post, then the entire topic will be removed "
 "as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:16
 msgid ""
 "If this message is the beginning of a conversation, all related messages "
 "will be removed as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:9
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:11
 msgid "Edit board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:22
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:36
 msgid ""
 "Changing the name of this board does not change its URL part. This will "
 "remain the same to not break any possible links into this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:58
 msgid "Change board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:56
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:70
 msgid "New child board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:63
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:62
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:77
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:84
 msgid ""
 "New boards will be added at the bottom of the board list for this category. "
 "You can move them via drag and drop to a position of your liking."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:79
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:75
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:93
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:97
 msgid "Create board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/categories.html:6
+#: aa_forum/templates/aa_forum/partials/administration/categories.html:5
 msgid ""
 "Here you can create, modify and delete categories and boards. You also can "
 "change their order via drag and drop."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:11
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:13
 msgid "Edit category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:19
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:35
 msgid "Expand/collapse category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:31
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:53
 msgid ""
 "Changing the name of this category does not change its URL part. This will "
 "remain the same to not break any possible links into this category."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:66
 msgid "Change category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:55
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:77
 msgid "New board"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:7
 msgid "Create new category"
 msgstr ""
 
@@ -687,24 +732,25 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:35
 msgid "Create category"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:21
-#: aa_forum/templates/aa_forum/partials/profile/form.html:21
+#: aa_forum/templates/aa_forum/partials/profile/form.html:22
 msgid "Submit"
 msgstr "Enviar"
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:6
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:7
 msgid "Forum index"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:27
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:49
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:51
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:6
 #, fuzzy
 #| msgid "Message"
 msgid "Modify message"
 msgstr "Mensaje"
 
@@ -729,67 +775,67 @@
 "¿Quieres ayudar a traducir esta aplicación a tu idioma o mejorar la "
 "traducción existente?"
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "¡Únete a nuestro equipo de traductores!"
 
-#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:9
+#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr "Los campos marcados con un asterisco son obligatorios"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:34
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:51
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
 msgid "New"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
 msgid "Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:66
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:65
 msgid "Unread"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:82
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:88
 msgid "Last post:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:86
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:25
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:96
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:26
 msgid "Re:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:103
 msgid "posted by:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:94
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:104
 msgid "posted at:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:7
+#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:8
 msgid "New topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/no-access.html:6
 msgid ""
 "You either don't have access to this board, or this board doesn't exist."
 msgstr ""
@@ -855,58 +901,58 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
 msgid "Last post"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:38
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:39
 msgid "Copy message link to clipboard"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:81
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:87
 msgid "Last modified:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:14
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:27
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:21
@@ -914,70 +960,67 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:6
 msgid "Modify topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:20
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:21
 msgid "Warning: this topic is locked! Only admins can reply."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:33
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:44
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
 msgid "Clear form"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:7
 msgid "Show all unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr "Alternar la navegación"
-
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:7
 msgid "Administration"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:12
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:13
 msgid "Categories and boards"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:6
-#: aa_forum/templates/aa_forum/view/profile/index.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:13
+#: aa_forum/templates/aa_forum/view/profile/index.html:7
 msgid "Profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:11
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:19
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:9
 msgid "Messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:23
 msgid "Inbox"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:18
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:18
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:17
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:17
 msgid "Date"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:22
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:21
 msgid "Sender"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:62
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:63
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:57
 #, fuzzy
 #| msgid "Message"
 msgid "Read message"
 msgstr "Mensaje"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:87
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:93
 msgid "No personal messages"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:8
 msgid "New personal message"
 msgstr ""
 
@@ -987,330 +1030,326 @@
 msgid "Send message"
 msgstr "Mensaje"
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:8
 msgid "Reply to:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:24
+#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:23
 msgid "Send reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:30
 #, fuzzy
 #| msgid "Message"
 msgid "Sent messages"
 msgstr "Mensaje"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:56
-msgid "Read Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:67
-msgid "Delete Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:81
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:87
 msgid "No personal messages sent"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:17
 #, fuzzy
 #| msgid "Message"
 msgid "New message"
 msgstr "Mensaje"
 
 #: aa_forum/templates/aa_forum/partials/profile/form.html:7
 msgid "User profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/search/search-form.html:7
+#: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+msgid "Forum: Unread topics"
+msgstr ""
+
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:6
 msgid "Administration (Forum settings)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:26
+#: aa_forum/templates/aa_forum/view/forum/index.html:27
 msgid "New posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:35
+#: aa_forum/templates/aa_forum/view/forum/index.html:36
 msgid "No new posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:22
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:21
 msgid "Start new topic in"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:38
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
 msgid "Start topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/topic.html:23
+#: aa_forum/templates/aa_forum/view/forum/topic.html:24
 msgid "Modify topic subject"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:6
 msgid "Unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:16
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:15
 msgid "Unread Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:31
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:30
 msgid "You have no unread topics …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:7
 msgid "Personal messages (Inbox)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:7
 msgid "Personal messages (New message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:39
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:35
 msgid "Enter the recipients name"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:7
 msgid "Personal messages (Reply to message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:7
 msgid "Personal messages (Sent messages)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:6
 msgid "Search results"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:22
+#: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:32
+#: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
-#: aa_forum/templatetags/aa_forum_datetime.py:57
+#: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
 msgstr ""
 
-#: aa_forum/views/admin.py:165
+#: aa_forum/views/admin.py:169
 msgid "<h4>Success!</h4><p>Category created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:205
+#: aa_forum/views/admin.py:212
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Category name changed from \"{category_name_old}\" to "
 "\"{category.name}\".</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:245
+#: aa_forum/views/admin.py:255
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Category \"{category_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:298 aa_forum/views/admin.py:354
+#: aa_forum/views/admin.py:311 aa_forum/views/admin.py:371
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{new_board.name}\" created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:409
+#: aa_forum/views/admin.py:430
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board.name}\" changed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:450
+#: aa_forum/views/admin.py:475
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:556
+#: aa_forum/views/admin.py:587
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:566 aa_forum/views/personal_messages.py:116
-#: aa_forum/views/personal_messages.py:237 aa_forum/views/profile.py:68
+#: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
+#: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:225
+#: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:282
+#: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:309
+#: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:329
+#: aa_forum/views/forum.py:340
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in is an announcement "
 "board and you don't have the permissions to start a topic there.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:386
+#: aa_forum/views/forum.py:399
 msgid ""
 "<h4>Error!</h4><p>Either subject or message is missing. Please make sure you "
 "enter both fields, as both fields are mandatory.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:442 aa_forum/views/forum.py:672
+#: aa_forum/views/forum.py:461 aa_forum/views/forum.py:706
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to view does not exist or you do "
 "not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:539
+#: aa_forum/views/forum.py:563
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to modify does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:561
+#: aa_forum/views/forum.py:585
 msgid "<h4>Error!</h4><p>You are not allowed to modify this topic!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:593
+#: aa_forum/views/forum.py:617
 msgid "<h4>Success!</h4><p>The topic subject has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:791
+#: aa_forum/views/forum.py:845
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to reply does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:847
+#: aa_forum/views/forum.py:922
 msgid "<h4>Error!</h4><p>Message field is mandatory and cannot be empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:856
+#: aa_forum/views/forum.py:931
 msgid "<h4>Error!</h4><p>Something went wrong, please try again.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:894
+#: aa_forum/views/forum.py:972
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been unlocked/re-opened.</"
 "p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:908
+#: aa_forum/views/forum.py:986
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been locked/closed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:949
+#: aa_forum/views/forum.py:1030
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{curent_topic}\" is no longer \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:963
+#: aa_forum/views/forum.py:1044
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{curent_topic}\" is now \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:998
+#: aa_forum/views/forum.py:1082
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{topic__subject}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1034
+#: aa_forum/views/forum.py:1124
 msgid "<h4>Error!</h4><p>The message doesn't exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1078
+#: aa_forum/views/forum.py:1174
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to modify does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1101
+#: aa_forum/views/forum.py:1197
 msgid "<h4>Error!</h4><p>You are not allowed to modify this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1128
+#: aa_forum/views/forum.py:1224
 msgid "<h4>Success!</h4><p>The message has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1151
+#: aa_forum/views/forum.py:1247
 msgid "<h4>Error!</h4><p>Mandatory form field is empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1241
+#: aa_forum/views/forum.py:1345
 msgid "<h4>Error!</h4><p>You are not allowed to delete this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1271
+#: aa_forum/views/forum.py:1375
 msgid "<h4>Success!</h4><p>The message has been deleted.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1296
+#: aa_forum/views/forum.py:1400
 msgid ""
 "<h4>Success!</h4><p>The message has been deleted.</p><p>This was the topics "
 "opening post, so the topic has been deleted as well.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:104
+#: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:190
+#: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:226
+#: aa_forum/views/personal_messages.py:238
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Reply to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:282
-#: aa_forum/views/personal_messages.py:319
+#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:335
 msgid ""
 "<h4>Error!</h4><p>The message you tried to remove does either not exist or "
 "is not yours to remove.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:314
 msgid "<h4>Success!</h4><p>Message removed from your inbox.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:337
+#: aa_forum/views/personal_messages.py:353
 msgid ""
 "<h4>Success!</h4><p>Message has been removed from your sent messages.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:352
+#: aa_forum/views/personal_messages.py:368
 msgid "<h4>Error!</h4><p>Something went wrong.</p>"
 msgstr ""
 
-#: aa_forum/views/profile.py:58
+#: aa_forum/views/profile.py:60
 msgid "<h4>Success!</h4><p>Profile saved.</p>"
 msgstr ""
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/fr_FR/LC_MESSAGES/django.po` & `aa_forum-2.1.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,588 +1,650 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# Author50CO <tkddlschry@gmail.com>, 2023.
+# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Mind of the Raven <okanieva@gmail.com>, 2024.
+# Rodpold Shard <rodpold@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 18:29+0200\n"
-"PO-Revision-Date: 2024-02-01 17:08+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/fr/>\n"
-"Language: fr_FR\n"
+"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"PO-Revision-Date: 2024-03-21 17:11+0000\n"
+"Last-Translator: Mind of the Raven <okanieva@gmail.com>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/ko/>\n"
+"Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 5.4.2\n"
 
-#: aa_forum/__init__.py:12 aa_forum/templates/aa_forum/base.html:5
-#: aa_forum/templates/aa_forum/partials/menu.html:14
+#: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
+#: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
-#: aa_forum/templates/aa_forum/view/forum/board.html:5
-#: aa_forum/templates/aa_forum/view/forum/index.html:6
+#: aa_forum/templates/aa_forum/view/forum/board.html:6
+#: aa_forum/templates/aa_forum/view/forum/index.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:8
-#: aa_forum/templates/aa_forum/view/forum/topic.html:5
+#: aa_forum/templates/aa_forum/view/forum/topic.html:6
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:7
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:9
-#: aa_forum/templates/aa_forum/view/profile/index.html:9
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
-msgstr ""
+msgstr "포럼"
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
-msgstr ""
+msgstr "AA 포럼 v{__version__}"
 
-#: aa_forum/forms.py:40
+#: aa_forum/forms.py:42
 msgid "This field is mandatory"
-msgstr "Ce champ est obligatoire"
+msgstr "필수 항목입니다"
 
-#: aa_forum/forms.py:91 aa_forum/forms.py:93 aa_forum/forms.py:124
-#: aa_forum/forms.py:126 aa_forum/forms.py:502
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:26
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:26
+#: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
+#: aa_forum/forms.py:171 aa_forum/forms.py:616
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
-msgstr ""
+msgstr "제목"
 
-#: aa_forum/forms.py:102 aa_forum/forms.py:321 aa_forum/forms.py:512
-#: aa_forum/forms.py:558
-msgid "Message"
-msgstr ""
+#: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
+#: aa_forum/forms.py:730
+msgid "You have forgotten the message!"
+msgstr "메시지를 잊으셨습니다!"
 
-#: aa_forum/forms.py:145 aa_forum/forms.py:183 aa_forum/forms.py:204
+#: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
-msgstr ""
+msgstr "이름"
 
-#: aa_forum/forms.py:147 aa_forum/forms.py:185
+#: aa_forum/forms.py:192 aa_forum/forms.py:230
 msgid "Category name"
-msgstr ""
+msgstr "카테고리 이름"
 
-#: aa_forum/forms.py:151 aa_forum/forms.py:162
+#: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
-msgstr ""
+msgstr "게시판"
 
-#: aa_forum/forms.py:153
+#: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
+"이 카테고리로(한 줄당 한 게시판) 게시판이 생성됩니다. 이 게시판은 그룹 제한"
+"이 없기 때문에 필요하면 나중에 추가할 수 있습니다."
 
-#: aa_forum/forms.py:206
+#: aa_forum/forms.py:251
 msgid "Board name"
-msgstr ""
+msgstr "게시판 이름"
 
-#: aa_forum/forms.py:210
+#: aa_forum/forms.py:255
 msgid "Description"
-msgstr ""
+msgstr "설명"
 
-#: aa_forum/forms.py:216
+#: aa_forum/forms.py:261
 msgid "Board description (optional)"
-msgstr ""
+msgstr "게시판 설명(선택사항)"
 
-#: aa_forum/forms.py:222
+#: aa_forum/forms.py:267
 msgid "Group restrictions"
-msgstr ""
+msgstr "그룹 제한"
 
-#: aa_forum/forms.py:224
+#: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
+"이렇게 진행할 경우 게시판 접근 권한이 선택한 그룹으로 제한됩니다. 선택하지 않"
+"을 경우 모든 사람이 이 게시판에 접근할 수 있습니다. (선택사항)"
 
-#: aa_forum/forms.py:232
+#: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:234
+#: aa_forum/forms.py:279
 msgid ""
 "Discord webhook URL for the channel to post about new topics in this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:247
+#: aa_forum/forms.py:292
 msgid "Use this Discord webhook for replies as well?"
 msgstr ""
 
-#: aa_forum/forms.py:249
+#: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
 msgstr ""
+"활성화할 경우 이 게시판 내 모든 게시글의 모든 답변이 정의된 디스코드 채널에 "
+"게시됩니다. (기본값:꺼짐)"
 
-#: aa_forum/forms.py:257
+#: aa_forum/forms.py:302
 msgid "Mark board as \"Announcement Board\""
-msgstr ""
+msgstr "선택된 게시글을 공지사항으로 등록"
 
-#: aa_forum/forms.py:259
+#: aa_forum/forms.py:304
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. This setting will "
 "not be inherited to child boards. (Default: NO)"
 msgstr ""
 
-#: aa_forum/forms.py:267
+#: aa_forum/forms.py:312
 msgid "Start topic restrictions for \"Announcement Boards\""
 msgstr ""
 
-#: aa_forum/forms.py:269
+#: aa_forum/forms.py:314
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
 msgstr ""
 
-#: aa_forum/forms.py:354
-msgid "Signature"
+#: aa_forum/forms.py:362
+#, fuzzy
+#| msgid "Delete"
+msgid "Close topic"
+msgstr "삭제"
+
+#: aa_forum/forms.py:364
+msgid "If checked, this topic will be closed after posting this message."
 msgstr ""
 
-#: aa_forum/forms.py:355
-msgid "Your signature will appear below your posts."
+#: aa_forum/forms.py:370
+#, fuzzy
+#| msgid "Delete"
+msgid "Reopen topic"
+msgstr "삭제"
+
+#: aa_forum/forms.py:372
+msgid "If checked, this topic will be reopened after posting this message."
 msgstr ""
 
-#: aa_forum/forms.py:359
+#: aa_forum/forms.py:409 aa_forum/forms.py:652 aa_forum/forms.py:717
+msgid "Message"
+msgstr "메시지"
+
+#: aa_forum/forms.py:446
 msgid "Website title"
 msgstr ""
 
-#: aa_forum/forms.py:361
+#: aa_forum/forms.py:448
 msgid "e.g.: My Homepage"
 msgstr ""
 
-#: aa_forum/forms.py:362
+#: aa_forum/forms.py:449
 msgid "Your website's title."
 msgstr ""
 
-#: aa_forum/forms.py:366
+#: aa_forum/forms.py:453
 msgid "Website URL"
 msgstr ""
 
-#: aa_forum/forms.py:370
+#: aa_forum/forms.py:457
 msgid ""
 "Your website's URL. (Don't forget to also set a title for your website, "
 "otherwise this field will be ignored.)"
 msgstr ""
 
-#: aa_forum/forms.py:376
+#: aa_forum/forms.py:463
 msgid "PM me on Discord when I get a new personal message"
 msgstr ""
 
-#: aa_forum/forms.py:378
+#: aa_forum/forms.py:466
 msgid ""
 "Information: There is currently no module installed that can handle Discord "
 "direct messages. Have a chat with your IT guys to remedy this."
 msgstr ""
 
-#: aa_forum/forms.py:419
+#: aa_forum/forms.py:475
+msgid "Show unread topics as widget on the dashboard"
+msgstr ""
+
+#: aa_forum/forms.py:478
+msgid ""
+"Activating this setting will ad a widget to your dashboard that shows unread "
+"topics in the forum."
+msgstr ""
+
+#: aa_forum/forms.py:507
+msgid "Signature"
+msgstr ""
+
+#: aa_forum/forms.py:508
+msgid "Your signature will appear below your posts."
+msgstr ""
+
+#: aa_forum/forms.py:532
 msgid ""
 "Ensure your signature has at most {max_signature_length} characters. "
 "(Currently: {len(signature)})"
 msgstr ""
 
-#: aa_forum/forms.py:440
+#: aa_forum/forms.py:554
 msgid "This is not a valid URL"
 msgstr ""
 
-#: aa_forum/forms.py:456
+#: aa_forum/forms.py:570
 msgid ""
 "How many messages per page should be displayed in a forum topic? (Default: "
 "15)"
 msgstr ""
 
-#: aa_forum/forms.py:466
+#: aa_forum/forms.py:580
 msgid ""
 "How many topics per page should be displayed in a forum category? (Default: "
 "10)"
 msgstr ""
 
-#: aa_forum/forms.py:476
+#: aa_forum/forms.py:590
 msgid ""
 "How long (Number of characters) is a user's signature allowed to be? "
 "(Default: 750)"
 msgstr ""
 
-#: aa_forum/forms.py:498
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:22
+#: aa_forum/forms.py:612
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:21
 msgid "Recipient"
 msgstr ""
 
-#: aa_forum/forms.py:504
+#: aa_forum/forms.py:618
 msgid "Hello there …"
 msgstr ""
 
-#: aa_forum/models.py:127
+#: aa_forum/models.py:139
 msgid "AA-Forum"
 msgstr ""
 
-#: aa_forum/models.py:131
+#: aa_forum/models.py:143
 msgid "Can access the AA-Forum module"
 msgstr ""
 
-#: aa_forum/models.py:134
+#: aa_forum/models.py:146
 msgid "Can manage the AA-Forum module (Category, topics and messages)"
 msgstr ""
 
-#: aa_forum/models.py:177
+#: aa_forum/models.py:193
 msgid "category"
 msgstr ""
 
-#: aa_forum/models.py:178
+#: aa_forum/models.py:194
 msgid "categories"
 msgstr ""
 
-#: aa_forum/models.py:222
+#: aa_forum/models.py:248
 msgid ""
 "Use this Discord webhook for replies as well? When activated every reply to "
 "any topic in this board will be posted to the defined Discord channel. "
 "(Child boards are excluded) Chose wisely! (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:240
+#: aa_forum/models.py:266
 msgid ""
 "User in at least one of these groups have access to this board. If no groups "
 "are selected, everyone with access to the forum has also access to this "
 "board."
 msgstr ""
 
-#: aa_forum/models.py:248
+#: aa_forum/models.py:274
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:259
+#: aa_forum/models.py:285
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so."
 msgstr ""
 
-#: aa_forum/models.py:295
+#: aa_forum/models.py:321
 msgid "board"
 msgstr ""
 
-#: aa_forum/models.py:296
+#: aa_forum/models.py:322
 msgid "boards"
 msgstr ""
 
-#: aa_forum/models.py:367
+#: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:578
+#: aa_forum/models.py:625
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:579
+#: aa_forum/models.py:626
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:736
+#: aa_forum/models.py:805
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:737
+#: aa_forum/models.py:806
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:872
+#: aa_forum/models.py:948
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:873
+#: aa_forum/models.py:949
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:920
+#: aa_forum/models.py:1003
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:921
+#: aa_forum/models.py:1004
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:922
+#: aa_forum/models.py:1005
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:927
+#: aa_forum/models.py:1010
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:932
+#: aa_forum/models.py:1015
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:937
+#: aa_forum/models.py:1020
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:1031
 msgid "setting"
-msgstr ""
+msgstr "설정"
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:1032
 msgid "settings"
-msgstr ""
+msgstr "설정"
 
-#: aa_forum/models.py:952
+#: aa_forum/models.py:1042
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:16
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
+#, fuzzy
+#| msgid "settings"
 msgid "Forum settings"
-msgstr ""
+msgstr "설정"
 
-#: aa_forum/models.py:978
+#: aa_forum/models.py:1069
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:979
+#: aa_forum/models.py:1070
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:982
+#: aa_forum/models.py:1080
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:30
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:7
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:38
+#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:8
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:56
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:73
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:59
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:75
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:69
+#, fuzzy
+#| msgid "Delete"
 msgid "Delete message"
-msgstr ""
+msgstr "삭제"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:13
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:8
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:23
+#, fuzzy
+#| msgid "Delete"
 msgid "Delete board"
-msgstr ""
+msgstr "삭제"
+
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
+msgid "Close"
+msgstr "닫기"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:22
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:22
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:21
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:21
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:21
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:20
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:20
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:20
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:19
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:19
 msgid "This action cannot be undone!"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:29
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:29
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:28
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:28
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:28
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:27
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:27
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
-msgstr ""
+msgstr "취소"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:34
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:34
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:33
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:33
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:33
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
-msgstr ""
+msgstr "삭제"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:15
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:16
 msgid "Are you sure you want to delete this category?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:17
 msgid "This will also remove all boards, topics and messages in this category."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:13
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:39
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:84
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
 msgid "Unlock/re-open topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:16
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:42
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:88
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
 msgid "Lock/close topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
 msgid "Are you sure you want to lock/close this topic?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:3
 msgid "Change sticky state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:13
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:9
 msgid "Remove \"sticky\" state from topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:16
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:12
 msgid "Set \"sticky\" state for topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:22
 msgid "Are you sure you want to remove the sticky state from this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
 msgid ""
 "Are you sure you want to make this topic sticky, so it always shows up on "
 "top of the topic list?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:39
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:37
 msgid "Unset sticky"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:42
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:97
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
+#, fuzzy
+#| msgid "Delete"
 msgid "Delete topic"
-msgstr ""
+msgstr "삭제"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:19
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:17
 msgid "This will also remove all messages in this topic."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:17
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:17
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:15
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:15
 msgid "Are you sure you want to delete this message?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:16
 msgid ""
 "If this message is the original post, then the entire topic will be removed "
 "as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:16
 msgid ""
 "If this message is the beginning of a conversation, all related messages "
 "will be removed as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:9
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:11
 msgid "Edit board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:22
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:36
 msgid ""
 "Changing the name of this board does not change its URL part. This will "
 "remain the same to not break any possible links into this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:58
 msgid "Change board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:56
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:70
 msgid "New child board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:63
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:62
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:77
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:84
 msgid ""
 "New boards will be added at the bottom of the board list for this category. "
 "You can move them via drag and drop to a position of your liking."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:79
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:75
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:93
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:97
 msgid "Create board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/categories.html:6
+#: aa_forum/templates/aa_forum/partials/administration/categories.html:5
 msgid ""
 "Here you can create, modify and delete categories and boards. You also can "
 "change their order via drag and drop."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:11
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:13
 msgid "Edit category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:19
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:35
 msgid "Expand/collapse category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:31
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:53
 msgid ""
 "Changing the name of this category does not change its URL part. This will "
 "remain the same to not break any possible links into this category."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:66
 msgid "Change category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:55
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:77
 msgid "New board"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:7
 msgid "Create new category"
 msgstr ""
 
@@ -597,28 +659,29 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:35
 msgid "Create category"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:21
-#: aa_forum/templates/aa_forum/partials/profile/form.html:21
+#: aa_forum/templates/aa_forum/partials/profile/form.html:22
 msgid "Submit"
-msgstr ""
+msgstr "전송"
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:6
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:7
 msgid "Forum index"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:27
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:49
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:51
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:6
 msgid "Modify message"
-msgstr ""
+msgstr "편집"
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:34
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:7
 msgid "Start new topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:40
@@ -629,75 +692,72 @@
 msgid "Search for:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr ""
-"Voulez-vous aider à traduire cette application dans votre langue ou "
-"améliorer la traduction existante ?"
+msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "Rejoignez notre équipe de traducteurs !"
+msgstr "번역가 팀에 참여하세요!"
 
-#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:9
+#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "Les champs marqués d'un astérisque (*) sont obligatoires"
+msgstr "별표 (*) 표시된 항목은 필수 항목입니다"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
-msgstr ""
+msgstr "작성된 게시글이 없습니다 . . ."
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:34
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
-msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:51
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
 msgid "New"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
 msgid "Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:66
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:65
 msgid "Unread"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:82
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:88
 msgid "Last post:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:86
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:25
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:96
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:26
 msgid "Re:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:103
 msgid "posted by:"
-msgstr ""
+msgstr "작성자:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:94
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:104
 msgid "posted at:"
-msgstr ""
+msgstr "작성 시간:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:7
+#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:8
 msgid "New topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/no-access.html:6
 msgid ""
 "You either don't have access to this board, or this board doesn't exist."
 msgstr ""
@@ -717,15 +777,15 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:10
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:39
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:10
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:39
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:9
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:38
 msgid "First"
-msgstr ""
+msgstr "첫 번째"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:20
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:24
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:46
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:22
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:26
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:48
@@ -735,482 +795,480 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:17
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:21
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:43
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:16
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:20
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:42
 msgid "Previous"
-msgstr ""
+msgstr "이전"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:63
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:74
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:76
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:60
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:71
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:60
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:71
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:59
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:70
 msgid "Next"
-msgstr ""
+msgstr "다음"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:69
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:78
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:71
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:80
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
-msgstr ""
+msgstr "마지막"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
 msgid "Last post"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:38
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:39
 msgid "Copy message link to clipboard"
-msgstr ""
+msgstr "복사"
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:81
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:87
 msgid "Last modified:"
-msgstr ""
+msgstr "편집일:"
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:14
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
 msgstr ""
+"참고 : 현재 이 게시글의 마지막 페이지에 있지 않음으로 최신 답글을 놓칠 수 있"
+"습니다."
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:27
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:21
 msgid "Modify"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:6
 msgid "Modify topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:20
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:21
 msgid "Warning: this topic is locked! Only admins can reply."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:33
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:44
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
 msgid "Clear form"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:7
 msgid "Show all unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:7
 msgid "Administration"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:12
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:13
 msgid "Categories and boards"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:6
-#: aa_forum/templates/aa_forum/view/profile/index.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:13
+#: aa_forum/templates/aa_forum/view/profile/index.html:7
 msgid "Profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:11
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:19
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:9
 msgid "Messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:23
 msgid "Inbox"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:18
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:18
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:17
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:17
 msgid "Date"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:22
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:21
 msgid "Sender"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:62
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:63
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:57
+#, fuzzy
+#| msgid "Message"
 msgid "Read message"
-msgstr ""
+msgstr "메시지"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:87
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:93
 msgid "No personal messages"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:8
 msgid "New personal message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:23
 msgid "Send message"
-msgstr ""
+msgstr "보내기"
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:8
 msgid "Reply to:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:24
+#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:23
 msgid "Send reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:30
 msgid "Sent messages"
-msgstr ""
+msgstr "발송된 메시지"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:56
-msgid "Read Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:67
-msgid "Delete Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:81
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:87
 msgid "No personal messages sent"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:17
+#, fuzzy
+#| msgid "Message"
 msgid "New message"
-msgstr ""
+msgstr "메시지"
 
 #: aa_forum/templates/aa_forum/partials/profile/form.html:7
 msgid "User profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/search/search-form.html:7
+#: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
+msgstr "검색 …"
+
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+msgid "Forum: Unread topics"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:6
 msgid "Administration (Forum settings)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:26
+#: aa_forum/templates/aa_forum/view/forum/index.html:27
 msgid "New posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:35
+#: aa_forum/templates/aa_forum/view/forum/index.html:36
 msgid "No new posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:22
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:21
 msgid "Start new topic in"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:38
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
 msgid "Start topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/topic.html:23
+#: aa_forum/templates/aa_forum/view/forum/topic.html:24
 msgid "Modify topic subject"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:6
 msgid "Unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:16
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:15
 msgid "Unread Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:31
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:30
 msgid "You have no unread topics …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:7
 msgid "Personal messages (Inbox)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:7
 msgid "Personal messages (New message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:39
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:35
 msgid "Enter the recipients name"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:7
 msgid "Personal messages (Reply to message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:7
 msgid "Personal messages (Sent messages)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:6
 msgid "Search results"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:22
+#: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
-msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:32
+#: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
-#: aa_forum/templatetags/aa_forum_datetime.py:57
+#: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
 msgstr ""
 
-#: aa_forum/views/admin.py:165
+#: aa_forum/views/admin.py:169
 msgid "<h4>Success!</h4><p>Category created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:205
+#: aa_forum/views/admin.py:212
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Category name changed from \"{category_name_old}\" to "
 "\"{category.name}\".</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:245
+#: aa_forum/views/admin.py:255
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Category \"{category_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:298 aa_forum/views/admin.py:354
+#: aa_forum/views/admin.py:311 aa_forum/views/admin.py:371
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{new_board.name}\" created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:409
+#: aa_forum/views/admin.py:430
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board.name}\" changed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:450
+#: aa_forum/views/admin.py:475
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:556
+#: aa_forum/views/admin.py:587
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:566 aa_forum/views/personal_messages.py:116
-#: aa_forum/views/personal_messages.py:237 aa_forum/views/profile.py:68
+#: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
+#: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:225
+#: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:282
+#: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:309
+#: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:329
+#: aa_forum/views/forum.py:340
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in is an announcement "
 "board and you don't have the permissions to start a topic there.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:386
+#: aa_forum/views/forum.py:399
 msgid ""
 "<h4>Error!</h4><p>Either subject or message is missing. Please make sure you "
 "enter both fields, as both fields are mandatory.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:442 aa_forum/views/forum.py:672
+#: aa_forum/views/forum.py:461 aa_forum/views/forum.py:706
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to view does not exist or you do "
 "not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:539
+#: aa_forum/views/forum.py:563
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to modify does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:561
+#: aa_forum/views/forum.py:585
 msgid "<h4>Error!</h4><p>You are not allowed to modify this topic!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:593
+#: aa_forum/views/forum.py:617
 msgid "<h4>Success!</h4><p>The topic subject has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:791
+#: aa_forum/views/forum.py:845
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to reply does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:847
+#: aa_forum/views/forum.py:922
 msgid "<h4>Error!</h4><p>Message field is mandatory and cannot be empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:856
+#: aa_forum/views/forum.py:931
 msgid "<h4>Error!</h4><p>Something went wrong, please try again.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:894
+#: aa_forum/views/forum.py:972
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been unlocked/re-opened.</"
 "p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:908
+#: aa_forum/views/forum.py:986
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been locked/closed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:949
+#: aa_forum/views/forum.py:1030
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{curent_topic}\" is no longer \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:963
+#: aa_forum/views/forum.py:1044
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{curent_topic}\" is now \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:998
+#: aa_forum/views/forum.py:1082
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{topic__subject}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1034
+#: aa_forum/views/forum.py:1124
 msgid "<h4>Error!</h4><p>The message doesn't exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1078
+#: aa_forum/views/forum.py:1174
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to modify does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1101
+#: aa_forum/views/forum.py:1197
 msgid "<h4>Error!</h4><p>You are not allowed to modify this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1128
+#: aa_forum/views/forum.py:1224
 msgid "<h4>Success!</h4><p>The message has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1151
+#: aa_forum/views/forum.py:1247
 msgid "<h4>Error!</h4><p>Mandatory form field is empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1241
+#: aa_forum/views/forum.py:1345
 msgid "<h4>Error!</h4><p>You are not allowed to delete this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1271
+#: aa_forum/views/forum.py:1375
 msgid "<h4>Success!</h4><p>The message has been deleted.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1296
+#: aa_forum/views/forum.py:1400
 msgid ""
 "<h4>Success!</h4><p>The message has been deleted.</p><p>This was the topics "
 "opening post, so the topic has been deleted as well.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:104
+#: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:190
+#: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:226
+#: aa_forum/views/personal_messages.py:238
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Reply to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:282
-#: aa_forum/views/personal_messages.py:319
+#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:335
 msgid ""
 "<h4>Error!</h4><p>The message you tried to remove does either not exist or "
 "is not yours to remove.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:314
 msgid "<h4>Success!</h4><p>Message removed from your inbox.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:337
+#: aa_forum/views/personal_messages.py:353
 msgid ""
 "<h4>Success!</h4><p>Message has been removed from your sent messages.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:352
+#: aa_forum/views/personal_messages.py:368
 msgid "<h4>Error!</h4><p>Something went wrong.</p>"
 msgstr ""
 
-#: aa_forum/views/profile.py:58
+#: aa_forum/views/profile.py:60
 msgid "<h4>Success!</h4><p>Profile saved.</p>"
 msgstr ""
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/it_IT/LC_MESSAGES/django.mo` & `aa_forum-2.1.0/aa_forum/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/it_IT/LC_MESSAGES/django.po` & `aa_forum-2.1.0/aa_forum/locale/django.pot`

 * *Files 4% similar despite different names*

```diff
@@ -1,588 +1,629 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 18:29+0200\n"
-"PO-Revision-Date: 2023-10-02 09:34+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/it/>\n"
-"Language: it_IT\n"
+"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=INTEGER; plural=EXPRESSION;\n"
 
-#: aa_forum/__init__.py:12 aa_forum/templates/aa_forum/base.html:5
-#: aa_forum/templates/aa_forum/partials/menu.html:14
+#: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
+#: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
-#: aa_forum/templates/aa_forum/view/forum/board.html:5
-#: aa_forum/templates/aa_forum/view/forum/index.html:6
+#: aa_forum/templates/aa_forum/view/forum/board.html:6
+#: aa_forum/templates/aa_forum/view/forum/index.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:8
-#: aa_forum/templates/aa_forum/view/forum/topic.html:5
+#: aa_forum/templates/aa_forum/view/forum/topic.html:6
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:7
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:9
-#: aa_forum/templates/aa_forum/view/profile/index.html:9
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
 msgstr ""
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr ""
 
-#: aa_forum/forms.py:40
+#: aa_forum/forms.py:42
 msgid "This field is mandatory"
-msgstr "Questo campo è obbligatorio"
+msgstr ""
 
-#: aa_forum/forms.py:91 aa_forum/forms.py:93 aa_forum/forms.py:124
-#: aa_forum/forms.py:126 aa_forum/forms.py:502
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:26
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:26
+#: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
+#: aa_forum/forms.py:171 aa_forum/forms.py:616
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr ""
 
-#: aa_forum/forms.py:102 aa_forum/forms.py:321 aa_forum/forms.py:512
-#: aa_forum/forms.py:558
-msgid "Message"
+#: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
+#: aa_forum/forms.py:730
+msgid "You have forgotten the message!"
 msgstr ""
 
-#: aa_forum/forms.py:145 aa_forum/forms.py:183 aa_forum/forms.py:204
+#: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
 msgstr ""
 
-#: aa_forum/forms.py:147 aa_forum/forms.py:185
+#: aa_forum/forms.py:192 aa_forum/forms.py:230
 msgid "Category name"
 msgstr ""
 
-#: aa_forum/forms.py:151 aa_forum/forms.py:162
+#: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
 msgstr ""
 
-#: aa_forum/forms.py:153
+#: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
 
-#: aa_forum/forms.py:206
+#: aa_forum/forms.py:251
 msgid "Board name"
 msgstr ""
 
-#: aa_forum/forms.py:210
+#: aa_forum/forms.py:255
 msgid "Description"
 msgstr ""
 
-#: aa_forum/forms.py:216
+#: aa_forum/forms.py:261
 msgid "Board description (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:222
+#: aa_forum/forms.py:267
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_forum/forms.py:224
+#: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:232
+#: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:234
+#: aa_forum/forms.py:279
 msgid ""
 "Discord webhook URL for the channel to post about new topics in this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:247
+#: aa_forum/forms.py:292
 msgid "Use this Discord webhook for replies as well?"
 msgstr ""
 
-#: aa_forum/forms.py:249
+#: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
 msgstr ""
 
-#: aa_forum/forms.py:257
+#: aa_forum/forms.py:302
 msgid "Mark board as \"Announcement Board\""
 msgstr ""
 
-#: aa_forum/forms.py:259
+#: aa_forum/forms.py:304
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. This setting will "
 "not be inherited to child boards. (Default: NO)"
 msgstr ""
 
-#: aa_forum/forms.py:267
+#: aa_forum/forms.py:312
 msgid "Start topic restrictions for \"Announcement Boards\""
 msgstr ""
 
-#: aa_forum/forms.py:269
+#: aa_forum/forms.py:314
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
 msgstr ""
 
-#: aa_forum/forms.py:354
-msgid "Signature"
+#: aa_forum/forms.py:362
+msgid "Close topic"
 msgstr ""
 
-#: aa_forum/forms.py:355
-msgid "Your signature will appear below your posts."
+#: aa_forum/forms.py:364
+msgid "If checked, this topic will be closed after posting this message."
+msgstr ""
+
+#: aa_forum/forms.py:370
+msgid "Reopen topic"
+msgstr ""
+
+#: aa_forum/forms.py:372
+msgid "If checked, this topic will be reopened after posting this message."
+msgstr ""
+
+#: aa_forum/forms.py:409 aa_forum/forms.py:652 aa_forum/forms.py:717
+msgid "Message"
 msgstr ""
 
-#: aa_forum/forms.py:359
+#: aa_forum/forms.py:446
 msgid "Website title"
 msgstr ""
 
-#: aa_forum/forms.py:361
+#: aa_forum/forms.py:448
 msgid "e.g.: My Homepage"
 msgstr ""
 
-#: aa_forum/forms.py:362
+#: aa_forum/forms.py:449
 msgid "Your website's title."
 msgstr ""
 
-#: aa_forum/forms.py:366
+#: aa_forum/forms.py:453
 msgid "Website URL"
 msgstr ""
 
-#: aa_forum/forms.py:370
+#: aa_forum/forms.py:457
 msgid ""
 "Your website's URL. (Don't forget to also set a title for your website, "
 "otherwise this field will be ignored.)"
 msgstr ""
 
-#: aa_forum/forms.py:376
+#: aa_forum/forms.py:463
 msgid "PM me on Discord when I get a new personal message"
 msgstr ""
 
-#: aa_forum/forms.py:378
+#: aa_forum/forms.py:466
 msgid ""
 "Information: There is currently no module installed that can handle Discord "
 "direct messages. Have a chat with your IT guys to remedy this."
 msgstr ""
 
-#: aa_forum/forms.py:419
+#: aa_forum/forms.py:475
+msgid "Show unread topics as widget on the dashboard"
+msgstr ""
+
+#: aa_forum/forms.py:478
+msgid ""
+"Activating this setting will ad a widget to your dashboard that shows unread "
+"topics in the forum."
+msgstr ""
+
+#: aa_forum/forms.py:507
+msgid "Signature"
+msgstr ""
+
+#: aa_forum/forms.py:508
+msgid "Your signature will appear below your posts."
+msgstr ""
+
+#: aa_forum/forms.py:532
 msgid ""
 "Ensure your signature has at most {max_signature_length} characters. "
 "(Currently: {len(signature)})"
 msgstr ""
 
-#: aa_forum/forms.py:440
+#: aa_forum/forms.py:554
 msgid "This is not a valid URL"
 msgstr ""
 
-#: aa_forum/forms.py:456
+#: aa_forum/forms.py:570
 msgid ""
 "How many messages per page should be displayed in a forum topic? (Default: "
 "15)"
 msgstr ""
 
-#: aa_forum/forms.py:466
+#: aa_forum/forms.py:580
 msgid ""
 "How many topics per page should be displayed in a forum category? (Default: "
 "10)"
 msgstr ""
 
-#: aa_forum/forms.py:476
+#: aa_forum/forms.py:590
 msgid ""
 "How long (Number of characters) is a user's signature allowed to be? "
 "(Default: 750)"
 msgstr ""
 
-#: aa_forum/forms.py:498
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:22
+#: aa_forum/forms.py:612
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:21
 msgid "Recipient"
 msgstr ""
 
-#: aa_forum/forms.py:504
+#: aa_forum/forms.py:618
 msgid "Hello there …"
 msgstr ""
 
-#: aa_forum/models.py:127
+#: aa_forum/models.py:139
 msgid "AA-Forum"
 msgstr ""
 
-#: aa_forum/models.py:131
+#: aa_forum/models.py:143
 msgid "Can access the AA-Forum module"
 msgstr ""
 
-#: aa_forum/models.py:134
+#: aa_forum/models.py:146
 msgid "Can manage the AA-Forum module (Category, topics and messages)"
 msgstr ""
 
-#: aa_forum/models.py:177
+#: aa_forum/models.py:193
 msgid "category"
 msgstr ""
 
-#: aa_forum/models.py:178
+#: aa_forum/models.py:194
 msgid "categories"
 msgstr ""
 
-#: aa_forum/models.py:222
+#: aa_forum/models.py:248
 msgid ""
 "Use this Discord webhook for replies as well? When activated every reply to "
 "any topic in this board will be posted to the defined Discord channel. "
 "(Child boards are excluded) Chose wisely! (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:240
+#: aa_forum/models.py:266
 msgid ""
 "User in at least one of these groups have access to this board. If no groups "
 "are selected, everyone with access to the forum has also access to this "
 "board."
 msgstr ""
 
-#: aa_forum/models.py:248
+#: aa_forum/models.py:274
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:259
+#: aa_forum/models.py:285
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so."
 msgstr ""
 
-#: aa_forum/models.py:295
+#: aa_forum/models.py:321
 msgid "board"
 msgstr ""
 
-#: aa_forum/models.py:296
+#: aa_forum/models.py:322
 msgid "boards"
 msgstr ""
 
-#: aa_forum/models.py:367
+#: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:578
+#: aa_forum/models.py:625
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:579
+#: aa_forum/models.py:626
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:736
+#: aa_forum/models.py:805
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:737
+#: aa_forum/models.py:806
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:872
+#: aa_forum/models.py:948
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:873
+#: aa_forum/models.py:949
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:920
+#: aa_forum/models.py:1003
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:921
+#: aa_forum/models.py:1004
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:922
+#: aa_forum/models.py:1005
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:927
+#: aa_forum/models.py:1010
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:932
+#: aa_forum/models.py:1015
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:937
+#: aa_forum/models.py:1020
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:1031
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:1032
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:952
+#: aa_forum/models.py:1042
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:16
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:978
+#: aa_forum/models.py:1069
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:979
+#: aa_forum/models.py:1070
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:982
+#: aa_forum/models.py:1080
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:30
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:7
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:38
+#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:8
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:56
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:73
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:59
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:75
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:69
 msgid "Delete message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:13
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:8
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:23
 msgid "Delete board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
+msgid "Close"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:22
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:22
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:21
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:21
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:21
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:20
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:20
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:20
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:19
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:19
 msgid "This action cannot be undone!"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:29
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:29
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:28
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:28
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:28
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:27
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:27
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:34
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:34
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:33
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:33
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:33
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:15
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:16
 msgid "Are you sure you want to delete this category?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:17
 msgid "This will also remove all boards, topics and messages in this category."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:13
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:39
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:84
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
 msgid "Unlock/re-open topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:16
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:42
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:88
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
 msgid "Lock/close topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
 msgid "Are you sure you want to lock/close this topic?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:3
 msgid "Change sticky state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:13
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:9
 msgid "Remove \"sticky\" state from topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:16
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:12
 msgid "Set \"sticky\" state for topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:22
 msgid "Are you sure you want to remove the sticky state from this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
 msgid ""
 "Are you sure you want to make this topic sticky, so it always shows up on "
 "top of the topic list?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:39
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:37
 msgid "Unset sticky"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:42
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:97
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
 msgid "Delete topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:19
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:17
 msgid "This will also remove all messages in this topic."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:17
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:17
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:15
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:15
 msgid "Are you sure you want to delete this message?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:16
 msgid ""
 "If this message is the original post, then the entire topic will be removed "
 "as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:16
 msgid ""
 "If this message is the beginning of a conversation, all related messages "
 "will be removed as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:9
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:11
 msgid "Edit board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:22
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:36
 msgid ""
 "Changing the name of this board does not change its URL part. This will "
 "remain the same to not break any possible links into this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:58
 msgid "Change board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:56
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:70
 msgid "New child board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:63
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:62
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:77
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:84
 msgid ""
 "New boards will be added at the bottom of the board list for this category. "
 "You can move them via drag and drop to a position of your liking."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:79
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:75
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:93
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:97
 msgid "Create board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/categories.html:6
+#: aa_forum/templates/aa_forum/partials/administration/categories.html:5
 msgid ""
 "Here you can create, modify and delete categories and boards. You also can "
 "change their order via drag and drop."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:11
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:13
 msgid "Edit category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:19
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:35
 msgid "Expand/collapse category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:31
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:53
 msgid ""
 "Changing the name of this category does not change its URL part. This will "
 "remain the same to not break any possible links into this category."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:66
 msgid "Change category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:55
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:77
 msgid "New board"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:7
 msgid "Create new category"
 msgstr ""
 
@@ -597,24 +638,25 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:35
 msgid "Create category"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:21
-#: aa_forum/templates/aa_forum/partials/profile/form.html:21
+#: aa_forum/templates/aa_forum/partials/profile/form.html:22
 msgid "Submit"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:6
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:7
 msgid "Forum index"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:27
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:49
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:51
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:6
 msgid "Modify message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:34
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:7
@@ -635,67 +677,67 @@
 "existing translation?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:9
+#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "I campi contrassegnati da un asterisco (*) sono obbligatori"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:34
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:51
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
 msgid "New"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
 msgid "Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:66
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:65
 msgid "Unread"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:82
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:88
 msgid "Last post:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:86
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:25
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:96
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:26
 msgid "Re:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:103
 msgid "posted by:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:94
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:104
 msgid "posted at:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:7
+#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:8
 msgid "New topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/no-access.html:6
 msgid ""
 "You either don't have access to this board, or this board doesn't exist."
 msgstr ""
@@ -761,58 +803,58 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
 msgid "Last post"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:38
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:39
 msgid "Copy message link to clipboard"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:81
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:87
 msgid "Last modified:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:14
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:27
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:21
@@ -820,68 +862,65 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:6
 msgid "Modify topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:20
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:21
 msgid "Warning: this topic is locked! Only admins can reply."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:33
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:44
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
 msgid "Clear form"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:7
 msgid "Show all unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:7
 msgid "Administration"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:12
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:13
 msgid "Categories and boards"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:6
-#: aa_forum/templates/aa_forum/view/profile/index.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:13
+#: aa_forum/templates/aa_forum/view/profile/index.html:7
 msgid "Profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:11
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:19
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:9
 msgid "Messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:23
 msgid "Inbox"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:18
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:18
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:17
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:17
 msgid "Date"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:22
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:21
 msgid "Sender"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:62
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:63
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:57
 msgid "Read message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:87
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:93
 msgid "No personal messages"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:8
 msgid "New personal message"
 msgstr ""
 
@@ -889,326 +928,322 @@
 msgid "Send message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:8
 msgid "Reply to:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:24
+#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:23
 msgid "Send reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:30
 msgid "Sent messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:56
-msgid "Read Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:67
-msgid "Delete Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:81
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:87
 msgid "No personal messages sent"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:17
 msgid "New message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/profile/form.html:7
 msgid "User profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/search/search-form.html:7
+#: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+msgid "Forum: Unread topics"
+msgstr ""
+
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:6
 msgid "Administration (Forum settings)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:26
+#: aa_forum/templates/aa_forum/view/forum/index.html:27
 msgid "New posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:35
+#: aa_forum/templates/aa_forum/view/forum/index.html:36
 msgid "No new posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:22
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:21
 msgid "Start new topic in"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:38
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
 msgid "Start topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/topic.html:23
+#: aa_forum/templates/aa_forum/view/forum/topic.html:24
 msgid "Modify topic subject"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:6
 msgid "Unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:16
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:15
 msgid "Unread Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:31
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:30
 msgid "You have no unread topics …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:7
 msgid "Personal messages (Inbox)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:7
 msgid "Personal messages (New message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:39
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:35
 msgid "Enter the recipients name"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:7
 msgid "Personal messages (Reply to message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:7
 msgid "Personal messages (Sent messages)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:6
 msgid "Search results"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:22
+#: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:32
+#: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
-#: aa_forum/templatetags/aa_forum_datetime.py:57
+#: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
 msgstr ""
 
-#: aa_forum/views/admin.py:165
+#: aa_forum/views/admin.py:169
 msgid "<h4>Success!</h4><p>Category created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:205
+#: aa_forum/views/admin.py:212
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Category name changed from \"{category_name_old}\" to "
 "\"{category.name}\".</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:245
+#: aa_forum/views/admin.py:255
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Category \"{category_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:298 aa_forum/views/admin.py:354
+#: aa_forum/views/admin.py:311 aa_forum/views/admin.py:371
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{new_board.name}\" created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:409
+#: aa_forum/views/admin.py:430
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board.name}\" changed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:450
+#: aa_forum/views/admin.py:475
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:556
+#: aa_forum/views/admin.py:587
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:566 aa_forum/views/personal_messages.py:116
-#: aa_forum/views/personal_messages.py:237 aa_forum/views/profile.py:68
+#: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
+#: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:225
+#: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:282
+#: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:309
+#: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:329
+#: aa_forum/views/forum.py:340
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in is an announcement "
 "board and you don't have the permissions to start a topic there.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:386
+#: aa_forum/views/forum.py:399
 msgid ""
 "<h4>Error!</h4><p>Either subject or message is missing. Please make sure you "
 "enter both fields, as both fields are mandatory.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:442 aa_forum/views/forum.py:672
+#: aa_forum/views/forum.py:461 aa_forum/views/forum.py:706
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to view does not exist or you do "
 "not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:539
+#: aa_forum/views/forum.py:563
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to modify does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:561
+#: aa_forum/views/forum.py:585
 msgid "<h4>Error!</h4><p>You are not allowed to modify this topic!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:593
+#: aa_forum/views/forum.py:617
 msgid "<h4>Success!</h4><p>The topic subject has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:791
+#: aa_forum/views/forum.py:845
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to reply does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:847
+#: aa_forum/views/forum.py:922
 msgid "<h4>Error!</h4><p>Message field is mandatory and cannot be empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:856
+#: aa_forum/views/forum.py:931
 msgid "<h4>Error!</h4><p>Something went wrong, please try again.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:894
+#: aa_forum/views/forum.py:972
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been unlocked/re-opened.</"
 "p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:908
+#: aa_forum/views/forum.py:986
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been locked/closed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:949
+#: aa_forum/views/forum.py:1030
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{curent_topic}\" is no longer \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:963
+#: aa_forum/views/forum.py:1044
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{curent_topic}\" is now \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:998
+#: aa_forum/views/forum.py:1082
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{topic__subject}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1034
+#: aa_forum/views/forum.py:1124
 msgid "<h4>Error!</h4><p>The message doesn't exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1078
+#: aa_forum/views/forum.py:1174
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to modify does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1101
+#: aa_forum/views/forum.py:1197
 msgid "<h4>Error!</h4><p>You are not allowed to modify this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1128
+#: aa_forum/views/forum.py:1224
 msgid "<h4>Success!</h4><p>The message has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1151
+#: aa_forum/views/forum.py:1247
 msgid "<h4>Error!</h4><p>Mandatory form field is empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1241
+#: aa_forum/views/forum.py:1345
 msgid "<h4>Error!</h4><p>You are not allowed to delete this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1271
+#: aa_forum/views/forum.py:1375
 msgid "<h4>Success!</h4><p>The message has been deleted.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1296
+#: aa_forum/views/forum.py:1400
 msgid ""
 "<h4>Success!</h4><p>The message has been deleted.</p><p>This was the topics "
 "opening post, so the topic has been deleted as well.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:104
+#: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:190
+#: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:226
+#: aa_forum/views/personal_messages.py:238
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Reply to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:282
-#: aa_forum/views/personal_messages.py:319
+#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:335
 msgid ""
 "<h4>Error!</h4><p>The message you tried to remove does either not exist or "
 "is not yours to remove.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:314
 msgid "<h4>Success!</h4><p>Message removed from your inbox.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:337
+#: aa_forum/views/personal_messages.py:353
 msgid ""
 "<h4>Success!</h4><p>Message has been removed from your sent messages.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:352
+#: aa_forum/views/personal_messages.py:368
 msgid "<h4>Error!</h4><p>Something went wrong.</p>"
 msgstr ""
 
-#: aa_forum/views/profile.py:58
+#: aa_forum/views/profile.py:60
 msgid "<h4>Success!</h4><p>Profile saved.</p>"
 msgstr ""
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/ja/LC_MESSAGES/django.po` & `aa_forum-2.1.0/aa_forum/locale/cs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,589 +1,630 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 18:29+0200\n"
-"PO-Revision-Date: 2023-10-02 09:34+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/ja/>\n"
-"Language: ja\n"
+"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
-#: aa_forum/__init__.py:12 aa_forum/templates/aa_forum/base.html:5
-#: aa_forum/templates/aa_forum/partials/menu.html:14
+#: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
+#: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
-#: aa_forum/templates/aa_forum/view/forum/board.html:5
-#: aa_forum/templates/aa_forum/view/forum/index.html:6
+#: aa_forum/templates/aa_forum/view/forum/board.html:6
+#: aa_forum/templates/aa_forum/view/forum/index.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:8
-#: aa_forum/templates/aa_forum/view/forum/topic.html:5
+#: aa_forum/templates/aa_forum/view/forum/topic.html:6
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:7
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:9
-#: aa_forum/templates/aa_forum/view/profile/index.html:9
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
 msgstr ""
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr ""
 
-#: aa_forum/forms.py:40
+#: aa_forum/forms.py:42
 msgid "This field is mandatory"
 msgstr ""
 
-#: aa_forum/forms.py:91 aa_forum/forms.py:93 aa_forum/forms.py:124
-#: aa_forum/forms.py:126 aa_forum/forms.py:502
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:26
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:26
+#: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
+#: aa_forum/forms.py:171 aa_forum/forms.py:616
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr ""
 
-#: aa_forum/forms.py:102 aa_forum/forms.py:321 aa_forum/forms.py:512
-#: aa_forum/forms.py:558
-msgid "Message"
+#: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
+#: aa_forum/forms.py:730
+msgid "You have forgotten the message!"
 msgstr ""
 
-#: aa_forum/forms.py:145 aa_forum/forms.py:183 aa_forum/forms.py:204
+#: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
 msgstr ""
 
-#: aa_forum/forms.py:147 aa_forum/forms.py:185
+#: aa_forum/forms.py:192 aa_forum/forms.py:230
 msgid "Category name"
 msgstr ""
 
-#: aa_forum/forms.py:151 aa_forum/forms.py:162
+#: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
 msgstr ""
 
-#: aa_forum/forms.py:153
+#: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
 
-#: aa_forum/forms.py:206
+#: aa_forum/forms.py:251
 msgid "Board name"
 msgstr ""
 
-#: aa_forum/forms.py:210
+#: aa_forum/forms.py:255
 msgid "Description"
 msgstr ""
 
-#: aa_forum/forms.py:216
+#: aa_forum/forms.py:261
 msgid "Board description (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:222
+#: aa_forum/forms.py:267
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_forum/forms.py:224
+#: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:232
+#: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:234
+#: aa_forum/forms.py:279
 msgid ""
 "Discord webhook URL for the channel to post about new topics in this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:247
+#: aa_forum/forms.py:292
 msgid "Use this Discord webhook for replies as well?"
 msgstr ""
 
-#: aa_forum/forms.py:249
+#: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
 msgstr ""
 
-#: aa_forum/forms.py:257
+#: aa_forum/forms.py:302
 msgid "Mark board as \"Announcement Board\""
 msgstr ""
 
-#: aa_forum/forms.py:259
+#: aa_forum/forms.py:304
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. This setting will "
 "not be inherited to child boards. (Default: NO)"
 msgstr ""
 
-#: aa_forum/forms.py:267
+#: aa_forum/forms.py:312
 msgid "Start topic restrictions for \"Announcement Boards\""
 msgstr ""
 
-#: aa_forum/forms.py:269
+#: aa_forum/forms.py:314
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
 msgstr ""
 
-#: aa_forum/forms.py:354
-msgid "Signature"
+#: aa_forum/forms.py:362
+msgid "Close topic"
 msgstr ""
 
-#: aa_forum/forms.py:355
-msgid "Your signature will appear below your posts."
+#: aa_forum/forms.py:364
+msgid "If checked, this topic will be closed after posting this message."
+msgstr ""
+
+#: aa_forum/forms.py:370
+msgid "Reopen topic"
+msgstr ""
+
+#: aa_forum/forms.py:372
+msgid "If checked, this topic will be reopened after posting this message."
 msgstr ""
 
-#: aa_forum/forms.py:359
+#: aa_forum/forms.py:409 aa_forum/forms.py:652 aa_forum/forms.py:717
+msgid "Message"
+msgstr ""
+
+#: aa_forum/forms.py:446
 msgid "Website title"
 msgstr ""
 
-#: aa_forum/forms.py:361
+#: aa_forum/forms.py:448
 msgid "e.g.: My Homepage"
 msgstr ""
 
-#: aa_forum/forms.py:362
+#: aa_forum/forms.py:449
 msgid "Your website's title."
 msgstr ""
 
-#: aa_forum/forms.py:366
+#: aa_forum/forms.py:453
 msgid "Website URL"
 msgstr ""
 
-#: aa_forum/forms.py:370
+#: aa_forum/forms.py:457
 msgid ""
 "Your website's URL. (Don't forget to also set a title for your website, "
 "otherwise this field will be ignored.)"
 msgstr ""
 
-#: aa_forum/forms.py:376
+#: aa_forum/forms.py:463
 msgid "PM me on Discord when I get a new personal message"
 msgstr ""
 
-#: aa_forum/forms.py:378
+#: aa_forum/forms.py:466
 msgid ""
 "Information: There is currently no module installed that can handle Discord "
 "direct messages. Have a chat with your IT guys to remedy this."
 msgstr ""
 
-#: aa_forum/forms.py:419
+#: aa_forum/forms.py:475
+msgid "Show unread topics as widget on the dashboard"
+msgstr ""
+
+#: aa_forum/forms.py:478
+msgid ""
+"Activating this setting will ad a widget to your dashboard that shows unread "
+"topics in the forum."
+msgstr ""
+
+#: aa_forum/forms.py:507
+msgid "Signature"
+msgstr ""
+
+#: aa_forum/forms.py:508
+msgid "Your signature will appear below your posts."
+msgstr ""
+
+#: aa_forum/forms.py:532
 msgid ""
 "Ensure your signature has at most {max_signature_length} characters. "
 "(Currently: {len(signature)})"
 msgstr ""
 
-#: aa_forum/forms.py:440
+#: aa_forum/forms.py:554
 msgid "This is not a valid URL"
 msgstr ""
 
-#: aa_forum/forms.py:456
+#: aa_forum/forms.py:570
 msgid ""
 "How many messages per page should be displayed in a forum topic? (Default: "
 "15)"
 msgstr ""
 
-#: aa_forum/forms.py:466
+#: aa_forum/forms.py:580
 msgid ""
 "How many topics per page should be displayed in a forum category? (Default: "
 "10)"
 msgstr ""
 
-#: aa_forum/forms.py:476
+#: aa_forum/forms.py:590
 msgid ""
 "How long (Number of characters) is a user's signature allowed to be? "
 "(Default: 750)"
 msgstr ""
 
-#: aa_forum/forms.py:498
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:22
+#: aa_forum/forms.py:612
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:21
 msgid "Recipient"
 msgstr ""
 
-#: aa_forum/forms.py:504
+#: aa_forum/forms.py:618
 msgid "Hello there …"
 msgstr ""
 
-#: aa_forum/models.py:127
+#: aa_forum/models.py:139
 msgid "AA-Forum"
 msgstr ""
 
-#: aa_forum/models.py:131
+#: aa_forum/models.py:143
 msgid "Can access the AA-Forum module"
 msgstr ""
 
-#: aa_forum/models.py:134
+#: aa_forum/models.py:146
 msgid "Can manage the AA-Forum module (Category, topics and messages)"
 msgstr ""
 
-#: aa_forum/models.py:177
+#: aa_forum/models.py:193
 msgid "category"
 msgstr ""
 
-#: aa_forum/models.py:178
+#: aa_forum/models.py:194
 msgid "categories"
 msgstr ""
 
-#: aa_forum/models.py:222
+#: aa_forum/models.py:248
 msgid ""
 "Use this Discord webhook for replies as well? When activated every reply to "
 "any topic in this board will be posted to the defined Discord channel. "
 "(Child boards are excluded) Chose wisely! (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:240
+#: aa_forum/models.py:266
 msgid ""
 "User in at least one of these groups have access to this board. If no groups "
 "are selected, everyone with access to the forum has also access to this "
 "board."
 msgstr ""
 
-#: aa_forum/models.py:248
+#: aa_forum/models.py:274
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:259
+#: aa_forum/models.py:285
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so."
 msgstr ""
 
-#: aa_forum/models.py:295
+#: aa_forum/models.py:321
 msgid "board"
 msgstr ""
 
-#: aa_forum/models.py:296
+#: aa_forum/models.py:322
 msgid "boards"
 msgstr ""
 
-#: aa_forum/models.py:367
+#: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:578
+#: aa_forum/models.py:625
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:579
+#: aa_forum/models.py:626
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:736
+#: aa_forum/models.py:805
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:737
+#: aa_forum/models.py:806
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:872
+#: aa_forum/models.py:948
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:873
+#: aa_forum/models.py:949
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:920
+#: aa_forum/models.py:1003
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:921
+#: aa_forum/models.py:1004
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:922
+#: aa_forum/models.py:1005
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:927
+#: aa_forum/models.py:1010
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:932
+#: aa_forum/models.py:1015
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:937
+#: aa_forum/models.py:1020
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:1031
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:1032
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:952
+#: aa_forum/models.py:1042
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:16
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:978
+#: aa_forum/models.py:1069
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:979
+#: aa_forum/models.py:1070
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:982
+#: aa_forum/models.py:1080
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:30
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:7
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:38
+#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:8
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:56
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:73
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:59
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:75
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:69
 msgid "Delete message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:13
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:8
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:23
 msgid "Delete board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
+msgid "Close"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:22
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:22
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:21
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:21
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:21
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:20
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:20
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:20
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:19
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:19
 msgid "This action cannot be undone!"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:29
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:29
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:28
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:28
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:28
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:27
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:27
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:34
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:34
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:33
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:33
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:33
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:15
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:16
 msgid "Are you sure you want to delete this category?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:17
 msgid "This will also remove all boards, topics and messages in this category."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:13
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:39
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:84
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
 msgid "Unlock/re-open topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:16
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:42
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:88
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
 msgid "Lock/close topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
 msgid "Are you sure you want to lock/close this topic?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:3
 msgid "Change sticky state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:13
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:9
 msgid "Remove \"sticky\" state from topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:16
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:12
 msgid "Set \"sticky\" state for topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:22
 msgid "Are you sure you want to remove the sticky state from this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
 msgid ""
 "Are you sure you want to make this topic sticky, so it always shows up on "
 "top of the topic list?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:39
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:37
 msgid "Unset sticky"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:42
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:97
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
 msgid "Delete topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:19
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:17
 msgid "This will also remove all messages in this topic."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:17
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:17
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:15
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:15
 msgid "Are you sure you want to delete this message?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:16
 msgid ""
 "If this message is the original post, then the entire topic will be removed "
 "as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:16
 msgid ""
 "If this message is the beginning of a conversation, all related messages "
 "will be removed as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:9
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:11
 msgid "Edit board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:22
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:36
 msgid ""
 "Changing the name of this board does not change its URL part. This will "
 "remain the same to not break any possible links into this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:58
 msgid "Change board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:56
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:70
 msgid "New child board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:63
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:62
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:77
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:84
 msgid ""
 "New boards will be added at the bottom of the board list for this category. "
 "You can move them via drag and drop to a position of your liking."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:79
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:75
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:93
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:97
 msgid "Create board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/categories.html:6
+#: aa_forum/templates/aa_forum/partials/administration/categories.html:5
 msgid ""
 "Here you can create, modify and delete categories and boards. You also can "
 "change their order via drag and drop."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:11
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:13
 msgid "Edit category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:19
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:35
 msgid "Expand/collapse category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:31
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:53
 msgid ""
 "Changing the name of this category does not change its URL part. This will "
 "remain the same to not break any possible links into this category."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:66
 msgid "Change category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:55
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:77
 msgid "New board"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:7
 msgid "Create new category"
 msgstr ""
 
@@ -598,24 +639,25 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:35
 msgid "Create category"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:21
-#: aa_forum/templates/aa_forum/partials/profile/form.html:21
+#: aa_forum/templates/aa_forum/partials/profile/form.html:22
 msgid "Submit"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:6
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:7
 msgid "Forum index"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:27
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:49
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:51
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:6
 msgid "Modify message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:34
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:7
@@ -636,66 +678,67 @@
 "existing translation?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:9
+#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:34
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
+msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:51
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
 msgid "New"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
 msgid "Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:66
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:65
 msgid "Unread"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:82
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:88
 msgid "Last post:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:86
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:25
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:96
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:26
 msgid "Re:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:103
 msgid "posted by:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:94
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:104
 msgid "posted at:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:7
+#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:8
 msgid "New topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/no-access.html:6
 msgid ""
 "You either don't have access to this board, or this board doesn't exist."
 msgstr ""
@@ -761,58 +804,58 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
 msgid "Last post"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:38
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:39
 msgid "Copy message link to clipboard"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:81
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:87
 msgid "Last modified:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:14
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:27
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:21
@@ -820,68 +863,65 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:6
 msgid "Modify topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:20
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:21
 msgid "Warning: this topic is locked! Only admins can reply."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:33
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:44
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
 msgid "Clear form"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:7
 msgid "Show all unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:7
 msgid "Administration"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:12
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:13
 msgid "Categories and boards"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:6
-#: aa_forum/templates/aa_forum/view/profile/index.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:13
+#: aa_forum/templates/aa_forum/view/profile/index.html:7
 msgid "Profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:11
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:19
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:9
 msgid "Messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:23
 msgid "Inbox"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:18
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:18
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:17
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:17
 msgid "Date"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:22
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:21
 msgid "Sender"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:62
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:63
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:57
 msgid "Read message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:87
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:93
 msgid "No personal messages"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:8
 msgid "New personal message"
 msgstr ""
 
@@ -889,325 +929,322 @@
 msgid "Send message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:8
 msgid "Reply to:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:24
+#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:23
 msgid "Send reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:30
 msgid "Sent messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:56
-msgid "Read Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:67
-msgid "Delete Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:81
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:87
 msgid "No personal messages sent"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:17
 msgid "New message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/profile/form.html:7
 msgid "User profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/search/search-form.html:7
+#: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+msgid "Forum: Unread topics"
+msgstr ""
+
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:6
 msgid "Administration (Forum settings)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:26
+#: aa_forum/templates/aa_forum/view/forum/index.html:27
 msgid "New posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:35
+#: aa_forum/templates/aa_forum/view/forum/index.html:36
 msgid "No new posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:22
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:21
 msgid "Start new topic in"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:38
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
 msgid "Start topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/topic.html:23
+#: aa_forum/templates/aa_forum/view/forum/topic.html:24
 msgid "Modify topic subject"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:6
 msgid "Unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:16
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:15
 msgid "Unread Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:31
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:30
 msgid "You have no unread topics …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:7
 msgid "Personal messages (Inbox)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:7
 msgid "Personal messages (New message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:39
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:35
 msgid "Enter the recipients name"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:7
 msgid "Personal messages (Reply to message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:7
 msgid "Personal messages (Sent messages)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:6
 msgid "Search results"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:22
+#: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
+msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:32
+#: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
-#: aa_forum/templatetags/aa_forum_datetime.py:57
+#: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
 msgstr ""
 
-#: aa_forum/views/admin.py:165
+#: aa_forum/views/admin.py:169
 msgid "<h4>Success!</h4><p>Category created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:205
+#: aa_forum/views/admin.py:212
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Category name changed from \"{category_name_old}\" to "
 "\"{category.name}\".</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:245
+#: aa_forum/views/admin.py:255
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Category \"{category_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:298 aa_forum/views/admin.py:354
+#: aa_forum/views/admin.py:311 aa_forum/views/admin.py:371
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{new_board.name}\" created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:409
+#: aa_forum/views/admin.py:430
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board.name}\" changed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:450
+#: aa_forum/views/admin.py:475
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:556
+#: aa_forum/views/admin.py:587
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:566 aa_forum/views/personal_messages.py:116
-#: aa_forum/views/personal_messages.py:237 aa_forum/views/profile.py:68
+#: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
+#: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:225
+#: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:282
+#: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:309
+#: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:329
+#: aa_forum/views/forum.py:340
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in is an announcement "
 "board and you don't have the permissions to start a topic there.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:386
+#: aa_forum/views/forum.py:399
 msgid ""
 "<h4>Error!</h4><p>Either subject or message is missing. Please make sure you "
 "enter both fields, as both fields are mandatory.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:442 aa_forum/views/forum.py:672
+#: aa_forum/views/forum.py:461 aa_forum/views/forum.py:706
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to view does not exist or you do "
 "not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:539
+#: aa_forum/views/forum.py:563
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to modify does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:561
+#: aa_forum/views/forum.py:585
 msgid "<h4>Error!</h4><p>You are not allowed to modify this topic!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:593
+#: aa_forum/views/forum.py:617
 msgid "<h4>Success!</h4><p>The topic subject has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:791
+#: aa_forum/views/forum.py:845
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to reply does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:847
+#: aa_forum/views/forum.py:922
 msgid "<h4>Error!</h4><p>Message field is mandatory and cannot be empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:856
+#: aa_forum/views/forum.py:931
 msgid "<h4>Error!</h4><p>Something went wrong, please try again.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:894
+#: aa_forum/views/forum.py:972
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been unlocked/re-opened.</"
 "p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:908
+#: aa_forum/views/forum.py:986
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been locked/closed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:949
+#: aa_forum/views/forum.py:1030
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{curent_topic}\" is no longer \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:963
+#: aa_forum/views/forum.py:1044
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{curent_topic}\" is now \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:998
+#: aa_forum/views/forum.py:1082
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{topic__subject}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1034
+#: aa_forum/views/forum.py:1124
 msgid "<h4>Error!</h4><p>The message doesn't exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1078
+#: aa_forum/views/forum.py:1174
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to modify does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1101
+#: aa_forum/views/forum.py:1197
 msgid "<h4>Error!</h4><p>You are not allowed to modify this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1128
+#: aa_forum/views/forum.py:1224
 msgid "<h4>Success!</h4><p>The message has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1151
+#: aa_forum/views/forum.py:1247
 msgid "<h4>Error!</h4><p>Mandatory form field is empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1241
+#: aa_forum/views/forum.py:1345
 msgid "<h4>Error!</h4><p>You are not allowed to delete this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1271
+#: aa_forum/views/forum.py:1375
 msgid "<h4>Success!</h4><p>The message has been deleted.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1296
+#: aa_forum/views/forum.py:1400
 msgid ""
 "<h4>Success!</h4><p>The message has been deleted.</p><p>This was the topics "
 "opening post, so the topic has been deleted as well.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:104
+#: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:190
+#: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:226
+#: aa_forum/views/personal_messages.py:238
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Reply to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:282
-#: aa_forum/views/personal_messages.py:319
+#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:335
 msgid ""
 "<h4>Error!</h4><p>The message you tried to remove does either not exist or "
 "is not yours to remove.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:314
 msgid "<h4>Success!</h4><p>Message removed from your inbox.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:337
+#: aa_forum/views/personal_messages.py:353
 msgid ""
 "<h4>Success!</h4><p>Message has been removed from your sent messages.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:352
+#: aa_forum/views/personal_messages.py:368
 msgid "<h4>Error!</h4><p>Something went wrong.</p>"
 msgstr ""
 
-#: aa_forum/views/profile.py:58
+#: aa_forum/views/profile.py:60
 msgid "<h4>Success!</h4><p>Profile saved.</p>"
 msgstr ""
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/ko_KR/LC_MESSAGES/django.po` & `aa_forum-2.1.0/aa_forum/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,597 +1,629 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Author50CO <tkddlschry@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 18:29+0200\n"
-"PO-Revision-Date: 2023-12-29 10:04+0000\n"
+"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"PO-Revision-Date: 2023-10-02 09:34+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/ko/>\n"
-"Language: ko_KR\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/it/>\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.0.2\n"
 
-#: aa_forum/__init__.py:12 aa_forum/templates/aa_forum/base.html:5
-#: aa_forum/templates/aa_forum/partials/menu.html:14
+#: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
+#: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
-#: aa_forum/templates/aa_forum/view/forum/board.html:5
-#: aa_forum/templates/aa_forum/view/forum/index.html:6
+#: aa_forum/templates/aa_forum/view/forum/board.html:6
+#: aa_forum/templates/aa_forum/view/forum/index.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:8
-#: aa_forum/templates/aa_forum/view/forum/topic.html:5
+#: aa_forum/templates/aa_forum/view/forum/topic.html:6
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:7
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:9
-#: aa_forum/templates/aa_forum/view/profile/index.html:9
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
-msgstr "포럼"
+msgstr ""
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
-msgstr "AA 포럼 v{__version__}"
+msgstr ""
 
-#: aa_forum/forms.py:40
+#: aa_forum/forms.py:42
 msgid "This field is mandatory"
-msgstr "필수 항목입니다"
+msgstr "Questo campo è obbligatorio"
 
-#: aa_forum/forms.py:91 aa_forum/forms.py:93 aa_forum/forms.py:124
-#: aa_forum/forms.py:126 aa_forum/forms.py:502
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:26
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:26
+#: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
+#: aa_forum/forms.py:171 aa_forum/forms.py:616
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
-msgstr "제목"
+msgstr ""
 
-#: aa_forum/forms.py:102 aa_forum/forms.py:321 aa_forum/forms.py:512
-#: aa_forum/forms.py:558
-msgid "Message"
-msgstr "메시지"
+#: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
+#: aa_forum/forms.py:730
+msgid "You have forgotten the message!"
+msgstr ""
 
-#: aa_forum/forms.py:145 aa_forum/forms.py:183 aa_forum/forms.py:204
+#: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
-msgstr "이름"
+msgstr ""
 
-#: aa_forum/forms.py:147 aa_forum/forms.py:185
+#: aa_forum/forms.py:192 aa_forum/forms.py:230
 msgid "Category name"
 msgstr ""
 
-#: aa_forum/forms.py:151 aa_forum/forms.py:162
+#: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
 msgstr ""
 
-#: aa_forum/forms.py:153
+#: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
 
-#: aa_forum/forms.py:206
+#: aa_forum/forms.py:251
 msgid "Board name"
 msgstr ""
 
-#: aa_forum/forms.py:210
+#: aa_forum/forms.py:255
 msgid "Description"
 msgstr ""
 
-#: aa_forum/forms.py:216
+#: aa_forum/forms.py:261
 msgid "Board description (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:222
+#: aa_forum/forms.py:267
 msgid "Group restrictions"
-msgstr "그룹 제한"
+msgstr ""
 
-#: aa_forum/forms.py:224
+#: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:232
+#: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:234
+#: aa_forum/forms.py:279
 msgid ""
 "Discord webhook URL for the channel to post about new topics in this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:247
+#: aa_forum/forms.py:292
 msgid "Use this Discord webhook for replies as well?"
 msgstr ""
 
-#: aa_forum/forms.py:249
+#: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
 msgstr ""
 
-#: aa_forum/forms.py:257
+#: aa_forum/forms.py:302
 msgid "Mark board as \"Announcement Board\""
 msgstr ""
 
-#: aa_forum/forms.py:259
+#: aa_forum/forms.py:304
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. This setting will "
 "not be inherited to child boards. (Default: NO)"
 msgstr ""
 
-#: aa_forum/forms.py:267
+#: aa_forum/forms.py:312
 msgid "Start topic restrictions for \"Announcement Boards\""
 msgstr ""
 
-#: aa_forum/forms.py:269
+#: aa_forum/forms.py:314
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
 msgstr ""
 
-#: aa_forum/forms.py:354
-msgid "Signature"
+#: aa_forum/forms.py:362
+msgid "Close topic"
 msgstr ""
 
-#: aa_forum/forms.py:355
-msgid "Your signature will appear below your posts."
+#: aa_forum/forms.py:364
+msgid "If checked, this topic will be closed after posting this message."
+msgstr ""
+
+#: aa_forum/forms.py:370
+msgid "Reopen topic"
+msgstr ""
+
+#: aa_forum/forms.py:372
+msgid "If checked, this topic will be reopened after posting this message."
+msgstr ""
+
+#: aa_forum/forms.py:409 aa_forum/forms.py:652 aa_forum/forms.py:717
+msgid "Message"
 msgstr ""
 
-#: aa_forum/forms.py:359
+#: aa_forum/forms.py:446
 msgid "Website title"
 msgstr ""
 
-#: aa_forum/forms.py:361
+#: aa_forum/forms.py:448
 msgid "e.g.: My Homepage"
 msgstr ""
 
-#: aa_forum/forms.py:362
+#: aa_forum/forms.py:449
 msgid "Your website's title."
 msgstr ""
 
-#: aa_forum/forms.py:366
+#: aa_forum/forms.py:453
 msgid "Website URL"
 msgstr ""
 
-#: aa_forum/forms.py:370
+#: aa_forum/forms.py:457
 msgid ""
 "Your website's URL. (Don't forget to also set a title for your website, "
 "otherwise this field will be ignored.)"
 msgstr ""
 
-#: aa_forum/forms.py:376
+#: aa_forum/forms.py:463
 msgid "PM me on Discord when I get a new personal message"
 msgstr ""
 
-#: aa_forum/forms.py:378
+#: aa_forum/forms.py:466
 msgid ""
 "Information: There is currently no module installed that can handle Discord "
 "direct messages. Have a chat with your IT guys to remedy this."
 msgstr ""
 
-#: aa_forum/forms.py:419
+#: aa_forum/forms.py:475
+msgid "Show unread topics as widget on the dashboard"
+msgstr ""
+
+#: aa_forum/forms.py:478
+msgid ""
+"Activating this setting will ad a widget to your dashboard that shows unread "
+"topics in the forum."
+msgstr ""
+
+#: aa_forum/forms.py:507
+msgid "Signature"
+msgstr ""
+
+#: aa_forum/forms.py:508
+msgid "Your signature will appear below your posts."
+msgstr ""
+
+#: aa_forum/forms.py:532
 msgid ""
 "Ensure your signature has at most {max_signature_length} characters. "
 "(Currently: {len(signature)})"
 msgstr ""
 
-#: aa_forum/forms.py:440
+#: aa_forum/forms.py:554
 msgid "This is not a valid URL"
 msgstr ""
 
-#: aa_forum/forms.py:456
+#: aa_forum/forms.py:570
 msgid ""
 "How many messages per page should be displayed in a forum topic? (Default: "
 "15)"
 msgstr ""
 
-#: aa_forum/forms.py:466
+#: aa_forum/forms.py:580
 msgid ""
 "How many topics per page should be displayed in a forum category? (Default: "
 "10)"
 msgstr ""
 
-#: aa_forum/forms.py:476
+#: aa_forum/forms.py:590
 msgid ""
 "How long (Number of characters) is a user's signature allowed to be? "
 "(Default: 750)"
 msgstr ""
 
-#: aa_forum/forms.py:498
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:22
+#: aa_forum/forms.py:612
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:21
 msgid "Recipient"
 msgstr ""
 
-#: aa_forum/forms.py:504
+#: aa_forum/forms.py:618
 msgid "Hello there …"
 msgstr ""
 
-#: aa_forum/models.py:127
+#: aa_forum/models.py:139
 msgid "AA-Forum"
 msgstr ""
 
-#: aa_forum/models.py:131
+#: aa_forum/models.py:143
 msgid "Can access the AA-Forum module"
 msgstr ""
 
-#: aa_forum/models.py:134
+#: aa_forum/models.py:146
 msgid "Can manage the AA-Forum module (Category, topics and messages)"
 msgstr ""
 
-#: aa_forum/models.py:177
+#: aa_forum/models.py:193
 msgid "category"
 msgstr ""
 
-#: aa_forum/models.py:178
+#: aa_forum/models.py:194
 msgid "categories"
 msgstr ""
 
-#: aa_forum/models.py:222
+#: aa_forum/models.py:248
 msgid ""
 "Use this Discord webhook for replies as well? When activated every reply to "
 "any topic in this board will be posted to the defined Discord channel. "
 "(Child boards are excluded) Chose wisely! (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:240
+#: aa_forum/models.py:266
 msgid ""
 "User in at least one of these groups have access to this board. If no groups "
 "are selected, everyone with access to the forum has also access to this "
 "board."
 msgstr ""
 
-#: aa_forum/models.py:248
+#: aa_forum/models.py:274
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:259
+#: aa_forum/models.py:285
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so."
 msgstr ""
 
-#: aa_forum/models.py:295
+#: aa_forum/models.py:321
 msgid "board"
 msgstr ""
 
-#: aa_forum/models.py:296
+#: aa_forum/models.py:322
 msgid "boards"
 msgstr ""
 
-#: aa_forum/models.py:367
+#: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:578
+#: aa_forum/models.py:625
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:579
+#: aa_forum/models.py:626
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:736
+#: aa_forum/models.py:805
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:737
+#: aa_forum/models.py:806
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:872
+#: aa_forum/models.py:948
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:873
+#: aa_forum/models.py:949
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:920
+#: aa_forum/models.py:1003
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:921
+#: aa_forum/models.py:1004
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:922
+#: aa_forum/models.py:1005
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:927
+#: aa_forum/models.py:1010
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:932
+#: aa_forum/models.py:1015
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:937
+#: aa_forum/models.py:1020
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:1031
 msgid "setting"
-msgstr "설정"
+msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:1032
 msgid "settings"
-msgstr "설정"
+msgstr ""
 
-#: aa_forum/models.py:952
+#: aa_forum/models.py:1042
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:16
-#, fuzzy
-#| msgid "settings"
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
-msgstr "설정"
+msgstr ""
 
-#: aa_forum/models.py:978
+#: aa_forum/models.py:1069
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:979
+#: aa_forum/models.py:1070
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:982
+#: aa_forum/models.py:1080
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:30
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:7
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:38
+#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:8
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:56
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:73
-#, fuzzy
-#| msgid "Delete"
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:59
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:75
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:69
 msgid "Delete message"
-msgstr "삭제"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:13
-#, fuzzy
-#| msgid "Delete"
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:8
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:23
 msgid "Delete board"
-msgstr "삭제"
+msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
+msgid "Close"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:22
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:22
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:21
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:21
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:21
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:20
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:20
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:20
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:19
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:19
 msgid "This action cannot be undone!"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:29
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:29
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:28
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:28
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:28
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:27
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:27
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:34
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:34
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:33
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:33
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:33
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
-msgstr "삭제"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:15
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:16
 msgid "Are you sure you want to delete this category?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:17
 msgid "This will also remove all boards, topics and messages in this category."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:13
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:39
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:84
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
 msgid "Unlock/re-open topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:16
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:42
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:88
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
 msgid "Lock/close topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
 msgid "Are you sure you want to lock/close this topic?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:3
 msgid "Change sticky state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:13
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:9
 msgid "Remove \"sticky\" state from topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:16
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:12
 msgid "Set \"sticky\" state for topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:22
 msgid "Are you sure you want to remove the sticky state from this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
 msgid ""
 "Are you sure you want to make this topic sticky, so it always shows up on "
 "top of the topic list?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:39
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:37
 msgid "Unset sticky"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:42
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:97
-#, fuzzy
-#| msgid "Delete"
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
 msgid "Delete topic"
-msgstr "삭제"
+msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:19
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:17
 msgid "This will also remove all messages in this topic."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:17
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:17
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:15
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:15
 msgid "Are you sure you want to delete this message?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:16
 msgid ""
 "If this message is the original post, then the entire topic will be removed "
 "as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:16
 msgid ""
 "If this message is the beginning of a conversation, all related messages "
 "will be removed as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:9
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:11
 msgid "Edit board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:22
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:36
 msgid ""
 "Changing the name of this board does not change its URL part. This will "
 "remain the same to not break any possible links into this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:58
 msgid "Change board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:56
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:70
 msgid "New child board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:63
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:62
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:77
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:84
 msgid ""
 "New boards will be added at the bottom of the board list for this category. "
 "You can move them via drag and drop to a position of your liking."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:79
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:75
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:93
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:97
 msgid "Create board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/categories.html:6
+#: aa_forum/templates/aa_forum/partials/administration/categories.html:5
 msgid ""
 "Here you can create, modify and delete categories and boards. You also can "
 "change their order via drag and drop."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:11
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:13
 msgid "Edit category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:19
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:35
 msgid "Expand/collapse category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:31
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:53
 msgid ""
 "Changing the name of this category does not change its URL part. This will "
 "remain the same to not break any possible links into this category."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:66
 msgid "Change category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:55
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:77
 msgid "New board"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:7
 msgid "Create new category"
 msgstr ""
 
@@ -606,30 +638,29 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:35
 msgid "Create category"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:21
-#: aa_forum/templates/aa_forum/partials/profile/form.html:21
+#: aa_forum/templates/aa_forum/partials/profile/form.html:22
 msgid "Submit"
-msgstr "전송"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:6
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:7
 msgid "Forum index"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:27
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:49
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:51
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:6
-#, fuzzy
-#| msgid "Message"
 msgid "Modify message"
-msgstr "메시지"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:34
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:7
 msgid "Start new topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:40
@@ -640,72 +671,73 @@
 msgid "Search for:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:9
+#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "별표 (*) 표시된 항목은 필수 항목입니다"
+msgstr "I campi contrassegnati da un asterisco (*) sono obbligatori"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:34
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
+msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:51
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
 msgid "New"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
 msgid "Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:66
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:65
 msgid "Unread"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:82
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:88
 msgid "Last post:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:86
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:25
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:96
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:26
 msgid "Re:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:103
 msgid "posted by:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:94
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:104
 msgid "posted at:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:7
+#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:8
 msgid "New topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/no-access.html:6
 msgid ""
 "You either don't have access to this board, or this board doesn't exist."
 msgstr ""
@@ -725,15 +757,15 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:10
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:39
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:10
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:39
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:9
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:38
 msgid "First"
-msgstr "첫 번째"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:20
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:24
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:46
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:22
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:26
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:48
@@ -743,86 +775,86 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:17
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:21
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:43
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:16
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:20
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:42
 msgid "Previous"
-msgstr "이전"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:63
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:74
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:76
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:60
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:71
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:60
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:71
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:59
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:70
 msgid "Next"
-msgstr "다음"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:69
 #: aa_forum/templates/aa_forum/partials/forum/board/pagination.html:78
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:71
 #: aa_forum/templates/aa_forum/partials/forum/topic/pagination.html:80
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
-msgstr "마지막"
+msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
 msgid "Last post"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:38
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:39
 msgid "Copy message link to clipboard"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:81
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:87
 msgid "Last modified:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:14
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:27
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:21
@@ -830,402 +862,388 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:6
 msgid "Modify topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:20
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:21
 msgid "Warning: this topic is locked! Only admins can reply."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:33
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:44
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
 msgid "Clear form"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:7
 msgid "Show all unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr "토글 메뉴"
-
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:7
 msgid "Administration"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:12
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:13
 msgid "Categories and boards"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:6
-#: aa_forum/templates/aa_forum/view/profile/index.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:13
+#: aa_forum/templates/aa_forum/view/profile/index.html:7
 msgid "Profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:11
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:19
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:9
 msgid "Messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:23
 msgid "Inbox"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:18
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:18
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:17
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:17
 msgid "Date"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:22
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:21
 msgid "Sender"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:62
-#, fuzzy
-#| msgid "Message"
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:63
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:57
 msgid "Read message"
-msgstr "메시지"
+msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:87
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:93
 msgid "No personal messages"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:8
 msgid "New personal message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:23
-#, fuzzy
-#| msgid "Message"
 msgid "Send message"
-msgstr "메시지"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:8
 msgid "Reply to:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:24
+#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:23
 msgid "Send reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:30
-#, fuzzy
-#| msgid "Message"
 msgid "Sent messages"
-msgstr "메시지"
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:56
-msgid "Read Message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:67
-msgid "Delete Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:81
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:87
 msgid "No personal messages sent"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:17
-#, fuzzy
-#| msgid "Message"
 msgid "New message"
-msgstr "메시지"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/profile/form.html:7
 msgid "User profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/search/search-form.html:7
+#: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
-msgstr "검색 …"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+msgid "Forum: Unread topics"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:6
 msgid "Administration (Forum settings)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:26
+#: aa_forum/templates/aa_forum/view/forum/index.html:27
 msgid "New posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:35
+#: aa_forum/templates/aa_forum/view/forum/index.html:36
 msgid "No new posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:22
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:21
 msgid "Start new topic in"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:38
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
 msgid "Start topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/topic.html:23
+#: aa_forum/templates/aa_forum/view/forum/topic.html:24
 msgid "Modify topic subject"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:6
 msgid "Unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:16
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:15
 msgid "Unread Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:31
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:30
 msgid "You have no unread topics …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:7
 msgid "Personal messages (Inbox)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:7
 msgid "Personal messages (New message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:39
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:35
 msgid "Enter the recipients name"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:7
 msgid "Personal messages (Reply to message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:7
 msgid "Personal messages (Sent messages)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:6
 msgid "Search results"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:22
+#: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
+msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:32
+#: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
-#: aa_forum/templatetags/aa_forum_datetime.py:57
+#: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
 msgstr ""
 
-#: aa_forum/views/admin.py:165
+#: aa_forum/views/admin.py:169
 msgid "<h4>Success!</h4><p>Category created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:205
+#: aa_forum/views/admin.py:212
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Category name changed from \"{category_name_old}\" to "
 "\"{category.name}\".</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:245
+#: aa_forum/views/admin.py:255
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Category \"{category_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:298 aa_forum/views/admin.py:354
+#: aa_forum/views/admin.py:311 aa_forum/views/admin.py:371
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{new_board.name}\" created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:409
+#: aa_forum/views/admin.py:430
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board.name}\" changed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:450
+#: aa_forum/views/admin.py:475
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:556
+#: aa_forum/views/admin.py:587
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:566 aa_forum/views/personal_messages.py:116
-#: aa_forum/views/personal_messages.py:237 aa_forum/views/profile.py:68
+#: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
+#: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:225
+#: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:282
+#: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:309
+#: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:329
+#: aa_forum/views/forum.py:340
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in is an announcement "
 "board and you don't have the permissions to start a topic there.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:386
+#: aa_forum/views/forum.py:399
 msgid ""
 "<h4>Error!</h4><p>Either subject or message is missing. Please make sure you "
 "enter both fields, as both fields are mandatory.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:442 aa_forum/views/forum.py:672
+#: aa_forum/views/forum.py:461 aa_forum/views/forum.py:706
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to view does not exist or you do "
 "not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:539
+#: aa_forum/views/forum.py:563
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to modify does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:561
+#: aa_forum/views/forum.py:585
 msgid "<h4>Error!</h4><p>You are not allowed to modify this topic!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:593
+#: aa_forum/views/forum.py:617
 msgid "<h4>Success!</h4><p>The topic subject has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:791
+#: aa_forum/views/forum.py:845
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to reply does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:847
+#: aa_forum/views/forum.py:922
 msgid "<h4>Error!</h4><p>Message field is mandatory and cannot be empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:856
+#: aa_forum/views/forum.py:931
 msgid "<h4>Error!</h4><p>Something went wrong, please try again.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:894
+#: aa_forum/views/forum.py:972
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been unlocked/re-opened.</"
 "p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:908
+#: aa_forum/views/forum.py:986
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been locked/closed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:949
+#: aa_forum/views/forum.py:1030
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{curent_topic}\" is no longer \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:963
+#: aa_forum/views/forum.py:1044
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{curent_topic}\" is now \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:998
+#: aa_forum/views/forum.py:1082
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{topic__subject}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1034
+#: aa_forum/views/forum.py:1124
 msgid "<h4>Error!</h4><p>The message doesn't exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1078
+#: aa_forum/views/forum.py:1174
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to modify does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1101
+#: aa_forum/views/forum.py:1197
 msgid "<h4>Error!</h4><p>You are not allowed to modify this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1128
+#: aa_forum/views/forum.py:1224
 msgid "<h4>Success!</h4><p>The message has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1151
+#: aa_forum/views/forum.py:1247
 msgid "<h4>Error!</h4><p>Mandatory form field is empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1241
+#: aa_forum/views/forum.py:1345
 msgid "<h4>Error!</h4><p>You are not allowed to delete this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1271
+#: aa_forum/views/forum.py:1375
 msgid "<h4>Success!</h4><p>The message has been deleted.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1296
+#: aa_forum/views/forum.py:1400
 msgid ""
 "<h4>Success!</h4><p>The message has been deleted.</p><p>This was the topics "
 "opening post, so the topic has been deleted as well.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:104
+#: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:190
+#: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:226
+#: aa_forum/views/personal_messages.py:238
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Reply to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:282
-#: aa_forum/views/personal_messages.py:319
+#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:335
 msgid ""
 "<h4>Error!</h4><p>The message you tried to remove does either not exist or "
 "is not yours to remove.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:314
 msgid "<h4>Success!</h4><p>Message removed from your inbox.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:337
+#: aa_forum/views/personal_messages.py:353
 msgid ""
 "<h4>Success!</h4><p>Message has been removed from your sent messages.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:352
+#: aa_forum/views/personal_messages.py:368
 msgid "<h4>Error!</h4><p>Something went wrong.</p>"
 msgstr ""
 
-#: aa_forum/views/profile.py:58
+#: aa_forum/views/profile.py:60
 msgid "<h4>Success!</h4><p>Profile saved.</p>"
 msgstr ""
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/ru/LC_MESSAGES/django.mo` & `aa_forum-2.1.0/aa_forum/locale/ru/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-forum/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.4.2\n"
 
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] "%(counter)s Результат"
 msgstr[1] "%(counter)s Результата"
 msgstr[2] "%(counter)s Результатов"
 msgstr[3] "%(counter)s Результатов"
@@ -318,14 +318,17 @@
 
 msgid "Child boards:"
 msgstr "Дочерние доски:"
 
 msgid "Clear form"
 msgstr "Очистить форму"
 
+msgid "Close"
+msgstr "Закрыть"
+
 msgid "Copy message link to clipboard"
 msgstr "Скопировать ссылку на сообщение в буфер обмена"
 
 msgid "Create board"
 msgstr "Создать доску"
 
 msgid "Create category"
@@ -336,17 +339,14 @@
 
 msgid "Date"
 msgstr "Дата"
 
 msgid "Delete"
 msgstr "Удалить"
 
-msgid "Delete Message"
-msgstr "Удалить сообщение"
-
 msgid "Delete board"
 msgstr "Удалить доску"
 
 msgid "Delete category"
 msgstr "Удалить категорию"
 
 msgid "Delete message"
@@ -637,17 +637,14 @@
 
 msgid "Profile"
 msgstr "Профиль"
 
 msgid "Re:"
 msgstr "Ответ на:"
 
-msgid "Read Message"
-msgstr "Прочитать сообщение"
-
 msgid "Read message"
 msgstr "Прочитать сообщение"
 
 msgid "Recipient"
 msgstr "Получатель"
 
 msgid "Remove \"sticky\" state from topic"
@@ -749,17 +746,14 @@
 "Только перечисленные группы будут иметь доступ к доске. Если группы не "
 "выбраны, все пользователи форума будут иметь доступ к доске. (Настройка не "
 "обязательна)"
 
 msgid "Timezone conversion"
 msgstr "Преобразование временной зоны"
 
-msgid "Toggle navigation"
-msgstr "Переключить навигацию"
-
 msgid "Topic is always on top"
 msgstr "Тема всегда в начале"
 
 msgid "Topic is locked"
 msgstr "Тема закрыта"
 
 msgid "Topics"
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/ru/LC_MESSAGES/django.po` & `aa_forum-2.1.0/aa_forum/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,643 +1,687 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 # Nikolay <nick.postnikov@gmail.com>, 2023.
 # Max <mark25@inbox.ru>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 18:29+0200\n"
-"PO-Revision-Date: 2023-10-03 11:36+0000\n"
-"Last-Translator: Max <mark25@inbox.ru>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/ru/>\n"
+"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"PO-Revision-Date: 2024-03-21 17:11+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.4.2\n"
 
-#: aa_forum/__init__.py:12 aa_forum/templates/aa_forum/base.html:5
-#: aa_forum/templates/aa_forum/partials/menu.html:14
+#: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
+#: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
-#: aa_forum/templates/aa_forum/view/forum/board.html:5
-#: aa_forum/templates/aa_forum/view/forum/index.html:6
+#: aa_forum/templates/aa_forum/view/forum/board.html:6
+#: aa_forum/templates/aa_forum/view/forum/index.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:8
-#: aa_forum/templates/aa_forum/view/forum/topic.html:5
+#: aa_forum/templates/aa_forum/view/forum/topic.html:6
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:7
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:9
-#: aa_forum/templates/aa_forum/view/profile/index.html:9
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
 msgstr "Форум"
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr "АА-форум v{__version__}"
 
-#: aa_forum/forms.py:40
+#: aa_forum/forms.py:42
 msgid "This field is mandatory"
 msgstr "Обязательное поле"
 
-#: aa_forum/forms.py:91 aa_forum/forms.py:93 aa_forum/forms.py:124
-#: aa_forum/forms.py:126 aa_forum/forms.py:502
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:26
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:26
+#: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
+#: aa_forum/forms.py:171 aa_forum/forms.py:616
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr "Тема"
 
-#: aa_forum/forms.py:102 aa_forum/forms.py:321 aa_forum/forms.py:512
-#: aa_forum/forms.py:558
-msgid "Message"
-msgstr "Сообщение"
+#: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
+#: aa_forum/forms.py:730
+msgid "You have forgotten the message!"
+msgstr ""
 
-#: aa_forum/forms.py:145 aa_forum/forms.py:183 aa_forum/forms.py:204
+#: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
 msgstr "Название"
 
-#: aa_forum/forms.py:147 aa_forum/forms.py:185
+#: aa_forum/forms.py:192 aa_forum/forms.py:230
 msgid "Category name"
 msgstr "Название категории"
 
-#: aa_forum/forms.py:151 aa_forum/forms.py:162
+#: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
 msgstr "Доски"
 
-#: aa_forum/forms.py:153
+#: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
 "Доски, создаваемые в этой категории (Одна доска в строке). Для досок не "
 "будут установлены ограничения по группам, их нужно добавить отдельно."
 
-#: aa_forum/forms.py:206
+#: aa_forum/forms.py:251
 msgid "Board name"
 msgstr "Название доски"
 
-#: aa_forum/forms.py:210
+#: aa_forum/forms.py:255
 msgid "Description"
 msgstr "Описание"
 
-#: aa_forum/forms.py:216
+#: aa_forum/forms.py:261
 msgid "Board description (optional)"
 msgstr "Описание доски (не обязательно)"
 
-#: aa_forum/forms.py:222
+#: aa_forum/forms.py:267
 msgid "Group restrictions"
 msgstr "Ограничения групп"
 
-#: aa_forum/forms.py:224
+#: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
 "Только перечисленные группы будут иметь доступ к доске. Если группы не "
 "выбраны, все пользователи форума будут иметь доступ к доске. (Настройка не "
 "обязательна)"
 
-#: aa_forum/forms.py:232
+#: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
 msgstr "Discord вебхук (не обязательно)"
 
-#: aa_forum/forms.py:234
+#: aa_forum/forms.py:279
 msgid ""
 "Discord webhook URL for the channel to post about new topics in this board. "
 "(This setting is optional)"
 msgstr ""
 "Discord вебхук URL канала для сообщений о новых темах на доске. (Настройка "
 "не обязательна)"
 
-#: aa_forum/forms.py:247
+#: aa_forum/forms.py:292
 msgid "Use this Discord webhook for replies as well?"
 msgstr "Использовать этот же Discord вебхук для ответов?"
 
-#: aa_forum/forms.py:249
+#: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
 msgstr ""
 "При включении каждый ответ в любой теме доски будет отправлен в канал "
 "Discord. (Дочерние доски не учитываются) Использовать с умом! (По умолчанию: "
 "ВЫКЛ)"
 
-#: aa_forum/forms.py:257
+#: aa_forum/forms.py:302
 msgid "Mark board as \"Announcement Board\""
 msgstr "Пометить доску как «Доска оповещений»"
 
-#: aa_forum/forms.py:259
+#: aa_forum/forms.py:304
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. This setting will "
 "not be inherited to child boards. (Default: NO)"
 msgstr ""
 "Пометка «Доска оповещений» обозначает, что только определенные группы могут "
 "начинать новые темы. Все остальные, кто имеет доступ, могут участвовать в "
 "обсуждениях. Эта настройка не распространяется на дочерние доски. (По "
 "умолчанию: НЕТ)"
 
-#: aa_forum/forms.py:267
+#: aa_forum/forms.py:312
 msgid "Start topic restrictions for \"Announcement Boards\""
 msgstr "Ограничения создания новых тем для «Доски оповещений»"
 
-#: aa_forum/forms.py:269
+#: aa_forum/forms.py:314
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
 msgstr ""
 "Пользователи из перечисленных групп смогут создавать новые темы на «Досках "
 "оповещений». Если группы не указаны, только админы форума смогут это делать. "
 "Эта настройка не распространяется на дочерние доски. (Подсказка: Это "
 "ограничение работает только для «Досок оповещений», см. настройку выше.)"
 
-#: aa_forum/forms.py:354
-msgid "Signature"
-msgstr "Подпись"
+#: aa_forum/forms.py:362
+#, fuzzy
+#| msgid "Lock/close topic"
+msgid "Close topic"
+msgstr "Заблокировать/закрыть тему"
 
-#: aa_forum/forms.py:355
-msgid "Your signature will appear below your posts."
-msgstr "Ваша подпись будет отображаться под Вашими сообщениями."
+#: aa_forum/forms.py:364
+msgid "If checked, this topic will be closed after posting this message."
+msgstr ""
+
+#: aa_forum/forms.py:370
+#, fuzzy
+#| msgid "Unlock/re-open topic"
+msgid "Reopen topic"
+msgstr "Разблокировать/открыть тему"
+
+#: aa_forum/forms.py:372
+msgid "If checked, this topic will be reopened after posting this message."
+msgstr ""
+
+#: aa_forum/forms.py:409 aa_forum/forms.py:652 aa_forum/forms.py:717
+msgid "Message"
+msgstr "Сообщение"
 
-#: aa_forum/forms.py:359
+#: aa_forum/forms.py:446
 msgid "Website title"
 msgstr "Заголовок вебсайта"
 
-#: aa_forum/forms.py:361
+#: aa_forum/forms.py:448
 msgid "e.g.: My Homepage"
 msgstr "например: Моя Веб Страница"
 
-#: aa_forum/forms.py:362
+#: aa_forum/forms.py:449
 msgid "Your website's title."
 msgstr "Заголовок Вашего вебсайта."
 
-#: aa_forum/forms.py:366
+#: aa_forum/forms.py:453
 msgid "Website URL"
 msgstr "URL вебсайта"
 
-#: aa_forum/forms.py:370
+#: aa_forum/forms.py:457
 msgid ""
 "Your website's URL. (Don't forget to also set a title for your website, "
 "otherwise this field will be ignored.)"
 msgstr ""
 "URL Вашего вебсайта. (Не забудьте также указать название, иначе это поле "
 "будет проигнорировано.)"
 
-#: aa_forum/forms.py:376
+#: aa_forum/forms.py:463
 msgid "PM me on Discord when I get a new personal message"
 msgstr "Отправлять ЛС в Discord при получении личного сообщения"
 
-#: aa_forum/forms.py:378
+#: aa_forum/forms.py:466
 msgid ""
 "Information: There is currently no module installed that can handle Discord "
 "direct messages. Have a chat with your IT guys to remedy this."
 msgstr ""
 "Информация: в настоящее время не установлены модуля для передачи ЛС в "
 "Discord. Обратитесь в IT поддержку."
 
-#: aa_forum/forms.py:419
+#: aa_forum/forms.py:475
+msgid "Show unread topics as widget on the dashboard"
+msgstr ""
+
+#: aa_forum/forms.py:478
+msgid ""
+"Activating this setting will ad a widget to your dashboard that shows unread "
+"topics in the forum."
+msgstr ""
+
+#: aa_forum/forms.py:507
+msgid "Signature"
+msgstr "Подпись"
+
+#: aa_forum/forms.py:508
+msgid "Your signature will appear below your posts."
+msgstr "Ваша подпись будет отображаться под Вашими сообщениями."
+
+#: aa_forum/forms.py:532
 msgid ""
 "Ensure your signature has at most {max_signature_length} characters. "
 "(Currently: {len(signature)})"
 msgstr ""
 "Убедитесь, что ваша подпись не более {max_signature_length} символов. "
 "(Сейчас: {len(signature)})"
 
-#: aa_forum/forms.py:440
+#: aa_forum/forms.py:554
 msgid "This is not a valid URL"
 msgstr "Некорректный URL"
 
-#: aa_forum/forms.py:456
+#: aa_forum/forms.py:570
 msgid ""
 "How many messages per page should be displayed in a forum topic? (Default: "
 "15)"
 msgstr "Сколько сообщений отображать на странице? (По умолчанию: 15)"
 
-#: aa_forum/forms.py:466
+#: aa_forum/forms.py:580
 msgid ""
 "How many topics per page should be displayed in a forum category? (Default: "
 "10)"
 msgstr "Сколько тем отображать на странице в категории? (По умолчанию: 10)"
 
-#: aa_forum/forms.py:476
+#: aa_forum/forms.py:590
 msgid ""
 "How long (Number of characters) is a user's signature allowed to be? "
 "(Default: 750)"
 msgstr ""
 "Какой длины (количество символов) может быть подпись пользователя? (По "
 "умолчанию: 750)"
 
-#: aa_forum/forms.py:498
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:22
+#: aa_forum/forms.py:612
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:21
 msgid "Recipient"
 msgstr "Получатель"
 
-#: aa_forum/forms.py:504
+#: aa_forum/forms.py:618
 msgid "Hello there …"
 msgstr "Привет…"
 
-#: aa_forum/models.py:127
+#: aa_forum/models.py:139
 msgid "AA-Forum"
 msgstr "АА-форум"
 
-#: aa_forum/models.py:131
+#: aa_forum/models.py:143
 msgid "Can access the AA-Forum module"
 msgstr "Имеет доступ к модулю АА-форум"
 
-#: aa_forum/models.py:134
+#: aa_forum/models.py:146
 msgid "Can manage the AA-Forum module (Category, topics and messages)"
 msgstr "Может управлять модулем АА-форум (категории, темы и сообщения)"
 
-#: aa_forum/models.py:177
+#: aa_forum/models.py:193
 msgid "category"
 msgstr "категория"
 
-#: aa_forum/models.py:178
+#: aa_forum/models.py:194
 msgid "categories"
 msgstr "категории"
 
-#: aa_forum/models.py:222
+#: aa_forum/models.py:248
 msgid ""
 "Use this Discord webhook for replies as well? When activated every reply to "
 "any topic in this board will be posted to the defined Discord channel. "
 "(Child boards are excluded) Chose wisely! (Default: NO)"
 msgstr ""
 "Использовать данный Discord Webhook для ответов? В случае активации каждый "
 "ответ в любой теме доски будет отправлен в канал Discord. (Дочерние доски не "
 "учитываются) Использовать с умом! (По умолчанию: НЕТ)"
 
-#: aa_forum/models.py:240
+#: aa_forum/models.py:266
 msgid ""
 "User in at least one of these groups have access to this board. If no groups "
 "are selected, everyone with access to the forum has also access to this "
 "board."
 msgstr ""
 "Пользователи любой из перечисленных групп будут иметь доступ к доске. Если "
 "группы не выбраны, все пользователи форума будут иметь доступ к доске."
 
-#: aa_forum/models.py:248
+#: aa_forum/models.py:274
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. (Default: NO)"
 msgstr ""
 "Пометка «Доска оповещений» обозначает, что только определенные группы могут "
 "начинать новые темы. Все остальные, кто имеет доступ, могут участвовать в "
 "обсуждениях. (По умолчанию: НЕТ)"
 
-#: aa_forum/models.py:259
+#: aa_forum/models.py:285
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so."
 msgstr ""
 "Пользователи из перечисленных групп смогут создавать новые темы на «Досках "
 "оповещений». Если группы не указаны, только админы форума смогут это делать."
 
-#: aa_forum/models.py:295
+#: aa_forum/models.py:321
 msgid "board"
 msgstr "доска"
 
-#: aa_forum/models.py:296
+#: aa_forum/models.py:322
 msgid "boards"
 msgstr "доски"
 
-#: aa_forum/models.py:367
+#: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
-"<h4>Предупреждение!</h4><p>На доске уже есть тема с таким же "
-"названием.</p><p>См.: <a href=\"{self.topic_url}\">{self._topic."
-"subject}</a></p>"
+"<h4>Предупреждение!</h4><p>На доске уже есть тема с таким же названием.</"
+"p><p>См.: <a href=\"{self.topic_url}\">{self._topic.subject}</a></p>"
 
-#: aa_forum/models.py:578
+#: aa_forum/models.py:625
 msgid "topic"
 msgstr "тема"
 
-#: aa_forum/models.py:579
+#: aa_forum/models.py:626
 msgid "topics"
 msgstr "темы"
 
-#: aa_forum/models.py:736
+#: aa_forum/models.py:805
 msgid "message"
 msgstr "сообщение"
 
-#: aa_forum/models.py:737
+#: aa_forum/models.py:806
 msgid "messages"
 msgstr "сообщения"
 
-#: aa_forum/models.py:872
+#: aa_forum/models.py:948
 msgid "personal message"
 msgstr "личное сообщение"
 
-#: aa_forum/models.py:873
+#: aa_forum/models.py:949
 msgid "personal messages"
 msgstr "личные сообщения"
 
-#: aa_forum/models.py:920
+#: aa_forum/models.py:1003
 msgid "Messages per page"
 msgstr "Сообщений на странице"
 
-#: aa_forum/models.py:921
+#: aa_forum/models.py:1004
 msgid "Topics per page"
 msgstr "Тем на странице"
 
-#: aa_forum/models.py:922
+#: aa_forum/models.py:1005
 msgid "User signature length"
 msgstr "Длина подписи пользователя"
 
-#: aa_forum/models.py:927
+#: aa_forum/models.py:1010
 msgid "Maximum number of messages per page in the topic view"
 msgstr "Максимальное количество сообщений на странице при просмотре темы"
 
-#: aa_forum/models.py:932
+#: aa_forum/models.py:1015
 msgid "Maximum number of topics per page in the board view"
 msgstr "Максимальное количество тем на странице при просмотре доски"
 
-#: aa_forum/models.py:937
+#: aa_forum/models.py:1020
 msgid "Maximum length of a users signature"
 msgstr "Максимальная длина подписи пользователя"
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:1031
 msgid "setting"
 msgstr "настройка"
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:1032
 msgid "settings"
 msgstr "настройки"
 
-#: aa_forum/models.py:952
+#: aa_forum/models.py:1042
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:16
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr "Настройки форума"
 
-#: aa_forum/models.py:978
+#: aa_forum/models.py:1069
 msgid "user profile"
 msgstr "профиль пользователя"
 
-#: aa_forum/models.py:979
+#: aa_forum/models.py:1070
 msgid "user profiles"
 msgstr "профили пользователей"
 
-#: aa_forum/models.py:982
+#: aa_forum/models.py:1080
 msgid "Forum user profile"
 msgstr "профиль пользователя"
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:30
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr "дата:"
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:7
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr "Ответить"
 
-#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:38
+#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:8
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:56
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:73
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:59
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:75
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:69
 msgid "Delete message"
 msgstr "Удалить сообщение"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:13
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:8
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:23
 msgid "Delete board"
 msgstr "Удалить доску"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
+msgid "Close"
+msgstr "Закрыть"
+
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr "Вы уверены, что хотите удалить эту доску?"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
 msgstr "Это также удалит все темы и сообщения на доске."
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:22
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:22
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:21
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:21
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:21
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:20
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:20
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:20
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:19
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:19
 msgid "This action cannot be undone!"
 msgstr "Это действие нельзя будет отменить!"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:29
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:29
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:28
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:28
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:28
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:27
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:27
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
 msgstr "Отмена"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:34
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:34
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:33
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:33
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:33
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
 msgstr "Удалить"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:15
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr "Удалить категорию"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:16
 msgid "Are you sure you want to delete this category?"
 msgstr "Вы уверены, что хотите удалить эту категорию?"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:17
 msgid "This will also remove all boards, topics and messages in this category."
 msgstr "Это также удалит все доски, темы и сообщения в категории."
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr "Изменить блокировку темы"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:13
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:39
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:84
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
 msgid "Unlock/re-open topic"
 msgstr "Разблокировать/открыть тему"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:16
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:42
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:88
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
 msgid "Lock/close topic"
 msgstr "Заблокировать/закрыть тему"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr "Вы уверены что хотите разблокировать эту тему?"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
 msgid "Are you sure you want to lock/close this topic?"
 msgstr "Вы уверены что хотите заблокировать эту тему?"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:3
 msgid "Change sticky state of topic"
 msgstr "Изменить свойство «Sticky» для темы"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:13
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:9
 msgid "Remove \"sticky\" state from topic"
 msgstr "Удалить свойство «Sticky» для темы"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:16
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:12
 msgid "Set \"sticky\" state for topic"
 msgstr "Установить свойство «sticky» для темы"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:22
 msgid "Are you sure you want to remove the sticky state from this topic?"
 msgstr "Вы уверены что хотите удалить свойство «sticky» для темы?"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
 msgid ""
 "Are you sure you want to make this topic sticky, so it always shows up on "
 "top of the topic list?"
 msgstr ""
 "Вы уверены что хотите установить свойство «sticky» для темы, чтобы она "
 "всегда отображалась в начале списка тем?"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:39
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:37
 msgid "Unset sticky"
 msgstr "Удалить свойство «sticky»"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:42
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr "Установить свойство «sticky»"
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:97
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
 msgid "Delete topic"
 msgstr "Удалить тему"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr "Вы уверены, что хотите удалить эту тему?"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:19
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:17
 msgid "This will also remove all messages in this topic."
 msgstr "Это также удалит все сообщения в этой теме."
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:17
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:17
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:15
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:15
 msgid "Are you sure you want to delete this message?"
 msgstr "Вы уверены, что хотите удалить это сообщение?"
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:16
 msgid ""
 "If this message is the original post, then the entire topic will be removed "
 "as well."
 msgstr ""
 "Если данное сообщение является началом темы, вся тема также будет удалена."
 
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:16
 msgid ""
 "If this message is the beginning of a conversation, all related messages "
 "will be removed as well."
 msgstr ""
 "Если данное сообщение является началом разговора, все сообщения разговора "
 "будут удалены."
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:9
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:11
 msgid "Edit board"
 msgstr "Редактировать доску"
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:22
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:36
 msgid ""
 "Changing the name of this board does not change its URL part. This will "
 "remain the same to not break any possible links into this board."
 msgstr ""
 "Изменение названия доски не поменяет URL. Это позволит сохранить "
 "работоспособность всех ранее созданных ссылок на эту доску."
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:58
 msgid "Change board"
 msgstr "Сменить доску"
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:56
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:70
 msgid "New child board"
 msgstr "Новая дочерняя доска"
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:63
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:62
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:77
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:84
 msgid ""
 "New boards will be added at the bottom of the board list for this category. "
 "You can move them via drag and drop to a position of your liking."
 msgstr ""
 "Новые доски будут добавлены в конец списка данной категории. В дальнейшем Вы "
 "сможете перетащить их на желаемую позицию."
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:79
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:75
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:93
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:97
 msgid "Create board"
 msgstr "Создать доску"
 
-#: aa_forum/templates/aa_forum/partials/administration/categories.html:6
+#: aa_forum/templates/aa_forum/partials/administration/categories.html:5
 msgid ""
 "Here you can create, modify and delete categories and boards. You also can "
 "change their order via drag and drop."
 msgstr ""
 "Здесь вы можете создавать, изменять и удалять категории и доски. Также можно "
 "менять порядок следования с помощью перетаскивания."
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:11
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:13
 msgid "Edit category"
 msgstr "Редактировать категорию"
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:19
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:35
 msgid "Expand/collapse category"
 msgstr "Развернуть/свернуть категорию"
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:31
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:53
 msgid ""
 "Changing the name of this category does not change its URL part. This will "
 "remain the same to not break any possible links into this category."
 msgstr ""
 "Изменение названия категории не поменяет URL. Это позволит сохранить "
 "работоспособность всех ранее созданных ссылок на эту категорию."
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:66
 msgid "Change category"
 msgstr "Сменить категорию"
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:55
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:77
 msgid "New board"
 msgstr "Новая доска"
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:7
 msgid "Create new category"
 msgstr "Создать новую категорию"
 
@@ -654,24 +698,25 @@
 "сможете перетащить их на желаемую позицию."
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:35
 msgid "Create category"
 msgstr "Создать категорию"
 
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:21
-#: aa_forum/templates/aa_forum/partials/profile/form.html:21
+#: aa_forum/templates/aa_forum/partials/profile/form.html:22
 msgid "Submit"
 msgstr "Отправить"
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:6
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:7
 msgid "Forum index"
 msgstr "Индекс форума"
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:27
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:49
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:51
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:6
 msgid "Modify message"
 msgstr "Изменить сообщение"
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:34
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:7
@@ -694,69 +739,69 @@
 "Вы хотите помочь перевести это приложение на ваш язык или улучшить текущий "
 "перевод?"
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Присоединяйтесь к нашей команде переводчиков!"
 
-#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:9
+#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr "Поля, отмеченные (*) обязательны"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr "Эта доска не содержит тем…"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:34
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] "К доске имеют доступ следующая группа:"
 msgstr[1] "К доске имеют доступ следующие группы:"
 msgstr[2] "К доске имеют доступ следующие группы:"
 msgstr[3] "К доске имеют доступ следующие группы:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr "Дочерние доски:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:51
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
 msgid "New"
 msgstr "Новый"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr "Сообщения"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
 msgid "Topics"
 msgstr "Темы"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:66
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:65
 msgid "Unread"
 msgstr "Непрочитанные"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:82
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:88
 msgid "Last post:"
 msgstr "Последнее сообщение:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:86
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:25
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:96
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:26
 msgid "Re:"
 msgstr "Ответ на:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:103
 msgid "posted by:"
 msgstr "отправитель:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:94
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:104
 msgid "posted at:"
 msgstr "отправлено:"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:7
+#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:8
 msgid "New topic"
 msgstr "Новая тема"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/no-access.html:6
 msgid ""
 "You either don't have access to this board, or this board doesn't exist."
 msgstr "У Вас нет прав доступа к доске или доска не существует."
@@ -822,58 +867,58 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr "Последний"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
 msgid "Topic is always on top"
 msgstr "Тема всегда в начале"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
 msgid "Topic is locked"
 msgstr "Тема закрыта"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
 msgid "Started by"
 msgstr "Запущена"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
 msgid "Replies"
 msgstr "Ответы"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
 msgid "Last post"
 msgstr "Последнее сообщение"
 
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
 msgid "Go to last message"
 msgstr "Перейти к последнему сообщению"
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
 msgid "Change topics sticky state"
 msgstr "Изменить свойство Sticky для темы"
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr "Отметить все темы как прочитанные"
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:38
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:39
 msgid "Copy message link to clipboard"
 msgstr "Скопировать ссылку на сообщение в буфер обмена"
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:81
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:87
 msgid "Last modified:"
 msgstr "Изменено:"
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:14
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
 msgstr ""
 "Примечание: Вы не на последней странице темы и могли пропустить свежие "
 "ответы."
 
@@ -883,68 +928,65 @@
 msgstr "Изменить"
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:6
 msgid "Modify topic"
 msgstr "Изменить тему"
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:20
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:21
 msgid "Warning: this topic is locked! Only admins can reply."
 msgstr "Внимание: эта тема закрыта! Отвечать могут только админы."
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:33
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:44
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
 msgid "Clear form"
 msgstr "Очистить форму"
 
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:7
 msgid "Show all unread topics"
 msgstr "Показать все непрочитанные темы"
 
-#: aa_forum/templates/aa_forum/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr "Переключить навигацию"
-
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:7
 msgid "Administration"
 msgstr "Администрирование"
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:12
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:13
 msgid "Categories and boards"
 msgstr "Категории и доски"
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:6
-#: aa_forum/templates/aa_forum/view/profile/index.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:13
+#: aa_forum/templates/aa_forum/view/profile/index.html:7
 msgid "Profile"
 msgstr "Профиль"
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:11
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:19
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:9
 msgid "Messages"
 msgstr "Сообщения"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:23
 msgid "Inbox"
 msgstr "Входящие"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:18
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:18
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:17
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:17
 msgid "Date"
 msgstr "Дата"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:22
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:21
 msgid "Sender"
 msgstr "Отправитель"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:62
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:63
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:57
 msgid "Read message"
 msgstr "Прочитать сообщение"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:87
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:93
 msgid "No personal messages"
 msgstr "Нет личных сообщений"
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:8
 msgid "New personal message"
 msgstr "Новое личное сообщение"
 
@@ -952,359 +994,357 @@
 msgid "Send message"
 msgstr "Отправить сообщение"
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:8
 msgid "Reply to:"
 msgstr "Кому:"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:24
+#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:23
 msgid "Send reply"
 msgstr "Ответить"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:30
 msgid "Sent messages"
 msgstr "Отправленные сообщения"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:56
-msgid "Read Message"
-msgstr "Прочитать сообщение"
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:67
-msgid "Delete Message"
-msgstr "Удалить сообщение"
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:81
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:87
 msgid "No personal messages sent"
 msgstr "Нет отправленных личных сообщений"
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:17
 msgid "New message"
 msgstr "Новое сообщение"
 
 #: aa_forum/templates/aa_forum/partials/profile/form.html:7
 msgid "User profile"
 msgstr "профиль пользователя"
 
-#: aa_forum/templates/aa_forum/partials/search/search-form.html:7
+#: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr "Поиск…"
 
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+#, fuzzy
+#| msgid "Unread topics"
+msgid "Forum: Unread topics"
+msgstr "Непрочитанные темы"
+
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr "Администрирование (Категории и доски)"
 
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:6
 msgid "Administration (Forum settings)"
 msgstr "Администрирование (Настройки)"
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:26
+#: aa_forum/templates/aa_forum/view/forum/index.html:27
 msgid "New posts"
 msgstr "Новые сообщения"
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:35
+#: aa_forum/templates/aa_forum/view/forum/index.html:36
 msgid "No new posts"
 msgstr "Нет новых сообщений"
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:22
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:21
 msgid "Start new topic in"
 msgstr "Начать новую тему в"
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:38
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
 msgid "Start topic"
 msgstr "Начать тему"
 
-#: aa_forum/templates/aa_forum/view/forum/topic.html:23
+#: aa_forum/templates/aa_forum/view/forum/topic.html:24
 msgid "Modify topic subject"
 msgstr "Изменить заголовок темы"
 
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:6
 msgid "Unread topics"
 msgstr "Непрочитанные темы"
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:16
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:15
 msgid "Unread Topics"
 msgstr "Непрочитанные темы"
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:31
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:30
 msgid "You have no unread topics …"
 msgstr "У Вас нет непрочитанных тем…"
 
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:7
 msgid "Personal messages (Inbox)"
 msgstr "Персональные сообщения (Входящие)"
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:7
 msgid "Personal messages (New message)"
 msgstr "Персональные сообщения (Новое сообщение)"
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:39
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:35
 msgid "Enter the recipients name"
 msgstr "Введите имя получателя"
 
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:7
 msgid "Personal messages (Reply to message)"
 msgstr "Персональные сообщения (Ответить на сообщение)"
 
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:7
 msgid "Personal messages (Sent messages)"
 msgstr "Персональные Сообщения (Отправленные сообщения)"
 
 #: aa_forum/templates/aa_forum/view/search/results.html:6
 msgid "Search results"
 msgstr "Результаты поиска"
 
-#: aa_forum/templates/aa_forum/view/search/results.html:22
+#: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] "%(counter)s Результат"
 msgstr[1] "%(counter)s Результата"
 msgstr[2] "%(counter)s Результатов"
 msgstr[3] "%(counter)s Результатов"
 
-#: aa_forum/templates/aa_forum/view/search/results.html:32
+#: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr "Ничего не найдено…"
 
-#: aa_forum/templatetags/aa_forum_datetime.py:57
+#: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
 msgstr "Преобразование временной зоны"
 
-#: aa_forum/views/admin.py:165
+#: aa_forum/views/admin.py:169
 msgid "<h4>Success!</h4><p>Category created.</p>"
 msgstr "<h4>Успех!</h4><p>Категория создана.</p>"
 
-#: aa_forum/views/admin.py:205
+#: aa_forum/views/admin.py:212
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Category name changed from \"{category_name_old}\" to "
 "\"{category.name}\".</p>"
 msgstr ""
 "<h4>Успех!</h4><p>Имя категории изменено с «{category_name_old}» на "
 "«{category.name}».</p>"
 
-#: aa_forum/views/admin.py:245
+#: aa_forum/views/admin.py:255
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Category \"{category_name}\" removed.</p>"
 msgstr "<h4>Успех!</h4><p>Категория «{category_name}» удалена.</p>"
 
-#: aa_forum/views/admin.py:298 aa_forum/views/admin.py:354
+#: aa_forum/views/admin.py:311 aa_forum/views/admin.py:371
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{new_board.name}\" created.</p>"
 msgstr "<h4>Успех!</h4><p>Доска «{new_board.name}» создана.</p>"
 
-#: aa_forum/views/admin.py:409
+#: aa_forum/views/admin.py:430
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board.name}\" changed.</p>"
 msgstr "<h4>Успех!</h4><p>Доска «{board.name}» изменена.</p>"
 
-#: aa_forum/views/admin.py:450
+#: aa_forum/views/admin.py:475
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board_name}\" removed.</p>"
 msgstr "<h4>Успех!</h4><p>Доска «{board_name}» удалена.</p>"
 
-#: aa_forum/views/admin.py:556
+#: aa_forum/views/admin.py:587
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr "<h4>Успех!</h4><p>Настройки обновлены.</p>"
 
-#: aa_forum/views/admin.py:566 aa_forum/views/personal_messages.py:116
-#: aa_forum/views/personal_messages.py:237 aa_forum/views/profile.py:68
+#: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
+#: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr "<h4>Ошибка!</h4><p>Что-то сломалось, проверьте введенные данные.</p>"
 
-#: aa_forum/views/forum.py:225
+#: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Доска, на которую вы пытаетесь попасть, не существует или "
 "Вам не доступна.</p>"
 
-#: aa_forum/views/forum.py:282
+#: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
-"<h4>Ошибка!</h4><p>Категория, в которую в попытались написать, не "
-"существует.</p>"
+"<h4>Ошибка!</h4><p>Категория, в которую в попытались написать, не существует."
+"</p>"
 
-#: aa_forum/views/forum.py:309
+#: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Доска, на которую вы пытаетесь написать, не существует "
 "или Вам не доступна.</p>"
 
-#: aa_forum/views/forum.py:329
+#: aa_forum/views/forum.py:340
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in is an announcement "
 "board and you don't have the permissions to start a topic there.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Доска, на которой вы пытались разместить сообщение, "
 "является доской объявлений, и у вас нет разрешений создавать там тему.</p>"
 
-#: aa_forum/views/forum.py:386
+#: aa_forum/views/forum.py:399
 msgid ""
 "<h4>Error!</h4><p>Either subject or message is missing. Please make sure you "
 "enter both fields, as both fields are mandatory.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Отсутствует название или текст сообщения. Заполните оба "
 "поля.</p>"
 
-#: aa_forum/views/forum.py:442 aa_forum/views/forum.py:672
+#: aa_forum/views/forum.py:461 aa_forum/views/forum.py:706
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to view does not exist or you do "
 "not have access to it.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Тема, которую вы пытаетесь посмотреть, не существует или "
 "Вам не доступна.</p>"
 
-#: aa_forum/views/forum.py:539
+#: aa_forum/views/forum.py:563
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to modify does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Тема, которую вы пытаетесь изменить, не существует или "
 "Вам не доступна.</p>"
 
-#: aa_forum/views/forum.py:561
+#: aa_forum/views/forum.py:585
 msgid "<h4>Error!</h4><p>You are not allowed to modify this topic!</p>"
 msgstr "<h4>Ошибка!</h4><p>Вам не разрешается изменять эту тему!</p>"
 
-#: aa_forum/views/forum.py:593
+#: aa_forum/views/forum.py:617
 msgid "<h4>Success!</h4><p>The topic subject has been updated.</p>"
 msgstr "<h4>Успех!</h4><p>Название темы изменено.</p>"
 
-#: aa_forum/views/forum.py:791
+#: aa_forum/views/forum.py:845
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to reply does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Тема, в которой вы пытаетесь ответить, не существует или "
 "Вам не доступна.</p>"
 
-#: aa_forum/views/forum.py:847
+#: aa_forum/views/forum.py:922
 msgid "<h4>Error!</h4><p>Message field is mandatory and cannot be empty.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Текст сообщения должен присутствовать и не может быть "
 "пустым.</p>"
 
-#: aa_forum/views/forum.py:856
+#: aa_forum/views/forum.py:931
 msgid "<h4>Error!</h4><p>Something went wrong, please try again.</p>"
 msgstr "<h4>Ошибка!</h4><p>Что-то пошло не так, попробуйте еще раз.</p>"
 
-#: aa_forum/views/forum.py:894
+#: aa_forum/views/forum.py:972
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been unlocked/re-opened.</"
 "p>"
 msgstr "<h4>Успех!</h4><p>Тема «{current_topic}» была открыта.</p>"
 
-#: aa_forum/views/forum.py:908
+#: aa_forum/views/forum.py:986
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been locked/closed.</p>"
 msgstr "<h4>Успех!</h4><p>Тема «{current_topic}» была закрыта.</p>"
 
-#: aa_forum/views/forum.py:949
+#: aa_forum/views/forum.py:1030
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{curent_topic}\" is no longer \"sticky\".</p>"
 msgstr "<h4>Успех!</h4><p>Тема «{curent_topic}» больше не «Sticky».</p>"
 
-#: aa_forum/views/forum.py:963
+#: aa_forum/views/forum.py:1044
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{curent_topic}\" is now \"sticky\".</p>"
 msgstr "<h4>Успех!</h4><p>Тема «{curent_topic}» теперь «Sticky».</p>"
 
-#: aa_forum/views/forum.py:998
+#: aa_forum/views/forum.py:1082
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{topic__subject}\" removed.</p>"
 msgstr "<h4>Успех!</h4><p>Тема «{topic__subject}» удалена.</p>"
 
-#: aa_forum/views/forum.py:1034
+#: aa_forum/views/forum.py:1124
 msgid "<h4>Error!</h4><p>The message doesn't exist.</p>"
 msgstr "<h4>Ошибка!</h4><p>Сообщение не существует.</p>"
 
-#: aa_forum/views/forum.py:1078
+#: aa_forum/views/forum.py:1174
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to modify does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Сообщение, которое Вы пытаетесь изменить, не существует "
 "или Вам не доступно.</p>"
 
-#: aa_forum/views/forum.py:1101
+#: aa_forum/views/forum.py:1197
 msgid "<h4>Error!</h4><p>You are not allowed to modify this message!</p>"
 msgstr "<h4>Ошибка!</h4><p>Вам не разрешается изменять это сообщение!</p>"
 
-#: aa_forum/views/forum.py:1128
+#: aa_forum/views/forum.py:1224
 msgid "<h4>Success!</h4><p>The message has been updated.</p>"
 msgstr "<h4>Успех!</h4><p>Сообщение изменено.</p>"
 
-#: aa_forum/views/forum.py:1151
+#: aa_forum/views/forum.py:1247
 msgid "<h4>Error!</h4><p>Mandatory form field is empty.</p>"
 msgstr "<h4>Ошибка!</h4><p>Необходимые поля формы не заполнены.</p>"
 
-#: aa_forum/views/forum.py:1241
+#: aa_forum/views/forum.py:1345
 msgid "<h4>Error!</h4><p>You are not allowed to delete this message!</p>"
 msgstr "<h4>Ошибка!</h4><p>Вам не разрешается удалять это сообщение!</p>"
 
-#: aa_forum/views/forum.py:1271
+#: aa_forum/views/forum.py:1375
 msgid "<h4>Success!</h4><p>The message has been deleted.</p>"
 msgstr "<h4>Успех!</h4><p>Сообщение удалено.</p>"
 
-#: aa_forum/views/forum.py:1296
+#: aa_forum/views/forum.py:1400
 msgid ""
 "<h4>Success!</h4><p>The message has been deleted.</p><p>This was the topics "
 "opening post, so the topic has been deleted as well.</p>"
 msgstr ""
 "<h4>Успех!</h4><p>Сообщение удалено.</p><p>Это было стартовое сообщение "
 "темы, так что вся тема также удалена.</p>"
 
-#: aa_forum/views/personal_messages.py:104
+#: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr ""
-"<h4>Успех!</h4><p>Сообщение пользователю {recipient_main_char} "
-"отправлено.</p>"
+"<h4>Успех!</h4><p>Сообщение пользователю {recipient_main_char} отправлено.</"
+"p>"
 
-#: aa_forum/views/personal_messages.py:190
+#: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Сообщение, на которое Вы пытаетесь ответить, не "
 "существует или Вы не являетесь получателем.</p>"
 
-#: aa_forum/views/personal_messages.py:226
+#: aa_forum/views/personal_messages.py:238
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Reply to {recipient_main_char} sent.</p>"
 msgstr ""
 "<h4>Успех!</h4><p>Ответ пользователю {recipient_main_char} отправлен.</p>"
 
-#: aa_forum/views/personal_messages.py:282
-#: aa_forum/views/personal_messages.py:319
+#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:335
 msgid ""
 "<h4>Error!</h4><p>The message you tried to remove does either not exist or "
 "is not yours to remove.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Сообщение, которое Вы пытаетесь удалить, не существует "
 "или оно не Ваше.</p>"
 
-#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:314
 msgid "<h4>Success!</h4><p>Message removed from your inbox.</p>"
 msgstr "<h4>Успех!</h4><p>Сообщение удалено из входящих.</p>"
 
-#: aa_forum/views/personal_messages.py:337
+#: aa_forum/views/personal_messages.py:353
 msgid ""
 "<h4>Success!</h4><p>Message has been removed from your sent messages.</p>"
 msgstr "<h4>Успех!</h4><p>Сообщение удалено из отправленных.</p>"
 
-#: aa_forum/views/personal_messages.py:352
+#: aa_forum/views/personal_messages.py:368
 msgid "<h4>Error!</h4><p>Something went wrong.</p>"
 msgstr "<h4>Упс!</h4><p>Что-то пошло не так!</p>"
 
-#: aa_forum/views/profile.py:58
+#: aa_forum/views/profile.py:60
 msgid "<h4>Success!</h4><p>Profile saved.</p>"
 msgstr "<h4>Успех!</h4><p>Профиль сохранен.</p>"
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/uk/LC_MESSAGES/django.mo` & `aa_forum-2.1.0/aa_forum/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/uk/LC_MESSAGES/django.po` & `aa_forum-2.1.0/aa_forum/locale/uk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,598 +3,643 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # "Andrii M." <elfleg0las88@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 18:29+0200\n"
+"POT-Creation-Date: 2024-04-03 14:16+0200\n"
 "PO-Revision-Date: 2023-10-02 09:34+0000\n"
 "Last-Translator: \"Andrii M.\" <elfleg0las88@gmail.com>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/uk/>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-forum/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 5.0.2\n"
 
-#: aa_forum/__init__.py:12 aa_forum/templates/aa_forum/base.html:5
-#: aa_forum/templates/aa_forum/partials/menu.html:14
+#: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
+#: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
-#: aa_forum/templates/aa_forum/view/forum/board.html:5
-#: aa_forum/templates/aa_forum/view/forum/index.html:6
+#: aa_forum/templates/aa_forum/view/forum/board.html:6
+#: aa_forum/templates/aa_forum/view/forum/index.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:8
-#: aa_forum/templates/aa_forum/view/forum/topic.html:5
+#: aa_forum/templates/aa_forum/view/forum/topic.html:6
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:7
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:9
-#: aa_forum/templates/aa_forum/view/profile/index.html:9
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
 msgstr ""
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr ""
 
-#: aa_forum/forms.py:40
+#: aa_forum/forms.py:42
 msgid "This field is mandatory"
 msgstr "Це поле обовʼязкове"
 
-#: aa_forum/forms.py:91 aa_forum/forms.py:93 aa_forum/forms.py:124
-#: aa_forum/forms.py:126 aa_forum/forms.py:502
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:26
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:26
+#: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
+#: aa_forum/forms.py:171 aa_forum/forms.py:616
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr "Тема"
 
-#: aa_forum/forms.py:102 aa_forum/forms.py:321 aa_forum/forms.py:512
-#: aa_forum/forms.py:558
-msgid "Message"
-msgstr "Повідомлення"
+#: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
+#: aa_forum/forms.py:730
+msgid "You have forgotten the message!"
+msgstr ""
 
-#: aa_forum/forms.py:145 aa_forum/forms.py:183 aa_forum/forms.py:204
+#: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
 msgstr "Назва"
 
-#: aa_forum/forms.py:147 aa_forum/forms.py:185
+#: aa_forum/forms.py:192 aa_forum/forms.py:230
 #, fuzzy
 #| msgid "Category Name"
 msgid "Category name"
 msgstr "Назва категорії"
 
-#: aa_forum/forms.py:151 aa_forum/forms.py:162
+#: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
 msgstr "Дошки"
 
-#: aa_forum/forms.py:153
+#: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
 
-#: aa_forum/forms.py:206
+#: aa_forum/forms.py:251
 #, fuzzy
 #| msgid "Boards"
 msgid "Board name"
 msgstr "Дошки"
 
-#: aa_forum/forms.py:210
+#: aa_forum/forms.py:255
 msgid "Description"
 msgstr ""
 
-#: aa_forum/forms.py:216
+#: aa_forum/forms.py:261
 msgid "Board description (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:222
+#: aa_forum/forms.py:267
 msgid "Group restrictions"
 msgstr "Групові обмеження"
 
-#: aa_forum/forms.py:224
+#: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:232
+#: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:234
+#: aa_forum/forms.py:279
 msgid ""
 "Discord webhook URL for the channel to post about new topics in this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:247
+#: aa_forum/forms.py:292
 msgid "Use this Discord webhook for replies as well?"
 msgstr ""
 
-#: aa_forum/forms.py:249
+#: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
 msgstr ""
 
-#: aa_forum/forms.py:257
+#: aa_forum/forms.py:302
 msgid "Mark board as \"Announcement Board\""
 msgstr ""
 
-#: aa_forum/forms.py:259
+#: aa_forum/forms.py:304
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. This setting will "
 "not be inherited to child boards. (Default: NO)"
 msgstr ""
 
-#: aa_forum/forms.py:267
+#: aa_forum/forms.py:312
 msgid "Start topic restrictions for \"Announcement Boards\""
 msgstr ""
 
-#: aa_forum/forms.py:269
+#: aa_forum/forms.py:314
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
 msgstr ""
 
-#: aa_forum/forms.py:354
-msgid "Signature"
+#: aa_forum/forms.py:362
+#, fuzzy
+#| msgid "Delete"
+msgid "Close topic"
+msgstr "Видалити"
+
+#: aa_forum/forms.py:364
+msgid "If checked, this topic will be closed after posting this message."
 msgstr ""
 
-#: aa_forum/forms.py:355
-msgid "Your signature will appear below your posts."
+#: aa_forum/forms.py:370
+#, fuzzy
+#| msgid "Delete"
+msgid "Reopen topic"
+msgstr "Видалити"
+
+#: aa_forum/forms.py:372
+msgid "If checked, this topic will be reopened after posting this message."
 msgstr ""
 
-#: aa_forum/forms.py:359
+#: aa_forum/forms.py:409 aa_forum/forms.py:652 aa_forum/forms.py:717
+msgid "Message"
+msgstr "Повідомлення"
+
+#: aa_forum/forms.py:446
 msgid "Website title"
 msgstr ""
 
-#: aa_forum/forms.py:361
+#: aa_forum/forms.py:448
 msgid "e.g.: My Homepage"
 msgstr ""
 
-#: aa_forum/forms.py:362
+#: aa_forum/forms.py:449
 msgid "Your website's title."
 msgstr ""
 
-#: aa_forum/forms.py:366
+#: aa_forum/forms.py:453
 msgid "Website URL"
 msgstr ""
 
-#: aa_forum/forms.py:370
+#: aa_forum/forms.py:457
 msgid ""
 "Your website's URL. (Don't forget to also set a title for your website, "
 "otherwise this field will be ignored.)"
 msgstr ""
 
-#: aa_forum/forms.py:376
+#: aa_forum/forms.py:463
 msgid "PM me on Discord when I get a new personal message"
 msgstr ""
 
-#: aa_forum/forms.py:378
+#: aa_forum/forms.py:466
 msgid ""
 "Information: There is currently no module installed that can handle Discord "
 "direct messages. Have a chat with your IT guys to remedy this."
 msgstr ""
 
-#: aa_forum/forms.py:419
+#: aa_forum/forms.py:475
+msgid "Show unread topics as widget on the dashboard"
+msgstr ""
+
+#: aa_forum/forms.py:478
+msgid ""
+"Activating this setting will ad a widget to your dashboard that shows unread "
+"topics in the forum."
+msgstr ""
+
+#: aa_forum/forms.py:507
+msgid "Signature"
+msgstr ""
+
+#: aa_forum/forms.py:508
+msgid "Your signature will appear below your posts."
+msgstr ""
+
+#: aa_forum/forms.py:532
 msgid ""
 "Ensure your signature has at most {max_signature_length} characters. "
 "(Currently: {len(signature)})"
 msgstr ""
 
-#: aa_forum/forms.py:440
+#: aa_forum/forms.py:554
 msgid "This is not a valid URL"
 msgstr ""
 
-#: aa_forum/forms.py:456
+#: aa_forum/forms.py:570
 msgid ""
 "How many messages per page should be displayed in a forum topic? (Default: "
 "15)"
 msgstr ""
 
-#: aa_forum/forms.py:466
+#: aa_forum/forms.py:580
 msgid ""
 "How many topics per page should be displayed in a forum category? (Default: "
 "10)"
 msgstr ""
 
-#: aa_forum/forms.py:476
+#: aa_forum/forms.py:590
 msgid ""
 "How long (Number of characters) is a user's signature allowed to be? "
 "(Default: 750)"
 msgstr ""
 
-#: aa_forum/forms.py:498
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:22
+#: aa_forum/forms.py:612
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:21
 msgid "Recipient"
 msgstr ""
 
-#: aa_forum/forms.py:504
+#: aa_forum/forms.py:618
 msgid "Hello there …"
 msgstr ""
 
-#: aa_forum/models.py:127
+#: aa_forum/models.py:139
 msgid "AA-Forum"
 msgstr ""
 
-#: aa_forum/models.py:131
+#: aa_forum/models.py:143
 msgid "Can access the AA-Forum module"
 msgstr ""
 
-#: aa_forum/models.py:134
+#: aa_forum/models.py:146
 msgid "Can manage the AA-Forum module (Category, topics and messages)"
 msgstr ""
 
-#: aa_forum/models.py:177
+#: aa_forum/models.py:193
 msgid "category"
 msgstr ""
 
-#: aa_forum/models.py:178
+#: aa_forum/models.py:194
 msgid "categories"
 msgstr ""
 
-#: aa_forum/models.py:222
+#: aa_forum/models.py:248
 msgid ""
 "Use this Discord webhook for replies as well? When activated every reply to "
 "any topic in this board will be posted to the defined Discord channel. "
 "(Child boards are excluded) Chose wisely! (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:240
+#: aa_forum/models.py:266
 msgid ""
 "User in at least one of these groups have access to this board. If no groups "
 "are selected, everyone with access to the forum has also access to this "
 "board."
 msgstr ""
 
-#: aa_forum/models.py:248
+#: aa_forum/models.py:274
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:259
+#: aa_forum/models.py:285
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so."
 msgstr ""
 
-#: aa_forum/models.py:295
+#: aa_forum/models.py:321
 msgid "board"
 msgstr ""
 
-#: aa_forum/models.py:296
+#: aa_forum/models.py:322
 msgid "boards"
 msgstr ""
 
-#: aa_forum/models.py:367
+#: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:578
+#: aa_forum/models.py:625
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:579
+#: aa_forum/models.py:626
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:736
+#: aa_forum/models.py:805
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:737
+#: aa_forum/models.py:806
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:872
+#: aa_forum/models.py:948
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:873
+#: aa_forum/models.py:949
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:920
+#: aa_forum/models.py:1003
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:921
+#: aa_forum/models.py:1004
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:922
+#: aa_forum/models.py:1005
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:927
+#: aa_forum/models.py:1010
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:932
+#: aa_forum/models.py:1015
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:937
+#: aa_forum/models.py:1020
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:1031
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:1032
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:952
+#: aa_forum/models.py:1042
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:16
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:978
+#: aa_forum/models.py:1069
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:979
+#: aa_forum/models.py:1070
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:982
+#: aa_forum/models.py:1080
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:30
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:7
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:38
+#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:8
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:56
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:73
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:59
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:75
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:69
 #, fuzzy
 #| msgid "Delete"
 msgid "Delete message"
 msgstr "Видалити"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:13
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:8
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:23
 #, fuzzy
 #| msgid "Delete"
 msgid "Delete board"
 msgstr "Видалити"
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
+msgid "Close"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:22
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:22
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:21
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:21
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:21
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:20
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:20
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:20
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:19
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:19
 msgid "This action cannot be undone!"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:29
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:29
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:28
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:28
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:28
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:27
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:27
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:34
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:34
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:33
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:33
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:33
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
 msgstr "Видалити"
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:15
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:16
 msgid "Are you sure you want to delete this category?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:17
 msgid "This will also remove all boards, topics and messages in this category."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:13
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:39
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:84
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
 msgid "Unlock/re-open topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:16
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:42
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:88
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
 msgid "Lock/close topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
 msgid "Are you sure you want to lock/close this topic?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:3
 msgid "Change sticky state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:13
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:9
 msgid "Remove \"sticky\" state from topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:16
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:12
 msgid "Set \"sticky\" state for topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:22
 msgid "Are you sure you want to remove the sticky state from this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
 msgid ""
 "Are you sure you want to make this topic sticky, so it always shows up on "
 "top of the topic list?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:39
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:37
 msgid "Unset sticky"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:42
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:97
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
 #, fuzzy
 #| msgid "Delete"
 msgid "Delete topic"
 msgstr "Видалити"
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:19
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:17
 msgid "This will also remove all messages in this topic."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:17
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:17
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:15
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:15
 msgid "Are you sure you want to delete this message?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:16
 msgid ""
 "If this message is the original post, then the entire topic will be removed "
 "as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:16
 msgid ""
 "If this message is the beginning of a conversation, all related messages "
 "will be removed as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:9
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:11
 msgid "Edit board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:22
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:36
 msgid ""
 "Changing the name of this board does not change its URL part. This will "
 "remain the same to not break any possible links into this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:58
 msgid "Change board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:56
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:70
 msgid "New child board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:63
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:62
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:77
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:84
 msgid ""
 "New boards will be added at the bottom of the board list for this category. "
 "You can move them via drag and drop to a position of your liking."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:79
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:75
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:93
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:97
 msgid "Create board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/categories.html:6
+#: aa_forum/templates/aa_forum/partials/administration/categories.html:5
 msgid ""
 "Here you can create, modify and delete categories and boards. You also can "
 "change their order via drag and drop."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:11
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:13
 msgid "Edit category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:19
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:35
 msgid "Expand/collapse category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:31
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:53
 msgid ""
 "Changing the name of this category does not change its URL part. This will "
 "remain the same to not break any possible links into this category."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:66
 msgid "Change category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:55
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:77
 msgid "New board"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:7
 msgid "Create new category"
 msgstr ""
 
@@ -609,24 +654,25 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:35
 msgid "Create category"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:21
-#: aa_forum/templates/aa_forum/partials/profile/form.html:21
+#: aa_forum/templates/aa_forum/partials/profile/form.html:22
 msgid "Submit"
 msgstr "Відправити"
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:6
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:7
 msgid "Forum index"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:27
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:49
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:51
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:6
 #, fuzzy
 #| msgid "Message"
 msgid "Modify message"
 msgstr "Повідомлення"
 
@@ -649,69 +695,69 @@
 "existing translation?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:9
+#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:34
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:51
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
 msgid "New"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
 msgid "Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:66
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:65
 msgid "Unread"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:82
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:88
 msgid "Last post:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:86
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:25
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:96
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:26
 msgid "Re:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:103
 msgid "posted by:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:94
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:104
 msgid "posted at:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:7
+#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:8
 msgid "New topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/no-access.html:6
 msgid ""
 "You either don't have access to this board, or this board doesn't exist."
 msgstr ""
@@ -777,58 +823,58 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
 msgid "Last post"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:38
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:39
 msgid "Copy message link to clipboard"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:81
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:87
 msgid "Last modified:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:14
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:27
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:21
@@ -836,70 +882,67 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:6
 msgid "Modify topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:20
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:21
 msgid "Warning: this topic is locked! Only admins can reply."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:33
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:44
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
 msgid "Clear form"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:7
 msgid "Show all unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:7
 msgid "Administration"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:12
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:13
 msgid "Categories and boards"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:6
-#: aa_forum/templates/aa_forum/view/profile/index.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:13
+#: aa_forum/templates/aa_forum/view/profile/index.html:7
 msgid "Profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:11
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:19
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:9
 msgid "Messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:23
 msgid "Inbox"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:18
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:18
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:17
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:17
 msgid "Date"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:22
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:21
 msgid "Sender"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:62
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:63
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:57
 #, fuzzy
 #| msgid "Message"
 msgid "Read message"
 msgstr "Повідомлення"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:87
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:93
 msgid "No personal messages"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:8
 msgid "New personal message"
 msgstr ""
 
@@ -909,332 +952,328 @@
 msgid "Send message"
 msgstr "Повідомлення"
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:8
 msgid "Reply to:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:24
+#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:23
 msgid "Send reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:30
 #, fuzzy
 #| msgid "Message"
 msgid "Sent messages"
 msgstr "Повідомлення"
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:56
-msgid "Read Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:67
-msgid "Delete Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:81
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:87
 msgid "No personal messages sent"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:17
 #, fuzzy
 #| msgid "Message"
 msgid "New message"
 msgstr "Повідомлення"
 
 #: aa_forum/templates/aa_forum/partials/profile/form.html:7
 msgid "User profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/search/search-form.html:7
+#: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+msgid "Forum: Unread topics"
+msgstr ""
+
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:6
 msgid "Administration (Forum settings)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:26
+#: aa_forum/templates/aa_forum/view/forum/index.html:27
 msgid "New posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:35
+#: aa_forum/templates/aa_forum/view/forum/index.html:36
 msgid "No new posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:22
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:21
 msgid "Start new topic in"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:38
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
 msgid "Start topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/topic.html:23
+#: aa_forum/templates/aa_forum/view/forum/topic.html:24
 msgid "Modify topic subject"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:6
 msgid "Unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:16
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:15
 msgid "Unread Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:31
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:30
 msgid "You have no unread topics …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:7
 msgid "Personal messages (Inbox)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:7
 msgid "Personal messages (New message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:39
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:35
 msgid "Enter the recipients name"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:7
 msgid "Personal messages (Reply to message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:7
 msgid "Personal messages (Sent messages)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:6
 msgid "Search results"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:22
+#: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:32
+#: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
-#: aa_forum/templatetags/aa_forum_datetime.py:57
+#: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
 msgstr ""
 
-#: aa_forum/views/admin.py:165
+#: aa_forum/views/admin.py:169
 msgid "<h4>Success!</h4><p>Category created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:205
+#: aa_forum/views/admin.py:212
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Category name changed from \"{category_name_old}\" to "
 "\"{category.name}\".</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:245
+#: aa_forum/views/admin.py:255
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Category \"{category_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:298 aa_forum/views/admin.py:354
+#: aa_forum/views/admin.py:311 aa_forum/views/admin.py:371
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{new_board.name}\" created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:409
+#: aa_forum/views/admin.py:430
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board.name}\" changed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:450
+#: aa_forum/views/admin.py:475
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:556
+#: aa_forum/views/admin.py:587
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:566 aa_forum/views/personal_messages.py:116
-#: aa_forum/views/personal_messages.py:237 aa_forum/views/profile.py:68
+#: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
+#: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:225
+#: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:282
+#: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:309
+#: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:329
+#: aa_forum/views/forum.py:340
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in is an announcement "
 "board and you don't have the permissions to start a topic there.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:386
+#: aa_forum/views/forum.py:399
 msgid ""
 "<h4>Error!</h4><p>Either subject or message is missing. Please make sure you "
 "enter both fields, as both fields are mandatory.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:442 aa_forum/views/forum.py:672
+#: aa_forum/views/forum.py:461 aa_forum/views/forum.py:706
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to view does not exist or you do "
 "not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:539
+#: aa_forum/views/forum.py:563
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to modify does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:561
+#: aa_forum/views/forum.py:585
 msgid "<h4>Error!</h4><p>You are not allowed to modify this topic!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:593
+#: aa_forum/views/forum.py:617
 msgid "<h4>Success!</h4><p>The topic subject has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:791
+#: aa_forum/views/forum.py:845
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to reply does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:847
+#: aa_forum/views/forum.py:922
 msgid "<h4>Error!</h4><p>Message field is mandatory and cannot be empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:856
+#: aa_forum/views/forum.py:931
 msgid "<h4>Error!</h4><p>Something went wrong, please try again.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:894
+#: aa_forum/views/forum.py:972
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been unlocked/re-opened.</"
 "p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:908
+#: aa_forum/views/forum.py:986
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been locked/closed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:949
+#: aa_forum/views/forum.py:1030
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{curent_topic}\" is no longer \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:963
+#: aa_forum/views/forum.py:1044
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{curent_topic}\" is now \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:998
+#: aa_forum/views/forum.py:1082
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{topic__subject}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1034
+#: aa_forum/views/forum.py:1124
 msgid "<h4>Error!</h4><p>The message doesn't exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1078
+#: aa_forum/views/forum.py:1174
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to modify does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1101
+#: aa_forum/views/forum.py:1197
 msgid "<h4>Error!</h4><p>You are not allowed to modify this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1128
+#: aa_forum/views/forum.py:1224
 msgid "<h4>Success!</h4><p>The message has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1151
+#: aa_forum/views/forum.py:1247
 msgid "<h4>Error!</h4><p>Mandatory form field is empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1241
+#: aa_forum/views/forum.py:1345
 msgid "<h4>Error!</h4><p>You are not allowed to delete this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1271
+#: aa_forum/views/forum.py:1375
 msgid "<h4>Success!</h4><p>The message has been deleted.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1296
+#: aa_forum/views/forum.py:1400
 msgid ""
 "<h4>Success!</h4><p>The message has been deleted.</p><p>This was the topics "
 "opening post, so the topic has been deleted as well.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:104
+#: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:190
+#: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:226
+#: aa_forum/views/personal_messages.py:238
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Reply to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:282
-#: aa_forum/views/personal_messages.py:319
+#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:335
 msgid ""
 "<h4>Error!</h4><p>The message you tried to remove does either not exist or "
 "is not yours to remove.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:314
 msgid "<h4>Success!</h4><p>Message removed from your inbox.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:337
+#: aa_forum/views/personal_messages.py:353
 msgid ""
 "<h4>Success!</h4><p>Message has been removed from your sent messages.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:352
+#: aa_forum/views/personal_messages.py:368
 msgid "<h4>Error!</h4><p>Something went wrong.</p>"
 msgstr ""
 
-#: aa_forum/views/profile.py:58
+#: aa_forum/views/profile.py:60
 msgid "<h4>Success!</h4><p>Profile saved.</p>"
 msgstr ""
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_forum-2.1.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,19 +7,25 @@
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-forum/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.4.2\n"
+
+msgid "Cancel"
+msgstr "取消"
 
 msgid "Category name"
 msgstr "分类名称"
 
+msgid "Close"
+msgstr "关闭"
+
 msgid "Delete"
 msgstr "删除"
 
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
```

### Comparing `aa_forum-2.0.0b3/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_forum-2.1.0/aa_forum/locale/nl/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,589 +1,629 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Dehao Wu <wudehao2000@163.com>, 2024.
-# Peter Pfeufer <info@ppfeufer.de>, 2024.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 18:29+0200\n"
-"PO-Revision-Date: 2024-02-06 07:10+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-forum/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"POT-Creation-Date: 2024-04-03 14:16+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: aa_forum/__init__.py:12 aa_forum/templates/aa_forum/base.html:5
-#: aa_forum/templates/aa_forum/partials/menu.html:14
+#: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
+#: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
-#: aa_forum/templates/aa_forum/view/forum/board.html:5
-#: aa_forum/templates/aa_forum/view/forum/index.html:6
+#: aa_forum/templates/aa_forum/view/forum/board.html:6
+#: aa_forum/templates/aa_forum/view/forum/index.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:8
-#: aa_forum/templates/aa_forum/view/forum/topic.html:5
+#: aa_forum/templates/aa_forum/view/forum/topic.html:6
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:7
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:9
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:9
-#: aa_forum/templates/aa_forum/view/profile/index.html:9
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/profile/index.html:8
 #: aa_forum/templates/aa_forum/view/search/results.html:7
 msgid "Forum"
-msgstr "论坛"
+msgstr ""
 
 #: aa_forum/apps.py:20
 #, python-brace-format
 msgid "AA Forum v{__version__}"
 msgstr ""
 
-#: aa_forum/forms.py:40
+#: aa_forum/forms.py:42
 msgid "This field is mandatory"
-msgstr "这个字段是必填的"
+msgstr ""
 
-#: aa_forum/forms.py:91 aa_forum/forms.py:93 aa_forum/forms.py:124
-#: aa_forum/forms.py:126 aa_forum/forms.py:502
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:26
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:26
+#: aa_forum/forms.py:116 aa_forum/forms.py:118 aa_forum/forms.py:169
+#: aa_forum/forms.py:171 aa_forum/forms.py:616
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:25
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:25
 msgid "Subject"
 msgstr ""
 
-#: aa_forum/forms.py:102 aa_forum/forms.py:321 aa_forum/forms.py:512
-#: aa_forum/forms.py:558
-msgid "Message"
+#: aa_forum/forms.py:145 aa_forum/forms.py:422 aa_forum/forms.py:665
+#: aa_forum/forms.py:730
+msgid "You have forgotten the message!"
 msgstr ""
 
-#: aa_forum/forms.py:145 aa_forum/forms.py:183 aa_forum/forms.py:204
+#: aa_forum/forms.py:190 aa_forum/forms.py:228 aa_forum/forms.py:249
 msgid "Name"
-msgstr "名字"
+msgstr ""
 
-#: aa_forum/forms.py:147 aa_forum/forms.py:185
+#: aa_forum/forms.py:192 aa_forum/forms.py:230
 msgid "Category name"
-msgstr "分类名称"
+msgstr ""
 
-#: aa_forum/forms.py:151 aa_forum/forms.py:162
+#: aa_forum/forms.py:196 aa_forum/forms.py:207
 msgid "Boards"
 msgstr ""
 
-#: aa_forum/forms.py:153
+#: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
 
-#: aa_forum/forms.py:206
+#: aa_forum/forms.py:251
 msgid "Board name"
 msgstr ""
 
-#: aa_forum/forms.py:210
+#: aa_forum/forms.py:255
 msgid "Description"
 msgstr ""
 
-#: aa_forum/forms.py:216
+#: aa_forum/forms.py:261
 msgid "Board description (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:222
+#: aa_forum/forms.py:267
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_forum/forms.py:224
+#: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:232
+#: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
 msgstr ""
 
-#: aa_forum/forms.py:234
+#: aa_forum/forms.py:279
 msgid ""
 "Discord webhook URL for the channel to post about new topics in this board. "
 "(This setting is optional)"
 msgstr ""
 
-#: aa_forum/forms.py:247
+#: aa_forum/forms.py:292
 msgid "Use this Discord webhook for replies as well?"
 msgstr ""
 
-#: aa_forum/forms.py:249
+#: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
 msgstr ""
 
-#: aa_forum/forms.py:257
+#: aa_forum/forms.py:302
 msgid "Mark board as \"Announcement Board\""
 msgstr ""
 
-#: aa_forum/forms.py:259
+#: aa_forum/forms.py:304
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. This setting will "
 "not be inherited to child boards. (Default: NO)"
 msgstr ""
 
-#: aa_forum/forms.py:267
+#: aa_forum/forms.py:312
 msgid "Start topic restrictions for \"Announcement Boards\""
 msgstr ""
 
-#: aa_forum/forms.py:269
+#: aa_forum/forms.py:314
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so. This setting will not be inherited to child boards. (Hint: These "
 "restrictions only take effect when a board is marked as \"Announcement "
 "Board\", see checkbox above.)"
 msgstr ""
 
-#: aa_forum/forms.py:354
-msgid "Signature"
+#: aa_forum/forms.py:362
+msgid "Close topic"
 msgstr ""
 
-#: aa_forum/forms.py:355
-msgid "Your signature will appear below your posts."
+#: aa_forum/forms.py:364
+msgid "If checked, this topic will be closed after posting this message."
+msgstr ""
+
+#: aa_forum/forms.py:370
+msgid "Reopen topic"
+msgstr ""
+
+#: aa_forum/forms.py:372
+msgid "If checked, this topic will be reopened after posting this message."
 msgstr ""
 
-#: aa_forum/forms.py:359
+#: aa_forum/forms.py:409 aa_forum/forms.py:652 aa_forum/forms.py:717
+msgid "Message"
+msgstr ""
+
+#: aa_forum/forms.py:446
 msgid "Website title"
 msgstr ""
 
-#: aa_forum/forms.py:361
+#: aa_forum/forms.py:448
 msgid "e.g.: My Homepage"
 msgstr ""
 
-#: aa_forum/forms.py:362
+#: aa_forum/forms.py:449
 msgid "Your website's title."
 msgstr ""
 
-#: aa_forum/forms.py:366
+#: aa_forum/forms.py:453
 msgid "Website URL"
 msgstr ""
 
-#: aa_forum/forms.py:370
+#: aa_forum/forms.py:457
 msgid ""
 "Your website's URL. (Don't forget to also set a title for your website, "
 "otherwise this field will be ignored.)"
 msgstr ""
 
-#: aa_forum/forms.py:376
+#: aa_forum/forms.py:463
 msgid "PM me on Discord when I get a new personal message"
 msgstr ""
 
-#: aa_forum/forms.py:378
+#: aa_forum/forms.py:466
 msgid ""
 "Information: There is currently no module installed that can handle Discord "
 "direct messages. Have a chat with your IT guys to remedy this."
 msgstr ""
 
-#: aa_forum/forms.py:419
+#: aa_forum/forms.py:475
+msgid "Show unread topics as widget on the dashboard"
+msgstr ""
+
+#: aa_forum/forms.py:478
+msgid ""
+"Activating this setting will ad a widget to your dashboard that shows unread "
+"topics in the forum."
+msgstr ""
+
+#: aa_forum/forms.py:507
+msgid "Signature"
+msgstr ""
+
+#: aa_forum/forms.py:508
+msgid "Your signature will appear below your posts."
+msgstr ""
+
+#: aa_forum/forms.py:532
 msgid ""
 "Ensure your signature has at most {max_signature_length} characters. "
 "(Currently: {len(signature)})"
 msgstr ""
 
-#: aa_forum/forms.py:440
+#: aa_forum/forms.py:554
 msgid "This is not a valid URL"
 msgstr ""
 
-#: aa_forum/forms.py:456
+#: aa_forum/forms.py:570
 msgid ""
 "How many messages per page should be displayed in a forum topic? (Default: "
 "15)"
 msgstr ""
 
-#: aa_forum/forms.py:466
+#: aa_forum/forms.py:580
 msgid ""
 "How many topics per page should be displayed in a forum category? (Default: "
 "10)"
 msgstr ""
 
-#: aa_forum/forms.py:476
+#: aa_forum/forms.py:590
 msgid ""
 "How long (Number of characters) is a user's signature allowed to be? "
 "(Default: 750)"
 msgstr ""
 
-#: aa_forum/forms.py:498
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:22
+#: aa_forum/forms.py:612
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:21
 msgid "Recipient"
 msgstr ""
 
-#: aa_forum/forms.py:504
+#: aa_forum/forms.py:618
 msgid "Hello there …"
 msgstr ""
 
-#: aa_forum/models.py:127
+#: aa_forum/models.py:139
 msgid "AA-Forum"
 msgstr ""
 
-#: aa_forum/models.py:131
+#: aa_forum/models.py:143
 msgid "Can access the AA-Forum module"
 msgstr ""
 
-#: aa_forum/models.py:134
+#: aa_forum/models.py:146
 msgid "Can manage the AA-Forum module (Category, topics and messages)"
 msgstr ""
 
-#: aa_forum/models.py:177
+#: aa_forum/models.py:193
 msgid "category"
 msgstr ""
 
-#: aa_forum/models.py:178
+#: aa_forum/models.py:194
 msgid "categories"
 msgstr ""
 
-#: aa_forum/models.py:222
+#: aa_forum/models.py:248
 msgid ""
 "Use this Discord webhook for replies as well? When activated every reply to "
 "any topic in this board will be posted to the defined Discord channel. "
 "(Child boards are excluded) Chose wisely! (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:240
+#: aa_forum/models.py:266
 msgid ""
 "User in at least one of these groups have access to this board. If no groups "
 "are selected, everyone with access to the forum has also access to this "
 "board."
 msgstr ""
 
-#: aa_forum/models.py:248
+#: aa_forum/models.py:274
 msgid ""
 "Mark this board as an \"Announcement Board\", meaning that only certain "
 "selected groups can start new topics. All others who have access to this "
 "board will still be able to discuss in the topics though. (Default: NO)"
 msgstr ""
 
-#: aa_forum/models.py:259
+#: aa_forum/models.py:285
 msgid ""
 "User in at least one of the selected groups will be able to start topics in "
 "\"Announcement Boards\". If no group is selected, only forum admins can do "
 "so."
 msgstr ""
 
-#: aa_forum/models.py:295
+#: aa_forum/models.py:321
 msgid "board"
 msgstr ""
 
-#: aa_forum/models.py:296
+#: aa_forum/models.py:322
 msgid "boards"
 msgstr ""
 
-#: aa_forum/models.py:367
+#: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
 
-#: aa_forum/models.py:578
+#: aa_forum/models.py:625
 msgid "topic"
 msgstr ""
 
-#: aa_forum/models.py:579
+#: aa_forum/models.py:626
 msgid "topics"
 msgstr ""
 
-#: aa_forum/models.py:736
+#: aa_forum/models.py:805
 msgid "message"
 msgstr ""
 
-#: aa_forum/models.py:737
+#: aa_forum/models.py:806
 msgid "messages"
 msgstr ""
 
-#: aa_forum/models.py:872
+#: aa_forum/models.py:948
 msgid "personal message"
 msgstr ""
 
-#: aa_forum/models.py:873
+#: aa_forum/models.py:949
 msgid "personal messages"
 msgstr ""
 
-#: aa_forum/models.py:920
+#: aa_forum/models.py:1003
 msgid "Messages per page"
 msgstr ""
 
-#: aa_forum/models.py:921
+#: aa_forum/models.py:1004
 msgid "Topics per page"
 msgstr ""
 
-#: aa_forum/models.py:922
+#: aa_forum/models.py:1005
 msgid "User signature length"
 msgstr ""
 
-#: aa_forum/models.py:927
+#: aa_forum/models.py:1010
 msgid "Maximum number of messages per page in the topic view"
 msgstr ""
 
-#: aa_forum/models.py:932
+#: aa_forum/models.py:1015
 msgid "Maximum number of topics per page in the board view"
 msgstr ""
 
-#: aa_forum/models.py:937
+#: aa_forum/models.py:1020
 msgid "Maximum length of a users signature"
 msgstr ""
 
-#: aa_forum/models.py:948
+#: aa_forum/models.py:1031
 msgid "setting"
 msgstr ""
 
-#: aa_forum/models.py:949
+#: aa_forum/models.py:1032
 msgid "settings"
 msgstr ""
 
-#: aa_forum/models.py:952
+#: aa_forum/models.py:1042
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:7
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:16
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:19
 msgid "Forum settings"
 msgstr ""
 
-#: aa_forum/models.py:978
+#: aa_forum/models.py:1069
 msgid "user profile"
 msgstr ""
 
-#: aa_forum/models.py:979
+#: aa_forum/models.py:1070
 msgid "user profiles"
 msgstr ""
 
-#: aa_forum/models.py:982
+#: aa_forum/models.py:1080
 msgid "Forum user profile"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:21
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:30
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:31
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html:21
 msgid "on:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:30
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:7
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:55
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:48
 msgid "Reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:38
+#: aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html:39
 #: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:8
 #: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:3
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:56
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:73
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:59
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:75
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:69
 msgid "Delete message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-board.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:13
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:8
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:23
 msgid "Delete board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:12
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:17
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:11
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:11
+msgid "Close"
+msgstr ""
+
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:16
 msgid "Are you sure you want to delete this board?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:17
 msgid "This will also remove all topics and messages in this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:22
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:22
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:21
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:21
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:21
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:20
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:20
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:20
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:19
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:19
 msgid "This action cannot be undone!"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:29
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:29
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:33
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:28
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:28
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:28
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:27
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:27
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:31
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:27
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:26
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:26
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:35
 msgid "Cancel"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:34
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:34
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:33
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:33
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:33
+#: aa_forum/templates/aa_forum/modals/administration/delete-board.html:32
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:32
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:32
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:31
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:31
 msgid "Delete"
-msgstr "删除"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/administration/delete-category.html:3
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:12
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:15
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:8
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:25
 msgid "Delete category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:18
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:16
 msgid "Are you sure you want to delete this category?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:19
+#: aa_forum/templates/aa_forum/modals/administration/delete-category.html:17
 msgid "This will also remove all boards, topics and messages in this category."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:3
 msgid "Change lock state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:13
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:39
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:84
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:9
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:37
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:89
 msgid "Unlock/re-open topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:16
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:42
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:88
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:12
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:40
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:99
 msgid "Lock/close topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:22
 msgid "Are you sure you want to unlock/re-open this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html:24
 msgid "Are you sure you want to lock/close this topic?"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:3
 msgid "Change sticky state of topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:13
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:9
 msgid "Remove \"sticky\" state from topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:16
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:12
 msgid "Set \"sticky\" state for topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:22
 msgid "Are you sure you want to remove the sticky state from this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:26
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:24
 msgid ""
 "Are you sure you want to make this topic sticky, so it always shows up on "
 "top of the topic list?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:39
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:37
 msgid "Unset sticky"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:42
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html:40
 msgid "Make sticky"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:3
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:12
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:97
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:8
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:120
 msgid "Delete topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:16
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:19
+#: aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html:17
 msgid "This will also remove all messages in this topic."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:17
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:17
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:15
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:15
 msgid "Are you sure you want to delete this message?"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html:16
 msgid ""
 "If this message is the original post, then the entire topic will be removed "
 "as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:18
+#: aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html:16
 msgid ""
 "If this message is the beginning of a conversation, all related messages "
 "will be removed as well."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:9
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:11
 msgid "Edit board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:22
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:36
 msgid ""
 "Changing the name of this board does not change its URL part. This will "
 "remain the same to not break any possible links into this board."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:58
 msgid "Change board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:56
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:70
 msgid "New child board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:63
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:62
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:77
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:84
 msgid ""
 "New boards will be added at the bottom of the board list for this category. "
 "You can move them via drag and drop to a position of your liking."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:79
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:75
+#: aa_forum/templates/aa_forum/partials/administration/board-loop.html:93
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:97
 msgid "Create board"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/categories.html:6
+#: aa_forum/templates/aa_forum/partials/administration/categories.html:5
 msgid ""
 "Here you can create, modify and delete categories and boards. You also can "
 "change their order via drag and drop."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:11
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:13
 msgid "Edit category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:19
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:35
 msgid "Expand/collapse category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:31
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:53
 msgid ""
 "Changing the name of this category does not change its URL part. This will "
 "remain the same to not break any possible links into this category."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:44
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:66
 msgid "Change category"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:55
+#: aa_forum/templates/aa_forum/partials/administration/category-loop.html:77
 msgid "New board"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:7
 msgid "Create new category"
 msgstr ""
 
@@ -598,24 +638,25 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/new-category.html:35
 msgid "Create category"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/administration/settings-form.html:21
-#: aa_forum/templates/aa_forum/partials/profile/form.html:21
+#: aa_forum/templates/aa_forum/partials/profile/form.html:22
 msgid "Submit"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:6
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:7
 msgid "Forum index"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:27
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:49
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:51
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-message.html:6
 msgid "Modify message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/breadcrumb.html:34
 #: aa_forum/templates/aa_forum/view/forum/new-topic.html:7
@@ -630,72 +671,73 @@
 msgid "Search for:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "加入我们的翻译团队吧！"
+msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:9
+#: aa_forum/templates/aa_forum/partials/form/required-field-hint.html:6
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "带有(*)星号符号的字段是必填的"
+msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board-index.html:27
 msgid "No topics have been started in this board …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:34
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
+msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:42
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:51
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:31
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
 msgid "New"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:60
 msgid "Posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:61
 msgid "Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:66
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:65
 msgid "Unread"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:82
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:88
 msgid "Last post:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:86
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:25
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:96
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:26
 msgid "Re:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:103
 msgid "posted by:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/board.html:94
+#: aa_forum/templates/aa_forum/partials/forum/board/board.html:104
 msgid "posted at:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:7
+#: aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html:8
 msgid "New topic"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/no-access.html:6
 msgid ""
 "You either don't have access to this board, or this board doesn't exist."
 msgstr ""
@@ -761,58 +803,58 @@
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:66
 #: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html:75
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:65
 #: aa_forum/templates/aa_forum/partials/search/pagination.html:74
 msgid "Last"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:38
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:36
 msgid "Topic is always on top"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:44
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:42
 msgid "Topic is locked"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:48
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:46
 msgid "Started by"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:59
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:62
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:57
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:60
 msgid "Replies"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:69
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:67
 msgid "Last post"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:71
 msgid "Go to last message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:93
+#: aa_forum/templates/aa_forum/partials/forum/board/topic.html:110
 msgid "Change topics sticky state"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html:7
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:12
 msgid "Mark all topics as read"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:38
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:39
 msgid "Copy message link to clipboard"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:81
+#: aa_forum/templates/aa_forum/partials/forum/topic/message.html:87
 msgid "Last modified:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:14
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:27
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:21
@@ -820,68 +862,65 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
 #: aa_forum/templates/aa_forum/view/forum/modify-topic.html:6
 msgid "Modify topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:20
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:21
 msgid "Warning: this topic is locked! Only admins can reply."
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:33
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
+#: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:44
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:36
 msgid "Clear form"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html:7
 msgid "Show all unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:7
 msgid "Administration"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:12
+#: aa_forum/templates/aa_forum/partials/menu/menu-admin.html:13
 msgid "Categories and boards"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:6
-#: aa_forum/templates/aa_forum/view/profile/index.html:8
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:13
+#: aa_forum/templates/aa_forum/view/profile/index.html:7
 msgid "Profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:11
+#: aa_forum/templates/aa_forum/partials/menu/menu-user.html:19
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:9
 msgid "Messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:23
 msgid "Inbox"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:18
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:18
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:17
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:17
 msgid "Date"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:22
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:21
 msgid "Sender"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:62
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:63
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:57
 msgid "Read message"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:87
+#: aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html:93
 msgid "No personal messages"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html:8
 msgid "New personal message"
 msgstr ""
 
@@ -889,325 +928,322 @@
 msgid "Send message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:8
 msgid "Reply to:"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:24
+#: aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html:23
 msgid "Send reply"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:10
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:9
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:30
 msgid "Sent messages"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:56
-msgid "Read Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:67
-msgid "Delete Message"
-msgstr ""
-
-#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:81
+#: aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html:87
 msgid "No personal messages sent"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html:17
 msgid "New message"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/profile/form.html:7
 msgid "User profile"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/partials/search/search-form.html:7
+#: aa_forum/templates/aa_forum/partials/search/search-form.html:13
 msgid "Search …"
 msgstr ""
 
+#: aa_forum/templates/aa_forum/partials/widgets/unread-topics.html:6
+msgid "Forum: Unread topics"
+msgstr ""
+
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:6
 msgid "Administration (Categories and boards)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:6
 msgid "Administration (Forum settings)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:26
+#: aa_forum/templates/aa_forum/view/forum/index.html:27
 msgid "New posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/index.html:35
+#: aa_forum/templates/aa_forum/view/forum/index.html:36
 msgid "No new posts"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:22
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:21
 msgid "Start new topic in"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/new-topic.html:38
+#: aa_forum/templates/aa_forum/view/forum/new-topic.html:37
 msgid "Start topic"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/topic.html:23
+#: aa_forum/templates/aa_forum/view/forum/topic.html:24
 msgid "Modify topic subject"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/forum/unread-topics.html:6
 msgid "Unread topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:16
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:15
 msgid "Unread Topics"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:31
+#: aa_forum/templates/aa_forum/view/forum/unread-topics.html:30
 msgid "You have no unread topics …"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/inbox.html:7
 msgid "Personal messages (Inbox)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:7
 msgid "Personal messages (New message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:39
+#: aa_forum/templates/aa_forum/view/personal-messages/new-message.html:35
 msgid "Enter the recipients name"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/reply-message.html:7
 msgid "Personal messages (Reply to message)"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:8
+#: aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html:7
 msgid "Personal messages (Sent messages)"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:6
 msgid "Search results"
 msgstr ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:22
+#: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
+msgstr[1] ""
 
-#: aa_forum/templates/aa_forum/view/search/results.html:32
+#: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
-#: aa_forum/templatetags/aa_forum_datetime.py:57
+#: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
 msgstr ""
 
-#: aa_forum/views/admin.py:165
+#: aa_forum/views/admin.py:169
 msgid "<h4>Success!</h4><p>Category created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:205
+#: aa_forum/views/admin.py:212
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Category name changed from \"{category_name_old}\" to "
 "\"{category.name}\".</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:245
+#: aa_forum/views/admin.py:255
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Category \"{category_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:298 aa_forum/views/admin.py:354
+#: aa_forum/views/admin.py:311 aa_forum/views/admin.py:371
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{new_board.name}\" created.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:409
+#: aa_forum/views/admin.py:430
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board.name}\" changed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:450
+#: aa_forum/views/admin.py:475
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Board \"{board_name}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:556
+#: aa_forum/views/admin.py:587
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr ""
 
-#: aa_forum/views/admin.py:566 aa_forum/views/personal_messages.py:116
-#: aa_forum/views/personal_messages.py:237 aa_forum/views/profile.py:68
+#: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
+#: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:225
+#: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:282
+#: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:309
+#: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:329
+#: aa_forum/views/forum.py:340
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in is an announcement "
 "board and you don't have the permissions to start a topic there.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:386
+#: aa_forum/views/forum.py:399
 msgid ""
 "<h4>Error!</h4><p>Either subject or message is missing. Please make sure you "
 "enter both fields, as both fields are mandatory.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:442 aa_forum/views/forum.py:672
+#: aa_forum/views/forum.py:461 aa_forum/views/forum.py:706
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to view does not exist or you do "
 "not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:539
+#: aa_forum/views/forum.py:563
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to modify does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:561
+#: aa_forum/views/forum.py:585
 msgid "<h4>Error!</h4><p>You are not allowed to modify this topic!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:593
+#: aa_forum/views/forum.py:617
 msgid "<h4>Success!</h4><p>The topic subject has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:791
+#: aa_forum/views/forum.py:845
 msgid ""
 "<h4>Error!</h4><p>The topic you were trying to reply does not exist or you "
 "do not have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:847
+#: aa_forum/views/forum.py:922
 msgid "<h4>Error!</h4><p>Message field is mandatory and cannot be empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:856
+#: aa_forum/views/forum.py:931
 msgid "<h4>Error!</h4><p>Something went wrong, please try again.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:894
+#: aa_forum/views/forum.py:972
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been unlocked/re-opened.</"
 "p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:908
+#: aa_forum/views/forum.py:986
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{current_topic}\" has been locked/closed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:949
+#: aa_forum/views/forum.py:1030
 #, python-brace-format
 msgid ""
 "<h4>Success!</h4><p>Topic \"{curent_topic}\" is no longer \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:963
+#: aa_forum/views/forum.py:1044
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{curent_topic}\" is now \"sticky\".</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:998
+#: aa_forum/views/forum.py:1082
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Topic \"{topic__subject}\" removed.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1034
+#: aa_forum/views/forum.py:1124
 msgid "<h4>Error!</h4><p>The message doesn't exist.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1078
+#: aa_forum/views/forum.py:1174
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to modify does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1101
+#: aa_forum/views/forum.py:1197
 msgid "<h4>Error!</h4><p>You are not allowed to modify this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1128
+#: aa_forum/views/forum.py:1224
 msgid "<h4>Success!</h4><p>The message has been updated.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1151
+#: aa_forum/views/forum.py:1247
 msgid "<h4>Error!</h4><p>Mandatory form field is empty.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1241
+#: aa_forum/views/forum.py:1345
 msgid "<h4>Error!</h4><p>You are not allowed to delete this message!</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1271
+#: aa_forum/views/forum.py:1375
 msgid "<h4>Success!</h4><p>The message has been deleted.</p>"
 msgstr ""
 
-#: aa_forum/views/forum.py:1296
+#: aa_forum/views/forum.py:1400
 msgid ""
 "<h4>Success!</h4><p>The message has been deleted.</p><p>This was the topics "
 "opening post, so the topic has been deleted as well.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:104
+#: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:190
+#: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:226
+#: aa_forum/views/personal_messages.py:238
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Reply to {recipient_main_char} sent.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:282
-#: aa_forum/views/personal_messages.py:319
+#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:335
 msgid ""
 "<h4>Error!</h4><p>The message you tried to remove does either not exist or "
 "is not yours to remove.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:298
+#: aa_forum/views/personal_messages.py:314
 msgid "<h4>Success!</h4><p>Message removed from your inbox.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:337
+#: aa_forum/views/personal_messages.py:353
 msgid ""
 "<h4>Success!</h4><p>Message has been removed from your sent messages.</p>"
 msgstr ""
 
-#: aa_forum/views/personal_messages.py:352
+#: aa_forum/views/personal_messages.py:368
 msgid "<h4>Error!</h4><p>Something went wrong.</p>"
 msgstr ""
 
-#: aa_forum/views/profile.py:58
+#: aa_forum/views/profile.py:60
 msgid "<h4>Success!</h4><p>Profile saved.</p>"
 msgstr ""
```

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0001_initial.py` & `aa_forum-2.1.0/aa_forum/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0002_default_settings.py` & `aa_forum-2.1.0/aa_forum/migrations/0002_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0004_board_use_webhook_for_replies.py` & `aa_forum-2.1.0/aa_forum/migrations/0004_board_use_webhook_for_replies.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0005_announcement_boards.py` & `aa_forum-2.1.0/aa_forum/migrations/0005_announcement_boards.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0006_reset_default_settings.py` & `aa_forum-2.1.0/aa_forum/migrations/0006_reset_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0007_change_settings_to_singleton.py` & `aa_forum-2.1.0/aa_forum/migrations/0007_change_settings_to_singleton.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0008_populate_default_settings.py` & `aa_forum-2.1.0/aa_forum/migrations/0008_populate_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0009_add_related_names.py` & `aa_forum-2.1.0/aa_forum/migrations/0009_add_related_names.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0010_better_setting_names.py` & `aa_forum-2.1.0/aa_forum/migrations/0010_better_setting_names.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0011_userprofile.py` & `aa_forum-2.1.0/aa_forum/migrations/0011_userprofile.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0012_personal_messages.py` & `aa_forum-2.1.0/aa_forum/migrations/0012_personal_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py` & `aa_forum-2.1.0/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py` & `aa_forum-2.1.0/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0016_fix_quotation_marks.py` & `aa_forum-2.1.0/aa_forum/migrations/0016_fix_quotation_marks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py` & `aa_forum-2.1.0/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/scripts/drop_tables.sql` & `aa_forum-2.1.0/aa_forum/scripts/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/scripts/fake_messages.py` & `aa_forum-2.1.0/aa_forum/scripts/fake_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/css/aa-forum.css` & `aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.css`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     }
 
     .aa-forum .aa-forum-message-body-last-edited {
         margin-top: 5rem;
     }
 
     .aa-forum .aa-forum-message-body img {
-        height: auto !important; /* to override inline style added by cKeditor */
+        height: auto !important; /* to override inline style added by CKEditor */
         max-width: 100%;
     }
 }
 
 /* Search view
 ------------------------------------------------------------------------------------- */
 @media all {
```

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/css/aa-forum.min.css` & `aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/css/aa-forum.min.css.map` & `aa_forum-2.1.0/aa_forum/static/aa_forum/css/aa-forum.min.css.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'sourcesContent'": "['/* Variable "*

 * *                     'definitions\\n------------------------------------------------------------------------------------- '*

 * *                     '*/\\n:root {\\n    --bg-hover-transition: background-color 0.25s '*

 * *                     'linear;\\n}\\n\\n/* '*

 * *                     'General\\n------------------------------------------------------------------------------------- '*

 * *                     '*/\\n@media all {\\n    .aa-forum .aa-forum-svg-wrapper {\\n        height: […]*

```diff
@@ -2,11 +2,11 @@
     "file": "aa-forum.css",
     "mappings": "AAEA,K,CACI,mD,CAKJ,WACI,+B,CACI,Q,CACA,O,CAOJ,mE,CACI,kB,CAOJ,kC,CACI,6B,CAIJ,0B,CADA,8B,CAEI,oB,CAGJ,yC,CACI,e,CAGJ,0D,CACI,Y,CAGJ,wCAA0C,yB,CACtC,Y,CAGJ,4B,CACI,W,CAOJ,iC,CACI,oB,CACA,S,CAGJ,oC,CACI,c,CAGJ,gD,CACI,c,CAOJ,iD,CACI,kB,CACA,qC,CAGJ,4D,CACI,e,CAGJ,uD,CACI,wB,CAGJ,2D,CACI,W,CACA,gB,CACA,U,CAGJ,sD,CACI,U,CAGJ,2C,CACI,Q,CAGJ,4C,CACI,oB,CACA,Q,CACA,S,CAGJ,yD,CACI,U,CACA,W,CACA,iB,CACA,U,CAGJ,0D,CACI,e,CACA,sB,CACA,kB,CACA,gB,CAGJ,+B,CACI,Y,CACA,iB,CAGJ,qD,CACI,W,CACA,U,CAGJ,gD,CACI,oB,CAGJ,0C,CACI,c,CAOJ,6C,CACI,oB,CACA,kB,CACA,Y,CACA,kB,CACA,qC,CAyBJ,+E,CAtBA,wD,CACI,e,CAGJ,mD,CACI,wB,CAGJ,mE,CACI,U,CAGJ,uE,CACI,W,CACA,gB,CACA,U,CAGJ,kE,CACI,U,CAOJ,mE,CACI,iB,CACA,S,CAGJ,uE,CACI,S,CAGJ,qE,CACI,U,CAGJ,gC,CACI,qC,CAGJ,gC,CACI,qC,CAGJ,2C,CACI,a,CAGJ,iD,CACI,a,CACA,kB,CACA,iB,CACA,qB,CAOJ,qD,CACI,c,CAGJ,mC,CACI,U,CAGJ,gC,CACI,qC,CAGJ,iD,CACI,qC,CACA,c,CAGJ,4C,CACI,e,CAGJ,oC,CACI,qB,CACA,c,CAOJ,uC,CACI,sB,CACA,Y,CACA,oB,CACA,mC,CAGJ,+C,CACI,c,CACA,kB,CACA,kB,CAGJ,yC,CACI,c,CACA,kB,CACA,iB,CACA,c,CACA,Y,CAGJ,yC,CACI,U,CAGJ,yC,CACI,8B,CACA,e,CACA,e,CAOJ,+C,CACI,Y,CACA,qC,CAGJ,qD,CACI,wB,CAGJ,sD,CACI,wC,CACA,e,CAGJ,sD,CACI,e,CAGJ,mD,CACI,e,CAGJ,qDAAqD,S,CACjD,8C,CAGJ,yD,CACI,gC,CAOJ,kC,CACI,kB,CACA,sB,CACA,sB,CACA,U,CAGJ,gD,CACI,oB,CACA,qB,CACA,c,CACA,a,CACA,oB,CAGJ,0C,CACI,Y,CAOJ,wC,CACI,c,CAGJ,8C,CACA,8C,CACA,8C,CACI,a,CACA,yC,CACA,mB,CAGJ,8B,CACI,kB,CAOJ,uB,CACI,qC,CACA,W,CAGJ,qB,CACI,mB,CACA,a,CAGJ,0C,CACI,qB,CAGJ,mD,CACI,4B,CACA,mB,CACA,S,CAOJ,yC,CACI,wB,CAOJ,6B,CACI,0C,CAGJ,8B,CACI,a,CAGJ,wB,CACI,yC,CAEA,qBAYR,A,iCAsBI,kE,CArBA,sD,CACI,S,CAGJ,uD,CACI,iB,CACA,S,CAGJ,2D,CACI,S,CAGJ,0B,CACI,Y,CAeJ,2B,CACI,sB,CACA,Y,CACA,gB,CAGJ,yC,CACI,U,CAGJ,kC,CACI,e,CACA,W,CAGJ,mC,CACI,YAYR,A,iCAEI,+C,CADA,sD,CAEI,kB,CACA,Y,CACA,oB,CACA,mC,CAGJ,yC,CAKA,8C,CADA,2C,CAHI,e,CAQJ,4C,CACI,YAMR,A,WACI,oC,CACI,W,CACA,c,CACA,e,CACA,qB,CACA,iB,CAGJ,2C,CACI,W,CACA,M,CACA,iB,CACA,K,CACA,Y",
     "names": [],
     "sources": [
         "aa-forum.css"
     ],
     "sourcesContent": [
-        "/* Variable definitions\n------------------------------------------------------------------------------------- */\n:root {\n    --bg-hover-transition: background-color 0.25s linear;\n}\n\n/* General\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-svg-wrapper {\n        height: 0;\n        width: 0;\n    }\n}\n\n/* Search Box\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-body #aa-forum-form-search-results .input-group {\n        margin-bottom: 1rem;\n    }\n}\n\n/* Administration :: Sortable categories and boards\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-ui-placeholder {\n        outline: 1px dashed rgb(0 0 0);\n    }\n\n    .aa-forum .categories-sortable,\n    .aa-forum .boards-sortable {\n        list-style-type: none;\n    }\n\n    .aa-forum .boards-sortable > li:first-child {\n        margin-top: 1rem;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"].collapsed .if-expanded {\n        display: none;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"]:not(.collapsed) .if-collapsed {\n        display: none;\n    }\n\n    .aa-forum .category-sortable {\n        cursor: move;\n    }\n}\n\n/* Breadcrumb\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-breadcrumb ul {\n        list-style-type: none;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li {\n        display: inline;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li:first-child {\n        padding-left: 0;\n    }\n}\n\n/* Category view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-category .aa-forum-board {\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-image svg {\n        height: 65px;\n        margin-top: -1rem;\n        width: 65px;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-board-name p:last-child {\n        margin: 0;\n    }\n\n    .aa-forum .aa-forum-board-group-restrictions {\n        list-style-type: none;\n        margin: 0;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-board-last-post .img-last-post-avatar {\n        float: left;\n        height: 55px;\n        margin-right: 1rem;\n        width: 55px;\n    }\n\n    .aa-forum .aa-forum-board-last-post .last-post-information {\n        overflow: hidden;\n        text-overflow: ellipsis;\n        white-space: nowrap;\n        word-wrap: normal;\n    }\n\n    .aa-forum .aa-forum-legend > span {\n        display: flex;\n        margin-right: 5rem;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-image svg {\n        height: 30px;\n        width: 30px;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-text {\n        display: inline-block;\n    }\n\n    .aa-forum .aa-forum-legend span:last-child {\n        margin-right: 0;\n    }\n}\n\n/* Board view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic {\n        align-content: center;\n        align-items: center;\n        display: flex;\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .aa-forum-topic-row:last-child .aa-forum-topic {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image {\n        width: 40px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image svg {\n        height: 35px;\n        margin-top: -1rem;\n        width: 35px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name p:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-actions {\n        width: 70px;\n    }\n\n    .aa-forum .aa-forum-topic-locked {\n        background-color: rgb(185 199 219 / 25%);\n    }\n\n    .aa-forum .aa-forum-topic-sticky {\n        background-color: rgb(255 220 104 / 25%);\n    }\n\n    .aa-forum .label-aa-forum-topic-new-message {\n        font-size: 55%;\n    }\n\n    .aa-forum .label-aa-forum-child-board-new-message {\n        font-size: 55%;\n        margin-left: 0.25rem;\n        padding: 0.3em 0.6em;\n        vertical-align: middle;\n    }\n}\n\n/* Message view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-message-author .img-author-avatar {\n        max-width: 100%;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-body {\n        border-top: 1px solid rgb(236 240 241);\n    }\n\n    .aa-forum .aa-forum-message-body-author-signature {\n        border-top: 1px solid rgb(236 240 241);\n        margin-top: 3em;\n    }\n\n    .aa-forum .aa-forum-message-body-last-edited {\n        margin-top: 5rem;\n    }\n\n    .aa-forum .aa-forum-message-body img {\n        height: auto !important; /* to override inline style added by cKeditor */\n        max-width: 100%;\n    }\n}\n\n/* Search view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-search-result-inner {\n        align-items: flex-start;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-search-results-total-number {\n        font-size: 2rem;\n        font-weight: bolder;\n        margin-bottom: 2rem;\n    }\n\n    .aa-forum .aa-forum-search-result-counter {\n        font-size: 3rem;\n        font-weight: bolder;\n        margin-right: 1rem;\n        min-width: 50px;\n        padding: 1rem;\n    }\n\n    .aa-forum .aa-forum-search-result-details {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-search-term-highlight {\n        color: rgb(255 114 0) !important;\n        font-size: 1.1em;\n        font-weight: bold;\n    }\n}\n\n/* Personal messages view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-personal-messages-item {\n        padding: 1rem;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-header {\n        border-bottom: 1px solid rgb(236 240 241);\n        font-weight: 700;\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-unread {\n        font-weight: 700;\n    }\n\n    .aa-forum .aa-forum-personal-messages-message .card {\n        margin-top: 2rem;\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item:has(a.active) {\n        background-color: var(--bs-secondary-bg-subtle);\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item > a.active {\n        color: rgb(var(--bs-primary-rgb));\n    }\n}\n\n/* Lightbox\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-lightbox-modal {\n        align-items: center;\n        display: flex !important;\n        justify-content: center;\n        z-index: -1;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal .modal-dialog {\n        display: inline-block;\n        height: auto !important;\n        max-height: 95%;\n        max-width: 95%;\n        width: auto !important;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal.fade.in {\n        z-index: 1050;\n    }\n}\n\n/* Buttons\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .btn-aa-forum-topic-moderation {\n        background: none;\n    }\n\n    .aa-forum .btn-aa-forum-topic-moderation.focus,\n    .aa-forum .btn-aa-forum-topic-moderation:focus,\n    .aa-forum .btn-aa-forum-topic-moderation:hover {\n        color: inherit;\n        outline: 5px auto -webkit-focus-ring-color;\n        outline-offset: -2px;\n    }\n\n    .aa-forum .btn-aa-forum-delete {\n        color: rgb(255 0 0);\n    }\n}\n\n/* SumoSelect\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .SumoSelect p {\n        border-radius: var(--bs-border-radius);\n        height: auto;\n    }\n\n    .aa-forum .SumoSelect {\n        color: rgb(54 54 54);\n        display: block;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > label > i {\n        background-image: none;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > span.placeholder {\n        background-color: transparent;\n        color: rgb(62 68 76);\n        opacity: 1;\n    }\n}\n\n/* Select2\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .select2-container--bootstrap-5 {\n        max-width: 100% !important;\n    }\n}\n\n/* CKEditor 5 (WYSIWYG editor)\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .ck-rounded-corners {\n        --ck-border-radius: var(--bs-border-radius);\n    }\n\n    .aa-forum .ck-editor__editable {\n        color: initial;\n    }\n\n    .aa-forum .ck-word-count {\n        color: var(--bs-secondary-color) !important;\n\n        --bs-text-opacity: 1;\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 768px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Category view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 60%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-legend {\n        display: flex;\n    }\n}\n\n/* Board view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: 60%;\n    }\n}\n\n/* Message view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-message {\n        align-items: flex-start;\n        display: flex;\n        flex-wrap: nowrap;\n    }\n\n    .aa-forum .aa-forum-message-author figure {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-author {\n        min-width: 150px;\n        width: 150px;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: 100%;\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 992px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Personal messages view (@media all and (min-width: 992px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 992px) {\n    .aa-forum .card-aa-forum-personal-messages-item-header,\n    .aa-forum .card-aa-forum-personal-messages-item {\n        align-items: center;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-personal-message-date {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-sender,\n    .aa-forum .aa-forum-personal-message-recipient {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-subject {\n        width: 100%;\n    }\n}\n\n/* Fix for oEmbed videos\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum figure.media .oembed-video {\n        height: auto;\n        max-width: 100%;\n        overflow: hidden;\n        padding-bottom: 56.25%;\n        position: relative;\n    }\n\n    .aa-forum figure.media .oembed-video > iframe {\n        height: 100%;\n        left: 0;\n        position: absolute;\n        top: 0;\n        width: 100%;\n    }\n}\n"
+        "/* Variable definitions\n------------------------------------------------------------------------------------- */\n:root {\n    --bg-hover-transition: background-color 0.25s linear;\n}\n\n/* General\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-svg-wrapper {\n        height: 0;\n        width: 0;\n    }\n}\n\n/* Search Box\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-body #aa-forum-form-search-results .input-group {\n        margin-bottom: 1rem;\n    }\n}\n\n/* Administration :: Sortable categories and boards\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-ui-placeholder {\n        outline: 1px dashed rgb(0 0 0);\n    }\n\n    .aa-forum .categories-sortable,\n    .aa-forum .boards-sortable {\n        list-style-type: none;\n    }\n\n    .aa-forum .boards-sortable > li:first-child {\n        margin-top: 1rem;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"].collapsed .if-expanded {\n        display: none;\n    }\n\n    .aa-forum [data-bs-toggle=\"collapse\"]:not(.collapsed) .if-collapsed {\n        display: none;\n    }\n\n    .aa-forum .category-sortable {\n        cursor: move;\n    }\n}\n\n/* Breadcrumb\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-breadcrumb ul {\n        list-style-type: none;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li {\n        display: inline;\n    }\n\n    .aa-forum .aa-forum-breadcrumb ul li:first-child {\n        padding-left: 0;\n    }\n}\n\n/* Category view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-category .aa-forum-board {\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-image svg {\n        height: 65px;\n        margin-top: -1rem;\n        width: 65px;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-board-name p:last-child {\n        margin: 0;\n    }\n\n    .aa-forum .aa-forum-board-group-restrictions {\n        list-style-type: none;\n        margin: 0;\n        padding: 0;\n    }\n\n    .aa-forum .aa-forum-board-last-post .img-last-post-avatar {\n        float: left;\n        height: 55px;\n        margin-right: 1rem;\n        width: 55px;\n    }\n\n    .aa-forum .aa-forum-board-last-post .last-post-information {\n        overflow: hidden;\n        text-overflow: ellipsis;\n        white-space: nowrap;\n        word-wrap: normal;\n    }\n\n    .aa-forum .aa-forum-legend > span {\n        display: flex;\n        margin-right: 5rem;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-image svg {\n        height: 30px;\n        width: 30px;\n    }\n\n    .aa-forum .aa-forum-legend .aa-forum-legend-text {\n        display: inline-block;\n    }\n\n    .aa-forum .aa-forum-legend span:last-child {\n        margin-right: 0;\n    }\n}\n\n/* Board view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic {\n        align-content: center;\n        align-items: center;\n        display: flex;\n        flex-direction: row;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .aa-forum-topic-row:last-child .aa-forum-topic {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image {\n        width: 40px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-image svg {\n        height: 35px;\n        margin-top: -1rem;\n        width: 35px;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name p:last-child {\n        margin-bottom: 0;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-actions {\n        width: 70px;\n    }\n\n    .aa-forum .aa-forum-topic-locked {\n        background-color: rgb(185 199 219 / 25%);\n    }\n\n    .aa-forum .aa-forum-topic-sticky {\n        background-color: rgb(255 220 104 / 25%);\n    }\n\n    .aa-forum .label-aa-forum-topic-new-message {\n        font-size: 55%;\n    }\n\n    .aa-forum .label-aa-forum-child-board-new-message {\n        font-size: 55%;\n        margin-left: 0.25rem;\n        padding: 0.3em 0.6em;\n        vertical-align: middle;\n    }\n}\n\n/* Message view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-message-author .img-author-avatar {\n        max-width: 100%;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-body {\n        border-top: 1px solid rgb(236 240 241);\n    }\n\n    .aa-forum .aa-forum-message-body-author-signature {\n        border-top: 1px solid rgb(236 240 241);\n        margin-top: 3em;\n    }\n\n    .aa-forum .aa-forum-message-body-last-edited {\n        margin-top: 5rem;\n    }\n\n    .aa-forum .aa-forum-message-body img {\n        height: auto !important; /* to override inline style added by CKEditor */\n        max-width: 100%;\n    }\n}\n\n/* Search view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-search-result-inner {\n        align-items: flex-start;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-search-results-total-number {\n        font-size: 2rem;\n        font-weight: bolder;\n        margin-bottom: 2rem;\n    }\n\n    .aa-forum .aa-forum-search-result-counter {\n        font-size: 3rem;\n        font-weight: bolder;\n        margin-right: 1rem;\n        min-width: 50px;\n        padding: 1rem;\n    }\n\n    .aa-forum .aa-forum-search-result-details {\n        width: 100%;\n    }\n\n    .aa-forum .aa-forum-search-term-highlight {\n        color: rgb(255 114 0) !important;\n        font-size: 1.1em;\n        font-weight: bold;\n    }\n}\n\n/* Personal messages view\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .card-aa-forum-personal-messages-item {\n        padding: 1rem;\n        transition: var(--bg-hover-transition);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item:hover {\n        background: rgb(0 0 0 / 5%);\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-header {\n        border-bottom: 1px solid rgb(236 240 241);\n        font-weight: 700;\n    }\n\n    .aa-forum .card-aa-forum-personal-messages-item-unread {\n        font-weight: 700;\n    }\n\n    .aa-forum .aa-forum-personal-messages-message .card {\n        margin-top: 2rem;\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item:has(a.active) {\n        background-color: var(--bs-secondary-bg-subtle);\n    }\n\n    .aa-forum li.aa-forum-messages-sidebar-menu-item > a.active {\n        color: rgb(var(--bs-primary-rgb));\n    }\n}\n\n/* Lightbox\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .aa-forum-lightbox-modal {\n        align-items: center;\n        display: flex !important;\n        justify-content: center;\n        z-index: -1;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal .modal-dialog {\n        display: inline-block;\n        height: auto !important;\n        max-height: 95%;\n        max-width: 95%;\n        width: auto !important;\n    }\n\n    .aa-forum .aa-forum-lightbox-modal.fade.in {\n        z-index: 1050;\n    }\n}\n\n/* Buttons\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .btn-aa-forum-topic-moderation {\n        background: none;\n    }\n\n    .aa-forum .btn-aa-forum-topic-moderation.focus,\n    .aa-forum .btn-aa-forum-topic-moderation:focus,\n    .aa-forum .btn-aa-forum-topic-moderation:hover {\n        color: inherit;\n        outline: 5px auto -webkit-focus-ring-color;\n        outline-offset: -2px;\n    }\n\n    .aa-forum .btn-aa-forum-delete {\n        color: rgb(255 0 0);\n    }\n}\n\n/* SumoSelect\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .SumoSelect p {\n        border-radius: var(--bs-border-radius);\n        height: auto;\n    }\n\n    .aa-forum .SumoSelect {\n        color: rgb(54 54 54);\n        display: block;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > label > i {\n        background-image: none;\n    }\n\n    .aa-forum .SumoSelect > .CaptionCont > span.placeholder {\n        background-color: transparent;\n        color: rgb(62 68 76);\n        opacity: 1;\n    }\n}\n\n/* Select2\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .select2-container--bootstrap-5 {\n        max-width: 100% !important;\n    }\n}\n\n/* CKEditor 5 (WYSIWYG editor)\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum .ck-rounded-corners {\n        --ck-border-radius: var(--bs-border-radius);\n    }\n\n    .aa-forum .ck-editor__editable {\n        color: initial;\n    }\n\n    .aa-forum .ck-word-count {\n        color: var(--bs-secondary-color) !important;\n\n        --bs-text-opacity: 1;\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 768px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Category view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .card-aa-forum-category .aa-forum-board-name {\n        width: 60%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-stats {\n        text-align: center;\n        width: 15%;\n    }\n\n    .aa-forum .card-aa-forum-category .aa-forum-board-last-post {\n        width: 25%;\n    }\n\n    .aa-forum .aa-forum-legend {\n        display: flex;\n    }\n}\n\n/* Board view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-topic-row .aa-forum-topic .aa-forum-topic-name {\n        width: 60%;\n    }\n}\n\n/* Message view (@media all and (min-width: 768px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 768px) {\n    .aa-forum .aa-forum-message {\n        align-items: flex-start;\n        display: flex;\n        flex-wrap: nowrap;\n    }\n\n    .aa-forum .aa-forum-message-author figure {\n        width: auto;\n    }\n\n    .aa-forum .aa-forum-message-author {\n        min-width: 150px;\n        width: 150px;\n    }\n\n    .aa-forum .aa-forum-message-wrapper {\n        width: 100%;\n    }\n}\n\n/*\n----------------------------------------------------------------------------------------\n                Responsive (@media all and (min-width: 992px))\n----------------------------------------------------------------------------------------\n*/\n\n/* Personal messages view (@media all and (min-width: 992px))\n------------------------------------------------------------------------------------- */\n@media all and (min-width: 992px) {\n    .aa-forum .card-aa-forum-personal-messages-item-header,\n    .aa-forum .card-aa-forum-personal-messages-item {\n        align-items: center;\n        display: flex;\n        flex-flow: row nowrap;\n        place-content: flex-start flex-start;\n    }\n\n    .aa-forum .aa-forum-personal-message-date {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-sender,\n    .aa-forum .aa-forum-personal-message-recipient {\n        min-width: 200px;\n    }\n\n    .aa-forum .aa-forum-personal-message-subject {\n        width: 100%;\n    }\n}\n\n/* Fix for oEmbed videos\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-forum figure.media .oembed-video {\n        height: auto;\n        max-width: 100%;\n        overflow: hidden;\n        padding-bottom: 56.25%;\n        position: relative;\n    }\n\n    .aa-forum figure.media .oembed-video > iframe {\n        height: 100%;\n        left: 0;\n        position: absolute;\n        top: 0;\n        width: 100%;\n    }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-admin.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map` & `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -17,20 +17,28 @@
         })
         .then((responseText) => {
             // console.log('Unread Forum Topics Widget: ', responseText);
 
             if (responseText !== '') {
                 aaForumUnreadTopicsWidgetContent.innerHTML = responseText;
 
+                // Show the widget area
                 const showWidgetArea = new bootstrap.Collapse(aaForumDashboardWidgets, { // eslint-disable-line no-unused-vars
                     show: true
                 });
 
+                // Show the widget
                 const showWidget = new bootstrap.Collapse(aaForumUnreadTopicsWidget, { // eslint-disable-line no-unused-vars
                     show: true
                 });
+
+                // Initialize Bootstrap tooltips
+                [].slice.call(document.querySelectorAll('[data-bs-tooltip="aa-forum"]'))
+                    .map((tooltipTriggerEl) => {
+                        return new bootstrap.Tooltip(tooltipTriggerEl);
+                    });
             }
         })
         .catch((error) => {
             console.log(error);
         });
 }
```

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,23 @@
 "use strict";
 const aaForumDashboardWidgets = document.getElementById("aa-forum-dashboard-widgets"),
     aaForumUnreadTopicsWidget = document.getElementById("aa-forum-dashboard-widget-unread-topics");
 if (aaForumUnreadTopicsWidget) {
     const a = aaForumUnreadTopicsWidget.querySelector(".aa-forum-dashboard-widget-unread-topics-content");
-    fetch(aaForumDashboardWidgetsSettings.unreadTopics.ajaxUrl).then(a => {
-        if (a.ok) return a.text();
+    fetch(aaForumDashboardWidgetsSettings.unreadTopics.ajaxUrl).then(o => {
+        if (o.ok) return o.text();
         throw new Error("Something went wrong")
-    }).then(e => {
-        if ("" !== e) {
-            a.innerHTML = e;
+    }).then(o => {
+        if ("" !== o) {
+            a.innerHTML = o;
             new bootstrap.Collapse(aaForumDashboardWidgets, {
                 show: !0
             }), new bootstrap.Collapse(aaForumUnreadTopicsWidget, {
                 show: !0
-            })
+            });
+            [].slice.call(document.querySelectorAll('[data-bs-tooltip="aa-forum"]')).map(o => new bootstrap.Tooltip(o))
         }
-    }).catch(a => {
-        console.log(a)
+    }).catch(o => {
+        console.log(o)
     })
 }
 //# sourceMappingURL=aa-forum-desktop-widgets.min.js.map
```

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map` & `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.85%*

 * *Differences: {"'mappings'": "'AAEA,aAEA,MAAMA,wBAA0BC,SAASC,eAAe,4BAA4B,EAC9EC,0BAA4BF,SAASC,eAAe,yCAAyC,EAEnG,GAAIC,0BAA2B,CAC3B,MAAMC,EAAmCD,0BAA0BE,cAAc,kDAAkD,EAEnIC,MAAMC,gCAAgCC,aAAaC,OAAO,EACrDC,KAAK,IACF,GAAIC,EAASC,GACT,OAAOD,EAASE,KAAK,EAEzB,MAAM,IAAIC,MAAM,sBAAsB,CAC1C,CAAC,EACAJ,KAAK,IAGF,GAAqB,KAAjBK,EAAqB,CACrBX,EAAiCY,UAAYD,EAGtB,IAAIE,UAAUC,SAASlB,wBAAyB,CACnEmB,KAAM,CAAA,CACV,CAAC,EAGkB,IAAIF,UAAUC,SAASf,0BAA2B,CACjEgB,KAAM,CAAA,CACV,CAAC,EAGD,GAAGC,MAAMC,KAAKpB,SAASqB,iBAAiB,8BAA8B,CAAC,EAClEC,IAAI,GAC […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "mappings": "AAEA,aAEA,MAAMA,wBAA0BC,SAASC,eAAe,4BAA4B,EAC9EC,0BAA4BF,SAASC,eAAe,yCAAyC,EAEnG,GAAIC,0BAA2B,CAC3B,MAAMC,EAAmCD,0BAA0BE,cAAc,kDAAkD,EAEnIC,MAAMC,gCAAgCC,aAAaC,OAAO,EACrDC,KAAK,IACF,GAAIC,EAASC,GACT,OAAOD,EAASE,KAAK,EAEzB,MAAM,IAAIC,MAAM,sBAAsB,CAC1C,CAAC,EACAJ,KAAK,IAGF,GAAqB,KAAjBK,EAAqB,CACrBX,EAAiCY,UAAYD,EAEtB,IAAIE,UAAUC,SAASlB,wBAAyB,CACnEmB,KAAM,CAAA,CACV,CAAC,EAEkB,IAAIF,UAAUC,SAASf,0BAA2B,CACjEgB,KAAM,CAAA,CACV,CAAC,CACL,CACJ,CAAC,EACAC,MAAM,IACHC,QAAQC,IAAIC,CAAK,CACrB,CAAC,CACT",
+    "mappings": "AAEA,aAEA,MAAMA,wBAA0BC,SAASC,eAAe,4BAA4B,EAC9EC,0BAA4BF,SAASC,eAAe,yCAAyC,EAEnG,GAAIC,0BAA2B,CAC3B,MAAMC,EAAmCD,0BAA0BE,cAAc,kDAAkD,EAEnIC,MAAMC,gCAAgCC,aAAaC,OAAO,EACrDC,KAAK,IACF,GAAIC,EAASC,GACT,OAAOD,EAASE,KAAK,EAEzB,MAAM,IAAIC,MAAM,sBAAsB,CAC1C,CAAC,EACAJ,KAAK,IAGF,GAAqB,KAAjBK,EAAqB,CACrBX,EAAiCY,UAAYD,EAGtB,IAAIE,UAAUC,SAASlB,wBAAyB,CACnEmB,KAAM,CAAA,CACV,CAAC,EAGkB,IAAIF,UAAUC,SAASf,0BAA2B,CACjEgB,KAAM,CAAA,CACV,CAAC,EAGD,GAAGC,MAAMC,KAAKpB,SAASqB,iBAAiB,8BAA8B,CAAC,EAClEC,IAAI,GACM,IAAIN,UAAUO,QAAQC,CAAgB,CAChD,CACT,CACJ,CAAC,EACAC,MAAM,IACHC,QAAQC,IAAIC,CAAK,CACrB,CAAC,CACT",
     "names": [
         "aaForumDashboardWidgets",
         "document",
         "getElementById",
         "aaForumUnreadTopicsWidget",
         "aaForumUnreadTopicsWidgetContent",
         "querySelector",
@@ -17,14 +17,20 @@
         "text",
         "Error",
         "responseText",
         "innerHTML",
         "bootstrap",
         "Collapse",
         "show",
+        "slice",
+        "call",
+        "querySelectorAll",
+        "map",
+        "Tooltip",
+        "tooltipTriggerEl",
         "catch",
         "console",
         "log",
         "error"
     ],
     "sources": [
         "aa-forum-desktop-widgets.js"
```

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,48 +1,46 @@
-/**
- * Replace oembed YouTube video with an iframe
- *
- * CKEditor5 oembed plugin is used to embed YouTube videos, and browsers cannot render the oembed element.
- * This function replaces the oembed element with an iframe and is using the YouTube-nocookie domain.
- *
- * @param {string} url The YouTube video URL
- * @returns {`<div class="oembed-video youtube-oembed-video"><iframe src="https://www.youtube-nocookie.com/embed/${string}" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>`}
- */
-const youtubeOembedToIframe = (url) => {
+$(document).ready(() => {
     'use strict';
 
-    let videoId = url.split('v=')[1];
-    const ampersandPosition = videoId.indexOf('&');
-
-    if (ampersandPosition !== -1) {
-        videoId = videoId.substring(0, ampersandPosition);
-    }
-
-    return `<div class="oembed-video youtube-oembed-video"><iframe src="https://www.youtube-nocookie.com/embed/${videoId}" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>`;
-};
+    /**
+     * Replace oembed YouTube video with an iframe
+     *
+     * CKEditor5 oembed plugin is used to embed YouTube videos, and browsers cannot render the oembed element.
+     * This function replaces the oembed element with an iframe and is using the YouTube-nocookie domain.
+     *
+     * @param {string} url The YouTube video URL
+     * @returns {`<div class="oembed-video youtube-oembed-video"><iframe src="${string}" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>`}
+     */
+    const youtubeOembedToIframe = (url) => {
+        let videoId = url.split('v=')[1];
+        const ampersandPosition = videoId.indexOf('&');
+        const embedUrl = 'https://www.youtube-nocookie.com/embed/';
 
+        if (ampersandPosition !== -1) {
+            videoId = videoId.substring(0, ampersandPosition);
+        }
 
-/**
- * Look for oembed elements and replace them with iframes
- */
-const checkForOembed = () => {
-    'use strict';
+        const videoUrl = embedUrl + videoId;
 
-    // Find all oembed elements and loop through them
-    $('.ck-content figure.media oembed').each((index, element) => {
-        const source = $(element).attr('url');
-
-        // Check if the source is a YouTube video
-        if (source.includes('youtube.com/watch')) {
-            // Replace the oembed element with an iframe
-            $(element).replaceWith(youtubeOembedToIframe(source));
-        }
-    });
-};
+        return `<div class="oembed-video youtube-oembed-video"><iframe src="${videoUrl}" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>`;
+    };
 
 
-$(document).ready(() => {
-    'use strict';
+    /**
+     * Look for oembed elements and replace them with iframes
+     */
+    const checkForOembed = () => {
+        // Find all oembed elements and loop through them
+        $('.ck-content figure.media oembed').each((index, element) => {
+            const source = $(element).attr('url');
+
+            // Check if the source is a YouTube video
+            if (source.includes('youtube.com/watch')) {
+                // Replace the oembed element with an iframe
+                $(element).replaceWith(youtubeOembedToIframe(source));
+            }
+        });
+    };
 
     // Run the checkForOembed function when the document is ready
     checkForOembed();
 });
```

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map` & `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333333%*

 * *Differences: {"'mappings'": "'AAAAA,EAAEC,QAAQ,EAAEC,MAAM,KACd,aAWA,MAAMC,EAAwB,IAC1BC,IAAIC,EAAUC,EAAIC,MAAM,IAAI,EAAE,GAC9B,MAAMC,EAAoBH,EAAQI,QAAQ,GAAG,EACvCC,EAAW,0CAMXC,GAJoB,CAAC,IAAvBH,IACAH,EAAUA,EAAQO,UAAU,EAAGJ,CAAiB,GAGnCE,EAAWL,GAE5B,qEAAsEM,oHAC1E,EAMME,EAAiB,KAEnBb,EAAE,iCAAiC,EAAEc,KAAK,CAACC,EAAOC,KAC9C,MAAMC,EAASjB,EAAEgB,CAAO,EAAEE,KAAK,KAAK,EAGhCD,EAAOE,SAAS,mBAAmB,GAEnCnB,EAAEgB,CAAO,EAAEI,YAAYjB,EAAsBc,CAAM,CAAC,CAE5D,CAAC,CACL,EAGAJ,EAAe,CACnB,CAAC'",*

 * * "'names'": "{insert: [(0, '$'), (1, 'document' […]*

```diff
@@ -1,28 +1,30 @@
 {
-    "mappings": "AASA,MAAMA,sBAAwB,IAC1B,aAEAC,IAAIC,EAAUC,EAAIC,MAAM,IAAI,EAAE,GAC9B,MAAMC,EAAoBH,EAAQI,QAAQ,GAAG,EAM7C,4GAHIJ,EADsB,CAAC,IAAvBG,EACUH,EAAQK,UAAU,EAAGF,CAAiB,EAGyDH,oHACjH,EAMMM,eAAiB,KACnB,aAGAC,EAAE,iCAAiC,EAAEC,KAAK,CAACC,EAAOC,KAC9C,MAAMC,EAASJ,EAAEG,CAAO,EAAEE,KAAK,KAAK,EAGhCD,EAAOE,SAAS,mBAAmB,GAEnCN,EAAEG,CAAO,EAAEI,YAAYhB,sBAAsBa,CAAM,CAAC,CAE5D,CAAC,CACL,EAGAJ,EAAEQ,QAAQ,EAAEC,MAAM,KACd,aAGAV,eAAe,CACnB,CAAC",
+    "mappings": "AAAAA,EAAEC,QAAQ,EAAEC,MAAM,KACd,aAWA,MAAMC,EAAwB,IAC1BC,IAAIC,EAAUC,EAAIC,MAAM,IAAI,EAAE,GAC9B,MAAMC,EAAoBH,EAAQI,QAAQ,GAAG,EACvCC,EAAW,0CAMXC,GAJoB,CAAC,IAAvBH,IACAH,EAAUA,EAAQO,UAAU,EAAGJ,CAAiB,GAGnCE,EAAWL,GAE5B,qEAAsEM,oHAC1E,EAMME,EAAiB,KAEnBb,EAAE,iCAAiC,EAAEc,KAAK,CAACC,EAAOC,KAC9C,MAAMC,EAASjB,EAAEgB,CAAO,EAAEE,KAAK,KAAK,EAGhCD,EAAOE,SAAS,mBAAmB,GAEnCnB,EAAEgB,CAAO,EAAEI,YAAYjB,EAAsBc,CAAM,CAAC,CAE5D,CAAC,CACL,EAGAJ,EAAe,CACnB,CAAC",
     "names": [
+        "$",
+        "document",
+        "ready",
         "youtubeOembedToIframe",
         "let",
         "videoId",
         "url",
         "split",
         "ampersandPosition",
         "indexOf",
+        "embedUrl",
+        "videoUrl",
         "substring",
         "checkForOembed",
-        "$",
         "each",
         "index",
         "element",
         "source",
         "attr",
         "includes",
-        "replaceWith",
-        "document",
-        "ready"
+        "replaceWith"
     ],
     "sources": [
         "aa-forum-oembed.js"
     ],
     "version": 3
 }
```

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map` & `aa_forum-2.1.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css` & `aa_forum-2.1.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/base.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/base.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html`

 * *Files 21% similar despite different names*

```diff
@@ -24,22 +24,24 @@
                         <div class="col-md-6">
                             <div class="float-end">
                                 {% if folder == "inbox" %}
                                     <a
                                         href="{% url 'aa_forum:personal_messages_message_reply' message.pk %}"
                                         class="btn btn-aa-forum-topic-moderation btn-sm"
                                         title="{% translate 'Reply' %}"
+                                        data-bs-tooltip="aa-forum"
                                     >
                                         <i class="fa-solid fa-reply-all"></i>
                                     </a>
                                 {% endif %}
 
                                 <button
                                     class="btn btn-aa-forum-topic-moderation btn-sm btn-aa-forum-delete"
                                     title="{% translate 'Delete message' %}"
+                                    data-bs-tooltip="aa-forum"
                                     data-bs-toggle="modal"
                                     data-bs-target="#delete-message-{{ message.pk }}"
                                 >
                                     <i class="fa-regular fa-trash-can"></i>
                                 </button>
                             </div>
                         </div>
@@ -64,11 +66,19 @@
             </div>
         </div>
     </div>
 
     <script>
         'use strict';
 
+        // Initialize tooltips
+        // Since this is loaded via AJAX,
+        // we need to reinitialize the tooltips
+        [].slice.call(document.querySelectorAll(`#message-{{ message.pk }} [data-bs-tooltip="aa-forum"]`))
+            .map((tooltipTriggerEl) => {
+                return new bootstrap.Tooltip(tooltipTriggerEl);
+            });
+
         // Look for oembed elements and replace them with iframes
         checkForOembed();
     </script>
 {% endif %}
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/administration/delete-board.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/administration/delete-board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/administration/delete-category.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/administration/delete-category.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/breadcrumb.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/administration/board-loop.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/board-loop.html`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,33 @@
 {% load i18n %}
 
 <li class="mb-3 p-3 {% if is_child_board %}child-{% endif %}board-sortable ui-state-default ui-sortable" data-board-id="{{ board.board_obj.pk }}" data-position="{{ board.board_obj.order }}">
     <div class="aa-forum-admin-board-name clearfix">
         {{ board.board_obj.name }}
 
         <div class="float-end">
-            <button class="btn btn-warning btn-sm" title="{% translate 'Edit board' %}" data-bs-toggle="collapse" data-bs-target="#collapseEditBoard-{{ board.board_obj.pk }}" aria-expanded="false" aria-controls="collapseEditBoard-{{ board.board_obj.pk }}">
+            <button
+                class="btn btn-warning btn-sm"
+                title="{% translate 'Edit board' %}"
+                data-bs-tooltip="aa-forum"
+                data-bs-toggle="collapse"
+                data-bs-target="#collapseEditBoard-{{ board.board_obj.pk }}"
+                aria-expanded="false"
+                aria-controls="collapseEditBoard-{{ board.board_obj.pk }}"
+            >
                 <i class="fa-solid fa-pencil"></i>
             </button>
 
-            <button class="btn btn-danger btn-sm" title="{% translate 'Delete board' %}" data-bs-toggle="modal" data-bs-target="#delete-board-{{ board.board_obj.pk }}">
+            <button
+                class="btn btn-danger btn-sm"
+                title="{% translate 'Delete board' %}"
+                data-bs-tooltip="aa-forum"
+                data-bs-toggle="modal"
+                data-bs-target="#delete-board-{{ board.board_obj.pk }}"
+            >
                 <i class="fa-regular fa-trash-can"></i>
             </button>
         </div>
     </div>
 
     <div class="collapse" id="collapseEditBoard-{{ board.board_obj.pk }}" style="margin-top: 1rem;">
         <div class="card card-body bg-light mb-3 py-3">
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/administration/categories.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/categories.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/administration/category-loop.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/category-loop.html`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,47 @@
 <li class="mb-3 category-sortable ui-state-default ui-sortable" data-category-id="{{ category.category_obj.pk }}" data-position="{{ category.category_obj.order }}">
     <div class="card card-default mb-0 aa-forum-admin-card-aa-forum-category">
         <div class="card-header">
             <div class="card-title mb-0">
                 {{ category.category_obj.name }}
 
                 <div class="float-end">
-                    <button class="btn btn-warning btn-sm" title="{% translate 'Edit category' %}" data-bs-toggle="collapse" data-bs-target="#collapseEditCategory-{{ category.category_obj.pk }}" aria-expanded="false" aria-controls="collapseEditCategory-{{ category.category_obj.pk }}">
+                    <button
+                        class="btn btn-warning btn-sm"
+                        title="{% translate 'Edit category' %}"
+                        data-bs-tooltip="aa-forum"
+                        data-bs-toggle="collapse"
+                        data-bs-target="#collapseEditCategory-{{ category.category_obj.pk }}"
+                        aria-expanded="false"
+                        aria-controls="collapseEditCategory-{{ category.category_obj.pk }}"
+                    >
                         <i class="fa-solid fa-pencil"></i>
                     </button>
 
-                    <button class="btn btn-danger btn-sm" title="{% translate 'Delete category' %}" data-bs-toggle="modal" data-bs-target="#delete-category-{{ category.category_obj.pk }}">
+                    <button
+                        class="btn btn-danger btn-sm"
+                        title="{% translate 'Delete category' %}"
+                        data-bs-tooltip="aa-forum"
+                        data-bs-toggle="modal"
+                        data-bs-target="#delete-category-{{ category.category_obj.pk }}"
+                    >
                         <i class="fa-regular fa-trash-can"></i>
                     </button>
 
-                    <button class="aa-forum-admin-expand-collapse-category btn btn-secondary btn-sm collapsed" title="{% translate 'Expand/collapse category' %}" data-bs-toggle="collapse" data-bs-target="#collapseCategory-{{ category.category_obj.pk }}" aria-expanded="false" aria-controls="collapseCategory-{{ category.category_obj.pk }}">
-                        <i class="if-collapsed fas fa-expand-alt"></i>
-                        <i class="if-expanded fas fa-compress-alt"></i>
+                    <button
+                        class="aa-forum-admin-expand-collapse-category btn btn-secondary btn-sm collapsed"
+                        title="{% translate 'Expand/collapse category' %}"
+                        data-bs-tooltip="aa-forum"
+                        data-bs-toggle="collapse"
+                        data-bs-target="#collapseCategory-{{ category.category_obj.pk }}"
+                        aria-expanded="false"
+                        aria-controls="collapseCategory-{{ category.category_obj.pk }}"
+                    >
+                        <i class="if-collapsed fa-solid fa-expand-alt"></i>
+                        <i class="if-expanded fa-solid fa-compress-alt"></i>
                     </button>
                 </div>
             </div>
         </div>
 
         <div class="card-body px-3 py-0">
             <div class="collapse mt-3" id="collapseEditCategory-{{ category.category_obj.pk }}">
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/administration/new-category.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/new-category.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/administration/settings-form.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/administration/settings-form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/board/board-index.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/board-index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/board/board.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/board.html`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,19 @@
                     loading="lazy"
                 >
             {% endwith %}
 
             <p class="mb-0 last-post-information small">
                 <b>{% translate "Last post:" %}</b>
 
-                <a href="{% url 'aa_forum:forum_message' board.category.slug board_latest_topic_board.slug board_latest_topic.slug board_last_message.pk %}" title="{{ board_latest_topic.subject }}">
+                <a
+                    href="{% url 'aa_forum:forum_message' board.category.slug board_latest_topic_board.slug board_latest_topic.slug board_last_message.pk %}"
+                    title="{{ board_latest_topic.subject }}"
+                    data-bs-tooltip="aa-forum"
+                >
                     {% if board.last_message != board.first_message %}
                         {% translate "Re:" %}
                     {% endif %}
 
                     {{ board_latest_topic.subject|truncatechars:25 }}
                 </a>
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/board/pagination.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/board/topic.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/board/topic.html`

 * *Files 16% similar despite different names*

```diff
@@ -29,21 +29,21 @@
                         {% translate "New" %}
                     </a>
                 {% endif %}
                 <br>
                 <span class="small">
                     {% if topic.is_sticky %}
                         <span class="aa-forum-topic-status-icon aa-forum-topic-status-sticky mx-1 my-0">
-                            <i class="fa-solid fa-thumbtack" title="{% translate 'Topic is always on top' %}"></i>
+                            <i class="fa-solid fa-thumbtack" title="{% translate 'Topic is always on top' %}" data-bs-tooltip="aa-forum"></i>
                         </span>
                     {% endif %}
 
                     {% if topic.is_locked %}
                         <span class="aa-forum-topic-status-icon aa-forum-topic-status-locked mx-1 my-0">
-                            <i class="fa-solid fa-lock" title="{% translate 'Topic is locked' %}"></i>
+                            <i class="fa-solid fa-lock" title="{% translate 'Topic is locked' %}" data-bs-tooltip="aa-forum"></i>
                         </span>
                     {% endif %}
 
                     {% translate "Started by" %} {{ topic.first_message.user_created|aa_forum_main_character_name }}
                 </span>
             </p>
         </div>
@@ -62,41 +62,70 @@
             </span>
         </div>
 
         <div class="aa-forum-topic-last-post hidden-xs">
             <span class="small">
                 {% translate "Last post" %} {{ topic.last_message.time_posted|aa_forum_time }}
 
-                <a href="{% url 'aa_forum:forum_message' topic.board.category.slug topic.board.slug topic.slug topic.last_message_id %}" title="{% translate 'Go to last message' %}" style="margin-left: 0.5rem;">
+                <a
+                    href="{% url 'aa_forum:forum_message' topic.board.category.slug topic.board.slug topic.slug topic.last_message_id %}"
+                    title="{% translate 'Go to last message' %}"
+                    data-bs-tooltip="aa-forum"
+                    class="ms-2"
+                >
                     <i class="fa-solid fa-right-to-bracket"></i>
                 </a>
 
                 <br>
                 by {{ topic.last_message.user_created|aa_forum_main_character_name }}
             </span>
         </div>
 
         <div class="aa-forum-topic-actions hidden-xs">
             {% if perms.aa_forum.manage_forum %}
                 <div class="text-end">
                     {% if topic.is_locked %}
-                        <button class="btn btn-aa-forum-topic-moderation btn-sm" title="{% translate 'Unlock/re-open topic' %}" data-bs-toggle="modal" data-bs-target="#topic-lock-state-change-{{ topic.pk }}">
+                        <button
+                            class="btn btn-aa-forum-topic-moderation btn-sm"
+                            title="{% translate 'Unlock/re-open topic' %}"
+                            data-bs-tooltip="aa-forum"
+                            data-bs-toggle="modal"
+                            data-bs-target="#topic-lock-state-change-{{ topic.pk }}"
+                        >
                             <i class="fa-solid fa-unlock"></i>
                         </button>
                     {% else %}
-                        <button class="btn btn-aa-forum-topic-moderation btn-sm" title="{% translate 'Lock/close topic' %}" data-bs-toggle="modal" data-bs-target="#topic-lock-state-change-{{ topic.pk }}">
+                        <button
+                            class="btn btn-aa-forum-topic-moderation btn-sm"
+                            title="{% translate 'Lock/close topic' %}"
+                            data-bs-tooltip="aa-forum"
+                            data-bs-toggle="modal"
+                            data-bs-target="#topic-lock-state-change-{{ topic.pk }}"
+                        >
                             <i class="fa-solid fa-lock"></i>
                         </button>
                     {% endif %}
 
-                    <button class="btn btn-aa-forum-topic-moderation btn-sm" title="{% translate 'Change topics sticky state' %}" data-bs-toggle="modal" data-bs-target="#topic-sticky-state-change-{{ topic.pk }}">
+                    <button
+                        class="btn btn-aa-forum-topic-moderation btn-sm"
+                        title="{% translate 'Change topics sticky state' %}"
+                        data-bs-tooltip="aa-forum"
+                        data-bs-toggle="modal"
+                        data-bs-target="#topic-sticky-state-change-{{ topic.pk }}"
+                    >
                         <i class="fa-solid fa-thumbtack"></i>
                     </button>
 
-                    <button class="btn btn-aa-forum-topic-moderation btn-sm" title="{% translate 'Delete topic' %}" data-bs-toggle="modal" data-bs-target="#delete-topic-{{ topic.pk }}">
+                    <button
+                        class="btn btn-aa-forum-topic-moderation btn-sm"
+                        title="{% translate 'Delete topic' %}"
+                        data-bs-tooltip="aa-forum"
+                        data-bs-toggle="modal"
+                        data-bs-target="#delete-topic-{{ topic.pk }}"
+                    >
                         <i class="fa-regular fa-trash-can"></i>
                     </button>
                 </div>
 
                 {% include "aa_forum/modals/forum/board/topic-change-lock-state.html" %}
                 {% include "aa_forum/modals/forum/board/topic-change-sticky-state.html" %}
                 {% include "aa_forum/modals/forum/board/topic-delete.html" %}
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/message.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/message.html`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,19 @@
             <div class="aa-forum-message-wrapper m-3">
                 <div class="aa-forum-message-header row mb-3">
                     <div class="d-lg-none d-md-none d-sm-none">
                         {% include "aa_forum/partials/forum/topic/message-author.html" %}
                     </div>
 
                     <div class="aa-forum-message-keyinfo col-md-6">
-                        <a href="{% url 'aa_forum:forum_message' message.topic.board.category.slug message.topic.board.slug message.topic.slug message.pk %}" title="{{ board_latest_topic.subject }}">
+                        <a
+                            href="{% url 'aa_forum:forum_message' message.topic.board.category.slug message.topic.board.slug message.topic.slug message.pk %}"
+                            title="{{ board_latest_topic.subject }}"
+                            data-bs-tooltip="aa-forum"
+                        >
                             {% if topic.first_message.pk != message.pk %}
                                 {% translate "Re:" %}
                             {% endif %}
 
                             {{ topic.subject }}
                         </a><br>
                         <small>« <b>{% translate "on:" %}</b> {{ message.time_posted|aa_forum_time }} »</small>
@@ -29,32 +33,35 @@
 
                     <div class="col-md-6">
                         {% if not search_term %}
                             <div class="float-end">
                                 <button
                                     class="btn btn-aa-forum-topic-moderation btn-sm btn-aa-forum-copy-to-clipboard"
                                     title="{% translate 'Copy message link to clipboard' %}"
+                                    data-bs-tooltip="aa-forum"
                                     data-clipboard-text="{{ SITE_URL }}{% url 'aa_forum:forum_message' message.topic.board.category.slug message.topic.board.slug message.topic.slug message.pk %}"
                                 >
                                     <i class="fa-regular fa-copy"></i>
                                 </button>
 
                                 {% if message_author == request.user or perms.aa_forum.manage_forum %}
                                     <a
                                         id="aa-forum-btn-modify-message-{{ message.pk }}"
                                         href="{% url 'aa_forum:forum_message_modify' topic.board.category.slug topic.board.slug topic.slug message.pk %}"
                                         class="btn btn-aa-forum-topic-moderation btn-sm"
                                         title="{% translate 'Modify message' %}"
+                                        data-bs-tooltip="aa-forum"
                                     >
                                         <i class="fa-solid fa-pencil"></i>
                                     </a>
 
                                     <button
                                         class="btn btn-aa-forum-topic-moderation btn-sm"
                                         title="{% translate 'Delete message' %}"
+                                        data-bs-tooltip="aa-forum"
                                         data-bs-toggle="modal"
                                         data-bs-target="#delete-message-{{ message.pk }}"
                                     >
                                         <i class="fa-regular fa-trash-can"></i>
                                     </button>
                                 {% endif %}
                             </div>
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                 {% translate "Note: You are not on the last page of this topic and may miss the most recent replies." %}
             </div>
         {% endif %}
 
         <form id="aa-forum-form-message-modify" autocomplete="off" action="{% url 'aa_forum:forum_message_modify' board.category.slug board.slug message.topic.slug message.pk %}" method="post">
             {% csrf_token %}
 
-            {% bootstrap_form form %}
+            {% bootstrap_field form.message %}
 
             {% include "aa_forum/partials/form/required-field-hint.html" %}
 
             <div class="form-group aa-forum-form-group aa-forum-form-modify-message float-end clearfix">
                 <button class="btn btn-primary btn-sm" type="submit">
                     {% translate "Modify" %}
                 </button>
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/reply.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/reply.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{% load aa_forum %}
 {% load i18n %}
 {% load django_bootstrap5 %}
 
 <div class="card card-default">
     <div class="card-header">
         <div class="card-title mb-0">
             {% translate "Reply" %}
@@ -20,15 +21,25 @@
                 {% translate "Warning: this topic is locked! Only admins can reply." %}
             </div>
         {% endif %}
 
         <form id="aa-forum-form-message-reply" autocomplete="off" action="{% url 'aa_forum:forum_topic_reply' topic.board.category.slug topic.board.slug topic.slug %}" method="post">
             {% csrf_token %}
 
-            {% bootstrap_form reply_form %}
+            {% bootstrap_field reply_form.message %}
+
+            {% if topic.first_message.user_created == request.user or perms.aa_forum.manage_forum %}
+                {% if not topic.is_locked %}
+                    {% bootstrap_field reply_form.close_topic %}
+                {% endif %}
+
+                {% if topic.is_locked and perms.aa_forum.manage_forum %}
+                    {% bootstrap_field reply_form.reopen_topic %}
+                {% endif %}
+            {% endif %}
 
             {% include "aa_forum/partials/form/required-field-hint.html" %}
 
             <div class="form-group aa-forum-form-group aa-forum-form-reply float-end clearfix">
                 <button class="btn btn-secondary btn-sm" type="reset">
                     {% translate "Clear form" %}
                 </button>
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/menu/menu-admin.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/menu/menu-admin.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/menu/menu-user.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/menu/menu-user.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html`

 * *Files 5% similar despite different names*

```diff
@@ -57,25 +57,27 @@
     {#                                </span>#}
     {#                            {% endif %}#}
 
                                 <span class="float-end">
                                     <button
                                         class="btn btn-aa-forum-topic-moderation btn-sm btn-read-personal-message"
                                         title="{% translate 'Read message' %}"
+                                        data-bs-tooltip="aa-forum"
                                         data-sender="{{ message.sender.pk }}"
                                         data-recipient="{{ message.recipient.pk }}"
                                         data-message="{{ message.pk }}"
                                         data-message-folder="inbox"
                                     >
                                         <i class="fa-solid fa-envelope-open"></i>
                                     </button>
 
                                     <button
                                         class="btn btn-aa-forum-topic-moderation btn-sm btn-aa-forum-delete"
                                         title="{% translate 'Delete message' %}"
+                                        data-bs-tooltip="aa-forum"
                                         data-bs-toggle="modal"
                                         data-bs-target="#delete-message-{{ message.pk }}"
                                     >
                                         <i class="fa-regular fa-trash-can"></i>
                                     </button>
                                 </span>
                             </div>
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html`

 * *Files 4% similar despite different names*

```diff
@@ -51,25 +51,27 @@
                             <div class="aa-forum-personal-message-subject">
                                 {{ message.subject }}
 
                                 <span class="float-end">
                                     <button
                                         class="btn btn-aa-forum-topic-moderation btn-sm btn-read-personal-message"
                                         title="{% translate 'Read message' %}"
+                                        data-bs-tooltip="aa-forum"
                                         data-sender="{{ message.sender.pk }}"
                                         data-recipient="{{ message.recipient.pk }}"
                                         data-message="{{ message.pk }}"
                                         data-message-folder="sent-messages"
                                     >
                                         <i class="fa-solid fa-envelope-open"></i>
                                     </button>
 
                                     <button
                                         class="btn btn-aa-forum-topic-moderation btn-sm btn-aa-forum-delete"
                                         title="{% translate 'Delete message' %}"
+                                        data-bs-tooltip="aa-forum"
                                         data-bs-toggle="modal"
                                         data-bs-target="#delete-message-{{ message.pk }}"
                                     >
                                         <i class="fa-regular fa-trash-can"></i>
                                     </button>
                                 </span>
                             </div>
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/profile/form.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/profile/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/search/pagination.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/search/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/partials/search/search-form.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/partials/search/search-form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,9 @@
     {% include "aa_forum/bundles/aa-forum-css.html" %}
 {% endblock %}
 
 {% block extra_javascript %}
     {% include "bundles/jquery-ui-js.html" %}
     {% include "aa_forum/bundles/sumoselect-js.html" %}
     {% include "aa_forum/bundles/aa-forum-admin-js.html" %}
+    {% include "aa_forum/bundles/aa-forum-bootstrap-js.html" %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -3,8 +3,9 @@
 translate "Forum" as app_title %} {{ page_title|title }} Â» {{ app_title }} {%
 endblock %} {% block aa_forum_body %}
 {% include "aa_forum/partials/administration/categories.html" %} {% endblock %}
 {% block extra_css %} {% include "bundles/jquery-ui-css.html" %} {% include
 "aa_forum/bundles/sumoselect-css.html" %} {% include "aa_forum/bundles/aa-
 forum-css.html" %} {% endblock %} {% block extra_javascript %} {% include
 "bundles/jquery-ui-js.html" %} {% include "aa_forum/bundles/sumoselect-js.html"
-%} {% include "aa_forum/bundles/aa-forum-admin-js.html" %} {% endblock %}
+%} {% include "aa_forum/bundles/aa-forum-admin-js.html" %} {% include
+"aa_forum/bundles/aa-forum-bootstrap-js.html" %} {% endblock %}
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/board.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/board.html`

 * *Files 19% similar despite different names*

```diff
@@ -17,7 +17,11 @@
         {% include "aa_forum/partials/forum/board/no-access.html" %}
     {% endif %}
 {% endblock %}
 
 {% block extra_css %}
     {% include "aa_forum/bundles/aa-forum-css.html" %}
 {% endblock %}
+
+{% block extra_javascript %}
+    {% include "aa_forum/bundles/aa-forum-bootstrap-js.html" %}
+{% endblock %}
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/index.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -38,7 +38,11 @@
         </div>
     </div>
 {% endblock %}
 
 {% block extra_css %}
     {% include "aa_forum/bundles/aa-forum-css.html" %}
 {% endblock %}
+
+{% block extra_javascript %}
+    {% include "aa_forum/bundles/aa-forum-bootstrap-js.html" %}
+{% endblock %}
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/modify-message.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/modify-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/modify-topic.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/modify-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/new-topic.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/new-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/topic.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/topic.html`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
                 {% if can_modify_subject %}
                     <a
                         id="aa-forum-btn-modify-topic-{{ topic.pk }}"
                         href="{% url 'aa_forum:forum_topic_modify' topic.board.category.slug topic.board.slug topic.slug %}"
                         class="btn btn-aa-forum-topic-moderation btn-sm float-end"
                         title="{% translate 'Modify topic subject' %}"
+                        data-bs-tooltip="aa-forum"
                     >
                         <i class="fa-solid fa-pencil"></i>
                     </a>
-
                 {% endif %}
             </div>
         </div>
     </div>
 
     {% include "aa_forum/partials/forum/topic/pagination.html" %}
 
@@ -52,14 +52,15 @@
 {% endblock %}
 
 {% block extra_javascript %}
     {% include "aa_forum/bundles/ckeditor5-js.html" %}
     {% include "aa_forum/bundles/aa-forum-ckeditor-js.html" %}
     {% include "aa_forum/bundles/aa-forum-oembed-js.html" %}
     {% include "bundles/clipboard-js.html" %}
+    {% include "aa_forum/bundles/aa-forum-bootstrap-js.html" %}
 
     <script>
         $(document).ready(function () {
             let clipboard = new ClipboardJS('.btn-aa-forum-copy-to-clipboard');
 
             clipboard.on('success', function (e) {
                 e.clearSelection();
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/forum/unread-topics.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/forum/unread-topics.html`

 * *Files 14% similar despite different names*

```diff
@@ -32,13 +32,14 @@
             </div>
         </div>
     {% endif %}
 {% endblock %}
 
 {% block extra_javascript %}
     {% include "aa_forum/bundles/aa-forum-oembed-js.html" %}
+    {% include "aa_forum/bundles/aa-forum-bootstrap-js.html" %}
 {% endblock %}
 
 {% block extra_css %}
     {% include "aa_forum/bundles/ckeditor5-css.html" %}
     {% include "aa_forum/bundles/aa-forum-css.html" %}
 {% endblock %}
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/personal-messages/inbox.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/inbox.html`

 * *Files 6% similar despite different names*

```diff
@@ -21,8 +21,9 @@
     {% include "aa_forum/bundles/ckeditor5-css.html" %}
     {% include "aa_forum/bundles/aa-forum-css.html" %}
 {% endblock %}
 
 {% block extra_javascript %}
     {% include "aa_forum/bundles/aa-forum-oembed-js.html" %}
     {% include "aa_forum/bundles/aa-forum-personal-messages-js.html" %}
+    {% include "aa_forum/bundles/aa-forum-bootstrap-js.html" %}
 {% endblock %}
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/personal-messages/new-message.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/new-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html`

 * *Files 6% similar despite different names*

```diff
@@ -21,8 +21,9 @@
     {% include "aa_forum/bundles/ckeditor5-css.html" %}
     {% include "aa_forum/bundles/aa-forum-css.html" %}
 {% endblock %}
 
 {% block extra_javascript %}
     {% include "aa_forum/bundles/aa-forum-personal-messages-js.html" %}
     {% include "aa_forum/bundles/aa-forum-oembed-js.html" %}
+    {% include "aa_forum/bundles/aa-forum-bootstrap-js.html" %}
 {% endblock %}
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/profile/index.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/profile/index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/search/results.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/search/results.html`

 * *Files 2% similar despite different names*

```diff
@@ -31,13 +31,14 @@
             {% translate "Nothing found …" %}
         {% endif %}
     {% endif %}
 {% endblock %}
 
 {% block extra_javascript %}
     {% include "aa_forum/bundles/aa-forum-oembed-js.html" %}
+    {% include "aa_forum/bundles/aa-forum-bootstrap-js.html" %}
 {% endblock %}
 
 {% block extra_css %}
     {% include "aa_forum/bundles/ckeditor5-css.html" %}
     {% include "aa_forum/bundles/aa-forum-css.html" %}
 {% endblock %}
```

### Comparing `aa_forum-2.0.0b3/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html` & `aa_forum-2.1.0/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/templatetags/aa_forum.py` & `aa_forum-2.1.0/aa_forum/templatetags/aa_forum.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,16 @@
         )
         link_title = _("Timezone conversion")
 
         return mark_safe(
             s=(
                 f"{formatted_forum_date} "
                 f'<sup>(<a href="{timezones_url}" target="_blank" rel="noopener noreferer" '
-                f'title="{link_title}"><i class="fa-solid fa-circle-question"></i></a>)</sup>'
+                f'title="{link_title}" data-bs-tooltip="aa-forum">'
+                '<i class="fa-solid fa-circle-question"></i></a>)</sup>'
             )
         )
 
     return formatted_forum_date
 
 
 @register.filter
@@ -260,15 +261,15 @@
     return_value = ""
     message_count = PersonalMessage.objects.get_personal_message_unread_count_for_user(
         user=user
     )
 
     if message_count > 0:
         return_value = mark_safe(
-            s=f'<span class="badge aa-forum-badge-personal-messages-unread-count">{message_count}</span>'  # pylint: disable=line-too-long
+            s=f'<span class="badge bg-light aa-forum-badge-personal-messages-unread-count">{message_count}</span>'  # pylint: disable=line-too-long
         )
 
     return return_value
 
 
 @register.filter
 def aa_forum_main_character_name(user: User) -> str:
```

### Comparing `aa_forum-2.0.0b3/aa_forum/tests/test_app_settings.py` & `aa_forum-2.1.0/aa_forum/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/tests/test_auth_hooks.py` & `aa_forum-2.1.0/aa_forum/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/tests/test_helpers.py` & `aa_forum-2.1.0/aa_forum/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/tests/test_integration.py` & `aa_forum-2.1.0/aa_forum/tests/test_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,19 @@
             character_id=1002,
             character_name="Peter Parker",
             permissions=["aa_forum.basic_access"],
         )
         cls.user_1003 = create_fake_user(
             character_id=1003, character_name="Lex Luthor", permissions=[]
         )
+        cls.user_1004 = create_fake_user(
+            character_id=1004,
+            character_name="Clark Kent",
+            permissions=["aa_forum.basic_access", "aa_forum.manage_forum"],
+        )
 
         cls.category = Category.objects.create(name="Science")
         cls.board = Board.objects.create(name="Physics", category=cls.category)
         cls.board_with_webhook = Board.objects.create(
             name="Chemistry",
             category=cls.category,
             discord_webhook="https://discord.com/webhook/",
@@ -210,15 +215,15 @@
             "Please make sure you enter both fields, "
             "as both fields are mandatory.</p>"
         )
         messages = list(response.context["messages"])
         self.assertEqual(first=len(messages), second=1)
         self.assertEqual(first=str(messages[0]), second=expected_message)
 
-    def test_should_not_create_new_topic_doe_to_message_missing(self):
+    def test_should_not_create_new_topic_due_to_message_missing(self):
         """
         Test should not create a new topic due to a missing/empty message
 
         :return:
         :rtype:
         """
 
@@ -525,14 +530,137 @@
         self.assertEqual(first=topic.messages.count(), second=6)
         self.assertTemplateUsed(
             response=response, template_name="aa_forum/view/forum/topic.html"
         )
         new_message = Message.objects.last()
         self.assertEqual(first=new_message.message, second="What is dark matter?")
 
+    def test_should_create_a_reply_and_close_topic_for_op(self):
+        """
+        Test should create a reply and close the topic (for OP)
+
+        :return:
+        :rtype:
+        """
+
+        # Create a new topic
+        self.app.set_user(user=self.user_1001)
+        page = self.app.get(url=self.board.get_absolute_url())
+
+        # Create a new topic
+        page = page.click(linkid="aa-forum-btn-new-topic-above-list")
+        form = page.forms["aa-forum-form-new-topic"]
+        form["subject"] = "Recent Discoveries"
+        form["message"] = "Energy of the Higgs boson"
+        form.submit().follow()
+
+        new_topic = Topic.objects.last()
+        page = self.app.get(url=new_topic.get_absolute_url())
+
+        # OP closes the topic
+        form = page.forms["aa-forum-form-message-reply"]
+        form["message"] = "What is dark matter?"
+        form["close_topic"] = True
+        response = form.submit().follow().follow()
+
+        # then
+        self.assertTemplateUsed(
+            response=response, template_name="aa_forum/view/forum/topic.html"
+        )
+        new_topic.refresh_from_db()
+        self.assertTrue(new_topic.is_locked)
+
+    def test_should_create_a_reply_and_close_topic_for_mod(self):
+        """
+        Test should create a reply and close the topic (for Mod)
+
+        :return:
+        :rtype:
+        """
+
+        # Create a new topic
+        self.app.set_user(user=self.user_1001)
+        page = self.app.get(url=self.board.get_absolute_url())
+
+        # Create a new topic
+        page = page.click(linkid="aa-forum-btn-new-topic-above-list")
+        form = page.forms["aa-forum-form-new-topic"]
+        form["subject"] = "Recent Discoveries"
+        form["message"] = "Energy of the Higgs boson"
+        form.submit().follow()
+        new_topic = Topic.objects.last()
+
+        # Log in the mod
+        self.app.set_user(user=self.user_1004)
+        page = self.app.get(url=new_topic.get_absolute_url())
+
+        # Mod closes the topic
+        form = page.forms["aa-forum-form-message-reply"]
+        form["message"] = "What is dark matter?"
+        form["close_topic"] = True
+        response = form.submit().follow().follow()
+
+        # then
+        self.assertTemplateUsed(
+            response=response, template_name="aa_forum/view/forum/topic.html"
+        )
+        new_topic.refresh_from_db()
+        self.assertTrue(new_topic.is_locked)
+
+    def test_should_create_a_reply_and_reopen_topic_for_mod(self):
+        """
+        Test should create a reply and reopen the topic (for Mod)
+
+        :return:
+        :rtype:
+        """
+
+        # Create a new topic
+        self.app.set_user(user=self.user_1001)
+        page = self.app.get(url=self.board.get_absolute_url())
+
+        # Create a new topic
+        page = page.click(linkid="aa-forum-btn-new-topic-above-list")
+        form = page.forms["aa-forum-form-new-topic"]
+        form["subject"] = "Recent Discoveries"
+        form["message"] = "Energy of the Higgs boson"
+        form.submit().follow()
+        new_topic = Topic.objects.last()
+        page = self.app.get(url=new_topic.get_absolute_url())
+
+        # OP closes the topic
+        form = page.forms["aa-forum-form-message-reply"]
+        form["message"] = "What is dark matter?"
+        form["close_topic"] = True
+        response = form.submit().follow().follow()
+
+        # then
+        self.assertTemplateUsed(
+            response=response, template_name="aa_forum/view/forum/topic.html"
+        )
+        new_topic.refresh_from_db()
+        self.assertTrue(new_topic.is_locked)
+
+        # Log in the mod
+        self.app.set_user(user=self.user_1004)
+        page = self.app.get(url=new_topic.get_absolute_url())
+
+        # Mod reopens the topic
+        form = page.forms["aa-forum-form-message-reply"]
+        form["message"] = "What is dark matter?"
+        form["reopen_topic"] = True
+        response = form.submit().follow().follow()
+
+        # then
+        self.assertTemplateUsed(
+            response=response, template_name="aa_forum/view/forum/topic.html"
+        )
+        new_topic.refresh_from_db()
+        self.assertFalse(new_topic.is_locked)
+
     def test_should_return_cleaned_message_string_on_topic_reply(self):
         """
         Test should return a clean/sanitized message string on topic reply
 
         :return:
         :rtype:
         """
```

### Comparing `aa_forum-2.0.0b3/aa_forum/tests/test_managers.py` & `aa_forum-2.1.0/aa_forum/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/tests/test_models.py` & `aa_forum-2.1.0/aa_forum/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/tests/test_signals.py` & `aa_forum-2.1.0/aa_forum/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/tests/test_templatetags.py` & `aa_forum-2.1.0/aa_forum/tests/test_templatetags.py`

 * *Files 1% similar despite different names*

```diff
@@ -756,22 +756,22 @@
         PersonalMessage.objects.create(
             sender=user_sender,
             recipient=user_receiver,
             subject="Foo",
             message="Bar",
         )
 
-        # when (template tage is triggered)
+        # when (template tag is triggered)
         response = personal_message_unread_count(user_receiver)
 
         # then
         self.assertEqual(
             first=response,
             second=(
-                '<span class="badge aa-forum-badge-personal-messages-unread-count">1</span>'  # pylint: disable=line-too-long
+                '<span class="badge bg-light aa-forum-badge-personal-messages-unread-count">1</span>'  # pylint: disable=line-too-long
             ),
         )
 
 
 class TestForumVersionedStatic(TestCase):
     """
     Tests for aa_forum_static template tag
@@ -1087,15 +1087,16 @@
         )
         link_title = "Timezone conversion"
         formatted_forum_date = "Aug. 17, 2021, 05:38:13"
 
         expected_result = (
             f"{formatted_forum_date} "
             f'<sup>(<a href="{timezones_url}" target="_blank" rel="noopener noreferer" '
-            f'title="{link_title}"><i class="fa-solid fa-circle-question"></i></a>)</sup>'
+            f'title="{link_title}" data-bs-tooltip="aa-forum">'
+            '<i class="fa-solid fa-circle-question"></i></a>)</sup>'
         )
 
         self.assertEqual(first=rendered_template, second=expected_result)
 
     def test_should_return_empty_date_and_time_string(self):
         """
         Test should return empty date and time string for message_date = ""
```

### Comparing `aa_forum-2.0.0b3/aa_forum/tests/test_views_admin.py` & `aa_forum-2.1.0/aa_forum/tests/test_views_admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/tests/test_views_forum.py` & `aa_forum-2.1.0/aa_forum/tests/test_views_forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/tests/utils.py` & `aa_forum-2.1.0/aa_forum/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/views/admin.py` & `aa_forum-2.1.0/aa_forum/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/views/forum.py` & `aa_forum-2.1.0/aa_forum/views/forum.py`

 * *Files 1% similar despite different names*

```diff
@@ -865,14 +865,35 @@
             new_message = Message(
                 topic=current_topic,
                 user_created=request.user,
                 message=form.cleaned_data["message"],
             )
             new_message.save()
 
+            # Check if the user has the rights to close or reopen the topic
+            if (
+                request.user.has_perm(perm="aa_forum.manage_forum")
+                or request.user == current_topic.first_message.user_created
+            ):
+                # Close the topic if requested
+                if (
+                    form.cleaned_data["close_topic"]
+                    and not form.cleaned_data["reopen_topic"]
+                ):
+                    current_topic.is_locked = True
+                    current_topic.save(update_fields=["is_locked"])
+
+                # Reopen the topic if requested
+                if (
+                    form.cleaned_data["reopen_topic"]
+                    and not form.cleaned_data["close_topic"]
+                ) and request.user.has_perm(perm="aa_forum.manage_forum"):
+                    current_topic.is_locked = False
+                    current_topic.save(update_fields=["is_locked"])
+
             # Send to webhook if one is configured
             if (
                 current_topic.board.discord_webhook is not None
                 and current_topic.board.use_webhook_for_replies is not False
             ):
                 send_message_to_discord_webhook(
                     board=current_topic.board,
```

### Comparing `aa_forum-2.0.0b3/aa_forum/views/personal_messages.py` & `aa_forum-2.1.0/aa_forum/views/personal_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/views/profile.py` & `aa_forum-2.1.0/aa_forum/views/profile.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/views/search.py` & `aa_forum-2.1.0/aa_forum/views/search.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/aa_forum/views/widgets.py` & `aa_forum-2.1.0/aa_forum/views/widgets.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/LICENSE` & `aa_forum-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_forum-2.0.0b3/README.md` & `aa_forum-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 Simple forum app for [Alliance Auth]
 
 ______________________________________________________________________
 
 <!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=1 -->
 
 - [AA Forum](#aa-forum)
-  - [⚠️ Before You Install This Module ⚠️](#%E2%9A%A0%EF%B8%8F-before-you-install-this-module-%E2%9A%A0%EF%B8%8F)
+  - [Before You Install This Module](#before-you-install-this-module)
   - [Overview](#overview)
     - [Features](#features)
     - [Screenshots](#screenshots)
       - [Forum Index](#forum-index)
       - [Topic Overview / Board Index](#topic-overview--board-index)
       - [Topic View](#topic-view)
       - [Start New Topic (ckEditor)](#start-new-topic-ckeditor)
@@ -45,15 +45,15 @@
   - [Translation Status](#translation-status)
   - [Contributing](#contributing)
 
 <!-- mdformat-toc end -->
 
 ______________________________________________________________________
 
-## ⚠️ Before You Install This Module ⚠️<a name="%E2%9A%A0%EF%B8%8F-before-you-install-this-module-%E2%9A%A0%EF%B8%8F"></a>
+## Before You Install This Module<a name="before-you-install-this-module"></a>
 
 This module needs quite some configuration done before working properly. You need to
 modify your Apache/Nginx configuration as well as the global URL config of Alliance
 Auth. So please only install if you know what you're doing/feel comfortable making
 these kinds of changes. For your own sanity, and mine :-)
 
 ## Overview<a name="overview"></a>
@@ -101,19 +101,21 @@
 
 ![Screenshot: Admin View]
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Forum needs at least Alliance Auth v4.0.0!**
+> **AA Forum >= 2.0.0 needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version of AA Forum that supports Alliance Auth v3 is `1.19.5`.
 
 **Important**: Please make sure you meet all preconditions before you proceed:
 
 - AA Forum is a plugin for Alliance Auth. If you don't have Alliance Auth running
   already, please install it first before proceeding. (see the official
   [AA installation guide] for details)
 - AA Forum needs a couple of changes made to your Webserver and Alliance Auth
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_forum-2.0.0b3/pyproject.toml` & `aa_forum-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "allianceauth>=4.0.0b2",
+    "allianceauth<5.0.0,>=4",
     "allianceauth-app-utils>=1.24",
     "dhooks-lite>=1.1",
     "django-ckeditor-5>=0.2.11",
     "unidecode>=1.3.7",
 ]
 [project.optional-dependencies]
 tests-allianceauth-latest = [
```

### Comparing `aa_forum-2.0.0b3/PKG-INFO` & `aa_forum-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: aa-forum
-Version: 2.0.0b3
+Version: 2.1.0
 Summary: Simple forum for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-forum/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-forum/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-forum
 Project-URL: Source, https://github.com/ppfeufer/aa-forum.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-forum/issues
@@ -698,15 +698,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.24
-Requires-Dist: allianceauth>=4.0.0b2
+Requires-Dist: allianceauth<5.0.0,>=4
 Requires-Dist: dhooks-lite>=1.1
 Requires-Dist: django-ckeditor-5>=0.2.11
 Requires-Dist: unidecode>=1.3.7
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: aa-timezones; extra == 'tests-allianceauth-latest'
 Requires-Dist: allianceauth-discordbot; extra == 'tests-allianceauth-latest'
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
@@ -736,15 +736,15 @@
 Simple forum app for [Alliance Auth]
 
 ______________________________________________________________________
 
 <!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=1 -->
 
 - [AA Forum](#aa-forum)
-  - [⚠️ Before You Install This Module ⚠️](#%E2%9A%A0%EF%B8%8F-before-you-install-this-module-%E2%9A%A0%EF%B8%8F)
+  - [Before You Install This Module](#before-you-install-this-module)
   - [Overview](#overview)
     - [Features](#features)
     - [Screenshots](#screenshots)
       - [Forum Index](#forum-index)
       - [Topic Overview / Board Index](#topic-overview--board-index)
       - [Topic View](#topic-view)
       - [Start New Topic (ckEditor)](#start-new-topic-ckeditor)
@@ -763,15 +763,15 @@
   - [Translation Status](#translation-status)
   - [Contributing](#contributing)
 
 <!-- mdformat-toc end -->
 
 ______________________________________________________________________
 
-## ⚠️ Before You Install This Module ⚠️<a name="%E2%9A%A0%EF%B8%8F-before-you-install-this-module-%E2%9A%A0%EF%B8%8F"></a>
+## Before You Install This Module<a name="before-you-install-this-module"></a>
 
 This module needs quite some configuration done before working properly. You need to
 modify your Apache/Nginx configuration as well as the global URL config of Alliance
 Auth. So please only install if you know what you're doing/feel comfortable making
 these kinds of changes. For your own sanity, and mine :-)
 
 ## Overview<a name="overview"></a>
@@ -819,19 +819,21 @@
 
 ![Screenshot: Admin View]
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Forum needs at least Alliance Auth v4.0.0!**
+> **AA Forum >= 2.0.0 needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version of AA Forum that supports Alliance Auth v3 is `1.19.5`.
 
 **Important**: Please make sure you meet all preconditions before you proceed:
 
 - AA Forum is a plugin for Alliance Auth. If you don't have Alliance Auth running
   already, please install it first before proceeding. (see the official
   [AA installation guide] for details)
 - AA Forum needs a couple of changes made to your Webserver and Alliance Auth
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

