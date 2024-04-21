# Comparing `tmp/odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1-py3-none-any.whl.zip` & `tmp/odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,55 +1,56 @@
-Zip file size: 63180 bytes, number of entries: 53
--rw-r--r--  2.0 unx     3870 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/README.rst
--rw-r--r--  2.0 unx      140 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/__init__.py
--rw-r--r--  2.0 unx     1014 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/__manifest__.py
--rw-r--r--  2.0 unx      362 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/blacklist.py
--rw-r--r--  2.0 unx    20132 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/compare.py
--rw-r--r--  2.0 unx     8287 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/upgrade_log.py
--rw-r--r--  2.0 unx    20150 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/i18n/ca.po
--rw-r--r--  2.0 unx    20316 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/i18n/fr.po
--rw-r--r--  2.0 unx    20080 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot
--rw-r--r--  2.0 unx     1104 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/migrations/14.0.1.0.0/pre-migrate.py
--rw-r--r--  2.0 unx      163 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/models/__init__.py
--rw-r--r--  2.0 unx     1031 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/models/ir_module_module.py
--rw-r--r--  2.0 unx    19198 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/models/upgrade_analysis.py
--rw-r--r--  2.0 unx      536 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/models/upgrade_attribute.py
--rw-r--r--  2.0 unx     3043 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py
--rw-r--r--  2.0 unx     5958 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/models/upgrade_record.py
--rw-r--r--  2.0 unx       65 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/__init__.py
--rw-r--r--  2.0 unx     1843 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py
--rw-r--r--  2.0 unx       66 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py
--rw-r--r--  2.0 unx      270 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py
--rw-r--r--  2.0 unx      371 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py
--rw-r--r--  2.0 unx      259 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py
--rw-r--r--  2.0 unx       84 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py
--rw-r--r--  2.0 unx      739 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py
--rw-r--r--  2.0 unx       19 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py
--rw-r--r--  2.0 unx       23 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py
--rw-r--r--  2.0 unx     1482 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py
--rw-r--r--  2.0 unx       23 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py
--rw-r--r--  2.0 unx     1032 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py
--rw-r--r--  2.0 unx       22 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py
--rw-r--r--  2.0 unx      397 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py
--rw-r--r--  2.0 unx      308 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.rst
--rw-r--r--  2.0 unx      675 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx      100 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/readme/ROADMAP.rst
--rw-r--r--  2.0 unx      696 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/security/ir.model.access.csv
--rw-r--r--  2.0 unx     9455 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/static/description/icon.png
--rw-r--r--  2.0 unx    14034 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/static/description/index.html
--rw-r--r--  2.0 unx       26 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/tests/__init__.py
--rw-r--r--  2.0 unx     1787 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/tests/test_module.py
--rw-r--r--  2.0 unx      200 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/views/menu.xml
--rw-r--r--  2.0 unx     2640 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml
--rw-r--r--  2.0 unx     2826 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml
--rw-r--r--  2.0 unx     2834 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml
--rw-r--r--  2.0 unx       82 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/wizards/__init__.py
--rw-r--r--  2.0 unx     4527 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py
--rw-r--r--  2.0 unx     4040 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py
--rw-r--r--  2.0 unx     1787 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
--rw-r--r--  2.0 unx     3289 b- defN 23-Sep-03 16:46 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
--rw-r--r--  2.0 unx     4573 b- defN 23-Sep-03 16:49 odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Sep-03 16:49 odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Sep-03 16:49 odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5935 b- defN 23-Sep-03 16:49 odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/RECORD
-53 files, 192011 bytes uncompressed, 53128 bytes compressed:  72.3%
+Zip file size: 66591 bytes, number of entries: 54
+-rw-r--r--  2.0 unx     3870 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/README.rst
+-rw-r--r--  2.0 unx      140 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/__init__.py
+-rw-r--r--  2.0 unx     1014 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/__manifest__.py
+-rw-r--r--  2.0 unx      362 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/blacklist.py
+-rw-r--r--  2.0 unx    20132 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/compare.py
+-rw-r--r--  2.0 unx     8287 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/upgrade_log.py
+-rw-r--r--  2.0 unx    20150 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/i18n/ca.po
+-rw-r--r--  2.0 unx    22576 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/i18n/es.po
+-rw-r--r--  2.0 unx    20316 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/i18n/fr.po
+-rw-r--r--  2.0 unx    20080 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot
+-rw-r--r--  2.0 unx     1104 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/migrations/14.0.1.0.0/pre-migrate.py
+-rw-r--r--  2.0 unx      163 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/models/__init__.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/models/ir_module_module.py
+-rw-r--r--  2.0 unx    19198 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/models/upgrade_analysis.py
+-rw-r--r--  2.0 unx      536 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/models/upgrade_attribute.py
+-rw-r--r--  2.0 unx     3043 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py
+-rw-r--r--  2.0 unx     5958 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/models/upgrade_record.py
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/__init__.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py
+-rw-r--r--  2.0 unx      270 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py
+-rw-r--r--  2.0 unx      371 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py
+-rw-r--r--  2.0 unx      259 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py
+-rw-r--r--  2.0 unx      739 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py
+-rw-r--r--  2.0 unx       19 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py
+-rw-r--r--  2.0 unx       23 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py
+-rw-r--r--  2.0 unx     1482 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py
+-rw-r--r--  2.0 unx       23 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py
+-rw-r--r--  2.0 unx      397 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py
+-rw-r--r--  2.0 unx      308 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.rst
+-rw-r--r--  2.0 unx      675 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/readme/DESCRIPTION.rst
+-rw-r--r--  2.0 unx      100 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/readme/ROADMAP.rst
+-rw-r--r--  2.0 unx      696 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/security/ir.model.access.csv
+-rw-r--r--  2.0 unx     9455 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/static/description/icon.png
+-rw-r--r--  2.0 unx    14034 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/static/description/index.html
+-rw-r--r--  2.0 unx       26 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/tests/__init__.py
+-rw-r--r--  2.0 unx     1787 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/tests/test_module.py
+-rw-r--r--  2.0 unx      200 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/views/menu.xml
+-rw-r--r--  2.0 unx     2640 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml
+-rw-r--r--  2.0 unx     2826 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml
+-rw-r--r--  2.0 unx     2834 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml
+-rw-r--r--  2.0 unx       82 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/wizards/__init__.py
+-rw-r--r--  2.0 unx     4527 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py
+-rw-r--r--  2.0 unx     4040 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py
+-rw-r--r--  2.0 unx     1787 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
+-rw-r--r--  2.0 unx     3289 b- defN 24-Apr-21 06:34 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
+-rw-r--r--  2.0 unx     4573 b- defN 24-Apr-21 06:36 odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 06:36 odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-21 06:36 odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6032 b- defN 24-Apr-21 06:36 odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/RECORD
+54 files, 214684 bytes uncompressed, 56385 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -15,14 +15,17 @@
 
 Filename: odoo/addons/upgrade_analysis/upgrade_log.py
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/i18n/ca.po
 Comment: 
 
