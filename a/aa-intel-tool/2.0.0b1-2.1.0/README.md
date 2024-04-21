# Comparing `tmp/aa_intel_tool-2.0.0b1.tar.gz` & `tmp/aa_intel_tool-2.1.0.tar.gz`

## Comparing `aa_intel_tool-2.0.0b1.tar` & `aa_intel_tool-2.1.0.tar`

### file list

```diff
@@ -1,125 +1,130 @@
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/__init__.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/admin.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/app_settings.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/apps.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/auth_hooks.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/constants.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/exceptions.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/form.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/models.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tasks.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/urls.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/helper/data_structure.py
--rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/helper/eve_character.py
--rw-r--r--   0        0        0    15493 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/django.pot
--rw-r--r--   0        0        0     8874 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16661 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15781 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15582 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15536 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18878 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11779 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    21722 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15786 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15721 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/management/commands/aa_intel_tool_load_eve_types.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/migrations/0001_initial.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/migrations/0002_alter_scan_raw_data.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/migrations/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/parser/__init__.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/parser/general.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/parser/helper/db.py
--rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/parser/module/chatlist.py
--rw-r--r--   0        0        0    11827 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/parser/module/dscan.py
--rw-r--r--   0        0        0     6371 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/parser/module/fleetcomp.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/scripts/drop_tables.sql
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.css
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css.map
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.js
--rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js.map
--rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.js
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js.map
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.js
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js.map
--rw-r--r--   0        0        0    21717 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.js
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js
--rw-r--r--   0        0        0     8511 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js.map
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.js
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js.map
--rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.js
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js.map
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.js
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js.map
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.js
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.min.js
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.min.js.map
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/base.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-chatscan-js.html
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-css.html
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-dscan-js.html
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-fleetcomp-js.html
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js.html
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/index/form.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/buttons.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/evetime.html
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid.html
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown.html
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/system-information.html
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details.html
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/views/index.html
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templatetags/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/templatetags/aa_intel_tool.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/__init__.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_access.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_admin.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_app_settings.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_auth_hooks.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_helper_data_structures.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_models.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_parser.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_parser_helper_db.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_templatetags.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/utils.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test-data/chatscan-faulty.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test-data/chatscan.txt
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test-data/dscan-german-client.txt
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test-data/dscan-russian-client.txt
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test-data/dscan.txt
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test-data/fleetcomp.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/views/__init__.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/views/ajax.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/aa_intel_tool/views/general.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/.gitignore
--rw-r--r--   0        0        0    35151 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/LICENSE
--rw-r--r--   0        0        0    12841 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/README.md
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0    55145 2020-02-02 00:00:00.000000 aa_intel_tool-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/__init__.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/admin.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/app_settings.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/apps.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/auth_hooks.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/constants.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/exceptions.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/form.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/models.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tasks.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/urls.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/helper/data_structure.py
+-rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/helper/eve_character.py
+-rw-r--r--   0        0        0    15632 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/django.pot
+-rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18871 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18980 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15721 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19059 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    15624 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15951 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11779 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    21861 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    15702 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15925 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/management/commands/aa_intel_tool_load_eve_types.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/migrations/0001_initial.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/migrations/0002_alter_scan_raw_data.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/migrations/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/__init__.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/general.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/helper/db.py
+-rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/module/chatlist.py
+-rw-r--r--   0        0        0    13148 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/module/dscan.py
+-rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/module/fleetcomp.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/scripts/drop_tables.sql
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.css
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css.map
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.js
+-rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js.map
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.js
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js.map
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.js
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js.map
+-rw-r--r--   0        0        0    23339 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.js
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js.map
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.js
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js.map
+-rw-r--r--   0        0        0     8525 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.js
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js.map
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.js
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js.map
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.js
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.min.js
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.min.js.map
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/base.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-chatscan-js.html
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-css.html
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-dscan-js.html
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-fleetcomp-js.html
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js.html
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/index/form.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/buttons.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/evetime.html
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid.html
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown.html
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/system-information.html
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details.html
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/index.html
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templatetags/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templatetags/aa_intel_tool.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/__init__.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_access.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_admin.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_app_settings.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_helper_data_structures.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_models.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_parser.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_parser_helper_db.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/utils.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/chatscan-faulty.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/chatscan.txt
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan-german-client.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan-russian-client.txt
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan.txt
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/fleetcomp.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/views/__init__.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/views/ajax.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/views/general.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/.gitignore
+-rw-r--r--   0        0        0    35151 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/LICENSE
+-rw-r--r--   0        0        0    12916 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/README.md
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    55219 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/PKG-INFO
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/admin.py` & `aa_intel_tool-2.1.0/aa_intel_tool/admin.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/app_settings.py` & `aa_intel_tool-2.1.0/aa_intel_tool/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/auth_hooks.py` & `aa_intel_tool-2.1.0/aa_intel_tool/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/constants.py` & `aa_intel_tool-2.1.0/aa_intel_tool/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 
 # Localised units
 distance_units_on_grid: str = """
     km|m    # Client in: English, German, Chinese, French, Japanese, Korean, Spanish
     |км|м   # Russian
 """
 distance_units_off_grid: str = """
-    AU|     # Client in: English, Chinese, Japanese, Korean, Spanish
-    UA|     # Client in: French
-    AE|     # German
-    а.е.    # Russian
+    AU      # Client in: English, Chinese, Japanese, Korean, Spanish
+    |UA     # Client in: French
+    |AE     # German
+    |а.е.   # Russian
 """
 
 distance_units = f"{distance_units_on_grid}|{distance_units_off_grid}"
 
 
 # Pre-compiled regex patterns used throughout the app
 REGEX_PATTERN = {
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/exceptions.py` & `aa_intel_tool-2.1.0/aa_intel_tool/exceptions.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/models.py` & `aa_intel_tool-2.1.0/aa_intel_tool/models.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tasks.py` & `aa_intel_tool-2.1.0/aa_intel_tool/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/urls.py` & `aa_intel_tool-2.1.0/aa_intel_tool/urls.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/helper/eve_character.py` & `aa_intel_tool-2.1.0/aa_intel_tool/helper/eve_character.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/django.pot` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/nl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-04 17:44+0200\n"
+"POT-Creation-Date: 2024-04-20 22:33+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=INTEGER; plural=EXPRESSION;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: aa_intel_tool/__init__.py:12
+#: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:10
+#: aa_intel_tool/templates/aa_intel_tool/base.html:10
+#: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html:5
 msgid "Intel Parser"
 msgstr ""
 
 #: aa_intel_tool/admin.py:79 aa_intel_tool/models.py:46
@@ -42,24 +42,24 @@
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_intel_tool/apps.py:21
 #, python-brace-format
 msgid "Intel Parser v{__version__}"
 msgstr ""
 
-#: aa_intel_tool/constants.py:71 aa_intel_tool/models.py:24
+#: aa_intel_tool/constants.py:58 aa_intel_tool/models.py:24
 msgid "Chat list"
 msgstr ""
 
-#: aa_intel_tool/constants.py:77 aa_intel_tool/models.py:22
+#: aa_intel_tool/constants.py:64 aa_intel_tool/models.py:22
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:28
 msgid "D-Scan"
 msgstr ""
 
-#: aa_intel_tool/constants.py:83 aa_intel_tool/models.py:23
+#: aa_intel_tool/constants.py:70 aa_intel_tool/models.py:23
 #: aa_intel_tool/models.py:123
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:33
 msgid "Fleet composition"
 msgstr ""
 
 #: aa_intel_tool/exceptions.py:34
 #, python-brace-format
@@ -161,136 +161,136 @@
 "No suitable parser found. Input is not a supported intel type or malformed …"
 msgstr ""
 
 #: aa_intel_tool/parser/general.py:80
 msgid "No data to parse …"
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:66
+#: aa_intel_tool/parser/module/chatlist.py:68
 msgid "Something went wrong while fetching the character information from ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:77
+#: aa_intel_tool/parser/module/chatlist.py:79
 msgid "Character unknown to ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:274
+#: aa_intel_tool/parser/module/chatlist.py:281
 msgid "The chat list module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:292
+#: aa_intel_tool/parser/module/chatlist.py:302
 #, python-brace-format
 msgid ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_intel_tool/parser/module/dscan.py:322
+#: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/fleetcomp.py:103
+#: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:8
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
 msgid "Permalink successfully copied"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:10
 msgid ""
 "Something went wrong. Nothing copied. Maybe your browser does not support "
 "this function."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:14
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:3
 msgid "Unaffiliated / No Alliance"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:16
 msgid "NPC Corp"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:19
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
 msgctxt "Decimal separator"
 msgid "."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
 msgctxt "Thousands separator"
 msgid ","
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
 msgid "No data available in this table"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
 msgctxt "Keep _END_ as it is. It will be replaced by a number."
 msgid "Showing _END_ entries"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
 msgctxt "Keep _MAX_ as it is. It will be replaced by a number."
 msgid "(filtered from _MAX_ total entries)"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:25
 msgid "No records available"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:26
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
 msgctxt "Keep _MENU_ as it is. It will be replaced by an HTML construct."
 msgid "Show _MENU_"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
 msgid "Loading …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
 msgid "Processing …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:30
 msgid "Nothing found, sorry …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:31
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:32
 msgid "Search …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:33
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
 msgid "First"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
 msgid "Last"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
 msgid "Next"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:37
 msgid "Previous"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:39
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
 msgid ": activate to sort column ascending"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:41
 msgid ": activate to sort column descending"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
@@ -318,15 +318,21 @@
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:21
 #, python-format
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:50
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
+msgid ""
+"Please keep in mind, parsing large amounts of data can take some time. Be "
+"patient, CCP's API is not the fastest to answer …"
+msgstr ""
+
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
 msgid "Working on it, please be patient …"
 msgstr ""
 
@@ -368,25 +374,25 @@
 msgid "Count"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:25
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:32
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:37
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:30
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:29
 msgid "Loading data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:31
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:38
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:43
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:35
 msgid "No data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:9
 msgid "Corporations breakdown"
 msgstr ""
@@ -446,14 +452,18 @@
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:19
 msgid "Ship class"
 msgstr ""
 
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
+msgid "Total mass (in kg):"
+msgstr ""
+
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr ""
@@ -482,24 +492,18 @@
 msgid "System"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:14
-msgid ""
-"Please keep in mind, parsing large amounts of data can take some time. Be "
-"patient, CCP's API is not the fastest to answer …"
-msgstr ""
-
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
 msgstr ""
 
 #: aa_intel_tool/views/general.py:60
 msgid "(System Error) Something unexpected happened."
 msgstr ""
 
-#: aa_intel_tool/views/general.py:99 aa_intel_tool/views/general.py:129
+#: aa_intel_tool/views/general.py:101 aa_intel_tool/views/general.py:131
 msgid "The scan you were looking for could not be found."
 msgstr ""
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/de/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/de/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-intel-tool/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.4.3\n"
 
 msgid "(System Error) Something unexpected happened."
 msgstr "(Systemfehler) Es ist etwas Unerwartetes passiert."
 
 msgid ": activate to sort column ascending"
 msgstr ": aktivieren, um die Spalte aufsteigend zu sortieren"
 
@@ -348,14 +348,17 @@
 msgid "The scan you were looking for could not be found."
 msgstr "Der gesuchte Scan konnte nicht gefunden werden."
 
 msgctxt "Thousands separator"
 msgid ","
 msgstr "."
 
+msgid "Total mass (in kg):"
+msgstr "Gesamtmasse (in kg):"
+
 msgid "Type"
 msgstr "Typ"
 
 msgid "Unaffiliated / No Alliance"
 msgstr "Unabhängig / Keine Allianz"
 
 msgid "Upwell structures"
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/de/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Peter Pfeufer <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-04 17:44+0200\n"
+"POT-Creation-Date: 2024-04-20 22:33+0200\n"
 "PO-Revision-Date: 2023-10-04 15:46+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: German <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-intel-tool/de/>\n"
+"Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-intel-tool/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.0.2\n"
 
-#: aa_intel_tool/__init__.py:12
+#: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:10
+#: aa_intel_tool/templates/aa_intel_tool/base.html:10
+#: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html:5
 msgid "Intel Parser"
 msgstr "Intel Parser"
 
 #: aa_intel_tool/admin.py:79 aa_intel_tool/models.py:46
@@ -42,24 +42,24 @@
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_intel_tool/apps.py:21
 #, python-brace-format
 msgid "Intel Parser v{__version__}"
 msgstr "Intel Parser v{__version__}"
 
-#: aa_intel_tool/constants.py:71 aa_intel_tool/models.py:24
+#: aa_intel_tool/constants.py:58 aa_intel_tool/models.py:24
 msgid "Chat list"
 msgstr "Chatliste"
 
-#: aa_intel_tool/constants.py:77 aa_intel_tool/models.py:22
+#: aa_intel_tool/constants.py:64 aa_intel_tool/models.py:22
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:28
 msgid "D-Scan"
 msgstr "D-Scan"
 
-#: aa_intel_tool/constants.py:83 aa_intel_tool/models.py:23
+#: aa_intel_tool/constants.py:70 aa_intel_tool/models.py:23
 #: aa_intel_tool/models.py:123
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:33
 msgid "Fleet composition"
 msgstr "Flottenzusammensetzung"
 
 #: aa_intel_tool/exceptions.py:34
 #, python-brace-format
@@ -163,143 +163,144 @@
 "Kein passender Parser gefunden. Die Eingabe ist kein unterstützter Inteltyp "
 "oder fehlerhaft …"
 
 #: aa_intel_tool/parser/general.py:80
 msgid "No data to parse …"
 msgstr "Keine Daten zum Parsen …"
 
-#: aa_intel_tool/parser/module/chatlist.py:66
+#: aa_intel_tool/parser/module/chatlist.py:68
 msgid "Something went wrong while fetching the character information from ESI."
 msgstr ""
 "Beim Abrufen der Charakterinformationen von ESI ist ein Fehler aufgetreten."
 
-#: aa_intel_tool/parser/module/chatlist.py:77
+#: aa_intel_tool/parser/module/chatlist.py:79
 msgid "Character unknown to ESI."
 msgstr "Charakter ist in ESI nicht bekannt."
 
-#: aa_intel_tool/parser/module/chatlist.py:274
+#: aa_intel_tool/parser/module/chatlist.py:281
 msgid "The chat list module is currently disabled."
 msgstr "Das Chatlistenmodul ist derzeit deaktiviert."
 
-#: aa_intel_tool/parser/module/chatlist.py:292
+#: aa_intel_tool/parser/module/chatlist.py:302
 #, python-brace-format
 msgid ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
 msgstr[0] ""
 "Chatscans sind derzeit auf maximal {max_allowed_pilots} Pilot pro Scan "
 "beschränkt. Deine Pilotenliste überschreitet diese Grenze."
 msgstr[1] ""
 "Chatscans sind derzeit auf maximal {max_allowed_pilots} Piloten pro Scan "
 "beschränkt. Deine Pilotenliste überschreitet diese Grenze."
 
-#: aa_intel_tool/parser/module/dscan.py:322
+#: aa_intel_tool/parser/module/dscan.py:350
+#: aa_intel_tool/parser/module/dscan.py:338
 msgid "The D-Scan module is currently disabled."
 msgstr "Das D-Scan-Modul ist derzeit deaktiviert."
 
-#: aa_intel_tool/parser/module/fleetcomp.py:103
+#: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
 msgstr "Das Flottenzusammensetzungsmodul ist derzeit deaktiviert."
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:8
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
 msgid "Permalink successfully copied"
 msgstr "Permalink erfolgreich kopiert"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:10
 msgid ""
 "Something went wrong. Nothing copied. Maybe your browser does not support "
 "this function."
 msgstr ""
 "Etwas ist schief gelaufen. Nichts kopiert. Möglicherweise unterstützt Dein "
 "Browser diese Funktion nicht."
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:14
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:3
 msgid "Unaffiliated / No Alliance"
 msgstr "Unabhängig / Keine Allianz"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:16
 msgid "NPC Corp"
 msgstr "NPC Corp"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:19
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
 msgctxt "Decimal separator"
 msgid "."
 msgstr ","
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
 msgctxt "Thousands separator"
 msgid ","
 msgstr "."
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
 msgid "No data available in this table"
 msgstr "In dieser Tabelle sind keine Daten verfügbar"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
 msgctxt "Keep _END_ as it is. It will be replaced by a number."
 msgid "Showing _END_ entries"
 msgstr "Zeige _END_ Einträge"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
 msgctxt "Keep _MAX_ as it is. It will be replaced by a number."
 msgid "(filtered from _MAX_ total entries)"
 msgstr "(gefiltert von _MAX_ Einträgen)"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:25
 msgid "No records available"
 msgstr "Keine Datensätze vorhanden"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:26
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
 msgctxt "Keep _MENU_ as it is. It will be replaced by an HTML construct."
 msgid "Show _MENU_"
 msgstr "Zeige _MENU_"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
 msgid "Loading …"
 msgstr "Lade …"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
 msgid "Processing …"
 msgstr "Verarbeite …"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:30
 msgid "Nothing found, sorry …"
 msgstr "Nichts gefunden, tut mir leid …"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:31
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:32
 msgid "Search …"
 msgstr "Suche …"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:33
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
 msgid "First"
 msgstr "Erster"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
 msgid "Last"
 msgstr "Letzter"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
 msgid "Next"
 msgstr "Nächster"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:37
 msgid "Previous"
 msgstr "Vorheriger"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:39
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
 msgid ": activate to sort column ascending"
 msgstr ": aktivieren, um die Spalte aufsteigend zu sortieren"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:41
 msgid ": activate to sort column descending"
 msgstr ": aktivieren, um die Spalte absteigend zu sortieren"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
@@ -329,15 +330,24 @@
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:21
 #, python-format
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] "Begrenzt auf maximal %(max_pilots)s Pilot pro Scan."
 msgstr[1] "Begrenzt auf maximal %(max_pilots)s Piloten pro Scan."
 
