# Comparing `tmp/oarepo-vocabularies-2.0.83.tar.gz` & `tmp/oarepo_vocabularies-2.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-vocabularies-2.0.83.tar", last modified: Fri Apr  5 13:19:58 2024, max compression
+gzip compressed data, was "oarepo_vocabularies-2.0.84.tar", last modified: Sun Apr 21 10:44:05 2024, max compression
```

## Comparing `oarepo-vocabularies-2.0.83.tar` & `oarepo_vocabularies-2.0.84.tar`

### file list

```diff
@@ -1,242 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.926771 oarepo-vocabularies-2.0.83/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-05 13:19:58.926771 oarepo-vocabularies-2.0.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.898771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.902771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/ext_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.902771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/hacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.902771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/models/ui.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.902771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.902771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.902771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/jsonschemas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/systemfields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.902771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.902771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/records/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.902771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/vocabulary_type/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/vocabulary_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/vocabulary_type/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/vocabulary_type/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.906771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.906771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/components/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/components/scanning_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.906771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/custom_fields/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/type_ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/ui_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.890771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.890771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.890771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.890771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.906771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.906771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.890771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.906771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.890771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.906771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.906771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.890771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.906771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.890771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.910771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.910771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.910771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.910771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/components/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/components/deposit.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/components/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.910771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/vocabulary_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/vocabulary_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/vocabulary_type/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.914771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/ITaxonomyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/IVocabularyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/TaxonomyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/VocabularyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/VocabularyItem.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.890771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.914771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/SidebarLink.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesForm.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSearch.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.914771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.894771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.894771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.894771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.914771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.914771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.918771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.918771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.918771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.918771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.918771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.918771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.918771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.918771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.918771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.918771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/index.js
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/VocabularyButtonSidebar.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.894771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.894771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.894771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/breadcrumb.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/grid.overrides
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/vocabulary_cf.variables
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.894771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.898771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.898771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.922771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/webpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.926771 oarepo-vocabularies-2.0.83/oarepo_vocabularies/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/views/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies/views/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:19:58.926771 oarepo-vocabularies-2.0.83/oarepo_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-05 13:19:58.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12004 2024-04-05 13:19:58.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:19:58.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-05 13:19:58.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-05 13:19:58.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 13:19:58.000000 oarepo-vocabularies-2.0.83/oarepo_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-05 13:19:58.926771 oarepo-vocabularies-2.0.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:15:30.000000 oarepo-vocabularies-2.0.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.890253 oarepo_vocabularies-2.0.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-21 10:44:05.890253 oarepo_vocabularies-2.0.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.826253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.830253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/ext_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.830253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/hacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.830253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.830253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.834253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.834253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/jsonschemas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/systemfields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.834253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.834253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/records/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.834253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/vocabulary_type/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/vocabulary_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/vocabulary_type/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/vocabulary_type/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.838253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.842253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/components/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/components/scanning_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.842253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/custom_fields/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/type_ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/ui_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.814253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.814253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.814253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.814253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.842253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.842253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.814253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.842253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.814253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.842253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.846253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.814253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.846253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.814253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.846253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.850253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.850253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.850253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/components/deposit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/components/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.854253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/vocabulary_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/vocabulary_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/vocabulary_type/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.854253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/ITaxonomyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/IVocabularyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/TaxonomyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/VocabularyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/VocabularyItem.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.814253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.858253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/SidebarLink.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesForm.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSearch.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.858253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.814253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.818253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.818253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.858253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.862253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.862253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.862253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.866253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.866253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.866253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.866253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.870253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.870253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.870253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.870253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.874253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.874253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.878253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/TreeSelectFieldModal.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/VocabularyTreeSelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.878253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.878253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.878253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.878253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/VocabularyButtonSidebar.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.882253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.818253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.882253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.882253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/tree-field.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.818253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.818253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.882253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/breadcrumb.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/grid.overrides
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.882253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/tree-field.variables
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/vocabulary_cf.variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.818253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.882253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.886253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.822253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.886253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.822253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.886253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/webpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.886253 oarepo_vocabularies-2.0.84/oarepo_vocabularies/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies/views/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:44:05.886253 oarepo_vocabularies-2.0.84/oarepo_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-21 10:44:05.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-04-21 10:44:05.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:44:05.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-21 10:44:05.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-21 10:44:05.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-21 10:44:05.000000 oarepo_vocabularies-2.0.84/oarepo_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-21 10:44:05.890253 oarepo_vocabularies-2.0.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 10:36:27.000000 oarepo_vocabularies-2.0.84/setup.py
```

### Comparing `oarepo-vocabularies-2.0.83/LICENSE` & `oarepo_vocabularies-2.0.84/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/MANIFEST.in` & `oarepo_vocabularies-2.0.84/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/PKG-INFO` & `oarepo_vocabularies-2.0.84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.83
+Version: 2.0.84
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: invenio-vocabularies
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
```

### Comparing `oarepo-vocabularies-2.0.83/README.md` & `oarepo_vocabularies-2.0.84/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/components.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/components.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/ext.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/resources/resource.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/resources/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,19 @@
             id=resource_requestctx.view_args["type"]
         ).one()
         if not authority_service:
             return "No authority getter.", 404
 
         # Get hits from authority.
         params = resource_requestctx.args
