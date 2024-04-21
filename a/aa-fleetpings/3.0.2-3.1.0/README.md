# Comparing `tmp/aa_fleetpings-3.0.2.tar.gz` & `tmp/aa_fleetpings-3.1.0.tar.gz`

## Comparing `aa_fleetpings-3.0.2.tar` & `aa_fleetpings-3.1.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/__init__.py
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/admin.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/app_settings.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/apps.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/auth_hooks.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/constants.py
--rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/form.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/managers.py
--rw-r--r--   0        0        0    17339 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/models.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/urls.py
--rw-r--r--   0        0        0    13953 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/views.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/helper/discord_webhook.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/helper/eve_images.py
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/helper/ping_context.py
--rw-r--r--   0        0        0    13803 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/django.pot
--rw-r--r--   0        0        0    13932 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    14182 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22749 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15436 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13947 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    13804 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    13849 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14415 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/pl_PL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    17350 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    23453 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24381 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14245 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    12854 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0001_initial.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0002_webhook_is_embed_description_change.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0003_fleetdoctrine_link.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0004_auto_20200915_1617.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0005_fleettype_restricted_to_group.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0008_auto_20210114_1733.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py
--rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0011_settings_and_verbose_names.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0013_fleetcomm_channel.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0014_update_models.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/migrations/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/static/fleetpings/css/fleetpings.css
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/static/fleetpings/css/fleetpings.min.css
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/static/fleetpings/css/fleetpings.min.css.map
--rw-r--r--   0        0        0    19511 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/static/fleetpings/js/fleetpings.js
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/static/fleetpings/js/fleetpings.min.js
--rw-r--r--   0        0        0     8936 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/static/fleetpings/js/fleetpings.min.js.map
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/LICENSE
--rw-r--r--   0        0        0    34864 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.js
--rw-r--r--   0        0        0    12465 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js
--rw-r--r--   0        0        0    53322 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js.map
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/readme.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/base.html
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/index.html
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/bundles/fleetpings-css.html
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/bundles/fleetpings-js.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/form.html
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/segments/fleet-comms.html
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/segments/fleet-formup-location.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/segments/fleet-type-loop.html
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/segments/ping-channel.html
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/segments/ping-targets-loop.html
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/header/page-header.html
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/ping/ping.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templatetags/__init__.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/templatetags/fleetpings.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/__init__.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_access.py
--rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_ajax_calls.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_helper_eve_images.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_installed_modules.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_model_discprdpingtarget.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_model_fleetcomm.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_model_fleetdoctrine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_model_fleettype.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_model_formuplocation.py
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_model_setting.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_model_webhook.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/test_templatetags.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/fleetpings/tests/utils.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/LICENSE
--rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/README.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/pyproject.toml
--rw-r--r--   0        0        0    51307 2020-02-02 00:00:00.000000 aa_fleetpings-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/__init__.py
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/admin.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/app_settings.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/apps.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/auth_hooks.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/constants.py
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/form.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/managers.py
+-rw-r--r--   0        0        0    17339 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/models.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/urls.py
+-rw-r--r--   0        0        0    13953 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/views.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/helper/discord_webhook.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/helper/eve_images.py
+-rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/helper/ping_context.py
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/django.pot
+-rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    14326 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20019 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15662 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14081 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    13804 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20501 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14556 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17350 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    23594 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    14069 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24522 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14386 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    12854 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0001_initial.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0002_webhook_is_embed_description_change.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0003_fleetdoctrine_link.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0004_auto_20200915_1617.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0005_fleettype_restricted_to_group.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0008_auto_20210114_1733.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py
+-rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0011_settings_and_verbose_names.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0013_fleetcomm_channel.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0014_update_models.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/css/fleetpings.css
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/css/fleetpings.min.css
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/css/fleetpings.min.css.map
+-rw-r--r--   0        0        0    19511 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.js
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.min.js
+-rw-r--r--   0        0        0     8936 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.min.js.map
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/LICENSE
+-rw-r--r--   0        0        0    34864 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.js
+-rw-r--r--   0        0        0    12465 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js
+-rw-r--r--   0        0        0    53322 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js.map
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/readme.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/base.html
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/index.html
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/bundles/fleetpings-css.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/bundles/fleetpings-js.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/form.html
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-comms.html
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-formup-location.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-type-loop.html
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/ping-channel.html
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/ping-targets-loop.html
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/header/page-header.html
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/ping/ping.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templatetags/__init__.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templatetags/fleetpings.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/__init__.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_access.py
+-rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_ajax_calls.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_helper_eve_images.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_installed_modules.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_discprdpingtarget.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleetcomm.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleetdoctrine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleettype.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_formuplocation.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_setting.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_webhook.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_templatetags.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/utils.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/LICENSE
+-rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/README.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    51307 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/PKG-INFO
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/admin.py` & `aa_fleetpings-3.1.0/fleetpings/admin.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/app_settings.py` & `aa_fleetpings-3.1.0/fleetpings/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/auth_hooks.py` & `aa_fleetpings-3.1.0/fleetpings/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/form.py` & `aa_fleetpings-3.1.0/fleetpings/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,7 +198,12 @@
         required=False,
         label=_("Create Optimer"),
         help_text=_(
             "If this checkbox is active, a fleet operations timer for this pre-ping "
             "will be created."
         ),
     )