-#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:50
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
+msgid ""
+"Please keep in mind, parsing large amounts of data can take some time. Be "
+"patient, CCP's API is not the fastest to answer …"
+msgstr ""
+"Bitte beachte, dass das Verarbeiten großer Datenmengen einige Zeit in "
+"Anspruch nehmen kann. Sei geduldig, die API von CCP ist nicht die Schnellste "
+"…"
+
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
 msgstr "Absenden"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
 msgid "Working on it, please be patient …"
 msgstr "Bei der Arbeit, bitte hab etwas Geduld …"
 
@@ -381,25 +391,25 @@
 msgid "Count"
 msgstr "Anzahl"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:25
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:32
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:37
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:30
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:29
 msgid "Loading data …"
 msgstr "Lade Daten …"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:31
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:38
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:43
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:35
 msgid "No data …"
 msgstr "Keine Daten …"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:9
 msgid "Corporations breakdown"
 msgstr "Aufschlüsselung der Corporationen"
@@ -459,14 +469,18 @@
 msgstr "Off Grid"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:19
 msgid "Ship class"
 msgstr "Schiffsklasse"
 
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
+msgid "Total mass (in kg):"
+msgstr "Gesamtmasse (in kg):"
+
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
 msgstr "Schiffstyp"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr "Keine Daten."
@@ -495,27 +509,18 @@
 msgid "System"
 msgstr "System"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr "Teilnahmedetails"
 
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:14
-msgid ""
-"Please keep in mind, parsing large amounts of data can take some time. Be "
-"patient, CCP's API is not the fastest to answer …"
-msgstr ""
-"Bitte beachte, dass das Verarbeiten großer Datenmengen einige Zeit in "
-"Anspruch nehmen kann. Sei geduldig, die API von CCP ist nicht die Schnellste "
-"…"
-
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
 msgstr "Die bereitgestellten Daten konnten nicht analysiert werden."
 
 #: aa_intel_tool/views/general.py:60
 msgid "(System Error) Something unexpected happened."
 msgstr "(Systemfehler) Es ist etwas Unerwartetes passiert."
 
-#: aa_intel_tool/views/general.py:99 aa_intel_tool/views/general.py:129
+#: aa_intel_tool/views/general.py:101 aa_intel_tool/views/general.py:131
 msgid "The scan you were looking for could not be found."
 msgstr "Der gesuchte Scan konnte nicht gefunden werden."
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/es/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/es/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/es/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 # Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
 # Peter Pfeufer <info@ppfeufer.de>, 2023.
 # Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-04 17:44+0200\n"
+"POT-Creation-Date: 2024-04-20 22:33+0200\n"
 "PO-Revision-Date: 2023-10-25 07:04+0000\n"
-"Last-Translator: Geovanny David Morales De la cruz <moralesgeovanny1996@gmail"
-".com>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-intel-tool/es/>\n"
+"Last-Translator: Geovanny David Morales De la cruz "
+"<moralesgeovanny1996@gmail.com>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-intel-tool/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.1\n"
 
-#: aa_intel_tool/__init__.py:12
+#: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:10
+#: aa_intel_tool/templates/aa_intel_tool/base.html:10
+#: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html:5
 msgid "Intel Parser"
 msgstr ""
 
 #: aa_intel_tool/admin.py:79 aa_intel_tool/models.py:46
@@ -48,26 +48,26 @@
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_intel_tool/apps.py:21
 #, fuzzy, python-brace-format
 #| msgid "Intel Tool v{__version__}"
 msgid "Intel Parser v{__version__}"
 msgstr "Herramienta de Intel v{__version__}"
 
-#: aa_intel_tool/constants.py:71 aa_intel_tool/models.py:24
+#: aa_intel_tool/constants.py:58 aa_intel_tool/models.py:24
 #, fuzzy
 #| msgid "Chat List"
 msgid "Chat list"
 msgstr "Lista de Chat"
 
-#: aa_intel_tool/constants.py:77 aa_intel_tool/models.py:22
+#: aa_intel_tool/constants.py:64 aa_intel_tool/models.py:22
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:28
 msgid "D-Scan"
 msgstr "D-Scan"
 
-#: aa_intel_tool/constants.py:83 aa_intel_tool/models.py:23
+#: aa_intel_tool/constants.py:70 aa_intel_tool/models.py:23
 #: aa_intel_tool/models.py:123
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:33
 msgid "Fleet composition"
 msgstr "Composición de Flota"
 
 #: aa_intel_tool/exceptions.py:34
 #, python-brace-format
@@ -177,136 +177,136 @@
 "No suitable parser found. Input is not a supported intel type or malformed …"
 msgstr ""
 
 #: aa_intel_tool/parser/general.py:80
 msgid "No data to parse …"
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:66
+#: aa_intel_tool/parser/module/chatlist.py:68
 msgid "Something went wrong while fetching the character information from ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:77
+#: aa_intel_tool/parser/module/chatlist.py:79
 msgid "Character unknown to ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:274
+#: aa_intel_tool/parser/module/chatlist.py:281
 msgid "The chat list module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:292
+#: aa_intel_tool/parser/module/chatlist.py:302
 #, python-brace-format
 msgid ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_intel_tool/parser/module/dscan.py:322
+#: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/fleetcomp.py:103
+#: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:8
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
 msgid "Permalink successfully copied"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:10
 msgid ""
 "Something went wrong. Nothing copied. Maybe your browser does not support "
 "this function."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:14
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:3
 msgid "Unaffiliated / No Alliance"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:16
 msgid "NPC Corp"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:19
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
 msgctxt "Decimal separator"
 msgid "."
 msgstr "."
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
 msgctxt "Thousands separator"
 msgid ","
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
 msgid "No data available in this table"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
 msgctxt "Keep _END_ as it is. It will be replaced by a number."
 msgid "Showing _END_ entries"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
 msgctxt "Keep _MAX_ as it is. It will be replaced by a number."
 msgid "(filtered from _MAX_ total entries)"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:25
 msgid "No records available"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:26
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
 msgctxt "Keep _MENU_ as it is. It will be replaced by an HTML construct."
 msgid "Show _MENU_"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
 msgid "Loading …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
 msgid "Processing …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:30
 msgid "Nothing found, sorry …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:31
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:32
 msgid "Search …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:33
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
 msgid "First"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
 msgid "Last"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
 msgid "Next"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:37
 msgid "Previous"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:39
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
 msgid ": activate to sort column ascending"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:41
 msgid ": activate to sort column descending"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
@@ -338,15 +338,21 @@
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:21
 #, python-format
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:50
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
+msgid ""
+"Please keep in mind, parsing large amounts of data can take some time. Be "
+"patient, CCP's API is not the fastest to answer …"
+msgstr ""
+
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
 msgstr "Enviar"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
 msgid "Working on it, please be patient …"
 msgstr ""
 
@@ -388,25 +394,25 @@
 msgid "Count"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:25
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:32
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:37
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:30
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:29
 msgid "Loading data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:31
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:38
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:43
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:35
 msgid "No data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:9
 msgid "Corporations breakdown"
 msgstr ""
@@ -466,14 +472,18 @@
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:19
 msgid "Ship class"
 msgstr ""
 
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
+msgid "Total mass (in kg):"
+msgstr ""
+
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
 msgstr "Tipo de Nave"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr ""
@@ -502,24 +512,18 @@
 msgid "System"
 msgstr "Sistema"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:14
-msgid ""
-"Please keep in mind, parsing large amounts of data can take some time. Be "
-"patient, CCP's API is not the fastest to answer …"
-msgstr ""
-
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
 msgstr ""
 
 #: aa_intel_tool/views/general.py:60
 msgid "(System Error) Something unexpected happened."
 msgstr ""
 
-#: aa_intel_tool/views/general.py:99 aa_intel_tool/views/general.py:129
+#: aa_intel_tool/views/general.py:101 aa_intel_tool/views/general.py:131
 msgid "The scan you were looking for could not be found."
 msgstr ""
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,24 +1,25 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: French (Alliance Auth Apps)\n"
+"Project-Id-Version: Chinese (Simplified) (Alliance Auth Apps)\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-intel-tool/fr/>\n"
-"Language: fr\n"
+"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/zh_Hans/>\n"
+"Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.3.1\n"
 
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr ""
-"Voulez-vous aider à traduire cette application dans votre langue ou "
-"améliorer la traduction existante ?"
+msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
 
 msgid "Join our team of translators!"