-        q, page, size = params.get("suggest"), params.get("page", 1), params.get("size", 20)
+        q, page, size = (
+            params.get("suggest"),
+            params.get("page", 1),
+            params.get("size", 20),
+        )
         results = authority_service.search(query=q, page=page, size=size)
 
         # Mark external, resolve uuid.
         ids = [item["id"] for item in results["hits"]["hits"]]
 
         internal_query = db.session.query(PersistentIdentifier.pid_value).filter(
             db.and_(
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/authorities/service.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/authorities/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/config.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,23 @@
     #         "en": "languages",
     #     },
     #     "description": {
     #         "cs": "slovnikovy typ ceskeho jazyka.",
     #         "en": "czech language vocabulary type.",
     #     },
     #     "hierarchical": False,
-    #     "props": {...},
+    #     "props": {"alpha3CodeNative": {
+    #                 "description": _("ISO 639-2 standard 3-letter language code"),
+    #                 "icon": None,
+    #                 "label": _("Alpha3 code (native)"),
+    #                 "multiple": False,
+    #                 "options": [],
+    #                 "placeholder": "eng, ces...",
+    #             }},
+    #     "custom_fields": ["names of custom fields from VOCABULARIES_CF to show in ui/serialize"],
     #     "dump_options": True
     # },
     # "organisms": {
     #    "authority": <authority service class>
     # }
 }
 
@@ -66,9 +74,7 @@
 
 DATASTREAMS_READERS = {"vocabulary": VocabularyReader}
 
 DATASTREAMS_WRITERS = {"vocabulary": VocabularyWriter}
 
 VOCABULARIES_FACET_CACHE_SIZE = 2048
 VOCABULARIES_FACET_CACHE_TTL = 60 * 24 * 24
-
-OAREPO_FINE_GRAINED_VOCABULARIES_PERMISSIONS = False
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ext.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ext.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,44 @@
+from functools import cached_property
+
+from invenio_base.utils import obj_or_import_string
+
+
 class OARepoVocabularies(object):
     """OARepo extension of Invenio-Vocabularies."""
 
     def __init__(self, app=None):
         """Extension initialization."""
         self.type_resource = None
         self.type_service = None
         if app:
             self.init_app(app)
 
     def init_app(self, app):
         """Flask application initialization."""
+        self.app = app
         self.init_config(app)
         self.init_services(app)
         self.init_resource(app)
         app.extensions["oarepo-vocabularies"] = self
 
     def init_services(self, app):
         """Initialize services."""
         self.type_service = app.config["OAREPO_VOCABULARY_TYPE_SERVICE"](
             config=app.config["OAREPO_VOCABULARY_TYPE_SERVICE_CONFIG"](),
         )
 
+    @cached_property
+    def ui_cache(self):
+        from oarepo_vocabularies.services.cache import VocabularyCache
+
+        return obj_or_import_string(
+            self.app.config.get("OAREPO_VOCABULARIES_UI_CACHE", VocabularyCache)
+        )()
+
     def init_config(self, app):
         """Initialize configuration."""
         from . import config
 
         for k in dir(config):
             if k.startswith("OAREPO_VOCABULARIES_"):
                 app.config.setdefault(k, getattr(config, k))
@@ -57,7 +71,16 @@
 
     def init_resource(self, app):
         """Initialize resources."""
         self.type_resource = app.config["OAREPO_VOCABULARY_TYPE_RESOURCE"](
             config=app.config["OAREPO_VOCABULARY_TYPE_RESOURCE_CONFIG"](),
             service=self.type_service,
         )
+
+    def get_config(self, vocabulary_name):
+        if isinstance(vocabulary_name, dict):
+            vocabulary_name = vocabulary_name.get("id")
+
+        vocabulary_type_metadata = self.app.config.get(
+            "INVENIO_VOCABULARY_TYPE_METADATA", {}
+        )
+        return vocabulary_type_metadata.get(vocabulary_name, {})
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/fixtures.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/fixtures.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/hacks.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/hacks.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/models/ui.json` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/models/ui.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/api.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/records/systemfields.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/records/systemfields.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/config.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/records/ui.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/ui.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/vocabulary_type/config.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/vocabulary_type/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/resources/vocabulary_type/resource.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/resources/vocabulary_type/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/components/hierarchy.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/components/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/config.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/custom_fields/hierarchy.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/custom_fields/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/permissions.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/schema.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/service.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -136,7 +136,15 @@
             record=record,
         )
         return super().delete(identity, id_, revision_id=revision_id, uow=uow, **kwargs)
 
     def get_vocabulary_permission_name(self, operation, vocabulary_type):
         vocabulary_type = vocabulary_type.replace("-", "_")
         return f"{operation}_{vocabulary_type}"
+
+    def search_many(self, identity, params):
+        # we are skipping Invenio vocabularies service here and calling
+        # explicitly its parent class. The reason is that invenio vocabs
+        # always filter the search by a single vocabulary type. The search_many
+        # use case is an optimization where we want to fetch multiple items
+        # from multiple vocabulary types in a single query.
+        return super(InvenioVocabulariesService, self).search(identity, params)
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/services/ui_schema.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/ui_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,10 +54,7 @@
         super().__init__(*args, **kwargs)
 
     created = LocalizedDateTime(dump_only=True)
     updated = LocalizedDateTime(dump_only=True)
     links = ma.fields.Raw(dump_only=True)
     title = VocabularyI18nStrUIField()
     type = ma.fields.Raw(dump_only=True)
-
-    def dump(self, *args, **kwargs):
-        return super().dump(*args, **kwargs)
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/translations/messages.pot` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/config.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/ext.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/components/deposit.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/services/cache.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,191 +1,209 @@
-import inspect
-import json
+import contextlib
+from collections import defaultdict
+from datetime import datetime, timezone
+from typing import Any, Dict, List
 
 import marshmallow
-from flask import current_app
-from invenio_records import Record
+from cachetools import TTLCache
+from invenio_access.permissions import system_identity
 from invenio_vocabularies.proxies import current_service as vocabulary_service
 from oarepo_runtime.i18n import get_locale
-from oarepo_ui.resources.components import UIResourceComponent
 
-from oarepo_vocabularies.records.api import find_vocabulary_relations
 from oarepo_vocabularies.services.ui_schema import VocabularyI18nStrUIField
 
-try:
-    pass
-except ImportError:
-    pass
+
+class VocabularyCacheItem:
+    last_modified: datetime
+    items: Dict[str, Any]
+
+    def __init__(self):
+        self.last_modified = datetime.fromtimestamp(0, timezone.utc)
+        self.items = {}
 
 
 class DepositI18nHierarchySchema(marshmallow.Schema):
     title = marshmallow.fields.List(VocabularyI18nStrUIField())
     ancestors = marshmallow.fields.List(marshmallow.fields.String())
 
 
 class VocabularyPrefetchSchema(marshmallow.Schema):
     title = VocabularyI18nStrUIField(data_key="text")
     hierarchy = marshmallow.fields.Nested(
-        DepositI18nHierarchySchema, data_key="hierarchy"
+        DepositI18nHierarchySchema(), data_key="hierarchy"
     )
-    props = marshmallow.fields.Dict(keys=marshmallow.fields.String(), values=marshmallow.fields.String())
-
+    props = marshmallow.fields.Dict(
+        keys=marshmallow.fields.String(), values=marshmallow.fields.String()
+    )
+    tags = marshmallow.fields.List(marshmallow.fields.String())
 
-class DepositVocabularyOptionsComponent(UIResourceComponent):
-    """
-    This component is used in deposit form of normal records. For small vocabularies,
-    it provides their values so that they might be displayed in, for example, a combo.
-    """
 
-    always_included_vocabularies = []
+class VocabularyCache:
+    cache: Dict[str, Dict[str, VocabularyCacheItem]]
+    """Language => vocabulary type => last modified + items"""
+    lru_terms_cache = TTLCache(maxsize=10000, ttl=3600)
 
-    def form_config(self, *, form_config, api_record, view_args, identity, **kwargs):
-        """
-        Adds vocabularies to the form config as in:
-        ```
-        "vocabularies": {
-            "languages": {
-              "definition": {...} # from INVENIO_VOCABULARY_TYPE_METADATA
-              "all": [{"value": "...", "text": "..."}],
-              "featured": [{"value": "...", "text": "..."}]
-            },
-            "bigVocabulary: {
-                "definition": {...} # from INVENIO_VOCABULARY_TYPE_METADATA
-                "url": "..."
-            },
-          }
-        ```
+    count_from_cache = 0
+    count_prefetched = 0
+    count_fetched = 0
 
-        The vocabularies which should be handled this way are configured
-        inside invenio.cfg:
+    def __init__(self):
+        self.cache = {}
 
-        ```
-        INVENIO_VOCABULARY_TYPE_METADATA = {
-            "languages": {
-                "dump_options": True,
-                # more configuration here
-            }
-        ```
-        """
-        if not isinstance(api_record, Record):
-            record_cls = self.resource.api_service.config.record_cls  # noqa
-            api_record = record_cls({})
+    @contextlib.contextmanager
+    def language_cache(self, language):
+        cached_language = {**self.cache.get(language, {})}
 
-        form_config.setdefault("vocabularies", {})
+        yield cached_language
+        self.cache[language] = cached_language
 
-        if current_app.config.get("VOCABULARIES_LANGUAGES_DISABLED"):
+    def update(self, vocabulary_types: List[str]):
+        if not vocabulary_types:
             return
 
-        vocabulary_config = current_app.config.get(
-            "INVENIO_VOCABULARY_TYPE_METADATA", {}
-        )
+        locale = get_locale()
 
-        used_vocabularies = self._get_used_vocabularies(api_record)
+        language = locale.language
 
-        (
-            vocabularies_to_prefetch,
-            form_config_vocabularies,
-        ) = self.create_form_config_vocabularies(
-            vocabulary_config, used_vocabularies=used_vocabularies
-        )
+        with self.language_cache(language) as cached_language:
 
-        form_config["vocabularies"] = form_config_vocabularies
-        self._prefetch_vocabularies_to_form_config(
-            form_config_vocabularies, vocabularies_to_prefetch, identity
+            if not self._check_modified(cached_language, vocabulary_types):
+                return
+
+            by_vocabulary_type = {}
+            max_modified = {}
+            for item, dumped_item in self._serialize_items(
+                locale, self._prefetch_vocabularies(vocabulary_types)
+            ):
+                by_vocabulary_type.setdefault(item["type"], {})[
+                    item["id"]
+                ] = dumped_item
+                if item["type"] not in max_modified:
+                    max_modified[item["type"]] = datetime.fromtimestamp(0, timezone.utc)
+
+                modified = datetime.fromisoformat(item["updated"])
+                if max_modified[item["type"]] < modified:
+                    max_modified[item["type"]] = modified
+
+            if not by_vocabulary_type:
+                return
+
+            for vocab_type, items in by_vocabulary_type.items():
+                if vocab_type not in cached_language:
+                    cached_language[vocab_type] = VocabularyCacheItem()
+                cached_language[vocab_type].items = items
+                self.count_prefetched += len(items)
+                cached_language[vocab_type].last_modified = max_modified[vocab_type]
+
+    def clear(self):
+        self.cache = {}
+        self.lru_terms_cache = TTLCache(maxsize=10000, ttl=3600)
+        self.count_from_cache = 0
+        self.count_fetched = 0
+        self.count_prefetched = 0
+
+    def _prefetch_vocabularies(self, vocabulary_types: List[str]):
+        yield from vocabulary_service.scan(
+            system_identity,
+            params={
+                "type": vocabulary_types,
+                "sort": "title",
+                "size": 1000,
+            },
+            preserve_order=True,
         )
 
-        for vocabularies in form_config["vocabularies"].values():
-            if "all" in vocabularies:
-                for voc in vocabularies["all"]:
-                    for _voc in vocabularies["all"]:
-                        if voc["value"] in _voc["hierarchy"]["ancestors"]:
-                            voc["element_type"] = "parent"
-                            break
-                    if "element_type" not in voc:
-                        voc["element_type"] = "leaf"
-
-    def _get_used_vocabularies(self, api_record):
-        used_vocabularies = [
-            vocab_field.vocabulary_type
-            for vocab_field in find_vocabulary_relations(api_record)
-        ]
-        for v in self.always_included_vocabularies:
-            if v not in used_vocabularies:
-                used_vocabularies.append(v)
-        return used_vocabularies
-
-    def _prefetch_vocabularies_to_form_config(
-        self, form_config_vocabularies, vocabularies_to_prefetch, identity
-    ):
-        schema = VocabularyPrefetchSchema(context={"locale": get_locale()})
-        for prefetched_item in self.prefetch_vocabulary_items(
-            identity, vocabularies_to_prefetch
-        ):
-            by_type = form_config_vocabularies[prefetched_item["type"]]
-            returned_item = {
-                "value": prefetched_item["id"],
-                **schema.dump(prefetched_item),
-            }
-            by_type["all"].append(returned_item)
-            if "featured" in prefetched_item.get("tags", []):
-                by_type["featured"].append(returned_item)
-
-    @staticmethod
-    def prefetch_vocabulary_items(identity, vocabularies_to_prefetch):
-        if vocabularies_to_prefetch:
-            yield from vocabulary_service.scan(
-                identity,
-                params={
-                    "type": vocabularies_to_prefetch,
-                    "sort": "title",
-                    "source": [
-                        "title",
-                        "hierarchy.title",
-                        "hierarchy.ancestors",
-                        "uuid",
-                        "version_id",
-                        "created",
-                        "updated",
-                        "pid",
-                        "type",
-                        "id",
-                        "tags",
-                        "props.*"
-                    ],
-                    "size": 1000,
-                },
-                # this needs the ScanningOrderComponent to be installed, otherwise does not sort
-                preserve_order=True,
-            )
-
-    @staticmethod
-    def create_form_config_vocabularies(
-        vocabulary_config,
-        used_vocabularies,
-    ):
-        form_config_vocabularies = {}
-        vocabularies_to_prefetch = []
-        for vocabulary_type in used_vocabularies:
-            vocabulary_definition = vocabulary_config.get(vocabulary_type, {})
-            form_config_vocabularies[vocabulary_type] = {
-                "definition": json.loads(
-                    json.dumps(vocabulary_definition, default=json_default)
+    def _check_modified(self, cached_language, vocabulary_types: List[str]):
+        params = {
+            "size": 1,
+            "updated_after": {
+                vt: (
+                    cached_language[vt].last_modified.isoformat()
+                    if vt in cached_language
+                    else None
                 )
-            }
-            if vocabulary_definition.get("dump_options"):
-                vocabularies_to_prefetch.append(vocabulary_type)
-                form_config_vocabularies[vocabulary_type]["all"] = []
-                form_config_vocabularies[vocabulary_type]["featured"] = []
-            else:
-                # TODO: use vocabulary service config and prefix???
-                form_config_vocabularies[vocabulary_type][
-                    "url"
-                ] = f"/api/vocabularies/{vocabulary_type}"
-        return vocabularies_to_prefetch, form_config_vocabularies
-
-
-def json_default(x):
-    if hasattr(x, "name"):
-        return x.name
-    if inspect.isclass(x):
-        return x.__name__
-    return type(x).__name__
+                for vt in vocabulary_types
+            },
+        }
+
+        result = vocabulary_service.search_many(
+            system_identity,
+            params=params,
+        )
+        return result.total > 0
+
+    def _serialize_items(self, locale, items):
+        schema = VocabularyPrefetchSchema(context={"locale": locale})
+
+        for item in items:
+            dumped_item = schema.dump(item)
+            yield item, dumped_item
+
+    def get(self, vocabulary_types: List[str]):
+        self.update(vocabulary_types)
+        language = get_locale().language
+        ret = {}
+        for vocabulary_type in vocabulary_types:
+            ret[vocabulary_type] = self.cache[language][vocabulary_type].items
+            self.count_from_cache += len(ret[vocabulary_type])
+
+        return ret
+
+    def resolve(self, ids):
+        """
+        Resolves vocabulary ids to their localized records.
+
+        :param ids: list of vocabulary ids in the form of tuple (type, id)
+        """
+        locale = get_locale()
+        language = locale.language
+
+        # check if these are in the lru cache
+        cached, uncached, uncached_small = self._split_cached_uncached(language, ids)
+
+        self.count_from_cache += len(cached)
+        self.count_prefetched += len(uncached_small)
+        self.count_fetched += len(uncached)
+
+        if uncached_small:
+            self._fill_from_small_vocabularies_cache(language, uncached_small, cached)
+
+        if uncached:
+            for item, serialized_item in self._serialize_items(
+                locale,
+                vocabulary_service.search_many(
+                    system_identity, params={"ids": uncached}
+                ),
+            ):
+                typed_id = (item["type"], item["id"])
+                cached[typed_id] = serialized_item
+                self.lru_terms_cache[(language, typed_id)] = serialized_item
+
+        return cached
+
+    def _fill_from_small_vocabularies_cache(self, language, uncached_small, cached):
+        # TODO: is there a performance improvement for uncached_small or should we treat all as uncached?
+        self.update(list(uncached_small.keys()))
+        cached_types = self.get(list(uncached_small.keys()))
+        for vocab_type, items in uncached_small.items():
+            for it in items:
+                cached[(vocab_type, it)] = cached_types[vocab_type][it]
+                self.lru_terms_cache[(language, (vocab_type, it))] = cached_types[
+                    vocab_type
+                ][it]
+
+    def _split_cached_uncached(self, language, ids):
+        cached = {}
+        uncached = []
+        uncached_small = defaultdict(list)
+        with self.language_cache(language) as cached_language:
+
+            for vocab_id in ids:
+                term = self.lru_terms_cache.get((language, vocab_id))
+                if term:
+                    cached[vocab_id] = term
+                else:
+                    if vocab_id[0] in cached_language:
+                        uncached_small[vocab_id[0]].append(vocab_id[1])
+                    else:
+                        uncached.append(vocab_id)
+        return cached, uncached, uncached_small
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/config.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/resource.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/vocabulary_type/config.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/vocabulary_type/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/VocabularyItem.jinja` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/VocabularyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
             Theme
 *******************************/
 
 /*
   The type is the type of the component as defined in semantic-ui - element, collection, view, module
   For simple component, 'element' is the correct type
 */
-@type    : 'collections';
+@type    : 'collection';
 
 /*
   This is the name of the component - though not required, keep it the same as the filename
 */
 @element : 'dl_table';
 
 /*******************************
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
             Theme
 *******************************/
 
 /*
   The type is the type of the component as defined in semantic-ui - element, collection, view, module
   For simple component, 'element' is the correct type
 */
-@type: "modules";
+@type: "module";
 
 /*
   This is the name of the component - though not required, keep it the same as the filename
 */
 @element: "vocabulary_cf";
 
 @import (multiple) "../../theme.config";
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/theme/webpack.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/theme/webpack.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/utils.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/ui/views.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/ui/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/views/api.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/views/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,11 +10,10 @@
     app = state.app
     ext = app.extensions["oarepo-vocabularies"]
 
     # Register service.
     sregistry = app.extensions["invenio-records-resources"].registry
     sregistry.register(ext.type_service, service_id=ext.type_service.config.service_id)
 
-    if app.config.get("OAREPO_FINE_GRAINED_VOCABULARIES_PERMISSIONS", False):
-        from oarepo_vocabularies.hacks import patch_invenio_vocabulary_service
+    from oarepo_vocabularies.hacks import patch_invenio_vocabulary_service
 
-        patch_invenio_vocabulary_service(app)
+    patch_invenio_vocabulary_service(app)
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies/views/app.py` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies/views/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,11 +12,10 @@
     app = state.app
     ext = app.extensions["oarepo-vocabularies"]
 
     # Register service.
     sregistry = app.extensions["invenio-records-resources"].registry
     sregistry.register(ext.type_service, service_id=ext.type_service.config.service_id)
 
-    if app.config.get("OAREPO_FINE_GRAINED_VOCABULARIES_PERMISSIONS", False):
-        from oarepo_vocabularies.hacks import patch_invenio_vocabulary_service
+    from oarepo_vocabularies.hacks import patch_invenio_vocabulary_service
 
-        patch_invenio_vocabulary_service(app)
+    patch_invenio_vocabulary_service(app)
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies.egg-info/PKG-INFO` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.83
+Version: 2.0.84
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: invenio-vocabularies
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies.egg-info/SOURCES.txt` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 oarepo_vocabularies/resources/ui.py
 oarepo_vocabularies/resources/records/__init__.py
 oarepo_vocabularies/resources/records/ui.py
 oarepo_vocabularies/resources/vocabulary_type/__init__.py
 oarepo_vocabularies/resources/vocabulary_type/config.py
 oarepo_vocabularies/resources/vocabulary_type/resource.py
 oarepo_vocabularies/services/__init__.py
+oarepo_vocabularies/services/cache.py
 oarepo_vocabularies/services/config.py
 oarepo_vocabularies/services/facets.py
 oarepo_vocabularies/services/permissions.py
 oarepo_vocabularies/services/schema.py
 oarepo_vocabularies/services/search.py
 oarepo_vocabularies/services/service.py
 oarepo_vocabularies/services/type_ui_schema.py
@@ -137,29 +138,34 @@
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/index.js
+oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/TreeSelectFieldModal.jsx
+oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/VocabularyTreeSelectField.jsx
+oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/VocabularyButtonSidebar.jsx
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
 oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
 oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
+oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/tree-field.less
 oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less
 oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/breadcrumb.overrides
 oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/grid.overrides
+oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/tree-field.variables
 oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/vocabulary_cf.variables
 oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json
 oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json
 oarepo_vocabularies/views/__init__.py
 oarepo_vocabularies/views/api.py
```

### Comparing `oarepo-vocabularies-2.0.83/oarepo_vocabularies.egg-info/entry_points.txt` & `oarepo_vocabularies-2.0.84/oarepo_vocabularies.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.83/setup.cfg` & `oarepo_vocabularies-2.0.84/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-vocabularies
-version = 2.0.83
+version = 2.0.84
 description = Support for custom fields and hierarchy on Invenio vocabularies
 authors = Mirek Simek <miroslav.simek@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