+Filename: odoo/addons/upgrade_analysis/i18n/es.po
+Comment: 
+
 Filename: odoo/addons/upgrade_analysis/i18n/fr.po
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/migrations/14.0.1.0.0/pre-migrate.py
@@ -141,20 +144,20 @@
 
 Filename: odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
 Comment: 
 
-Filename: odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/METADATA
+Filename: odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/WHEEL
+Filename: odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/top_level.txt
+Filename: odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/RECORD
+Filename: odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/METADATA` & `odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-upgrade-analysis
-Version: 14.0.3.0.1.dev1
+Version: 14.0.3.0.1.dev3
 Summary: Performs a difference analysis between modules installed on two different Odoo instances
 Home-page: https://github.com/OCA/server-tools
 Author: Therp BV, Opener B.V., GRAP, Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/RECORD` & `odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 odoo/addons/upgrade_analysis/README.rst,sha256=TCrDlQNicKHxe0UmY6DTWh0Bc0r0EYiew725Pmk5_yg,3870
 odoo/addons/upgrade_analysis/__init__.py,sha256=1X8E6viDvX9QCI3au33OFkjFkJbFw6TazruSkrDurdI,140
 odoo/addons/upgrade_analysis/__manifest__.py,sha256=H35xBioXMECgNehypz7DmNxkZ1aUa-JvP9MoJLSfI1A,1014
 odoo/addons/upgrade_analysis/blacklist.py,sha256=BIu8cYUB6j3FYtSaRcs4nSxB6yUwyjhxzOaex1AiIHY,362
 odoo/addons/upgrade_analysis/compare.py,sha256=XSetlfvLS0LBy9nI5kF1gcneaaMo7kjd2uAwPz4KSoQ,20132
 odoo/addons/upgrade_analysis/upgrade_log.py,sha256=YmtBMckR8X5sDF0Fp_OWffzCM0UCzspXhY14jD54_vA,8287
 odoo/addons/upgrade_analysis/i18n/ca.po,sha256=AIfEDTXjsGJxZVpdg3lvZJrHpHykgXETddaau9FoixI,20150