+    fleet_duration = forms.CharField(
+        required=False,
+        label=_("Duration"),
+        help_text=_("How long approximately will the fleet be?"),
+    )
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/managers.py` & `aa_fleetpings-3.1.0/fleetpings/managers.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/models.py` & `aa_fleetpings-3.1.0/fleetpings/models.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/urls.py` & `aa_fleetpings-3.1.0/fleetpings/urls.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/views.py` & `aa_fleetpings-3.1.0/fleetpings/views.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/helper/discord_webhook.py` & `aa_fleetpings-3.1.0/fleetpings/helper/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/helper/eve_images.py` & `aa_fleetpings-3.1.0/fleetpings/helper/eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/helper/ping_context.py` & `aa_fleetpings-3.1.0/fleetpings/helper/ping_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         "ping_channel": {
             "webhook": ping_channel_webhook,
             "embed_color": ping_channel_webhook_embed_color,
         },
         "fleet_type": str(form_data["fleet_type"]),
         "fleet_commander": str(form_data["fleet_commander"]),
         "fleet_name": str(form_data["fleet_name"]),
+        "fleet_duration": str(form_data["fleet_duration"]),
         "formup_location": str(form_data["formup_location"]),
         "is_pre_ping": bool(form_data["pre_ping"]),
         "is_formup_now": bool(form_data["formup_now"]),
         "formup_time": {
             "datetime_string": str(form_data["formup_time"]),
             "timestamp": str(form_data["formup_timestamp"]),
         },
@@ -144,15 +145,15 @@
             )
     else:
         if ping_context["fleet_type"]:
             webhook_ping_text_header += f'{ping_context["fleet_type"]} '
 
         webhook_ping_text_header += "Fleet is up"
 
-        # Add fcName if we have one
+        # Add FC name if we have one
         if ping_context["fleet_commander"]:
             webhook_ping_text_header += f' under {ping_context["fleet_commander"]}'
 
     webhook_ping_text_header += "**\n** **"
 
     # Add FC name if we have one
     if ping_context["fleet_commander"]:
@@ -191,14 +192,21 @@
 
             # Add local time
             webhook_ping_text_content += (
                 "\n**Formup (Local Time):** "
                 f'<t:{ping_context["formup_time"]["timestamp"]}:F>'
                 f' (<t:{ping_context["formup_time"]["timestamp"]}:R>)'
             )