-msgstr "Rejoignez notre équipe de traducteurs !"
+msgstr "加入我们的翻译团队吧！"
+
+msgid "Ship type"
+msgstr "舰船类型"
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/django.pot`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# erka Ekanon <M6musicT@hotmail.fr>, 2024.
-# Peter Pfeufer <info@ppfeufer.de>, 2024.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-04 17:44+0200\n"
-"PO-Revision-Date: 2024-01-12 19:05+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-intel-tool/fr/>\n"
-"Language: fr_FR\n"
+"POT-Creation-Date: 2024-04-20 22:33+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=INTEGER; plural=EXPRESSION;\n"
 
-#: aa_intel_tool/__init__.py:12
+#: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:10
+#: aa_intel_tool/templates/aa_intel_tool/base.html:10
+#: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html:5
 msgid "Intel Parser"
 msgstr ""
 
 #: aa_intel_tool/admin.py:79 aa_intel_tool/models.py:46
@@ -43,24 +42,24 @@
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_intel_tool/apps.py:21
 #, python-brace-format
 msgid "Intel Parser v{__version__}"
 msgstr ""
 
-#: aa_intel_tool/constants.py:71 aa_intel_tool/models.py:24
+#: aa_intel_tool/constants.py:58 aa_intel_tool/models.py:24
 msgid "Chat list"
 msgstr ""
 
-#: aa_intel_tool/constants.py:77 aa_intel_tool/models.py:22
+#: aa_intel_tool/constants.py:64 aa_intel_tool/models.py:22
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:28
 msgid "D-Scan"
 msgstr ""
 
-#: aa_intel_tool/constants.py:83 aa_intel_tool/models.py:23
+#: aa_intel_tool/constants.py:70 aa_intel_tool/models.py:23
 #: aa_intel_tool/models.py:123
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:33
 msgid "Fleet composition"
 msgstr ""
 
 #: aa_intel_tool/exceptions.py:34
 #, python-brace-format
@@ -162,136 +161,136 @@
 "No suitable parser found. Input is not a supported intel type or malformed …"
 msgstr ""
 
 #: aa_intel_tool/parser/general.py:80
 msgid "No data to parse …"
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:66
+#: aa_intel_tool/parser/module/chatlist.py:68
 msgid "Something went wrong while fetching the character information from ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:77
+#: aa_intel_tool/parser/module/chatlist.py:79
 msgid "Character unknown to ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:274
+#: aa_intel_tool/parser/module/chatlist.py:281
 msgid "The chat list module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:292
+#: aa_intel_tool/parser/module/chatlist.py:302
 #, python-brace-format
 msgid ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_intel_tool/parser/module/dscan.py:322
+#: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/fleetcomp.py:103
+#: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:8
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
 msgid "Permalink successfully copied"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:10
 msgid ""
 "Something went wrong. Nothing copied. Maybe your browser does not support "
 "this function."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:14
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:3
 msgid "Unaffiliated / No Alliance"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:16
 msgid "NPC Corp"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:19
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
 msgctxt "Decimal separator"
 msgid "."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
 msgctxt "Thousands separator"
 msgid ","
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
 msgid "No data available in this table"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
 msgctxt "Keep _END_ as it is. It will be replaced by a number."
 msgid "Showing _END_ entries"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
 msgctxt "Keep _MAX_ as it is. It will be replaced by a number."
 msgid "(filtered from _MAX_ total entries)"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:25
 msgid "No records available"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:26
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
 msgctxt "Keep _MENU_ as it is. It will be replaced by an HTML construct."
 msgid "Show _MENU_"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
 msgid "Loading …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
 msgid "Processing …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:30
 msgid "Nothing found, sorry …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:31
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:32
 msgid "Search …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:33
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
 msgid "First"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
 msgid "Last"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
 msgid "Next"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:37
 msgid "Previous"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:39
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
 msgid ": activate to sort column ascending"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:41
 msgid ": activate to sort column descending"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
@@ -299,20 +298,18 @@
 msgstr[1] ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
-"Voulez-vous aider à traduire cette application dans votre langue ou "
-"améliorer la traduction existante ?"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "Rejoignez notre équipe de traducteurs !"
+msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:10
 msgid "What can I paste?"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:16
 msgid "Chat member list"
@@ -321,15 +318,21 @@
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:21
 #, python-format
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:50
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
+msgid ""
+"Please keep in mind, parsing large amounts of data can take some time. Be "
+"patient, CCP's API is not the fastest to answer …"
+msgstr ""
+
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
 msgid "Working on it, please be patient …"
 msgstr ""
 
@@ -371,25 +374,25 @@
 msgid "Count"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:25
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:32
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:37
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:30
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:29
 msgid "Loading data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:31
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:38
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:43
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:35
 msgid "No data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:9
 msgid "Corporations breakdown"
 msgstr ""
@@ -449,14 +452,18 @@
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:19
 msgid "Ship class"
 msgstr ""
 
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
+msgid "Total mass (in kg):"
+msgstr ""
+
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr ""
@@ -485,24 +492,18 @@
 msgid "System"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:14
-msgid ""
-"Please keep in mind, parsing large amounts of data can take some time. Be "
-"patient, CCP's API is not the fastest to answer …"
-msgstr ""
-
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
 msgstr ""
 
 #: aa_intel_tool/views/general.py:60
 msgid "(System Error) Something unexpected happened."
 msgstr ""
 
-#: aa_intel_tool/views/general.py:99 aa_intel_tool/views/general.py:129
+#: aa_intel_tool/views/general.py:101 aa_intel_tool/views/general.py:131
 msgid "The scan you were looking for could not be found."
 msgstr ""
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-04 17:44+0200\n"
+"POT-Creation-Date: 2024-04-20 22:33+0200\n"
 "PO-Revision-Date: 2023-10-04 15:46+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-intel-tool/it/>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-intel-tool/it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.0.2\n"
 
-#: aa_intel_tool/__init__.py:12
+#: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:10
+#: aa_intel_tool/templates/aa_intel_tool/base.html:10
+#: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html:5
 msgid "Intel Parser"
 msgstr ""
 
 #: aa_intel_tool/admin.py:79 aa_intel_tool/models.py:46
@@ -43,24 +43,24 @@
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_intel_tool/apps.py:21
 #, python-brace-format
 msgid "Intel Parser v{__version__}"
 msgstr ""
 
-#: aa_intel_tool/constants.py:71 aa_intel_tool/models.py:24
+#: aa_intel_tool/constants.py:58 aa_intel_tool/models.py:24
 msgid "Chat list"
 msgstr ""
 
-#: aa_intel_tool/constants.py:77 aa_intel_tool/models.py:22
+#: aa_intel_tool/constants.py:64 aa_intel_tool/models.py:22
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:28
 msgid "D-Scan"
 msgstr ""
 
-#: aa_intel_tool/constants.py:83 aa_intel_tool/models.py:23
+#: aa_intel_tool/constants.py:70 aa_intel_tool/models.py:23
 #: aa_intel_tool/models.py:123
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:33
 msgid "Fleet composition"
 msgstr ""
 
 #: aa_intel_tool/exceptions.py:34
 #, python-brace-format
@@ -162,136 +162,136 @@
 "No suitable parser found. Input is not a supported intel type or malformed …"
 msgstr ""
 
 #: aa_intel_tool/parser/general.py:80
 msgid "No data to parse …"
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:66
+#: aa_intel_tool/parser/module/chatlist.py:68
 msgid "Something went wrong while fetching the character information from ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:77
+#: aa_intel_tool/parser/module/chatlist.py:79
 msgid "Character unknown to ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:274
+#: aa_intel_tool/parser/module/chatlist.py:281
 msgid "The chat list module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:292
+#: aa_intel_tool/parser/module/chatlist.py:302
 #, python-brace-format
 msgid ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_intel_tool/parser/module/dscan.py:322
+#: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/fleetcomp.py:103
+#: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:8
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
 msgid "Permalink successfully copied"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:10
 msgid ""
 "Something went wrong. Nothing copied. Maybe your browser does not support "
 "this function."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:14
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:3
 msgid "Unaffiliated / No Alliance"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:16
 msgid "NPC Corp"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:19
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
 msgctxt "Decimal separator"
 msgid "."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
 msgctxt "Thousands separator"
 msgid ","
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
 msgid "No data available in this table"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
 msgctxt "Keep _END_ as it is. It will be replaced by a number."
 msgid "Showing _END_ entries"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
 msgctxt "Keep _MAX_ as it is. It will be replaced by a number."
 msgid "(filtered from _MAX_ total entries)"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:25
 msgid "No records available"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:26
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
 msgctxt "Keep _MENU_ as it is. It will be replaced by an HTML construct."
 msgid "Show _MENU_"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
 msgid "Loading …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
 msgid "Processing …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:30
 msgid "Nothing found, sorry …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:31
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:32
 msgid "Search …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:33
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
 msgid "First"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
 msgid "Last"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
 msgid "Next"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:37
 msgid "Previous"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:39
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
 msgid ": activate to sort column ascending"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:41
 msgid ": activate to sort column descending"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
@@ -319,15 +319,21 @@
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:21
 #, python-format
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:50
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
+msgid ""
+"Please keep in mind, parsing large amounts of data can take some time. Be "
+"patient, CCP's API is not the fastest to answer …"
+msgstr ""
+
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
 msgid "Working on it, please be patient …"
 msgstr ""
 
@@ -369,25 +375,25 @@
 msgid "Count"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:25
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:32
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:37
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:30
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:29
 msgid "Loading data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:31
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:38
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:43
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:35
 msgid "No data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:9
 msgid "Corporations breakdown"
 msgstr ""
@@ -447,14 +453,18 @@
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:19
 msgid "Ship class"
 msgstr ""
 
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
+msgid "Total mass (in kg):"
+msgstr ""
+
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr ""
@@ -483,24 +493,18 @@
 msgid "System"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:14
-msgid ""
-"Please keep in mind, parsing large amounts of data can take some time. Be "
-"patient, CCP's API is not the fastest to answer …"
-msgstr ""
-
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
 msgstr ""
 
 #: aa_intel_tool/views/general.py:60
 msgid "(System Error) Something unexpected happened."
 msgstr ""
 
-#: aa_intel_tool/views/general.py:99 aa_intel_tool/views/general.py:129
+#: aa_intel_tool/views/general.py:101 aa_intel_tool/views/general.py:131
 msgid "The scan you were looking for could not be found."
 msgstr ""
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/ja/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-04 17:44+0200\n"
+"POT-Creation-Date: 2024-04-20 22:33+0200\n"
 "PO-Revision-Date: 2023-10-04 15:46+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-intel-tool/ja/>\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-intel-tool/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.0.2\n"
 
-#: aa_intel_tool/__init__.py:12
+#: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:10
+#: aa_intel_tool/templates/aa_intel_tool/base.html:10
+#: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html:5
 msgid "Intel Parser"
 msgstr ""
 
 #: aa_intel_tool/admin.py:79 aa_intel_tool/models.py:46
@@ -43,24 +43,24 @@
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_intel_tool/apps.py:21
 #, python-brace-format
 msgid "Intel Parser v{__version__}"
 msgstr ""
 
-#: aa_intel_tool/constants.py:71 aa_intel_tool/models.py:24
+#: aa_intel_tool/constants.py:58 aa_intel_tool/models.py:24
 msgid "Chat list"
 msgstr ""
 
-#: aa_intel_tool/constants.py:77 aa_intel_tool/models.py:22
+#: aa_intel_tool/constants.py:64 aa_intel_tool/models.py:22
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:28
 msgid "D-Scan"
 msgstr ""
 
-#: aa_intel_tool/constants.py:83 aa_intel_tool/models.py:23
+#: aa_intel_tool/constants.py:70 aa_intel_tool/models.py:23
 #: aa_intel_tool/models.py:123
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:33
 msgid "Fleet composition"
 msgstr ""
 
 #: aa_intel_tool/exceptions.py:34
 #, python-brace-format
@@ -162,135 +162,135 @@
 "No suitable parser found. Input is not a supported intel type or malformed …"
 msgstr ""
 
 #: aa_intel_tool/parser/general.py:80
 msgid "No data to parse …"
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:66
+#: aa_intel_tool/parser/module/chatlist.py:68
 msgid "Something went wrong while fetching the character information from ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:77
+#: aa_intel_tool/parser/module/chatlist.py:79
 msgid "Character unknown to ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:274
+#: aa_intel_tool/parser/module/chatlist.py:281
 msgid "The chat list module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:292
+#: aa_intel_tool/parser/module/chatlist.py:302
 #, python-brace-format
 msgid ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
 msgstr[0] ""
 
-#: aa_intel_tool/parser/module/dscan.py:322
+#: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/fleetcomp.py:103
+#: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:8
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
 msgid "Permalink successfully copied"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:10
 msgid ""
 "Something went wrong. Nothing copied. Maybe your browser does not support "
 "this function."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:14
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:3
 msgid "Unaffiliated / No Alliance"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:16
 msgid "NPC Corp"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:19
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
 msgctxt "Decimal separator"
 msgid "."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
 msgctxt "Thousands separator"
 msgid ","
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
 msgid "No data available in this table"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
 msgctxt "Keep _END_ as it is. It will be replaced by a number."
 msgid "Showing _END_ entries"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
 msgctxt "Keep _MAX_ as it is. It will be replaced by a number."
 msgid "(filtered from _MAX_ total entries)"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:25
 msgid "No records available"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:26
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
 msgctxt "Keep _MENU_ as it is. It will be replaced by an HTML construct."
 msgid "Show _MENU_"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
 msgid "Loading …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
 msgid "Processing …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:30
 msgid "Nothing found, sorry …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:31
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:32
 msgid "Search …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:33
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
 msgid "First"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
 msgid "Last"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
 msgid "Next"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:37
 msgid "Previous"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:39
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
 msgid ": activate to sort column ascending"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:41
 msgid ": activate to sort column descending"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
@@ -316,15 +316,21 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:21
 #, python-format
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] ""
 
-#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:50
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
+msgid ""
+"Please keep in mind, parsing large amounts of data can take some time. Be "
+"patient, CCP's API is not the fastest to answer …"
+msgstr ""
+
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
 msgid "Working on it, please be patient …"
 msgstr ""
 
@@ -366,25 +372,25 @@
 msgid "Count"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:25
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:32
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:37
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:30
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:29
 msgid "Loading data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:31
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:38
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:43
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:35
 msgid "No data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:9
 msgid "Corporations breakdown"
 msgstr ""
@@ -444,14 +450,18 @@
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:19
 msgid "Ship class"
 msgstr ""
 
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
+msgid "Total mass (in kg):"
+msgstr ""
+
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr ""
@@ -480,24 +490,18 @@
 msgid "System"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:14
-msgid ""
-"Please keep in mind, parsing large amounts of data can take some time. Be "
-"patient, CCP's API is not the fastest to answer …"
-msgstr ""
-
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
 msgstr ""
 
 #: aa_intel_tool/views/general.py:60
 msgid "(System Error) Something unexpected happened."
 msgstr ""
 
-#: aa_intel_tool/views/general.py:99 aa_intel_tool/views/general.py:129
+#: aa_intel_tool/views/general.py:101 aa_intel_tool/views/general.py:131
 msgid "The scan you were looking for could not be found."
 msgstr ""
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-intel-tool/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.4.2\n"
 
 msgid "(System Error) Something unexpected happened."
 msgstr "(성계 오류) 예측하지 못한 오류 발생."
 
 msgid ": activate to sort column ascending"
 msgstr ": 열 오름차순으로 정렬 활성화"
 
@@ -114,15 +114,15 @@
 msgid "Interesting on grid"
 msgstr "그리드 내 주요 요소"
 
 msgid "Invalid scan data"
 msgstr "유효하지 않은 데이터"
 
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr "번역팀에 참여하세요!"
 
 msgctxt "Keep _END_ as it is. It will be replaced by a number."
 msgid "Showing _END_ entries"
 msgstr "_END_ 개의 결과 표시중"
 
 msgctxt "Keep _MAX_ as it is. It will be replaced by a number."
 msgid "(filtered from _MAX_ total entries)"
@@ -229,23 +229,29 @@
 
 msgid "Processed scan data"
 msgstr "처리된 스캔 데이터"
 
 msgid "Processing …"
 msgstr "처리 중 …"
 
+msgid "Raw data"
+msgstr "원본 데이터"
+
 msgid "Scan"
 msgstr "스캔"
 
 msgid "Scan data"
 msgstr "스캔 데이터"
 
 msgid "Scan hash"
 msgstr "스캔 해시"
 
+msgid "Scan raw data"
+msgstr "스캔 데이터"
+
 msgid "Scan section"
 msgstr "스캔 범위"
 
 msgid "Scan type"
 msgstr "스캔 종류"
 
 msgid "Scans"
@@ -298,15 +304,15 @@
 msgid "Structures (on grid)"
 msgstr "구조물 (그리드 이내)"
 
 msgid "Submit"
 msgstr "전송"
 
 msgid "System"
-msgstr "성계"
+msgstr "시스템"
 
 msgid "System information"
 msgstr "성계 정보"
 
 msgid "The D-Scan module is currently disabled."
 msgstr "전방위 스캐너 모듈이 비활성화된 상태입니다."
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Author50CO <tkddlschry@gmail.com>, 2023.
 # Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Mind of the Raven <okanieva@gmail.com>, 2024.
+# Rodpold Shard <rodpold@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-04 17:44+0200\n"
-"PO-Revision-Date: 2023-10-04 15:47+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-intel-tool/ko/>\n"
+"POT-Creation-Date: 2024-04-20 22:33+0200\n"
+"PO-Revision-Date: 2024-03-22 00:11+0000\n"
+"Last-Translator: Mind of the Raven <okanieva@gmail.com>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-intel-tool/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.4.2\n"
 
-#: aa_intel_tool/__init__.py:12
+#: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:10
+#: aa_intel_tool/templates/aa_intel_tool/base.html:10
+#: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html:5
 msgid "Intel Parser"
 msgstr "인텔 파싱"
 
 #: aa_intel_tool/admin.py:79 aa_intel_tool/models.py:46
@@ -34,35 +36,33 @@
 msgstr "스캔 종류"
 
 #: aa_intel_tool/admin.py:94
 msgid "Open in a new browser tab"
 msgstr "새 탭에서 열기"
 
 #: aa_intel_tool/admin.py:100
-#, fuzzy
-#| msgid "RAW data"
 msgid "Raw data"
-msgstr "처리 이전 데이터"
+msgstr "원본 데이터"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_intel_tool/apps.py:21
 #, python-brace-format
 msgid "Intel Parser v{__version__}"
 msgstr "인텔 파싱 v{__version__}"
 
-#: aa_intel_tool/constants.py:71 aa_intel_tool/models.py:24
+#: aa_intel_tool/constants.py:58 aa_intel_tool/models.py:24
 msgid "Chat list"
 msgstr "챗 리스트"
 
-#: aa_intel_tool/constants.py:77 aa_intel_tool/models.py:22
+#: aa_intel_tool/constants.py:64 aa_intel_tool/models.py:22
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:28
 msgid "D-Scan"
 msgstr "전방위 스캐너"
 
-#: aa_intel_tool/constants.py:83 aa_intel_tool/models.py:23
+#: aa_intel_tool/constants.py:70 aa_intel_tool/models.py:23
 #: aa_intel_tool/models.py:123
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:33
 msgid "Fleet composition"
 msgstr "함대 구성"
 
 #: aa_intel_tool/exceptions.py:34
 #, python-brace-format
@@ -82,16 +82,14 @@
 msgstr "스캔 해시"
 
 #: aa_intel_tool/models.py:37
 msgid "Creation date/time"
 msgstr "생성 날짜/시간"
 
 #: aa_intel_tool/models.py:40
-#, fuzzy
-#| msgid "Scan data"
 msgid "Scan raw data"
 msgstr "스캔 데이터"
 
 #: aa_intel_tool/models.py:55 aa_intel_tool/models.py:132
 msgid "Scan"
 msgstr "스캔"
 
@@ -160,144 +158,147 @@
 #: aa_intel_tool/models.py:152 aa_intel_tool/models.py:153
 msgid "Scan data"
 msgstr "스캔 데이터"
 
 #: aa_intel_tool/parser/general.py:46
 msgid ""
 "No suitable parser found. Input is not a supported intel type or malformed …"
-msgstr "지원하는 파서를 찾을 수 없습니다. 지원하지 않는 인텔 타입이거나, 잘못된 "
-"형식입니다…"
+msgstr ""
+"지원하는 파서를 찾을 수 없습니다. 지원하지 않는 인텔 타입이거나, 잘못된 형식"
+"입니다…"
 
 #: aa_intel_tool/parser/general.py:80
 msgid "No data to parse …"
 msgstr "가져올 데이터가 없습니다…"
 
-#: aa_intel_tool/parser/module/chatlist.py:66
+#: aa_intel_tool/parser/module/chatlist.py:68
 msgid "Something went wrong while fetching the character information from ESI."
 msgstr "ESI에서 캐릭터 정보를 가져오는 중 오류가 발생했습니다."
 
-#: aa_intel_tool/parser/module/chatlist.py:77
+#: aa_intel_tool/parser/module/chatlist.py:79
 msgid "Character unknown to ESI."
 msgstr "ESI에 등록되지 않은 캐릭터입니다."
 
-#: aa_intel_tool/parser/module/chatlist.py:274
+#: aa_intel_tool/parser/module/chatlist.py:281
 msgid "The chat list module is currently disabled."
 msgstr "챗 리스트 모듈이 비활성화된 상태입니다."
 
-#: aa_intel_tool/parser/module/chatlist.py:292
+#: aa_intel_tool/parser/module/chatlist.py:302
 #, python-brace-format
 msgid ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
-msgstr[0] "챗 스캔 파일럿 수는 최대 {max_allowed_pilots}명으로 제한되어 있습니다. "
-"입력한 파일럿 수가 제한을 초과합니다."
+msgstr[0] ""
+"챗 스캔 파일럿 수는 최대 {max_allowed_pilots}명으로 제한되어 있습니다. 입력"
+"한 파일럿 수가 제한을 초과합니다."
 
-#: aa_intel_tool/parser/module/dscan.py:322
+#: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr "전방위 스캐너 모듈이 비활성화된 상태입니다."
 
-#: aa_intel_tool/parser/module/fleetcomp.py:103
+#: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
 msgstr "함대 구성 모듈이 비활성화된 상태입니다."
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:8
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
 msgid "Permalink successfully copied"
 msgstr "고유링크가 성공적으로 복사되었습니다"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:10
 msgid ""
 "Something went wrong. Nothing copied. Maybe your browser does not support "
 "this function."
-msgstr "뭔가 잘못됐습니다. 복사되지 않았습니다. 브라우저가 이 기능을 지원하지 않을 "
-"수도 있습니다."
+msgstr ""
+"뭔가 잘못됐습니다. 복사되지 않았습니다. 브라우저가 이 기능을 지원하지 않을 수"
+"도 있습니다."
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:14
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:3
 msgid "Unaffiliated / No Alliance"
 msgstr "얼라이언스 없음"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:16
 msgid "NPC Corp"
 msgstr "NPC 코퍼레이션"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:19
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
 msgctxt "Decimal separator"
 msgid "."
 msgstr "."
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
 msgctxt "Thousands separator"
 msgid ","
 msgstr ","
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
 msgid "No data available in this table"
 msgstr "테이블에 유효한 데이터가 없습니다"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
 msgctxt "Keep _END_ as it is. It will be replaced by a number."
 msgid "Showing _END_ entries"
 msgstr "_END_ 개의 결과 표시중"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
 msgctxt "Keep _MAX_ as it is. It will be replaced by a number."
 msgid "(filtered from _MAX_ total entries)"
 msgstr "총 _MAX_ 개의 결과 에서 필터링됨"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:25
 msgid "No records available"
 msgstr "사용 가능한 레코드가 없습니다"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:26
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
 msgctxt "Keep _MENU_ as it is. It will be replaced by an HTML construct."
 msgid "Show _MENU_"
 msgstr "_MENU_ 보기"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
 msgid "Loading …"
 msgstr "로딩 …"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
 msgid "Processing …"
 msgstr "처리 중 …"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:30
 msgid "Nothing found, sorry …"
 msgstr "아무것도 찾지 못했습니다, 죄송합니다 …"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:31
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:32
 msgid "Search …"
 msgstr "검색 …"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:33
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
 msgid "First"
 msgstr "첫 번째"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
 msgid "Last"
 msgstr "마지막"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
 msgid "Next"
 msgstr "다음"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:37
 msgid "Previous"
 msgstr "이전"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:39
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
 msgid ": activate to sort column ascending"
 msgstr ": 열 오름차순으로 정렬 활성화"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:41
 msgid ": activate to sort column descending"
 msgstr ": 열 내림차순으로 정렬 활성화"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
@@ -307,15 +308,15 @@
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr "번역팀에 참여하세요!"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:10
 msgid "What can I paste?"
 msgstr "무엇을 붙여넣을 수 있나요?"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:16
 msgid "Chat member list"
@@ -323,15 +324,23 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:21
 #, python-format
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] "스캔 당 최대 %(max_pilots)s명으로 제한되어 있습니다."
 
-#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:50
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
+msgid ""
+"Please keep in mind, parsing large amounts of data can take some time. Be "
+"patient, CCP's API is not the fastest to answer …"
+msgstr ""
+"기억해주세요, 큰 데이터를 가져오는 데에는 시간이 걸립니다. CCP의 API는 느린 "
+"것으로 유명합니다, 조금만 기다려 주세요 …"
+
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
 msgstr "전송"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
 msgid "Working on it, please be patient …"
 msgstr "작업 중입니다, 잠시만 기다려 주세요 …"
 
@@ -377,25 +386,25 @@
 msgid "Count"
 msgstr "갯수"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:25
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:32
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:37
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:30
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:29
 msgid "Loading data …"
 msgstr "데이터 로딩 중 …"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:31
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:38
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:43
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:35
 msgid "No data …"
 msgstr "데이터 없음 …"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:9
 msgid "Corporations breakdown"
 msgstr "코퍼레이션별 분류"
@@ -455,14 +464,18 @@
 msgstr "그리드 밖"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:19
 msgid "Ship class"
 msgstr "함급"
 
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
+msgid "Total mass (in kg):"
+msgstr ""
+
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
 msgstr "함선 종류"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr "데이터 없음."
@@ -487,31 +500,24 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:6
 msgid "Who is flying what"
 msgstr "함선 및 파일럿"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:22
 msgid "System"
-msgstr "성계"
+msgstr "시스템"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr "참가 세부 사항"
 
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:14
-msgid ""
-"Please keep in mind, parsing large amounts of data can take some time. Be "
-"patient, CCP's API is not the fastest to answer …"
-msgstr "기억해주세요, 큰 데이터를 가져오는 데에는 시간이 걸립니다. CCP의 API는 느린 "
-"것으로 유명합니다, 조금만 기다려 주세요 …"
-
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
 msgstr "제공된 데이터를 가져올 수 없습니다."
 
 #: aa_intel_tool/views/general.py:60
 msgid "(System Error) Something unexpected happened."
 msgstr "(성계 오류) 예측하지 못한 오류 발생."
 
-#: aa_intel_tool/views/general.py:99 aa_intel_tool/views/general.py:129
+#: aa_intel_tool/views/general.py:101 aa_intel_tool/views/general.py:131
 msgid "The scan you were looking for could not be found."
 msgstr "요구하는 스캔을 찾을 수 없습니다."
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/ru/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/ru/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 # Nikolay <nick.postnikov@gmail.com>, 2023.
 # Peter Pfeufer <info@ppfeufer.de>, 2023.
 # Max <mark25@inbox.ru>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-04 17:44+0200\n"
+"POT-Creation-Date: 2024-04-20 22:33+0200\n"
 "PO-Revision-Date: 2023-10-04 15:47+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-intel-tool/ru/>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-intel-tool/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 5.0.2\n"
 
-#: aa_intel_tool/__init__.py:12
+#: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:10
+#: aa_intel_tool/templates/aa_intel_tool/base.html:10
+#: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html:5
 msgid "Intel Parser"
 msgstr "Анализатор Скана"
 
 #: aa_intel_tool/admin.py:79 aa_intel_tool/models.py:46
@@ -45,24 +45,24 @@
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_intel_tool/apps.py:21
 #, python-brace-format
 msgid "Intel Parser v{__version__}"
 msgstr "Анализатор Скана v{__version__}"
 
-#: aa_intel_tool/constants.py:71 aa_intel_tool/models.py:24
+#: aa_intel_tool/constants.py:58 aa_intel_tool/models.py:24
 msgid "Chat list"
 msgstr "Список чата"
 
-#: aa_intel_tool/constants.py:77 aa_intel_tool/models.py:22
+#: aa_intel_tool/constants.py:64 aa_intel_tool/models.py:22
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:28
 msgid "D-Scan"
 msgstr "Подскан"
 
-#: aa_intel_tool/constants.py:83 aa_intel_tool/models.py:23
+#: aa_intel_tool/constants.py:70 aa_intel_tool/models.py:23
 #: aa_intel_tool/models.py:123
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:33
 msgid "Fleet composition"
 msgstr "Состав флота"
 
 #: aa_intel_tool/exceptions.py:34
 #, python-brace-format
@@ -166,27 +166,27 @@
 "Не найден подходящий анализатор. Формат входных данных не поддерживается или "
 "данные неполны …"
 
 #: aa_intel_tool/parser/general.py:80
 msgid "No data to parse …"
 msgstr "Нет данных для анализа …"
 
-#: aa_intel_tool/parser/module/chatlist.py:66
+#: aa_intel_tool/parser/module/chatlist.py:68
 msgid "Something went wrong while fetching the character information from ESI."
 msgstr "Что-то пошло не так при загрузке информации о персонаже через ESI."
 
-#: aa_intel_tool/parser/module/chatlist.py:77
+#: aa_intel_tool/parser/module/chatlist.py:79
 msgid "Character unknown to ESI."
 msgstr "Персонаж не известен для ESI."
 
-#: aa_intel_tool/parser/module/chatlist.py:274
+#: aa_intel_tool/parser/module/chatlist.py:281
 msgid "The chat list module is currently disabled."
 msgstr "Анализатор списка чата отключен."
 
-#: aa_intel_tool/parser/module/chatlist.py:292
+#: aa_intel_tool/parser/module/chatlist.py:302
 #, python-brace-format
 msgid ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
@@ -199,115 +199,115 @@
 msgstr[2] ""
 "Анализатор чата в настоящее время ограничен максимум {max_allowed_pilots} "
 "пилотами в скане. Размер вашего списка превышает это ограничение."
 msgstr[3] ""
 "Анализатор чата в настоящее время ограничен максимум одним пилотом в скане. "
 "Размер вашего списка превышает это ограничение."
 
-#: aa_intel_tool/parser/module/dscan.py:322
+#: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr "Анализатор подскана отключен."
 
-#: aa_intel_tool/parser/module/fleetcomp.py:103
+#: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
 msgstr "Анализатор состава флота отключен."
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:8
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
 msgid "Permalink successfully copied"
 msgstr "Постоянная ссылка успешно скопирована"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:10
 msgid ""
 "Something went wrong. Nothing copied. Maybe your browser does not support "
 "this function."
 msgstr ""
 "Что-то пошло не так. Ничего не скопировано. Возможно, ваш браузер не "
 "поддерживает данную функцию."
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:14
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:3
 msgid "Unaffiliated / No Alliance"
 msgstr "Неаффилированный / Нет альянса"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:16
 msgid "NPC Corp"
 msgstr "NPC корпорация"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:19
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
 msgctxt "Decimal separator"
 msgid "."
 msgstr ","
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
 msgctxt "Thousands separator"
 msgid ","
 msgstr " "
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
 msgid "No data available in this table"
 msgstr "Данные в таблице отсутствуют"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
 msgctxt "Keep _END_ as it is. It will be replaced by a number."
 msgid "Showing _END_ entries"
 msgstr "Отображаются _END_ записей"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
 msgctxt "Keep _MAX_ as it is. It will be replaced by a number."
 msgid "(filtered from _MAX_ total entries)"
 msgstr "(отфильтрованы из _MAX_ записей)"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:25
 msgid "No records available"
 msgstr "Записи недоступны"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:26
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
 msgctxt "Keep _MENU_ as it is. It will be replaced by an HTML construct."
 msgid "Show _MENU_"
 msgstr "Показывать _MENU_"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
 msgid "Loading …"
 msgstr "Загрузка …"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
 msgid "Processing …"
 msgstr "Обработка …"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:30
 msgid "Nothing found, sorry …"
 msgstr "Ничего не найдено …"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:31
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:32
 msgid "Search …"
 msgstr "Поиск…"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:33
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
 msgid "First"
 msgstr "Первый"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
 msgid "Last"
 msgstr "Последний"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
 msgid "Next"
 msgstr "Следующий"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:37
 msgid "Previous"
 msgstr "Предыдущий"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:39
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
 msgid ": activate to sort column ascending"
 msgstr ": активируйте для сортировки по возрастанию"
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:41
 msgid ": activate to sort column descending"
 msgstr ": активируйте для сортировки по убыванию"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
@@ -341,15 +341,23 @@
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] "Ограничен максимум %(max_pilots)s пилотом в скане."
 msgstr[1] "Ограничен максимум %(max_pilots)s пилотами в скане."
 msgstr[2] "Ограничен максимум %(max_pilots)s пилотами в скане."
 msgstr[3] "Ограничен максимум одним пилотом в скане."
 
-#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:50
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
+msgid ""
+"Please keep in mind, parsing large amounts of data can take some time. Be "
+"patient, CCP's API is not the fastest to answer …"
+msgstr ""
+"Помните, что обработка большого объема данных может занять некоторое время. "
+"Будьте терпеливы, CCP API не самое быстрое …"
+
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
 msgstr "Отправить"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
 msgid "Working on it, please be patient …"
 msgstr "Работаем над этим, потерпите …"
 
@@ -391,25 +399,25 @@
 msgid "Count"
 msgstr "Количество"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:25
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:32
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:37
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:30
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:29
 msgid "Loading data …"
 msgstr "Загрузка данных …"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:31
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:38
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:43
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:35
 msgid "No data …"
 msgstr "Нет данных …"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:9
 msgid "Corporations breakdown"
 msgstr "Разбивка по корпорациям"
@@ -469,14 +477,18 @@
 msgstr "Вне грида"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:19
 msgid "Ship class"
 msgstr "Класс корабля"
 
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
+msgid "Total mass (in kg):"
+msgstr ""
+
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
 msgstr "Тип корабля"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr "Нет данных."
@@ -505,26 +517,18 @@
 msgid "System"
 msgstr "Система"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr "Подробности участия"
 
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:14
-msgid ""
-"Please keep in mind, parsing large amounts of data can take some time. Be "
-"patient, CCP's API is not the fastest to answer …"
-msgstr ""
-"Помните, что обработка большого объема данных может занять некоторое время. "
-"Будьте терпеливы, CCP API не самое быстрое …"
-
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
 msgstr "Предоставленные данные не могут быть проанализированы."
 
 #: aa_intel_tool/views/general.py:60
 msgid "(System Error) Something unexpected happened."
 msgstr "(Системная ошибка) Случилось что-то непредвиденное."
 
-#: aa_intel_tool/views/general.py:99 aa_intel_tool/views/general.py:129
+#: aa_intel_tool/views/general.py:101 aa_intel_tool/views/general.py:131
 msgid "The scan you were looking for could not be found."
 msgstr "Скан, который вы ищите, не может быть найден."
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/uk/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/uk/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/uk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Peter Pfeufer <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-04 17:44+0200\n"
+"POT-Creation-Date: 2024-04-20 22:33+0200\n"
 "PO-Revision-Date: 2023-10-04 15:47+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-intel-tool/uk/>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-intel-tool/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 5.0.2\n"
 
-#: aa_intel_tool/__init__.py:12
+#: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:10
+#: aa_intel_tool/templates/aa_intel_tool/base.html:10
+#: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html:5
 msgid "Intel Parser"
 msgstr ""
 
 #: aa_intel_tool/admin.py:79 aa_intel_tool/models.py:46
@@ -43,24 +43,24 @@
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_intel_tool/apps.py:21
 #, python-brace-format
 msgid "Intel Parser v{__version__}"
 msgstr ""
 
-#: aa_intel_tool/constants.py:71 aa_intel_tool/models.py:24
+#: aa_intel_tool/constants.py:58 aa_intel_tool/models.py:24
 msgid "Chat list"
 msgstr ""
 
-#: aa_intel_tool/constants.py:77 aa_intel_tool/models.py:22
+#: aa_intel_tool/constants.py:64 aa_intel_tool/models.py:22
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:28
 msgid "D-Scan"
 msgstr ""
 
-#: aa_intel_tool/constants.py:83 aa_intel_tool/models.py:23
+#: aa_intel_tool/constants.py:70 aa_intel_tool/models.py:23
 #: aa_intel_tool/models.py:123
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:33
 msgid "Fleet composition"
 msgstr ""
 
 #: aa_intel_tool/exceptions.py:34
 #, python-brace-format
@@ -162,138 +162,138 @@
 "No suitable parser found. Input is not a supported intel type or malformed …"
 msgstr ""
 
 #: aa_intel_tool/parser/general.py:80
 msgid "No data to parse …"
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:66
+#: aa_intel_tool/parser/module/chatlist.py:68
 msgid "Something went wrong while fetching the character information from ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:77
+#: aa_intel_tool/parser/module/chatlist.py:79
 msgid "Character unknown to ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:274
+#: aa_intel_tool/parser/module/chatlist.py:281
 msgid "The chat list module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:292
+#: aa_intel_tool/parser/module/chatlist.py:302
 #, python-brace-format
 msgid ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
 
-#: aa_intel_tool/parser/module/dscan.py:322
+#: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/fleetcomp.py:103
+#: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:8
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
 msgid "Permalink successfully copied"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:10
 msgid ""
 "Something went wrong. Nothing copied. Maybe your browser does not support "
 "this function."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:14
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:3
 msgid "Unaffiliated / No Alliance"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:16
 msgid "NPC Corp"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:19
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
 msgctxt "Decimal separator"
 msgid "."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
 msgctxt "Thousands separator"
 msgid ","
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
 msgid "No data available in this table"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
 msgctxt "Keep _END_ as it is. It will be replaced by a number."
 msgid "Showing _END_ entries"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
 msgctxt "Keep _MAX_ as it is. It will be replaced by a number."
 msgid "(filtered from _MAX_ total entries)"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:25
 msgid "No records available"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:26
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
 msgctxt "Keep _MENU_ as it is. It will be replaced by an HTML construct."
 msgid "Show _MENU_"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
 msgid "Loading …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
 msgid "Processing …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:30
 msgid "Nothing found, sorry …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:31
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:32
 msgid "Search …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:33
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
 msgid "First"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
 msgid "Last"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
 msgid "Next"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:37
 msgid "Previous"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:39
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
 msgid ": activate to sort column ascending"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:41
 msgid ": activate to sort column descending"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
@@ -325,15 +325,21 @@
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
 
-#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:50
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
+msgid ""
+"Please keep in mind, parsing large amounts of data can take some time. Be "
+"patient, CCP's API is not the fastest to answer …"
+msgstr ""
+
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
 msgstr "Відправити"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
 msgid "Working on it, please be patient …"
 msgstr ""
 
@@ -375,25 +381,25 @@
 msgid "Count"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:25
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:32
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:37
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:30
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:29
 msgid "Loading data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:31
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:38
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:43
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:35
 msgid "No data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:9
 msgid "Corporations breakdown"
 msgstr ""
@@ -453,14 +459,18 @@
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:19
 msgid "Ship class"
 msgstr ""
 
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
+msgid "Total mass (in kg):"
+msgstr ""
+
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr ""
@@ -489,24 +499,18 @@
 msgid "System"
 msgstr "Система"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:14
-msgid ""
-"Please keep in mind, parsing large amounts of data can take some time. Be "
-"patient, CCP's API is not the fastest to answer …"
-msgstr ""
-
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
 msgstr ""
 
 #: aa_intel_tool/views/general.py:60
 msgid "(System Error) Something unexpected happened."
 msgstr ""
 
-#: aa_intel_tool/views/general.py:99 aa_intel_tool/views/general.py:129
+#: aa_intel_tool/views/general.py:101 aa_intel_tool/views/general.py:131
 msgid "The scan you were looking for could not be found."
 msgstr ""
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.0/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Dehao Wu <wudehao2000@163.com>, 2024.
 # Faer Yili <yilifaer@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-04 17:44+0200\n"
+"POT-Creation-Date: 2024-04-20 22:33+0200\n"
 "PO-Revision-Date: 2024-01-11 21:04+0000\n"
 "Last-Translator: Dehao Wu <wudehao2000@163.com>\n"
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-intel-tool/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.3.1\n"
 
-#: aa_intel_tool/__init__.py:12
+#: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:6
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:10
+#: aa_intel_tool/templates/aa_intel_tool/base.html:10
+#: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html:5
 msgid "Intel Parser"
 msgstr ""
 
 #: aa_intel_tool/admin.py:79 aa_intel_tool/models.py:46
@@ -43,24 +43,24 @@
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_intel_tool/apps.py:21
 #, python-brace-format
 msgid "Intel Parser v{__version__}"
 msgstr ""
 
-#: aa_intel_tool/constants.py:71 aa_intel_tool/models.py:24
+#: aa_intel_tool/constants.py:58 aa_intel_tool/models.py:24
 msgid "Chat list"
 msgstr ""
 
-#: aa_intel_tool/constants.py:77 aa_intel_tool/models.py:22
+#: aa_intel_tool/constants.py:64 aa_intel_tool/models.py:22
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:28
 msgid "D-Scan"
 msgstr ""
 
-#: aa_intel_tool/constants.py:83 aa_intel_tool/models.py:23
+#: aa_intel_tool/constants.py:70 aa_intel_tool/models.py:23
 #: aa_intel_tool/models.py:123
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:33
 msgid "Fleet composition"
 msgstr ""
 
 #: aa_intel_tool/exceptions.py:34
 #, python-brace-format
@@ -162,135 +162,135 @@
 "No suitable parser found. Input is not a supported intel type or malformed …"
 msgstr ""
 
 #: aa_intel_tool/parser/general.py:80
 msgid "No data to parse …"
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:66
+#: aa_intel_tool/parser/module/chatlist.py:68
 msgid "Something went wrong while fetching the character information from ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:77
+#: aa_intel_tool/parser/module/chatlist.py:79
 msgid "Character unknown to ESI."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:274
+#: aa_intel_tool/parser/module/chatlist.py:281
 msgid "The chat list module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/chatlist.py:292
+#: aa_intel_tool/parser/module/chatlist.py:302
 #, python-brace-format
 msgid ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
 msgstr[0] ""
 
-#: aa_intel_tool/parser/module/dscan.py:322
+#: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/parser/module/fleetcomp.py:103
+#: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:8
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
 msgid "Permalink successfully copied"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:9
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:10
 msgid ""
 "Something went wrong. Nothing copied. Maybe your browser does not support "
 "this function."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:14
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:3
 msgid "Unaffiliated / No Alliance"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:16
 msgid "NPC Corp"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:19
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
 msgctxt "Decimal separator"
 msgid "."
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:20
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
 msgctxt "Thousands separator"
 msgid ","
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:21
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
 msgid "No data available in this table"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:22
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
 msgctxt "Keep _END_ as it is. It will be replaced by a number."
 msgid "Showing _END_ entries"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:23
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
 msgctxt "Keep _MAX_ as it is. It will be replaced by a number."
 msgid "(filtered from _MAX_ total entries)"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:24
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:25
 msgid "No records available"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:26
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
 msgctxt "Keep _MENU_ as it is. It will be replaced by an HTML construct."
 msgid "Show _MENU_"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:27
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
 msgid "Loading …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:28
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
 msgid "Processing …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:29
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:30
 msgid "Nothing found, sorry …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:31
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:32
 msgid "Search …"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:33
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
 msgid "First"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:34
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
 msgid "Last"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:35
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
 msgid "Next"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:36
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:37
 msgid "Previous"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:39
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
 msgid ": activate to sort column ascending"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:40
+#: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:41
 msgid ": activate to sort column descending"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
@@ -316,15 +316,21 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:21
 #, python-format
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] ""
 
-#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:50
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
+msgid ""
+"Please keep in mind, parsing large amounts of data can take some time. Be "
+"patient, CCP's API is not the fastest to answer …"
+msgstr ""
+
+#: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
 msgid "Working on it, please be patient …"
 msgstr ""
 
@@ -366,25 +372,25 @@
 msgid "Count"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:25
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:32
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:37
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:30
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:29
 msgid "Loading data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:35
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:31
-#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:38
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:43
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:35
 msgid "No data …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:9
 msgid "Corporations breakdown"
 msgstr ""
@@ -444,14 +450,18 @@
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:19
 msgid "Ship class"
 msgstr ""
 
+#: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
+msgid "Total mass (in kg):"
+msgstr ""
+
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
 msgstr "舰船类型"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr ""
@@ -480,24 +490,18 @@
 msgid "System"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr ""
 
-#: aa_intel_tool/templates/aa_intel_tool/views/index.html:14
-msgid ""
-"Please keep in mind, parsing large amounts of data can take some time. Be "
-"patient, CCP's API is not the fastest to answer …"
-msgstr ""
-
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
 msgstr ""
 
 #: aa_intel_tool/views/general.py:60
 msgid "(System Error) Something unexpected happened."
 msgstr ""
 
-#: aa_intel_tool/views/general.py:99 aa_intel_tool/views/general.py:129
+#: aa_intel_tool/views/general.py:101 aa_intel_tool/views/general.py:131
 msgid "The scan you were looking for could not be found."
 msgstr ""
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/management/commands/aa_intel_tool_load_eve_types.py` & `aa_intel_tool-2.1.0/aa_intel_tool/management/commands/aa_intel_tool_load_eve_types.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/migrations/0001_initial.py` & `aa_intel_tool-2.1.0/aa_intel_tool/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/parser/general.py` & `aa_intel_tool-2.1.0/aa_intel_tool/parser/general.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/parser/helper/db.py` & `aa_intel_tool-2.1.0/aa_intel_tool/parser/helper/db.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/parser/module/chatlist.py` & `aa_intel_tool-2.1.0/aa_intel_tool/parser/module/chatlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     }
 
     # Add eve links if requested
     if with_evelinks:
         corporation_info["dotlan"] = dotlan.corporation_url(
             name=eve_character.corporation_name
         )
-        corporation_info["zkillboard"] = zkillboard.alliance_url(
+        corporation_info["zkillboard"] = zkillboard.corporation_url(
             eve_id=eve_character.corporation_id
         )
 
     # Add alliance info if requested
     if with_alliance_info:
         corporation_info["alliance"] = _parse_alliance_info(
             eve_character=eve_character, with_evelinks=with_evelinks
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/parser/module/dscan.py` & `aa_intel_tool-2.1.0/aa_intel_tool/parser/module/dscan.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,37 +100,55 @@
     :type counter:
     :return:
     :rtype:
     """
 
     ships = {"all": {}, "ongrid": {}, "offgrid": {}, "types": {}}
 
+    # Ship types
+    # Get all ship types
+    #
+    # Ship type list:
+    #   - eve_type[0] = ID
+    #   - eve_type[1] = Name
+    #   - eve_type[2] = Group ID
+    #   - eve_type[3] = Group Name
+    #   - eve_type[4] = Mass
     eve_types_ships = eve_types.filter(
         eve_group__eve_category_id__exact=EveCategoryId.SHIP
     )
 
     # Loop through all ships types
     for eve_type in eve_types_ships:
         # Info for "All Ships" table
         if eve_type[0] in counter["all"]:
             if eve_type[1] not in ships["all"]:
                 ships["all"][eve_type[1]] = _get_type_info_dict(eve_type=eve_type)
                 ships["all"][eve_type[1]]["count"] = counter["all"][eve_type[0]]
+                ships["all"][eve_type[1]]["mass"] = (
+                    eve_type[4] * counter["all"][eve_type[0]]
+                )
 
         # Info for "On Grid" table
         if eve_type[0] in counter["ongrid"]:
             if eve_type[1] not in ships["ongrid"]:
                 ships["ongrid"][eve_type[1]] = _get_type_info_dict(eve_type=eve_type)
                 ships["ongrid"][eve_type[1]]["count"] = counter["ongrid"][eve_type[0]]
+                ships["ongrid"][eve_type[1]]["mass"] = (
+                    eve_type[4] * counter["ongrid"][eve_type[0]]
+                )
 
         # Info for "Off Grid" table
         if eve_type[0] in counter["offgrid"]:
             if eve_type[1] not in ships["offgrid"]:
                 ships["offgrid"][eve_type[1]] = _get_type_info_dict(eve_type=eve_type)
                 ships["offgrid"][eve_type[1]]["count"] = counter["offgrid"][eve_type[0]]
+                ships["offgrid"][eve_type[1]]["mass"] = (
+                    eve_type[4] * counter["offgrid"][eve_type[0]]
+                )
 
         # Info for "Ship Types" table
         if eve_type[3] not in ships["types"]:
             ships["types"][eve_type[3]] = {
                 "id": eve_type[2],
                 "name": eve_type[3],
                 "count": 0,
@@ -264,40 +282,52 @@
 
     :param scan_data:
     :type scan_data:
     :return:
     :rtype:
     """
 
+    # AA Intel Tool
+    from aa_intel_tool.constants import (  # pylint: disable=import-outside-toplevel
+        REGEX_PATTERN,
+    )
+
     ansiblex_destination = None
     counter = {"all": {}, "ongrid": {}, "offgrid": {}, "type": {}}
     eve_ids = {"all": [], "ongrid": [], "offgrid": []}
 
     # Let's split this list up
     #
-    # line[0] => Item ID
-    # line[1] => Name
-    # line[2] => Ship Class / Structure Type
-    # line[3] => Distance
+    # line.group(1) => Item ID
+    # line.group(2) => Name
+    # line.group(3) => Ship Class / Structure Type
+    # line.group(4) => Distance
     #
     # Loop through all lines
     for entry in scan_data:
-        line = re.split(pattern=r"\t+", string=entry.rstrip("\t"))
-        entry_id = int(line[0])
+        # Apparently you can copy/paste a tab into the ship name, which will cause the split by tab to fail.
+        # The regex is detecting the D-Scan correctly though. But splitting by tab might put the ship class as distance.
+        # See https://github.com/ppfeufer/aa-intel-tool/issues/82
+        #
+        # This is why we use re.search() to get the parts of the D-Scan entry, instead of re-split()
+        #
+        # Thanks CCP for sanitizing your inputs! 😂
+        line = re.search(pattern=REGEX_PATTERN["dscan"], string=entry)
+        entry_id = int(line.group(1))
 
         counter["all"][entry_id] = counter["all"].get(entry_id, 0) + 1
 
         # Check if the entry is "on grid" or not
-        if _is_on_grid(line[3]):
+        if _is_on_grid(line.group(4)):
             counter["ongrid"][entry_id] = counter["ongrid"].get(entry_id, 0) + 1
 
             # If it is an Ansiblex Jump Gate, get its destination system
             if entry_id == UpwellStructureId.ANSIBLEX_JUMP_GATE:
                 ansiblex_destination = _get_ansiblex_jumpgate_destination(
-                    ansiblex_name=line[1]
+                    ansiblex_name=line.group(2)
                 )
 
             eve_ids["ongrid"].append(entry_id)
         else:
             counter["offgrid"][entry_id] = counter["offgrid"].get(entry_id, 0) + 1
 
             eve_ids["offgrid"].append(entry_id)
@@ -326,15 +356,17 @@
             ansiblex_destination,  # pylint: disable=unused-variable
             counter,
             eve_ids,
         ) = _get_scan_details(scan_data=scan_data)
 
         eve_types = EveType.objects.bulk_get_or_create_esi(
             ids=set(eve_ids["all"]), include_children=True
-        ).values_list("id", "name", "eve_group__id", "eve_group__name", named=True)
+        ).values_list(
+            "id", "name", "eve_group__id", "eve_group__name", "mass", named=True
+        )
 
         # Parse the data parts
         ships = _get_ships(eve_types=eve_types, counter=counter)
         upwell_structures = _get_upwell_structures_on_grid(
             eve_types=eve_types,
             counter=counter,
             # ansiblex_destination=ansiblex_destination,
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/parser/module/fleetcomp.py` & `aa_intel_tool-2.1.0/aa_intel_tool/parser/module/fleetcomp.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,26 +45,29 @@
         .filter(category=EveEntity.CATEGORY_INVENTORY_TYPE)
         .values_list("id", flat=True)
     )
 
     # Get ship class details
     ship_class_details = EveType.objects.bulk_get_or_create_esi(
         ids=set(ship_class_ids), include_children=True
-    ).values_list("id", "name", "eve_group__id", "eve_group__name", named=True)
+    ).values_list("id", "name", "eve_group__id", "eve_group__name", "mass", named=True)
 
     # Loop through ship classes
     for ship_class in ship_class_details:
         # Build ship class dict
         ships["class"][ship_class.name]["id"] = ship_class.id
         ships["class"][ship_class.name]["name"] = ship_class.name
         ships["class"][ship_class.name]["type_id"] = ship_class.eve_group__id
         ships["class"][ship_class.name]["type_name"] = ship_class.eve_group__name
         ships["class"][ship_class.name]["image"] = eveimageserver.type_icon_url(
             type_id=ship_class.id, size=32
         )
+        ships["class"][ship_class.name]["mass"] = (
+            ship_class.mass * ships["class"][ship_class.name]["count"]
+        )
 
         # Build ship type dict
         ships["type"][ship_class.eve_group__name]["id"] = ship_class.eve_group__id
         ships["type"][ship_class.eve_group__name]["name"] = ship_class.eve_group__name
 
     # Pilots
     pilot_details = _get_character_info(scan_data=list(set(pilots)))
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.css` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.css`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css.map` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js.map` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js.map` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js.map` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,21 @@
-/* global aaIntelToolJsL10n, aaIntelToolJsOptions, addDscanHightlight, removeDscanHightlight, changeDscanStickyHighlight, fetchAjaxData, shipInfoPanel */
+/* global aaIntelToolJsL10n, aaIntelToolJsOptions, addDscanHightlight, removeDscanHightlight, changeDscanStickyHighlight, fetchAjaxData, shipInfoPanel, Intl */
 
 $(() => {
     'use strict';
 
     const elementShipClassesAllTable = $('table.aa-intel-dscan-ship-classes-all-list');
     const elementDscanCountAll = $('span#aa-intel-dscan-all-count');
+    const elementDscanMassAll = $('span#aa-intel-dscan-all-mass');
     const elementShipClassesOngridTable = $('table.aa-intel-dscan-ship-classes-ongrid-list');
     const elementDscanCountOngrid = $('span#aa-intel-dscan-ongrid-count');
+    const elementDscanMassOnGrid = $('span#aa-intel-dscan-ongrid-mass');
     const elementShipClassesOffgridTable = $('table.aa-intel-dscan-ship-classes-offgrid-list');
     const elementDscanCountOffgrid = $('span#aa-intel-dscan-offgrid-count');
+    const elementDscanMassOffGrid = $('span#aa-intel-dscan-offgrid-mass');
     const elementShipTypesTable = $('table.aa-intel-dscan-ship-types-list');
     const elementUpwellStructuresTable = $('table.aa-intel-dscan-upwell-structures-list');
     const elementDscanCountUpwellStructures = $('span#aa-intel-dscan-upwell-structures-count');
     const elementDeployablesTable = $('table.aa-intel-dscan-deployables-list');
     const elementDscanCountDeployables = $('span#aa-intel-dscan-deployables-count');
     const elementStarbasesTable = $('table.aa-intel-dscan-starbases-list');
     const elementDscanCountStarbases = $('span#aa-intel-dscan-starbases-count');
@@ -68,14 +71,24 @@
                     createdRow: (row, data) => {
                         // D-Scan total count
                         const currentTotal = elementDscanCountAll.html();
                         const newTotal = parseInt(currentTotal) + data.count;
 
                         elementDscanCountAll.html(newTotal);
 
+                        const currentMass = elementDscanMassAll.data('mass') || 0;
+                        const newMass = parseInt(currentMass) + data.mass;
+
+                        elementDscanMassAll.data('mass', newMass);
+                        elementDscanMassAll.html(
+                            new Intl.NumberFormat(
+                                aaIntelToolJsL10n.language
+                            ).format(newMass)
+                        );
+
                         $(row)
                             .attr('data-shipclass-id', data.id)
                             .attr('data-shiptype-id', data.type_id);
 
                         // Highlight
                         $(row).mouseenter(() => {
                             addDscanHightlight('shipclass', $(row));
@@ -150,14 +163,24 @@
                     createdRow: (row, data) => {
                         // D-Scan total count
                         const currentTotal = elementDscanCountOngrid.html();
                         const newTotal = parseInt(currentTotal) + data.count;
 
                         elementDscanCountOngrid.html(newTotal);
 
+                        const currentMass = elementDscanMassOnGrid.data('mass') || 0;
+                        const newMass = parseInt(currentMass) + data.mass;
+
+                        elementDscanMassOnGrid.data('mass', newMass);
+                        elementDscanMassOnGrid.html(
+                            new Intl.NumberFormat(
+                                aaIntelToolJsL10n.language
+                            ).format(newMass)
+                        );
+
                         $(row)
                             .attr('data-shipclass-id', data.id)
                             .attr('data-shiptype-id', data.type_id);
 
                         // Highlight
                         $(row).mouseenter(() => {
                             addDscanHightlight('shipclass', $(row));
@@ -232,14 +255,24 @@
                     createdRow: (row, data) => {
                         // D-Scan total count
                         const currentTotal = elementDscanCountOffgrid.html();
                         const newTotal = parseInt(currentTotal) + data.count;
 
                         elementDscanCountOffgrid.html(newTotal);
 
+                        const currentMass = elementDscanMassOffGrid.data('mass') || 0;
+                        const newMass = parseInt(currentMass) + data.mass;
+
+                        elementDscanMassOffGrid.data('mass', newMass);
+                        elementDscanMassOffGrid.html(
+                            new Intl.NumberFormat(
+                                aaIntelToolJsL10n.language
+                            ).format(newMass)
+                        );
+
                         $(row)
                             .attr('data-shipclass-id', data.id)
                             .attr('data-shiptype-id', data.type_id);
 
                         // Highlight
                         $(row).mouseenter(() => {
                             addDscanHightlight('shipclass', $(row));
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,25 @@
 $(() => {
     "use strict";
     const e = $("table.aa-intel-dscan-ship-classes-all-list"),
-        l = $("span#aa-intel-dscan-all-count"),
+        o = $("span#aa-intel-dscan-all-count"),
+        i = $("span#aa-intel-dscan-all-mass"),
         t = $("table.aa-intel-dscan-ship-classes-ongrid-list"),
-        n = $("span#aa-intel-dscan-ongrid-count"),
+        d = $("span#aa-intel-dscan-ongrid-count"),
+        r = $("span#aa-intel-dscan-ongrid-mass"),
         s = $("table.aa-intel-dscan-ship-classes-offgrid-list"),
-        i = $("span#aa-intel-dscan-offgrid-count"),
-        o = $("table.aa-intel-dscan-ship-types-list"),
-        d = $("table.aa-intel-dscan-upwell-structures-list"),
-        r = $("span#aa-intel-dscan-upwell-structures-count"),
-        c = $("table.aa-intel-dscan-deployables-list"),
-        h = $("span#aa-intel-dscan-deployables-count"),
-        g = $("table.aa-intel-dscan-starbases-list"),
-        p = $("span#aa-intel-dscan-starbases-count");
+        c = $("span#aa-intel-dscan-offgrid-count"),
+        g = $("span#aa-intel-dscan-offgrid-mass"),
+        l = $("table.aa-intel-dscan-ship-types-list"),
+        n = $("table.aa-intel-dscan-upwell-structures-list"),
+        h = $("span#aa-intel-dscan-upwell-structures-count"),
+        m = $("table.aa-intel-dscan-deployables-list"),
+        p = $("span#aa-intel-dscan-deployables-count"),
+        u = $("table.aa-intel-dscan-starbases-list"),
+        b = $("span#aa-intel-dscan-starbases-count");
     fetchAjaxData(aaIntelToolJsOptions.ajax.getShipClassesAll).then(a => {
         a && ($("div.aa-intel-loading-table-info-all").addClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-all").removeClass("d-none") : ($("div.table-dscan-ship-classes-all").removeClass("d-none"), e.DataTable({
             data: a,
             paging: !1,
             language: aaIntelToolJsL10n.dataTables.translation,
             lengthChange: !1,
             dom: "<'row'<'col-sm-12'f>><'row'<'col-sm-12'tr>><'row'<'col-sm-12'i>>",
@@ -42,17 +45,19 @@
                     $(a).addClass("text-end")
                 }
             }, {
                 targets: 2,
                 visible: !1
             }],
             createdRow: (t, a) => {
-                const e = l.html(),
-                    s = parseInt(e) + a.count;
-                l.html(s), $(t).attr("data-shipclass-id", a.id).attr("data-shiptype-id", a.type_id), $(t).mouseenter(() => {
+                const e = o.html(),
+                    s = parseInt(e) + a.count,
+                    l = (o.html(s), i.data("mass") || 0),
+                    n = parseInt(l) + a.mass;
+                i.data("mass", n), i.html(new Intl.NumberFormat(aaIntelToolJsL10n.language).format(n)), $(t).attr("data-shipclass-id", a.id).attr("data-shiptype-id", a.type_id), $(t).mouseenter(() => {
                     addDscanHightlight("shipclass", $(t))
                 }).mouseleave(() => {
                     removeDscanHightlight("shipclass", $(t))
                 }), $(t).click(a => {
                     const e = $(a.target);
                     e.hasClass("aa-intel-information-link") ? a.stopPropagation() : changeDscanStickyHighlight("shipclass", $(t))
                 })
@@ -87,17 +92,19 @@
                     $(a).addClass("text-end")
                 }
             }, {
                 targets: 2,
                 visible: !1
             }],
             createdRow: (t, a) => {
-                const e = n.html(),
-                    s = parseInt(e) + a.count;
-                n.html(s), $(t).attr("data-shipclass-id", a.id).attr("data-shiptype-id", a.type_id), $(t).mouseenter(() => {
+                const e = d.html(),
+                    s = parseInt(e) + a.count,
+                    l = (d.html(s), r.data("mass") || 0),
+                    n = parseInt(l) + a.mass;
+                r.data("mass", n), r.html(new Intl.NumberFormat(aaIntelToolJsL10n.language).format(n)), $(t).attr("data-shipclass-id", a.id).attr("data-shiptype-id", a.type_id), $(t).mouseenter(() => {
                     addDscanHightlight("shipclass", $(t))
                 }).mouseleave(() => {
                     removeDscanHightlight("shipclass", $(t))
                 }), $(t).click(a => {
                     const e = $(a.target);
                     e.hasClass("aa-intel-information-link") ? a.stopPropagation() : changeDscanStickyHighlight("shipclass", $(t))
                 })
@@ -132,28 +139,30 @@
                     $(a).addClass("text-end")
                 }
             }, {
                 targets: 2,
                 visible: !1
             }],
             createdRow: (t, a) => {
-                const e = i.html(),
-                    s = parseInt(e) + a.count;
-                i.html(s), $(t).attr("data-shipclass-id", a.id).attr("data-shiptype-id", a.type_id), $(t).mouseenter(() => {
+                const e = c.html(),
+                    s = parseInt(e) + a.count,
+                    l = (c.html(s), g.data("mass") || 0),
+                    n = parseInt(l) + a.mass;
+                g.data("mass", n), g.html(new Intl.NumberFormat(aaIntelToolJsL10n.language).format(n)), $(t).attr("data-shipclass-id", a.id).attr("data-shiptype-id", a.type_id), $(t).mouseenter(() => {
                     addDscanHightlight("shipclass", $(t))
                 }).mouseleave(() => {
                     removeDscanHightlight("shipclass", $(t))
                 }), $(t).click(a => {
                     const e = $(a.target);
                     e.hasClass("aa-intel-information-link") ? a.stopPropagation() : changeDscanStickyHighlight("shipclass", $(t))
                 })
             }
         })))
     }), fetchAjaxData(aaIntelToolJsOptions.ajax.getShipTypes).then(a => {
-        a && ($("div.aa-intel-loading-table-info-ship-types").addClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-ship-types").removeClass("d-none") : ($("div.table-dscan-ship-types").removeClass("d-none"), o.DataTable({
+        a && ($("div.aa-intel-loading-table-info-ship-types").addClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-ship-types").removeClass("d-none") : ($("div.table-dscan-ship-types").removeClass("d-none"), l.DataTable({
             data: a,
             paging: !1,
             language: aaIntelToolJsL10n.dataTables.translation,
             lengthChange: !1,
             dom: "<'row'<'col-sm-12'f>><'row'<'col-sm-12'tr>><'row'<'col-sm-12'i>>",
             columns: [{
                 data: "name"
@@ -178,15 +187,15 @@
                 }), $(t).click(a => {
                     const e = $(a.target);
                     e.hasClass("aa-intel-information-link") ? a.stopPropagation() : changeDscanStickyHighlight("shiptype", $(t))
                 })
             }
         })))
     }), fetchAjaxData(aaIntelToolJsOptions.ajax.getStructuresOnGrid).then(a => {
-        a && ($("div.aa-intel-loading-table-info-upwell-structures").addClass("d-none"), $("div#aa-intel-dscan-row-interesting-on-grid").removeClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-upwell-structures").removeClass("d-none") : ($("div.col-aa-intel-upwell-structures").removeClass("d-none"), d.DataTable({
+        a && ($("div.aa-intel-loading-table-info-upwell-structures").addClass("d-none"), $("div#aa-intel-dscan-row-interesting-on-grid").removeClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-upwell-structures").removeClass("d-none") : ($("div.col-aa-intel-upwell-structures").removeClass("d-none"), n.DataTable({
             data: a,
             paging: !1,
             language: aaIntelToolJsL10n.dataTables.translation,
             lengthChange: !1,
             dom: "<'row'<'col-sm-12'f>><'row'<'col-sm-12'tr>><'row'<'col-sm-12'i>>",
             columns: [{
                 data: a => shipInfoPanel(a)
@@ -200,25 +209,25 @@
                 targets: 1,
                 width: 45,
                 createdCell: a => {
                     $(a).addClass("text-end")
                 }
             }],
             createdRow: (a, e) => {
-                const t = r.html(),
+                const t = h.html(),
                     s = parseInt(t) + e.count;
-                r.html(s), $(a).attr("data-shiptype-id", e.id), $(a).mouseenter(() => {
+                h.html(s), $(a).attr("data-shiptype-id", e.id), $(a).mouseenter(() => {
                     $(a).addClass("aa-intel-highlight")
                 }).mouseleave(() => {
                     $(a).removeClass("aa-intel-highlight")
                 })
             }
         })))
     }), fetchAjaxData(aaIntelToolJsOptions.ajax.getDeployablesOnGrid).then(a => {
-        a && ($("div.aa-intel-loading-table-info-deployables").addClass("d-none"), $("div#aa-intel-dscan-row-interesting-on-grid").removeClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-deployables").removeClass("d-none") : ($("div.col-aa-intel-deployables").removeClass("d-none"), c.DataTable({
+        a && ($("div.aa-intel-loading-table-info-deployables").addClass("d-none"), $("div#aa-intel-dscan-row-interesting-on-grid").removeClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-deployables").removeClass("d-none") : ($("div.col-aa-intel-deployables").removeClass("d-none"), m.DataTable({
             data: a,
             paging: !1,
             language: aaIntelToolJsL10n.dataTables.translation,
             lengthChange: !1,
             dom: "<'row'<'col-sm-12'f>><'row'<'col-sm-12'tr>><'row'<'col-sm-12'i>>",
             columns: [{
                 data: a => shipInfoPanel(a)
@@ -232,25 +241,25 @@
                 targets: 1,
                 width: 45,
                 createdCell: a => {
                     $(a).addClass("text-end")
                 }
             }],
             createdRow: (a, e) => {
-                const t = h.html(),
+                const t = p.html(),
                     s = parseInt(t) + e.count;
-                h.html(s), $(a).attr("data-shiptype-id", e.id), $(a).mouseenter(() => {
+                p.html(s), $(a).attr("data-shiptype-id", e.id), $(a).mouseenter(() => {
                     $(a).addClass("aa-intel-highlight")
                 }).mouseleave(() => {
                     $(a).removeClass("aa-intel-highlight")
                 })
             }
         })))
     }), fetchAjaxData(aaIntelToolJsOptions.ajax.getStarbasesOnGrid).then(a => {
-        a && ($("div.aa-intel-loading-table-info-starbases").addClass("d-none"), $("div#aa-intel-dscan-row-interesting-on-grid").removeClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-starbases").removeClass("d-none") : ($("div.col-aa-intel-starbases").removeClass("d-none"), g.DataTable({
+        a && ($("div.aa-intel-loading-table-info-starbases").addClass("d-none"), $("div#aa-intel-dscan-row-interesting-on-grid").removeClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-starbases").removeClass("d-none") : ($("div.col-aa-intel-starbases").removeClass("d-none"), u.DataTable({
             data: a,
             paging: !1,
             language: aaIntelToolJsL10n.dataTables.translation,
             lengthChange: !1,
             dom: "<'row'<'col-sm-12'f>><'row'<'col-sm-12'tr>><'row'<'col-sm-12'i>>",
             columns: [{
                 data: a => shipInfoPanel(a)
@@ -264,17 +273,17 @@
                 targets: 1,
                 width: 45,
                 createdCell: a => {
                     $(a).addClass("text-end")
                 }
             }],
             createdRow: (a, e) => {
-                const t = p.html(),
+                const t = b.html(),
                     s = parseInt(t) + e.count;
-                p.html(s), $(a).attr("data-shiptype-id", e.id), $(a).mouseenter(() => {
+                b.html(s), $(a).attr("data-shiptype-id", e.id), $(a).mouseenter(() => {
                     $(a).addClass("aa-intel-highlight")
                 }).mouseleave(() => {
                     $(a).removeClass("aa-intel-highlight")
                 })
             }
         })))
     })
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js.map` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js.map`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8605769230769231%*

 * *Differences: {"'mappings'": "'AAEAA,EAAE,KACE,aAEA,MAAMC,EAA6BD,EAAE,4CAA4C,EAC3EE,EAAuBF,EAAE,+BAA+B,EACxDG,EAAsBH,EAAE,8BAA8B,EACtDI,EAAgCJ,EAAE,+CAA+C,EACjFK,EAA0BL,EAAE,kCAAkC,EAC9DM,EAAyBN,EAAE,iCAAiC,EAC5DO,EAAiCP,EAAE,gDAAgD,EACnFQ,EAA2BR,EAAE,mCAAmC,EAChES,EAA0BT,EAAE,kCAAkC,EAC9DU,EAAwBV,EAAE,sCAAsC,EAChEW,EAA+BX,EAAE,6CAA6C,EAC9EY,EAAoCZ,EAAE,6CAA6C,EACnFa,EAA0Bb,EAAE,uCAAuC,EACnEc,EAA+Bd,EAAE,uCAAuC,EACxEe,EAAwBf,EAAE,qCAAqC,EAC/DgB,EAA6BhB,EAAE,qCAAqC,EAM1EiB,cAAcC,qBAAqBC,KAAKC,iBAAiB,EAAEC,KAAKC,IACxDA,IAC […]*

```diff
@@ -1,17 +1,20 @@
 {
-    "mappings": "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",
+    "mappings": "AAEAA,EAAE,KACE,aAEA,MAAMC,EAA6BD,EAAE,4CAA4C,EAC3EE,EAAuBF,EAAE,+BAA+B,EACxDG,EAAsBH,EAAE,8BAA8B,EACtDI,EAAgCJ,EAAE,+CAA+C,EACjFK,EAA0BL,EAAE,kCAAkC,EAC9DM,EAAyBN,EAAE,iCAAiC,EAC5DO,EAAiCP,EAAE,gDAAgD,EACnFQ,EAA2BR,EAAE,mCAAmC,EAChES,EAA0BT,EAAE,kCAAkC,EAC9DU,EAAwBV,EAAE,sCAAsC,EAChEW,EAA+BX,EAAE,6CAA6C,EAC9EY,EAAoCZ,EAAE,6CAA6C,EACnFa,EAA0Bb,EAAE,uCAAuC,EACnEc,EAA+Bd,EAAE,uCAAuC,EACxEe,EAAwBf,EAAE,qCAAqC,EAC/DgB,EAA6BhB,EAAE,qCAAqC,EAM1EiB,cAAcC,qBAAqBC,KAAKC,iBAAiB,EAAEC,KAAKC,IACxDA,IACAtB,EAAE,qCAAqC,EAAEuB,SAAS,QAAQ,EAEpB,IAAlCC,OAAOC,KAAKH,CAAS,EAAEI,OACvB1B,EAAE,mCAAmC,EAAE2B,YAAY,QAAQ,GAE3D3B,EAAE,kCAAkC,EAAE2B,YAAY,QAAQ,EAE1D1B,EAA2B2B,UAAU,CACjCC,KAAMP,EACNQ,OAAQ,CAAA,EACRC,SAAUC,kBAAkBC,WAAWC,YACvCC,aAAc,CAAA,EACdC,IACI,mEAGJC,QAAS,CACL,CACIR,KAAM,GACKS,cAAcT,CAAI,CAEjC,EACA,CACIA,KAAM,OACV,EACA,CACIA,KAAM,WACV,GAEJU,MAAO,CACH,CAAC,EAAG,SAERC,WAAY,CACR,CACIC,QAAS,EACTC,YAAa,IACT1C,EAAE2C,CAAE,EAAEpB,SAAS,eAAe,CAClC,CACJ,EACA,CACIkB,QAAS,EACTG,MAAO,GACPF,YAAa,IACT1C,EAAE2C,CAAE,EAAEpB,SAAS,UAAU,CAC7B,CACJ,EACA,CACIkB,QAAS,EACTI,QAAS,CAAA,CACb,GAEJC,WAAY,CAACC,EAAKlB,KAEd,MAAMmB,EAAe9C,EAAqB+C,KAAK,EACzCC,EAAWC,SAASH,CAAY,EAAInB,EAAKuB,MAIzCC,GAFNnD,EAAqB+C,KAAKC,CAAQ,EAEd/C,EAAoB0B,KAAK,MAAM,GAAK,GAClDyB,EAAUH,SAASE,CAAW,EAAIxB,EAAK0B,KAE7CpD,EAAoB0B,KAAK,OAAQyB,CAAO,EACxCnD,EAAoB8C,KAChB,IAAIO,KAAKC,aACLzB,kBAAkBD,QACtB,EAAE2B,OAAOJ,CAAO,CACpB,EAEAtD,EAAE+C,CAAG,EACAY,KAAK,oBAAqB9B,EAAK+B,EAAE,EACjCD,KAAK,mBAAoB9B,EAAKgC,OAAO,EAG1C7D,EAAE+C,CAAG,EAAEe,WAAW,KACdC,mBAAmB,YAAa/D,EAAE+C,CAAG,CAAC,CAC1C,CAAC,EAAEiB,WAAW,KACVC,sBAAsB,YAAajE,EAAE+C,CAAG,CAAC,CAC7C,CAAC,EAGD/C,EAAE+C,CAAG,EAAEmB,MAAM,IACT,MAAMC,EAASnE,EAAEoE,EAAMD,MAAM,EAEzBA,EAAOE,SAAS,2BAA2B,EAC3CD,EAAME,gBAAgB,EAEtBC,2BAA2B,YAAavE,EAAE+C,CAAG,CAAC,CAEtD,CAAC,CACL,CACJ,CAAC,GAGb,CAAC,EAMD9B,cAAcC,qBAAqBC,KAAKqD,oBAAoB,EAAEnD,KAAKC,IAC3DA,IACAtB,EAAE,wCAAwC,EAAEuB,SAAS,QAAQ,EAEvB,IAAlCC,OAAOC,KAAKH,CAAS,EAAEI,OACvB1B,EAAE,sCAAsC,EAAE2B,YAAY,QAAQ,GAE9D3B,EAAE,qCAAqC,EAAE2B,YAAY,QAAQ,EAE7DvB,EAA8BwB,UAAU,CACpCC,KAAMP,EACNQ,OAAQ,CAAA,EACRC,SAAUC,kBAAkBC,WAAWC,YACvCC,aAAc,CAAA,EACdC,IACI,mEAGJC,QAAS,CACL,CACIR,KAAM,GACKS,cAAcT,CAAI,CAEjC,EACA,CACIA,KAAM,OACV,EACA,CACIA,KAAM,WACV,GAEJU,MAAO,CACH,CAAC,EAAG,SAERC,WAAY,CACR,CACIC,QAAS,EACTC,YAAa,IACT1C,EAAE2C,CAAE,EAAEpB,SAAS,eAAe,CAClC,CACJ,EACA,CACIkB,QAAS,EACTG,MAAO,GACPF,YAAa,IACT1C,EAAE2C,CAAE,EAAEpB,SAAS,UAAU,CAC7B,CACJ,EACA,CACIkB,QAAS,EACTI,QAAS,CAAA,CACb,GAEJC,WAAY,CAACC,EAAKlB,KAEd,MAAMmB,EAAe3C,EAAwB4C,KAAK,EAC5CC,EAAWC,SAASH,CAAY,EAAInB,EAAKuB,MAIzCC,GAFNhD,EAAwB4C,KAAKC,CAAQ,EAEjB5C,EAAuBuB,KAAK,MAAM,GAAK,GACrDyB,EAAUH,SAASE,CAAW,EAAIxB,EAAK0B,KAE7CjD,EAAuBuB,KAAK,OAAQyB,CAAO,EAC3ChD,EAAuB2C,KACnB,IAAIO,KAAKC,aACLzB,kBAAkBD,QACtB,EAAE2B,OAAOJ,CAAO,CACpB,EAEAtD,EAAE+C,CAAG,EACAY,KAAK,oBAAqB9B,EAAK+B,EAAE,EACjCD,KAAK,mBAAoB9B,EAAKgC,OAAO,EAG1C7D,EAAE+C,CAAG,EAAEe,WAAW,KACdC,mBAAmB,YAAa/D,EAAE+C,CAAG,CAAC,CAC1C,CAAC,EAAEiB,WAAW,KACVC,sBAAsB,YAAajE,EAAE+C,CAAG,CAAC,CAC7C,CAAC,EAGD/C,EAAE+C,CAAG,EAAEmB,MAAM,IACT,MAAMC,EAASnE,EAAEoE,EAAMD,MAAM,EAEzBA,EAAOE,SAAS,2BAA2B,EAC3CD,EAAME,gBAAgB,EAEtBC,2BAA2B,YAAavE,EAAE+C,CAAG,CAAC,CAEtD,CAAC,CACL,CACJ,CAAC,GAGb,CAAC,EAMD9B,cAAcC,qBAAqBC,KAAKsD,qBAAqB,EAAEpD,KAAKC,IAC5DA,IACAtB,EAAE,yCAAyC,EAAEuB,SAAS,QAAQ,EAExB,IAAlCC,OAAOC,KAAKH,CAAS,EAAEI,OACvB1B,EAAE,uCAAuC,EAAE2B,YAAY,QAAQ,GAE/D3B,EAAE,sCAAsC,EAAE2B,YAAY,QAAQ,EAE9DpB,EAA+BqB,UAAU,CACrCC,KAAMP,EACNQ,OAAQ,CAAA,EACRC,SAAUC,kBAAkBC,WAAWC,YACvCC,aAAc,CAAA,EACdC,IACI,mEAGJC,QAAS,CACL,CACIR,KAAM,GACKS,cAAcT,CAAI,CAEjC,EACA,CACIA,KAAM,OACV,EACA,CACIA,KAAM,WACV,GAEJU,MAAO,CACH,CAAC,EAAG,SAERC,WAAY,CACR,CACIC,QAAS,EACTC,YAAa,IACT1C,EAAE2C,CAAE,EAAEpB,SAAS,eAAe,CAClC,CACJ,EACA,CACIkB,QAAS,EACTG,MAAO,GACPF,YAAa,IACT1C,EAAE2C,CAAE,EAAEpB,SAAS,UAAU,CAC7B,CACJ,EACA,CACIkB,QAAS,EACTI,QAAS,CAAA,CACb,GAEJC,WAAY,CAACC,EAAKlB,KAEd,MAAMmB,EAAexC,EAAyByC,KAAK,EAC7CC,EAAWC,SAASH,CAAY,EAAInB,EAAKuB,MAIzCC,GAFN7C,EAAyByC,KAAKC,CAAQ,EAElBzC,EAAwBoB,KAAK,MAAM,GAAK,GACtDyB,EAAUH,SAASE,CAAW,EAAIxB,EAAK0B,KAE7C9C,EAAwBoB,KAAK,OAAQyB,CAAO,EAC5C7C,EAAwBwC,KACpB,IAAIO,KAAKC,aACLzB,kBAAkBD,QACtB,EAAE2B,OAAOJ,CAAO,CACpB,EAEAtD,EAAE+C,CAAG,EACAY,KAAK,oBAAqB9B,EAAK+B,EAAE,EACjCD,KAAK,mBAAoB9B,EAAKgC,OAAO,EAG1C7D,EAAE+C,CAAG,EAAEe,WAAW,KACdC,mBAAmB,YAAa/D,EAAE+C,CAAG,CAAC,CAC1C,CAAC,EAAEiB,WAAW,KACVC,sBAAsB,YAAajE,EAAE+C,CAAG,CAAC,CAC7C,CAAC,EAGD/C,EAAE+C,CAAG,EAAEmB,MAAM,IACT,MAAMC,EAASnE,EAAEoE,EAAMD,MAAM,EAEzBA,EAAOE,SAAS,2BAA2B,EAC3CD,EAAME,gBAAgB,EAEtBC,2BAA2B,YAAavE,EAAE+C,CAAG,CAAC,CAEtD,CAAC,CACL,CACJ,CAAC,GAGb,CAAC,EAMD9B,cAAcC,qBAAqBC,KAAKuD,YAAY,EAAErD,KAAKC,IACnDA,IACAtB,EAAE,4CAA4C,EAAEuB,SAAS,QAAQ,EAE3B,IAAlCC,OAAOC,KAAKH,CAAS,EAAEI,OACvB1B,EAAE,0CAA0C,EAAE2B,YAAY,QAAQ,GAElE3B,EAAE,4BAA4B,EAAE2B,YAAY,QAAQ,EAEpDjB,EAAsBkB,UAAU,CAC5BC,KAAMP,EACNQ,OAAQ,CAAA,EACRC,SAAUC,kBAAkBC,WAAWC,YACvCC,aAAc,CAAA,EACdC,IACI,mEAGJC,QAAS,CACL,CACIR,KAAM,MACV,EACA,CACIA,KAAM,OACV,GAEJU,MAAO,CACH,CAAC,EAAG,SAERC,WAAY,CACR,CACIC,QAAS,EACTG,MAAO,GACPF,YAAa,IACT1C,EAAE2C,CAAE,EAAEpB,SAAS,UAAU,CAC7B,CACJ,GAEJuB,WAAY,CAACC,EAAKlB,KACd7B,EAAE+C,CAAG,EAAEY,KAAK,mBAAoB9B,EAAK+B,EAAE,EAGvC5D,EAAE+C,CAAG,EAAEe,WAAW,KACdC,mBAAmB,WAAY/D,EAAE+C,CAAG,CAAC,CACzC,CAAC,EAAEiB,WAAW,KACVC,sBAAsB,WAAYjE,EAAE+C,CAAG,CAAC,CAC5C,CAAC,EAGD/C,EAAE+C,CAAG,EAAEmB,MAAM,IACT,MAAMC,EAASnE,EAAEoE,EAAMD,MAAM,EAEzBA,EAAOE,SAAS,2BAA2B,EAC3CD,EAAME,gBAAgB,EAEtBC,2BAA2B,WAAYvE,EAAE+C,CAAG,CAAC,CAErD,CAAC,CACL,CACJ,CAAC,GAGb,CAAC,EAMD9B,cAAcC,qBAAqBC,KAAKwD,mBAAmB,EAAEtD,KAAKC,IAC1DA,IACAtB,EAAE,mDAAmD,EAAEuB,SAAS,QAAQ,EACxEvB,EAAE,4CAA4C,EAAE2B,YAAY,QAAQ,EAE9B,IAAlCH,OAAOC,KAAKH,CAAS,EAAEI,OACvB1B,EAAE,iDAAiD,EAAE2B,YAAY,QAAQ,GAEzE3B,EAAE,oCAAoC,EAAE2B,YAAY,QAAQ,EAE5DhB,EAA6BiB,UAAU,CACnCC,KAAMP,EACNQ,OAAQ,CAAA,EACRC,SAAUC,kBAAkBC,WAAWC,YACvCC,aAAc,CAAA,EACdC,IACI,mEAGJC,QAAS,CACL,CACIR,KAAM,GACKS,cAAcT,CAAI,CAEjC,EACA,CACIA,KAAM,OACV,GAEJU,MAAO,CACH,CAAC,EAAG,SAERC,WAAY,CACR,CACIC,QAAS,EACTG,MAAO,GACPF,YAAa,IACT1C,EAAE2C,CAAE,EAAEpB,SAAS,UAAU,CAC7B,CACJ,GAEJuB,WAAY,CAACC,EAAKlB,KAEd,MAAMmB,EAAepC,EAAkCqC,KAAK,EACtDC,EAAWC,SAASH,CAAY,EAAInB,EAAKuB,MAE/CxC,EAAkCqC,KAAKC,CAAQ,EAE/ClD,EAAE+C,CAAG,EAAEY,KAAK,mBAAoB9B,EAAK+B,EAAE,EAGvC5D,EAAE+C,CAAG,EAAEe,WAAW,KACd9D,EAAE+C,CAAG,EAAExB,SAAS,oBAAoB,CACxC,CAAC,EAAEyC,WAAW,KACVhE,EAAE+C,CAAG,EAAEpB,YAAY,oBAAoB,CAC3C,CAAC,CACL,CACJ,CAAC,GAGb,CAAC,EAMDV,cAAcC,qBAAqBC,KAAKyD,oBAAoB,EAAEvD,KAAKC,IAC3DA,IACAtB,EAAE,6CAA6C,EAAEuB,SAAS,QAAQ,EAClEvB,EAAE,4CAA4C,EAAE2B,YAAY,QAAQ,EAE9B,IAAlCH,OAAOC,KAAKH,CAAS,EAAEI,OACvB1B,EAAE,2CAA2C,EAAE2B,YAAY,QAAQ,GAEnE3B,EAAE,8BAA8B,EAAE2B,YAAY,QAAQ,EAEtDd,EAAwBe,UAAU,CAC9BC,KAAMP,EACNQ,OAAQ,CAAA,EACRC,SAAUC,kBAAkBC,WAAWC,YACvCC,aAAc,CAAA,EACdC,IACI,mEAGJC,QAAS,CACL,CACIR,KAAM,GACKS,cAAcT,CAAI,CAEjC,EACA,CACIA,KAAM,OACV,GAEJU,MAAO,CACH,CAAC,EAAG,SAERC,WAAY,CACR,CACIC,QAAS,EACTG,MAAO,GACPF,YAAa,IACT1C,EAAE2C,CAAE,EAAEpB,SAAS,UAAU,CAC7B,CACJ,GAEJuB,WAAY,CAACC,EAAKlB,KAEd,MAAMmB,EAAelC,EAA6BmC,KAAK,EACjDC,EAAWC,SAASH,CAAY,EAAInB,EAAKuB,MAE/CtC,EAA6BmC,KAAKC,CAAQ,EAE1ClD,EAAE+C,CAAG,EAAEY,KAAK,mBAAoB9B,EAAK+B,EAAE,EAGvC5D,EAAE+C,CAAG,EAAEe,WAAW,KACd9D,EAAE+C,CAAG,EAAExB,SAAS,oBAAoB,CACxC,CAAC,EAAEyC,WAAW,KACVhE,EAAE+C,CAAG,EAAEpB,YAAY,oBAAoB,CAC3C,CAAC,CACL,CACJ,CAAC,GAGb,CAAC,EAMDV,cAAcC,qBAAqBC,KAAK0D,kBAAkB,EAAExD,KAAKC,IACzDA,IACAtB,EAAE,2CAA2C,EAAEuB,SAAS,QAAQ,EAChEvB,EAAE,4CAA4C,EAAE2B,YAAY,QAAQ,EAE9B,IAAlCH,OAAOC,KAAKH,CAAS,EAAEI,OACvB1B,EAAE,yCAAyC,EAAE2B,YAAY,QAAQ,GAEjE3B,EAAE,4BAA4B,EAAE2B,YAAY,QAAQ,EAEpDZ,EAAsBa,UAAU,CAC5BC,KAAMP,EACNQ,OAAQ,CAAA,EACRC,SAAUC,kBAAkBC,WAAWC,YACvCC,aAAc,CAAA,EACdC,IACI,mEAGJC,QAAS,CACL,CACIR,KAAM,GACKS,cAAcT,CAAI,CAEjC,EACA,CACIA,KAAM,OACV,GAEJU,MAAO,CACH,CAAC,EAAG,SAERC,WAAY,CACR,CACIC,QAAS,EACTG,MAAO,GACPF,YAAa,IACT1C,EAAE2C,CAAE,EAAEpB,SAAS,UAAU,CAC7B,CACJ,GAEJuB,WAAY,CAACC,EAAKlB,KAEd,MAAMmB,EAAehC,EAA2BiC,KAAK,EAC/CC,EAAWC,SAASH,CAAY,EAAInB,EAAKuB,MAE/CpC,EAA2BiC,KAAKC,CAAQ,EAExClD,EAAE+C,CAAG,EAAEY,KAAK,mBAAoB9B,EAAK+B,EAAE,EAGvC5D,EAAE+C,CAAG,EAAEe,WAAW,KACd9D,EAAE+C,CAAG,EAAExB,SAAS,oBAAoB,CACxC,CAAC,EAAEyC,WAAW,KACVhE,EAAE+C,CAAG,EAAEpB,YAAY,oBAAoB,CAC3C,CAAC,CACL,CACJ,CAAC,GAGb,CAAC,CACL,CAAC",
     "names": [
         "$",
         "elementShipClassesAllTable",
         "elementDscanCountAll",
+        "elementDscanMassAll",
         "elementShipClassesOngridTable",
         "elementDscanCountOngrid",
+        "elementDscanMassOnGrid",
         "elementShipClassesOffgridTable",
         "elementDscanCountOffgrid",
+        "elementDscanMassOffGrid",
         "elementShipTypesTable",
         "elementUpwellStructuresTable",
         "elementDscanCountUpwellStructures",
         "elementDeployablesTable",
         "elementDscanCountDeployables",
         "elementStarbasesTable",
         "elementDscanCountStarbases",
@@ -47,14 +50,20 @@
         "createdRow",
         "row",
         "currentTotal",
         "html",
         "newTotal",
         "parseInt",
         "count",
+        "currentMass",
+        "newMass",
+        "mass",
+        "Intl",
+        "NumberFormat",
+        "format",
         "attr",
         "id",
         "type_id",
         "mouseenter",
         "addDscanHightlight",
         "mouseleave",
         "removeDscanHightlight",
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js.map` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,14 @@
-/* global fetchAjaxData, aaIntelToolJsOptions, aaIntelToolJsL10n, shipInfoPanel, pilotInfoPanel, addFleetcompositionHightlight, removeFleetcompositionHightlight */
+/* global fetchAjaxData, aaIntelToolJsOptions, aaIntelToolJsL10n, shipInfoPanel, pilotInfoPanel, addFleetcompositionHightlight, removeFleetcompositionHightlight, Intl */
 
 $(() => {
     'use strict';
 
     const elementShipClassesTable = $('table.aa-intel-dscan-ship-classes-ship-classes-list');
+    const elementShipClassesMass = $('span#aa-intel-dscan-ship-classes-mass');
     const elementShipTypesTable = $('table.aa-intel-dscan-ship-types-list');
     const elementFleetcompositionTable = $('table.aa-intel-fleetcomp-pilot-ships-list');
     const elementPilotsCount = $('span#aa-intel-fleet-participation-count');
 
 
     /**
      * Datatable Ship Classes
@@ -53,14 +54,24 @@
                             $(td).addClass('text-end');
                         }
                     }, {
                         targets: 2,
                         visible: false
                     }],
                     createdRow: (row, data) => {
+                        const currentMass = elementShipClassesMass.data('mass') || 0;
+                        const newMass = parseInt(currentMass) + data.mass;
+
+                        elementShipClassesMass.data('mass', newMass);
+                        elementShipClassesMass.html(
+                            new Intl.NumberFormat(
+                                aaIntelToolJsL10n.language
+                            ).format(newMass)
+                        );
+
                         $(row)
                             .attr('data-shipclass-id', data.id)
                             .attr('data-shiptype-id', data.type_id);
 
                         // Highlight
                         $(row).mouseenter(() => {
                             addFleetcompositionHightlight('shipclass', $(row));
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,56 +1,59 @@
 $(() => {
     "use strict";
-    const a = $("table.aa-intel-dscan-ship-classes-ship-classes-list"),
+    const e = $("table.aa-intel-dscan-ship-classes-ship-classes-list"),
+        l = $("span#aa-intel-dscan-ship-classes-mass"),
         t = $("table.aa-intel-dscan-ship-types-list"),
         s = $("table.aa-intel-fleetcomp-pilot-ships-list"),
-        l = $("span#aa-intel-fleet-participation-count");
-    fetchAjaxData(aaIntelToolJsOptions.ajax.getShipClasses).then(e => {
-        e && ($("div.aa-intel-loading-table-info-ship-classes").addClass("d-none"), 0 === Object.keys(e).length ? $("div.aa-intel-empty-table-info-ship-classes").removeClass("d-none") : ($("div.table-dscan-ship-classes-ship-classes").removeClass("d-none"), a.DataTable({
-            data: e,
+        i = $("span#aa-intel-fleet-participation-count");
+    fetchAjaxData(aaIntelToolJsOptions.ajax.getShipClasses).then(a => {
+        a && ($("div.aa-intel-loading-table-info-ship-classes").addClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-ship-classes").removeClass("d-none") : ($("div.table-dscan-ship-classes-ship-classes").removeClass("d-none"), e.DataTable({
+            data: a,
             paging: !1,
             language: aaIntelToolJsL10n.dataTables.translation,
             lengthChange: !1,
             dom: "<'row'<'col-sm-12'f>><'row'<'col-sm-12'tr>><'row'<'col-sm-12'i>>",
             columns: [{
-                data: e => shipInfoPanel(e)
+                data: a => shipInfoPanel(a)
             }, {
                 data: "count"
             }, {
                 data: "type_name"
             }],
             order: [
                 [1, "desc"]
             ],
             columnDefs: [{
                 targets: 0,
-                createdCell: e => {
-                    $(e).addClass("text-ellipsis")
+                createdCell: a => {
+                    $(a).addClass("text-ellipsis")
                 }
             }, {
                 targets: 1,
                 width: 45,
-                createdCell: e => {
-                    $(e).addClass("text-end")
+                createdCell: a => {
+                    $(a).addClass("text-end")
                 }
             }, {
                 targets: 2,
                 visible: !1
             }],
-            createdRow: (e, a) => {
-                $(e).attr("data-shipclass-id", a.id).attr("data-shiptype-id", a.type_id), $(e).mouseenter(() => {
-                    addFleetcompositionHightlight("shipclass", $(e))
+            createdRow: (a, e) => {
+                const t = l.data("mass") || 0,
+                    s = parseInt(t) + e.mass;
+                l.data("mass", s), l.html(new Intl.NumberFormat(aaIntelToolJsL10n.language).format(s)), $(a).attr("data-shipclass-id", e.id).attr("data-shiptype-id", e.type_id), $(a).mouseenter(() => {
+                    addFleetcompositionHightlight("shipclass", $(a))
                 }).mouseleave(() => {
-                    removeFleetcompositionHightlight("shipclass", $(e))
+                    removeFleetcompositionHightlight("shipclass", $(a))
                 })
             }
         })))
-    }), fetchAjaxData(aaIntelToolJsOptions.ajax.getShipTypes).then(e => {
-        e && ($("div.aa-intel-loading-table-info-ship-types").addClass("d-none"), 0 === Object.keys(e).length ? $("div.aa-intel-empty-table-info-ship-types").removeClass("d-none") : ($("div.table-dscan-ship-types").removeClass("d-none"), t.DataTable({
-            data: e,
+    }), fetchAjaxData(aaIntelToolJsOptions.ajax.getShipTypes).then(a => {
+        a && ($("div.aa-intel-loading-table-info-ship-types").addClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-ship-types").removeClass("d-none") : ($("div.table-dscan-ship-types").removeClass("d-none"), t.DataTable({
+            data: a,
             paging: !1,
             language: aaIntelToolJsL10n.dataTables.translation,
             lengthChange: !1,
             dom: "<'row'<'col-sm-12'f>><'row'<'col-sm-12'tr>><'row'<'col-sm-12'i>>",
             columns: [{
                 data: "name"
             }, {
@@ -58,55 +61,55 @@
             }],
             order: [
                 [1, "desc"]
             ],
             columnDefs: [{
                 targets: 1,
                 width: 45,
-                createdCell: e => {
-                    $(e).addClass("text-end")
+                createdCell: a => {
+                    $(a).addClass("text-end")
                 }
             }],
-            createdRow: (e, a) => {
-                $(e).attr("data-shiptype-id", a.id), $(e).mouseenter(() => {
-                    addFleetcompositionHightlight("shiptype", $(e))
+            createdRow: (a, e) => {
+                $(a).attr("data-shiptype-id", e.id), $(a).mouseenter(() => {
+                    addFleetcompositionHightlight("shiptype", $(a))
                 }).mouseleave(() => {
-                    removeFleetcompositionHightlight("shiptype", $(e))
+                    removeFleetcompositionHightlight("shiptype", $(a))
                 })
             }
         })))
-    }), fetchAjaxData(aaIntelToolJsOptions.ajax.getFleetComposition).then(e => {
-        e && ($("div.aa-intel-loading-table-info-fleetcomp-pilot-ships").addClass("d-none"), 0 === Object.keys(e).length ? $("div.aa-intel-empty-table-info-fleetcomp-pilot-ships").removeClass("d-none") : ($("div.table-fleetcomp-pilot-ships").removeClass("d-none"), s.DataTable({
-            data: e,
+    }), fetchAjaxData(aaIntelToolJsOptions.ajax.getFleetComposition).then(a => {
+        a && ($("div.aa-intel-loading-table-info-fleetcomp-pilot-ships").addClass("d-none"), 0 === Object.keys(a).length ? $("div.aa-intel-empty-table-info-fleetcomp-pilot-ships").removeClass("d-none") : ($("div.table-fleetcomp-pilot-ships").removeClass("d-none"), s.DataTable({
+            data: a,
             paging: !1,
             language: aaIntelToolJsL10n.dataTables.translation,
             lengthChange: !1,
             dom: "<'row'<'col-sm-12'f>><'row'<'col-sm-12'tr>><'row'<'col-sm-12'i>>",
             columns: [{
-                data: e => pilotInfoPanel(e)
+                data: a => pilotInfoPanel(a)
             }, {
                 data: "ship"
             }, {
                 data: "solarsystem"
             }],
             order: [
                 [0, "asc"]
             ],
             columnDefs: [{
                 targets: 0,
-                createdCell: e => {
-                    $(e).addClass("fix-eve-image-position")
+                createdCell: a => {
+                    $(a).addClass("fix-eve-image-position")
                 }
             }],
-            createdRow: (e, a) => {
-                const t = l.html(),
+            createdRow: (a, e) => {
+                const t = i.html(),
                     s = parseInt(t) + 1;
-                l.html(s), $(e).attr("data-shipclass-id", a.ship_id).attr("data-shiptype-id", a.ship_type_id), $(e).mouseenter(() => {
-                    addFleetcompositionHightlight("shiptype", $(e))
+                i.html(s), $(a).attr("data-shipclass-id", e.ship_id).attr("data-shiptype-id", e.ship_type_id), $(a).mouseenter(() => {
+                    addFleetcompositionHightlight("shiptype", $(a))
                 }).mouseleave(() => {
-                    removeFleetcompositionHightlight("shiptype", $(e))
+                    removeFleetcompositionHightlight("shiptype", $(a))
                 })
             }
         })))
     })
 });
 //# sourceMappingURL=aa-intel-tool-fleetcomposition.min.js.map
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js.map` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js.map`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8524590163934427%*

 * *Differences: {"'mappings'": "'AAEAA,EAAE,KACE,aAEA,MAAMC,EAA0BD,EAAE,qDAAqD,EACjFE,EAAyBF,EAAE,uCAAuC,EAClEG,EAAwBH,EAAE,sCAAsC,EAChEI,EAA+BJ,EAAE,2CAA2C,EAC5EK,EAAqBL,EAAE,yCAAyC,EAMtEM,cAAcC,qBAAqBC,KAAKC,cAAc,EAAEC,KAAKC,IACrDA,IACAX,EAAE,8CAA8C,EAAEY,SAAS,QAAQ,EAE7B,IAAlCC,OAAOC,KAAKH,CAAS,EAAEI,OACvBf,EAAE,4CAA4C,EAAEgB,YAAY,QAAQ,GAEpEhB,EAAE,2CAA2C,EAAEgB,YAAY,QAAQ,EAEnEf,EAAwBgB,UAAU,CAC9BC,KAAMP,EACNQ,OAAQ,CAAA,EACRC,SAAUC,kBAAkBC,WAAWC,YACvCC,aAAc,CAAA,EACdC,IACI,mEAGJC,QAAS,CACL,CACIR,KAAM,GACKS,cAAcT,CAAI,CAE […]*

```diff
@@ -1,12 +1,13 @@
 {
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "$",
         "elementShipClassesTable",
+        "elementShipClassesMass",
         "elementShipTypesTable",
         "elementFleetcompositionTable",
         "elementPilotsCount",
         "fetchAjaxData",
         "aaIntelToolJsOptions",
         "ajax",
         "getShipClasses",
@@ -33,28 +34,34 @@
         "targets",
         "createdCell",
         "td",
         "width",
         "visible",
         "createdRow",
         "row",
+        "currentMass",
+        "newMass",
+        "parseInt",
+        "mass",
+        "html",
+        "Intl",
+        "NumberFormat",
+        "format",
         "attr",
         "id",
         "type_id",
         "mouseenter",
         "addFleetcompositionHightlight",
         "mouseleave",
         "removeFleetcompositionHightlight",
         "getShipTypes",
         "getFleetComposition",
         "pilotInfoPanel",
         "currentTotal",
-        "html",
         "newTotal",
-        "parseInt",
         "ship_id",
         "ship_type_id"
     ],
     "sources": [
         "aa-intel-tool-fleetcomposition.js"
     ],
     "version": 3
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -41,40 +41,40 @@
 };
 
 
 /**
  * Get the link HTML to EveWho for a pilot
  *
  * @param {string} href
- * @returns {`<a class="aa-intel-information-link" href="${string}" target="_blank" rel="noopener noreferer">evewho <sup><small><i class="fas fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`}
+ * @returns {`<a class="aa-intel-information-link" href="${string}" target="_blank" rel="noopener noreferer">evewho <sup><small><i class="fa-solid fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`}
  */
 const eveWhoLinkHtml = (href) => {
-    return `<a class="aa-intel-information-link" href="${href}" target="_blank" rel="noopener noreferer">evewho <sup><small><i class="fas fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`;
+    return `<a class="aa-intel-information-link" href="${href}" target="_blank" rel="noopener noreferer">evewho <sup><small><i class="fa-solid fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`;
 };
 
 
 /**
  * Get the link HTML to zKillboard
  *
  * @param {string} href
- * @returns {`<a class="aa-intel-information-link" href="${string}" target="_blank" rel="noopener noreferer">zkillboard <sup><small><i class="fas fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`}
+ * @returns {`<a class="aa-intel-information-link" href="${string}" target="_blank" rel="noopener noreferer">zkillboard <sup><small><i class="fa-solid fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`}
  */
 const zkillboardLinkHtml = (href) => {
-    return `<a class="aa-intel-information-link" href="${href}" target="_blank" rel="noopener noreferer">zkillboard <sup><small><i class="fas fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`;
+    return `<a class="aa-intel-information-link" href="${href}" target="_blank" rel="noopener noreferer">zkillboard <sup><small><i class="fa-solid fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`;
 };
 
 
 /**
  * Get the link HTML to dotlan
  *
  * @param {string} href
- * @returns {`<a class="aa-intel-information-link" href="${string}" target="_blank" rel="noopener noreferer">dotlan <sup><small><i class="fas fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`}
+ * @returns {`<a class="aa-intel-information-link" href="${string}" target="_blank" rel="noopener noreferer">dotlan <sup><small><i class="fa-solid fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`}
  */
 const dotlanLinkHtml = (href) => {
-    return `<a class="aa-intel-information-link" href="${href}" target="_blank" rel="noopener noreferer">dotlan <sup><small><i class="fas fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`;
+    return `<a class="aa-intel-information-link" href="${href}" target="_blank" rel="noopener noreferer">dotlan <sup><small><i class="fa-solid fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`;
 };
 
 
 /**
  * Pilot info element in datatable
  *
  * @param {Object} pilotData
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,23 @@
 "use strict";
 const fetchAjaxData = async a => fetch(a).then(a => a.ok ? Promise.resolve(a) : Promise.reject(new Error("Failed to load"))).then(a => a.json()).then(a => a).catch(function(a) {
-    console.log("Error: " + a.message)
-}), eveImageHtml = (a, e, l, n = 32) => `<img class="eve-image rounded" data-eveid="${a}" src="${l}" alt="${e}" title="${e}" loading="lazy" width="${n}" height="${n}">`, eveWhoLinkHtml = a => `<a class="aa-intel-information-link" href="${a}" target="_blank" rel="noopener noreferer">evewho <sup><small><i class="fas fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`, zkillboardLinkHtml = a => `<a class="aa-intel-information-link" href="${a}" target="_blank" rel="noopener noreferer">zkillboard <sup><small><i class="fas fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`, dotlanLinkHtml = a => `<a class="aa-intel-information-link" href="${a}" target="_blank" rel="noopener noreferer">dotlan <sup><small><i class="fas fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`, pilotInfoPanel = a => {
+    console.log(`Error: ${a.message}`)
+}), eveImageHtml = (a, e, l, n = 32) => `<img class="eve-image rounded" data-eveid="${a}" src="${l}" alt="${e}" title="${e}" loading="lazy" width="${n}" height="${n}">`, eveWhoLinkHtml = a => `<a class="aa-intel-information-link" href="${a}" target="_blank" rel="noopener noreferer">evewho <sup><small><i class="fa-solid fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`, zkillboardLinkHtml = a => `<a class="aa-intel-information-link" href="${a}" target="_blank" rel="noopener noreferer">zkillboard <sup><small><i class="fa-solid fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`, dotlanLinkHtml = a => `<a class="aa-intel-information-link" href="${a}" target="_blank" rel="noopener noreferer">dotlan <sup><small><i class="fa-solid fa-external-link-alt" aria-hidden="true"></i></small></sup></a>`, pilotInfoPanel = a => {
     const e = `<span class="aa-intel-pilot-avatar-wrapper">${eveImageHtml(a.id,a.name,a.portrait)}</span>`;
     let l = `<span class="aa-intel-pilot-information-wrapper"><span class="aa-intel-pilot-name-wrapper">${a.name}</span>`;
     return l += `<span class="aa-intel-pilot-links-wrapper"><small>${eveWhoLinkHtml(a.evewho)} | ${zkillboardLinkHtml(a.zkillboard)}</small></span>`, e + l
 }, corporationInfoPanel = (a, e = !1) => {
     const l = `<span class="aa-intel-corporation-logo-wrapper">${eveImageHtml(a.id,a.name,a.logo)}</span>`;
     let n = `<span class="aa-intel-corporation-information-wrapper"><span class="aa-intel-corporation-name-wrapper">${a.name}</span>`;
-    return n += '<span class="aa-intel-corporation-links-wrapper"><small>', 1e6 <= a.id && a.id <= 2e6 ? n += `(${aaIntelToolJsL10n.scanData.npcCorp})` : n += `${dotlanLinkHtml(a.dotlan)} | ${zkillboardLinkHtml(a.zkillboard)}</small></span>`, n += "</span>", e ? l : l + n
+    return n += `<span class="aa-intel-corporation-links-wrapper"><small>`, 1e6 <= a.id && a.id <= 2e6 ? n += `(${aaIntelToolJsL10n.scanData.npcCorp})` : n += `${dotlanLinkHtml(a.dotlan)} | ${zkillboardLinkHtml(a.zkillboard)}</small></span>`, n += `</span>`, e ? l : l + n
 }, allianceInfoPanel = (a, e = !1) => {
     "" === a.name && (a.name = aaIntelToolJsL10n.scanData.empty);
     const l = `<span class="aa-intel-corporation-logo-wrapper">${eveImageHtml(a.id,a.name,a.logo)}</span>`;
     let n = `<span class="aa-intel-alliance-information-wrapper"><span class="aa-intel-alliance-name-wrapper">${a.name}</span>`;
-    return 1 < a.id && (n += `<span class="aa-intel-alliance-links-wrapper"><small>${dotlanLinkHtml(a.dotlan)} | ${zkillboardLinkHtml(a.zkillboard)}</small></span>`), n += "</span>", e ? 1 === a.id ? "" : l : l + n
+    return 1 < a.id && (n += `<span class="aa-intel-alliance-links-wrapper"><small>${dotlanLinkHtml(a.dotlan)} | ${zkillboardLinkHtml(a.zkillboard)}</small></span>`), n += `</span>`, e ? 1 === a.id ? "" : l : l + n
 }, shipInfoPanel = a => {
     const e = `<span class="aa-intel-ship-image-wrapper">${eveImageHtml(a.id,a.name,a.image)}</span>`,
         l = `<span class="aa-intel-ship-information-wrapper"><span class="aa-intel-ship-name-wrapper">${a.name}</span></span>`;
     return e + l
 };
 $(() => {
     const a = $("button#btn-copy-permalink-to-clipboard"),
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js.map` & `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'mappings'": "'AAEA,aAQA,MAAMA,cAAgBC,MAAOC,GACZC,MAAMD,CAAG,EACjBE,KAAKC,GACEA,EAASC,GACFC,QAAQC,QAAQH,CAAQ,EAExBE,QAAQE,OAAO,IAAIC,MAAM,gBAAgB,CAAC,CAExD,EACAN,KAAKC,GAAYA,EAASM,KAAK,CAAC,EAChCP,KAAKQ,GACKA,CACV,EACAC,MAAM,SAAUC,GACbC,QAAQC,cAAcF,EAAMG,SAAS,CACzC,CAAC,EAaHC,aAAe,CAACC,EAAOC,EAASC,EAAaC,EAAY,mDACNH,WAAeE,WAAqBD,aAAmBA,4BAAkCE,cAAsBA,MAUlKC,eAAiB,iDACkCC,oJAUnDC,mBAAqB,iDAC8BD,wJAUnDE,eAAiB,iDACkCF,oJAUnDG,eAAiB,IACnB,MAAMC,iDAA2DV,aAAaW,EAAUC,GAAID,EAAUE,KAAMF,EAAUG,QAAQ,WAC9HC,IAAIC,gGA […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "fetchAjaxData",
         "async",
         "url",
         "fetch",
         "then",
         "response",
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/base.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/base.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-fleetcomp-js.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-fleetcomp-js.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% load i18n %}
 
 <script>
     const aaIntelToolJsL10n = {
+        language: '{{ LANGUAGE_CODE }}',
         copyToClipboard: {
             permalink: {
                 text: {
                     success: '{% translate "Permalink successfully copied" %}',
                     error: '{% translate "Something went wrong. Nothing copied. Maybe your browser does not support this function." %}'
                 }
             }
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/index/form.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/index/form.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/buttons.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/buttons.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,19 @@
                                 {% translate "Ship class" as table_header %}
                                 {{ table_header|title }}
                             </th>
                             <th>{% translate "Count" %}</th>
                         </tr>
                     </thead>
                 </table>
+
+                <div class="text-center mt-3">
+                    {% translate "Total mass (in kg):" %}
+                    <span id="aa-intel-dscan-{{ dscan_section }}-mass" data-mass="0"></span>
+                </div>
             </div>
 
             <div class="aa-intel-loading-table-info aa-intel-loading-table-info-{{ dscan_section }} aa-callout aa-callout-info">
                 <p>
                     {% translate "Loading data …" %}
                 </p>
             </div>
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
 {% load i18n %}
 ******** {{{{ sseeccttiioonn__hheeaaddeerr||ttiittllee }}}} {{%% iiff nnoott oommiitt__ccoouunntteerr %%}} ((00)) {{%% eennddiiff %%}} ********
 {{%% ttrraannssllaattee ""SShhiipp ccllaassss"" aass ttaabbllee__hheeaaddeerr %%}} {{ {{%% ttrraannssllaattee ""CCoouunntt"" %%}}
 {{ ttaabbllee__hheeaaddeerr||ttiittllee }}}}
+{% translate "Total mass (in kg):" %}
 {% translate "Loading data â¦" %}
 {% translate "No data â¦" %}
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/views/index.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/index.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html` & `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/templatetags/aa_intel_tool.py` & `aa_intel_tool-2.1.0/aa_intel_tool/templatetags/aa_intel_tool.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_access.py` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         cls.user_1001 = create_fake_user(
             character_id=1001, character_name="Peter Parker"
         )
 
         cls.html_menu = f"""
             <li class="d-flex flex-wrap m-2 p-2 pt-0 pb-0 mt-0 mb-0 me-0 pe-0">
                 <i class="nav-link fa-solid fa-clipboard-list fa-fw align-self-center me-3 active"></i>
-                <a class="nav-link flex-fill align-self-center me-auto" href="{reverse('aa_intel_tool:intel_tool_index')}">
+                <a class="nav-link flex-fill align-self-center me-auto active" href="{reverse('aa_intel_tool:intel_tool_index')}">
                     Intel Parser
                 </a>
             </li>
         """
 
         cls.header_top = '<div class="navbar-brand">Intel Parser</div>'
```

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_admin.py` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_app_settings.py` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_auth_hooks.py` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_helper_data_structures.py` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_helper_data_structures.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_models.py` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_parser.py` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_parser_helper_db.py` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_parser_helper_db.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test_templatetags.py` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/utils.py` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test-data/dscan-german-client.txt` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan-german-client.txt`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test-data/dscan-russian-client.txt` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan-russian-client.txt`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/tests/test-data/dscan.txt` & `aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan.txt`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/views/ajax.py` & `aa_intel_tool-2.1.0/aa_intel_tool/views/ajax.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/aa_intel_tool/views/general.py` & `aa_intel_tool-2.1.0/aa_intel_tool/views/general.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/LICENSE` & `aa_intel_tool-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.0.0b1/README.md` & `aa_intel_tool-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -72,19 +72,21 @@
 
 ![Image: Fleet Composition Module]
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Intel Tool needs at least Alliance Auth v4.0.0!**
+> **AA Intel Tool >= 2.0.0 needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `1.2.0`.
 
 **Important**: Please make sure you meet all preconditions before you proceed:
 
 - AA Intel Tool is a plugin for [Alliance Auth]. If you don't have Alliance Auth running
   already, please install it first before proceeding. (see the official
   [Alliance Auth installation guide] for details)
 - AA Intel Tool needs [Eve Universe] to function. Please make sure it is installed,
```

### Comparing `aa_intel_tool-2.0.0b1/pyproject.toml` & `aa_intel_tool-2.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "allianceauth>=4.0.0b1",
+    "allianceauth<5.0.0,>=4",
     "allianceauth-app-utils>=1.19.1",
     "django-eveuniverse>=1.3",
 ]
 [project.optional-dependencies]
 tests-allianceauth-latest = [
     "coverage",
     "django-webtest",
```

### Comparing `aa_intel_tool-2.0.0b1/PKG-INFO` & `aa_intel_tool-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: aa-intel-tool
-Version: 2.0.0b1
+Version: 2.1.0
 Summary: A simple parser for D-Scans and more for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-intel-tool/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-intel-tool/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-intel-tool
 Project-URL: Source, https://github.com/ppfeufer/aa-intel-tool.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-intel-tool/issues
@@ -698,15 +698,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.19.1
-Requires-Dist: allianceauth>=4.0.0b1
+Requires-Dist: allianceauth<5.0.0,>=4
 Requires-Dist: django-eveuniverse>=1.3
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-webtest; extra == 'tests-allianceauth-latest'
 Description-Content-Type: text/markdown
 
 # AA Intel Tool<a name="aa-intel-tool"></a>
@@ -783,19 +783,21 @@
 
 ![Image: Fleet Composition Module]
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Intel Tool needs at least Alliance Auth v4.0.0!**
+> **AA Intel Tool >= 2.0.0 needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `1.2.0`.
 
 **Important**: Please make sure you meet all preconditions before you proceed:
 
 - AA Intel Tool is a plugin for [Alliance Auth]. If you don't have Alliance Auth running
   already, please install it first before proceeding. (see the official
   [Alliance Auth installation guide] for details)
 - AA Intel Tool needs [Eve Universe] to function. Please make sure it is installed,
```