+odoo/addons/upgrade_analysis/i18n/es.po,sha256=waoj2hqK9fEUhyeLlZ8ldrwEmv9CIvRK3DS9FqCTTPA,22576
 odoo/addons/upgrade_analysis/i18n/fr.po,sha256=WUBWKeuF1PAmh4ueVFyMPn1GzlpgRZvNM2l7iahHaf0,20316
 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot,sha256=cXcuEZ7Tf6zTBHEAfVfPFnUNwYYFaQoaYvrYA2WsK5g,20080
 odoo/addons/upgrade_analysis/migrations/14.0.1.0.0/pre-migrate.py,sha256=OI6whyj_0eY4ZojhwhLqzC9X5htTO6eXJ0RInLED8L0,1104
 odoo/addons/upgrade_analysis/models/__init__.py,sha256=V3z7qRHAST0ArkG6eGCgABdDHniOvY7Mcna8I4M5duk,163
 odoo/addons/upgrade_analysis/models/ir_module_module.py,sha256=Wy2bfWlulZ-ucpxh6flDgGcvCPBpeL1TztPCxW1x-9U,1031
 odoo/addons/upgrade_analysis/models/upgrade_analysis.py,sha256=cs0JdaNJVvIJAtFW5V1D7O_CI9vbJwssyvqpwc2dGD4,19198
 odoo/addons/upgrade_analysis/models/upgrade_attribute.py,sha256=j2K_dqArvAHThW51VWhiNSiyoy9g5BnPS01khhaaovw,536
@@ -43,11 +44,11 @@
 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml,sha256=pBTVmGOGkohO1tguxKFXAWGHkrSVJdok3jjuhERcGa4,2826
 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml,sha256=oBxhlkz42bJxhrFMydpKpEDYt1sX0Z9WMipuA5Bpq2M,2834
 odoo/addons/upgrade_analysis/wizards/__init__.py,sha256=6973yn8jkeAaHm-ofIILbHUCB6KQ7RUMSDCK0Xk18xE,82
 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py,sha256=DTeLN_1rez_v82EA16H2Bsk4TGk9aA_n7Wn6_qQoKUE,4527
 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py,sha256=4g8E1EdR83R84hGVWHx45JVjnz8naQlBfvHNj5bNE6Q,4040
 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml,sha256=80IblSl5Jux1jYoh0bJGBJikNRk39HDgiRylMWPdkJo,1787
 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml,sha256=_6uw3NVhdBp_gP5mybo--AI97n3_v6tIcyX2Z0WoCrE,3289
-odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/METADATA,sha256=_ps_a4QHrUMaj22QCdCj27Ls1K-I4F0MJutnc_iXino,4573
-odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_upgrade_analysis-14.0.3.0.1.dev1.dist-info/RECORD,,
+odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/METADATA,sha256=K34Gf4tADucrXs6bzFS6ByUsEeTUAeReViAYt0LNjEU,4573
+odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_upgrade_analysis-14.0.3.0.1.dev3.dist-info/RECORD,,
```