+
+    # Check if fleet duration is available
+    if ping_context["fleet_duration"]:
+        webhook_ping_text_content += (
+            f'\n**Duration (approximately):** {ping_context["fleet_duration"]}'
+        )
+
     # Check if fleet comms is available
     if ping_context["fleet_comms"]:
         webhook_ping_text_content += f'\n**Comms:** {ping_context["fleet_comms"]}'
 
     # Check if doctrine is available
     if ping_context["doctrine"]["name"]:
         webhook_ping_text_content += (
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/django.pot` & `aa_fleetpings-3.1.0/fleetpings/locale/django.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-20 17:22+0100\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -179,14 +179,22 @@
 
 #: fleetpings/form.py:201
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
@@ -459,15 +467,15 @@
 "existing translation?"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 msgid "Create ping"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/cs/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/cs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-20 17:22+0100\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
 msgid "Fleet comm"
@@ -180,14 +181,22 @@
 
 #: fleetpings/form.py:201
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
@@ -460,15 +469,15 @@
 "existing translation?"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 msgid "Create ping"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/de/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.0/fleetpings/locale/de/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetpings/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.4.3\n"
 
 msgid ""
 "\n"
 "                <code>@everyone</code>\n"
 "                includes also all the people in this channel who are offline "
 "and\n"
 "                possibly asleep at the moment and might be waking up when "
@@ -109,14 +109,17 @@
 
 msgid "Doctrine link"
 msgstr "Doktrin Link"
 
 msgid "Don't ping"
 msgstr "Nicht pingen"
 
+msgid "Duration"
+msgstr "Dauer"
+
 msgid "Embed color"
 msgstr "Embed Farbe"
 
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
@@ -198,14 +201,17 @@
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
 "Hinweis: Du kannst {discord_markdown_link} nutzen um den Text zu formatieren."
 
 msgid "Home Defense"
 msgstr "Heimatverteidigung"
 
+msgid "How long approximately will the fleet be?"
+msgstr "Wie lange wird die Flotte etwa dauern?"
+
 msgid "ID of the Discord role to ping"
 msgstr "ID der Discord Rolle zum Pingen"
 
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/de/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
-"PO-Revision-Date: 2024-03-16 09:25+0000\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
+"PO-Revision-Date: 2024-04-21 13:51+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-fleetpings/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.4.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr "Flotten-Ankündigungen"
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
@@ -192,14 +192,22 @@
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 "Wenn dieses Kontrollkästchen aktiviert ist, wird ein Op Timer für diesen Pre-"
 "Ping erstellt."
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr "Dauer"
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr "Wie lange wird die Flotte etwa dauern?"
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr "Du solltest zunächst den Discord Service installieren …"
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
@@ -506,15 +514,15 @@
 "Du möchtest helfen diese App in Deine Sprache zu übersetzen oder die "
 "bestehende Übersetzung verbessern?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Tritt unserm Team von Übersetzern bei!"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 msgid "Create ping"
 msgstr "Ping erstellen"
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
 "Bitte überlege zweimal, ob Du wirklich <code>@everyone</code> pingen musst."
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/es/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.0/fleetpings/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/es/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/es/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
 # Peter Pfeufer <info@ppfeufer.de>, 2023.
 # Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
 "PO-Revision-Date: 2023-10-25 07:04+0000\n"
 "Last-Translator: Geovanny David Morales De la cruz "
 "<moralesgeovanny1996@gmail.com>\n"
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetpings/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
@@ -216,14 +216,22 @@
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 "Si esta casilla de verificación está activa, se creará un temporizador de "
 "operaciones de flota para este pre-ping."
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr "Es posible que desee instalar primero el servicio de Discord …"
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "¿Está seguro de que tiene su Discord vinculado a su Alliance Auth?"
@@ -567,15 +575,15 @@
 "¿Quieres ayudar a traducir esta aplicación a tu idioma o mejorar la "
 "traducción existente?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "¡Únete a nuestro equipo de traductores!"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 #, fuzzy
 #| msgid "Create Ping"
 msgid "Create ping"
 msgstr "Crear Ping"
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -15,14 +15,20 @@
 
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Êtes-vous sûr d'avoir lié Discord à votre Alliance Auth ?"
 
 msgid "Can access this app"
 msgstr "Peut accéder à cette application"
 
+msgid "Discord ID"
+msgstr "ID Discord"
+
+msgid "Discord Markdown"
+msgstr "Discord Markdown"
+
 msgid "Discord channel"
 msgstr "Canal Discord"
 
 msgid "Discord ping target"
 msgstr "Cible du ping Discord"
 
 msgid "Discord ping targets"
@@ -70,14 +76,17 @@
 
 msgid "Is enabled"
 msgstr "Est activé"
 
 msgid "Join our team of translators!"
 msgstr "Rejoignez notre équipe de traducteurs !"
 
+msgid "Name"
+msgstr "Nom"
+
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Nom du rôle Discord à pinger. (Remarque : il doit s'agir d'un groupe d'AAuth "
 "synchronisé avec Discord.)"
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/fr_FR/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # erka Ekanon <M6musicT@hotmail.fr>, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
+# Matthias P <randomusernetcom@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
-"PO-Revision-Date: 2024-04-01 09:51+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-fleetpings/fr/>\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
+"PO-Revision-Date: 2024-04-17 23:13+0000\n"
+"Last-Translator: Matthias P <randomusernetcom@gmail.com>\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-fleetpings/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 5.4.3\n"
 
@@ -66,15 +67,15 @@
 #: fleetpings/apps.py:21
 #, python-brace-format
 msgid "Fleet Pings v{__version__}"
 msgstr ""
 
 #: fleetpings/form.py:27
 msgid "Discord Markdown"
-msgstr ""
+msgstr "Discord Markdown"
 
 #: fleetpings/form.py:34
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
 "Astuce : Vous pouvez utiliser {discord_markdown_link} pour formater le texte."
 
@@ -182,14 +183,22 @@
 
 #: fleetpings/form.py:201
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr "Vous souhaiterez peut-être d’abord installer le service Discord…"
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Êtes-vous sûr d'avoir lié Discord à votre Alliance Auth ?"
@@ -205,15 +214,15 @@
 #: fleetpings/models.py:127
 msgid "Short name to identify this comms"
 msgstr ""
 
 #: fleetpings/models.py:128 fleetpings/models.py:184 fleetpings/models.py:272
 #: fleetpings/models.py:434
 msgid "Name"
-msgstr ""
+msgstr "Nom"
 
 #: fleetpings/models.py:134
 msgid "In which channel is the fleet?"
 msgstr ""
 
 #: fleetpings/models.py:135
 msgid "Channel"
@@ -294,15 +303,15 @@
 
 #: fleetpings/models.py:334
 msgid "ID of the Discord role to ping"
 msgstr "ID du rôle Discord à pinger"
 
 #: fleetpings/models.py:335
 msgid "Discord ID"
-msgstr ""
+msgstr "ID Discord"
 
 #: fleetpings/models.py:343 fleetpings/models.py:521
 msgid "Restrict ping rights to the following groups …"
 msgstr "Restreindre les droits de ping aux groupes suivants…"
 
 #: fleetpings/models.py:419
 msgid "Discord ping target"
@@ -472,15 +481,15 @@
 "Voulez-vous aider à traduire cette application dans votre langue ou "
 "améliorer la traduction existante ?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Rejoignez notre équipe de traducteurs !"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 msgid "Create ping"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/it_IT/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
 "PO-Revision-Date: 2023-09-24 13:14+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetpings/it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -181,14 +181,22 @@
 
 #: fleetpings/form.py:201
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
@@ -461,15 +469,15 @@
 "existing translation?"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 msgid "Create ping"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/ja/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/ja/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
 "PO-Revision-Date: 2023-09-24 13:14+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetpings/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -181,14 +181,22 @@
 
 #: fleetpings/form.py:201
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
@@ -461,15 +469,15 @@
 "existing translation?"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 msgid "Create ping"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/ko_KR/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # Author50CO <tkddlschry@gmail.com>, 2023.
 # Peter Pfeufer <info@ppfeufer.de>, 2023.
 # Mind of the Raven <okanieva@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
 "PO-Revision-Date: 2024-03-22 01:11+0000\n"
 "Last-Translator: Mind of the Raven <okanieva@gmail.com>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-fleetpings/ko/>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-fleetpings/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.4.2\n"
 
@@ -199,14 +199,22 @@
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 "이 체크박스가 활성화되어 있으면, 이 예고 핑에 대한 함대 옵 타이머가 생성됩니"
 "다."
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr "디스코드 서비스를 먼저 설치해주세요…"
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "디스코드가 Alliance Auth와 연동되어 있나요?"
@@ -430,18 +438,18 @@
 msgid ""
 "Whether to verify webhooks URLs or not. Note: When unchecked, webhook URLs "
 "will not be verified, so the app can be used with non-Discord webhooks as "
 "well. When disabling webhook verification and using non-Discord webhooks, it "
 "is up to you to make sure your webhook understands a payload that is "
 "formatted for Discord webhooks."
 msgstr ""
-"웹훅 URL 검사여부 설정. 설명: 체크가 해제되어 있을 경우 URL을 검사하지 "
-"않습니다, 따라서 디스코드가 아닌 URL도 사용할 수 있습니다. 웹훅 검사를 "
-"해제하고 디스코드가 아닌 웹훅을 사용할 경우, 웹훅이 전송할 부하를 감당할 수 "
-"있을지의 판단여부는 사용자의 몫입니다."
+"웹훅 URL 검사여부 설정. 설명: 체크가 해제되어 있을 경우 URL을 검사하지 않습니"
+"다, 따라서 디스코드가 아닌 URL도 사용할 수 있습니다. 웹훅 검사를 해제하고 디"
+"스코드가 아닌 웹훅을 사용할 경우, 웹훅이 전송할 부하를 감당할 수 있을지의 판"
+"단여부는 사용자의 몫입니다."
 
 #: fleetpings/models.py:655
 msgid "Default highlight color for the webhook embed."
 msgstr "웹훅 embed 기본 하이라이트 색상."
 
 #: fleetpings/models.py:667
 #, fuzzy
@@ -471,25 +479,25 @@
 
 #: fleetpings/templates/fleetpings/index.html:51
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
-"필수 정보가 누락되었습니다. 옵 타이머를 생성하려면, 다음 정보를 모두 "
-"제공해야 합니다:<br>» FC 이름<br>» 플릿 이름<br>» 폼업 지역<br>» 폼업 "
-"시각<br>» 함선/독트린"
+"필수 정보가 누락되었습니다. 옵 타이머를 생성하려면, 다음 정보를 모두 제공해"
+"야 합니다:<br>» FC 이름<br>» 플릿 이름<br>» 폼업 지역<br>» 폼업 시각<br>» 함"
+"선/독트린"
 
 #: fleetpings/templates/fleetpings/index.html:56
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
-"필수 정보가 누락되었습니다. SRP 항목을 생성하려면, 다음 정보를 기입해야 "
-"합니다:<br>» 함대 이름<br>» 함선 / 독트린"
+"필수 정보가 누락되었습니다. SRP 항목을 생성하려면, 다음 정보를 기입해야 합니"
+"다:<br>» 함대 이름<br>» 함선 / 독트린"
 
 #: fleetpings/templates/fleetpings/index.html:60
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
 msgstr ""
 "오류! 핑이 클립보드에 복사되지 않았습니다. 브라우저가 이 기능을 지원하지 않"
@@ -509,15 +517,15 @@
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "번역팀에 참여하세요!"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 #, fuzzy
 #| msgid "Create Ping"
 msgid "Create ping"
 msgstr "핑 생성"
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/nl/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/nl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-20 17:22+0100\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
 msgid "Fleet comm"
@@ -179,14 +180,22 @@
 
 #: fleetpings/form.py:201
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
@@ -459,15 +468,15 @@
 "existing translation?"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 msgid "Create ping"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/pl_PL/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.0/fleetpings/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/pl_PL/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-20 17:22+0100\n"
-"PO-Revision-Date: 2024-04-05 06:53+0000\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
+"PO-Revision-Date: 2024-04-07 13:07+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Polish <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-fleetpings/pl/>\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-fleetpings/pl/>\n"
 "Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
 "X-Generator: Weblate 5.4.3\n"
@@ -181,14 +181,22 @@
 
 #: fleetpings/form.py:201
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
@@ -465,15 +473,15 @@
 "Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
 "tłumaczenia?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Dołącz do naszego zespołu tłumaczy!"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 msgid "Create ping"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/ru/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.0/fleetpings/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/ru/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # Nikolay <nick.postnikov@gmail.com>, 2023.
 # Max <mark25@inbox.ru>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
 "PO-Revision-Date: 2023-10-03 11:34+0000\n"
 "Last-Translator: Max <mark25@inbox.ru>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetpings/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -193,14 +193,22 @@
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 "Если флажок активен, будет создан специальный таймер сбора для данного "
 "предварительно пинга."
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr "Возможно, Вам следует сначала установить сервис Discord …"
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Вы уверены, что Ваш Discord связан с Вашим Alliance Auth?"
@@ -499,15 +507,15 @@
 "Вы хотите помочь перевести это приложение на ваш язык или улучшить текущий "
 "перевод?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Присоединяйтесь к нашей команде переводчиков!"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 msgid "Create ping"
 msgstr "Создать пинг"
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr "Подумайте дважды перед тем, как пинговать <code>@everyone</code>."
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/sk/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/sk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-20 17:22+0100\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
 msgid "Fleet comm"
@@ -180,14 +181,22 @@
 
 #: fleetpings/form.py:201
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
@@ -460,15 +469,15 @@
 "existing translation?"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 msgid "Create ping"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/uk/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.0/fleetpings/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/uk/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # "Andrii M." <elfleg0las88@gmail.com>, 2023.
 # Madz Cooper <i.sviridjuk@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
 "PO-Revision-Date: 2024-03-02 23:10+0000\n"
 "Last-Translator: Madz Cooper <i.sviridjuk@gmail.com>\n"
 "Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetpings/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -228,14 +228,22 @@
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 "Якщо цей прапорець активний, буде створено таймер операцій флоту для цього "
 "попереднього пінгу."
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr "Можливо, ви захочете спочатку встановити службу Discord …"
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Ви впевнені, що ваш Discord пов'язаний з вашим Alliance Auth?"
@@ -564,15 +572,15 @@
 "existing translation?"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 #, fuzzy
 #| msgid "Create Ping"
 msgid "Create ping"
 msgstr "Створити пінг"
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.0/fleetpings/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.0/fleetpings/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Faer Yili <yilifaer@gmail.com>, 2024.
 # Dehao Wu <wudehao2000@163.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 21:21+0100\n"
+"POT-Creation-Date: 2024-04-21 09:10+0200\n"
 "PO-Revision-Date: 2024-01-11 21:04+0000\n"
 "Last-Translator: Dehao Wu <wudehao2000@163.com>\n"
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-fleetpings/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -181,14 +181,22 @@
 
 #: fleetpings/form.py:201
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
 msgstr ""
 
+#: fleetpings/form.py:207
+msgid "Duration"
+msgstr ""
+
+#: fleetpings/form.py:208
+msgid "How long approximately will the fleet be?"
+msgstr ""
+
 #: fleetpings/models.py:41
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: fleetpings/models.py:49
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
@@ -461,15 +469,15 @@
 "existing translation?"
 msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "加入我们的翻译团队吧！"
 
-#: fleetpings/templates/fleetpings/partials/form/form.html:69
+#: fleetpings/templates/fleetpings/partials/form/form.html:72
 msgid "Create ping"
 msgstr ""
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:6
 msgid "Please think twice if you really need to ping <code>@everyone</code>."
 msgstr ""
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0001_initial.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0002_webhook_is_embed_description_change.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0002_webhook_is_embed_description_change.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0003_fleetdoctrine_link.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0003_fleetdoctrine_link.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0004_auto_20200915_1617.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0004_auto_20200915_1617.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0005_fleettype_restricted_to_group.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0005_fleettype_restricted_to_group.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0008_auto_20210114_1733.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0008_auto_20210114_1733.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0011_settings_and_verbose_names.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0011_settings_and_verbose_names.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0013_fleetcomm_channel.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0013_fleetcomm_channel.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0014_update_models.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0014_update_models.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py` & `aa_fleetpings-3.1.0/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/static/fleetpings/js/fleetpings.js` & `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/static/fleetpings/js/fleetpings.min.js` & `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/static/fleetpings/js/fleetpings.min.js.map` & `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/LICENSE` & `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.js` & `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js` & `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js.map` & `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/readme.md` & `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/readme.md`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/base.html` & `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/base.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/index.html` & `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/index.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/form.html` & `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/form.html`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,17 @@
             <div class="fleetpings-create-optimer clearfix" style="display: none;">
                 {% bootstrap_field form.optimer %}
             </div>
         {% endif %}
 
         {% bootstrap_field form.formup_now %}
 
+        <!-- fleet_duration -->
+        {% bootstrap_field form.fleet_duration %}
+
         <!-- fleet_comms -->
         {% bootstrap_field form.fleet_comms %}
 
         <!-- fleet_doctrine -->
         {% bootstrap_field form.fleet_doctrine %}
         {% bootstrap_field form.fleet_doctrine_url show_label=False %}
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html` & `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html` & `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html` & `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html` & `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html` & `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <p>
+    {# @ Mention #}
     {% if ping_target.at_mention %}
         {{ ping_target.at_mention }} ::
     {% endif %}
 
-    {#Headline#}
+    {# Headline #}
     **
 
     {% if is_pre_ping %}
         {% if not ping_target.at_mention %}\{% endif %}### PRE PING ###
 
         {% if fleet_type %}
             / (Upcoming) {{ fleet_type }} Fleet
@@ -20,82 +21,88 @@
         {% endif %}
     {% endif %}
 
     **
 
     <br>
 
-    {#Add FC name if we have one#}
+    {# Add FC name if we have one #}
     {% if fleet_commander %}
         <br>
         **FC:** {{ fleet_commander }}
     {% endif %}
 
-    {#Check if fleet name is available#}
+    {# Check if fleet name is available #}
     {% if fleet_name %}
         <br>
         **Fleet Name:** {{ fleet_name }}
     {% endif %}
 
-    {#Check for formup location#}
+    {# Check for formup location #}
     {% if formup_location %}
         <br>
         **Formup Location:** {{ formup_location }}
     {% endif %}
 
-    {#Check if form-up time is available#}
+    {# Check if form-up time is available #}
     {% if is_formup_now %}
         <br>
         **Formup Time:** NOW
     {% else %}
         <br>
         {% if formup_time.datetime_string %}
             **Formup (EVE Time):** {{ formup_time.datetime_string }}
         {% endif %}
 
         {% if formup_time.timestamp %}
-            {#Check if aa-timezones is available#}
+            {# Check if aa-timezones is available #}
             {% if timezones_installed %}
                 ([Time Zone Conversion]({{ SITE_URL }}{% url "timezones:index" formup_time.timestamp %}))
             {% endif %}
 
-            {#Add local time#}
+            {# Add local time #}
             <br>
             **Formup (Local Time):** &lt;t:{{ formup_time.timestamp }}:F&gt; (&lt;t:{{ formup_time.timestamp }}:R&gt;)
         {% endif %}
     {% endif %}
 
-    {#Check if fleet comms is available#}
+    {# Check if fleet duration is available #}
+    {% if fleet_duration %}
+        <br>
+        **Duration (approximately):** {{ fleet_duration }}
+    {% endif %}
+
+    {# Check if fleet comms is available #}
     {% if fleet_comms %}
         <br>
         **Comms:** {{ fleet_comms }}
     {% endif %}
 
-    {#Check if doctrine is available#}
+    {# Check if doctrine is available #}
     {% if doctrine.name %}
         <br>
         **Ships / Doctrine:** {{ doctrine.name }}
 
-        {#Check for doctrine link#}
+        {# Check for doctrine link #}
         {% if doctrine.link %}
             ([Doctrine Link]({{ doctrine.link }}))
         {% endif %}
     {% endif %}
 
-    {#Check if srp is available#}
+    {# Check if srp is available #}
     {% if srp.has_srp %}
         <br>
         **SRP:** Yes
 
-        {#Check if we have an SRP link#}
+        {# Check if we have an SRP link #}
         {% if srp.link.link %}
             (SRP Code: [{{ srp.link.code }}]({{ srp.link.link }}))
         {% endif %}
     {% endif %}
 
-    {#Check if additional information is available#}
+    {# Check if additional information is available #}
     {% if additional_information %}
         <br><br>
         **Additional Information:**<br>
         {{ additional_information|linebreaksbr }}
     {% endif %}
 </p>
```

### Comparing `aa_fleetpings-3.0.2/fleetpings/templates/fleetpings/partials/ping/ping.html` & `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/ping/ping.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/templatetags/fleetpings.py` & `aa_fleetpings-3.1.0/fleetpings/templatetags/fleetpings.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_access.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_ajax_calls.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_ajax_calls.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_auth_hooks.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_helper_eve_images.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_helper_eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_installed_modules.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_model_discprdpingtarget.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_model_discprdpingtarget.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_model_fleetcomm.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleetcomm.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_model_fleetdoctrine.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleetdoctrine.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_model_fleettype.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleettype.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_model_formuplocation.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_model_formuplocation.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_model_setting.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_model_setting.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_model_webhook.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_model_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/test_templatetags.py` & `aa_fleetpings-3.1.0/fleetpings/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/fleetpings/tests/utils.py` & `aa_fleetpings-3.1.0/fleetpings/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/LICENSE` & `aa_fleetpings-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/README.md` & `aa_fleetpings-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/pyproject.toml` & `aa_fleetpings-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.0.2/PKG-INFO` & `aa_fleetpings-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-fleetpings
-Version: 3.0.2
+Version: 3.1.0
 Summary: Fleet Ping Tool for Alliance Auth supporting pings via webhooks to Discord.
 Project-URL: Changelog, https://github.com/ppfeufer/aa-fleetpings/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-fleetpings/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-fleetpings
 Project-URL: Source, https://github.com/ppfeufer/aa-fleetpings.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-fleetpings/issues
```

