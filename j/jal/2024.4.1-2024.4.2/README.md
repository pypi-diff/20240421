# Comparing `tmp/jal-2024.4.1.tar.gz` & `tmp/jal-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jal-2024.4.1.tar", last modified: Tue Apr  9 11:13:21 2024, max compression
+gzip compressed data, was "jal-2024.4.2.tar", last modified: Sun Apr 21 14:43:55 2024, max compression
```

## Comparing `jal-2024.4.1.tar` & `jal-2024.4.2.tar`

### file list

```diff
@@ -1,268 +1,268 @@
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.869265 jal-2024.4.1/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2024-02-09 22:49:30.000000 jal-2024.4.1/MANIFEST.in
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3127 2024-04-09 11:13:21.869265 jal-2024.4.1/PKG-INFO
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.832598 jal-2024.4.1/docs/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6563 2024-02-09 22:49:30.000000 jal-2024.4.1/docs/README.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.835931 jal-2024.4.1/jal/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2024-04-09 11:09:19.000000 jal-2024.4.1/jal/__init__.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     7465 2024-04-08 17:32:39.000000 jal-2024.4.1/jal/constants.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.835931 jal-2024.4.1/jal/data_export/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21391 2024-04-01 21:45:52.000000 jal-2024.4.1/jal/data_export/dlsg.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.835931 jal-2024.4.1/jal/data_export/tax_reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/tax_reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1998 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/tax_reports/portugal.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7223 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/data_export/tax_reports/portugal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1808 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/tax_reports/russia.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35270 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/data_export/tax_reports/russia.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7465 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/data_export/taxes.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5484 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/taxes_flow.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.839265 jal-2024.4.1/jal/data_export/templates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/tax_prt_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/tax_prt_shares.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/tax_rus_bonds.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/tax_rus_corporate_actions.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/tax_rus_crypto.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5131 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/tax_rus_derivatives.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/tax_rus_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/tax_rus_fees.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1248 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/tax_rus_flow.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/tax_rus_interests.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5292 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_export/templates/tax_rus_trades.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10769 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/data_export/xlsx.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.839265 jal-2024.4.1/jal/data_import/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.839265 jal-2024.4.1/jal/data_import/broker_statements/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/broker_statements/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    72693 2024-04-09 10:20:42.000000 jal-2024.4.1/jal/data_import/broker_statements/ibkr.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20169 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/broker_statements/just2trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9470 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/broker_statements/kit.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33578 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/broker_statements/openbroker.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15460 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/broker_statements/psb.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3687 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/broker_statements/revolut_crypto.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    28079 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/broker_statements/tvoy.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12579 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/broker_statements/vtb.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/category_recognizer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/import_schema.json
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.842598 jal-2024.4.1/jal/data_import/receipt_api/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/receipt_api/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12505 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/receipt_api/eu_lidl_plus.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12586 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/receipt_api/pt_pingo_doce.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1951 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/receipt_api/receipt_api.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2855 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/receipt_api/receipts.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16972 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/receipt_api/ru_fns.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16059 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/shop_receipt.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38404 2024-04-08 13:37:19.000000 jal-2024.4.1/jal/data_import/statement.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11360 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/statement_xls.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6625 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/data_import/statement_xml.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4202 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/data_import/statements.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.842598 jal-2024.4.1/jal/db/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/db/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20620 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/db/account.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    22515 2024-03-26 21:53:39.000000 jal-2024.4.1/jal/db/asset.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6139 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/db/backup_restore.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10566 2024-03-07 13:08:38.000000 jal-2024.4.1/jal/db/balances_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/db/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6299 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/db/closed_trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/db/country.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20303 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/db/db.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4585 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/db/deposit.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4109 2024-04-06 22:22:24.000000 jal-2024.4.1/jal/db/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16837 2024-03-24 14:22:32.000000 jal-2024.4.1/jal/db/holdings_model.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16683 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/db/ledger.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    67562 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/db/operations.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9859 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/db/operations_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/db/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    18453 2024-04-08 17:32:39.000000 jal-2024.4.1/jal/db/reference_models.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2989 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/db/settings.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2279 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/db/tag.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6762 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/db/tax_estimator.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10752 2024-02-11 21:17:50.000000 jal-2024.4.1/jal/db/trades_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5882 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/db/tree_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1642 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/db/view_model.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.849265 jal-2024.4.1/jal/img/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/aux_ibkr.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/aux_j2t.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/aux_kit.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/aux_openbroker.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/aux_psb.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      958 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/aux_revolut.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      348 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/aux_tvoy.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33310 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/aux_vtb.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/flag_en.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      704 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/flag_pt.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/flag_ru.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/img/tag_bank.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/img/tag_card.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/img/tag_cash.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/img/tag_investing.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_add.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-12 22:14:19.000000 jal-2024.4.1/jal/img/ui_add_child.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_amortization.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_buy.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_cancel.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_chart.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_clean.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_copy.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_coupon.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_delisting.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/img/ui_deposit_account.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_deposit_close.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_deposit_open.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_details.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_dividend.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_dividend_stock.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_fee.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_interest.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_jal.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_list.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_merger.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_minus.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_ok.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_plus.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_remove.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_renaming.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_sell.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_spinoff.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_split.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_tag.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_tax.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/img/ui_total.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_transfer_asset_in.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_transfer_asset_out.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_transfer_in.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_transfer_out.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/img/ui_vesting.ico
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1740 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/jal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    95194 2024-04-08 17:32:39.000000 jal-2024.4.1/jal/jal_init.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.849265 jal-2024.4.1/jal/languages/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/languages/en.qm
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)   114655 2024-04-01 21:49:59.000000 jal-2024.4.1/jal/languages/ru.qm
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.849265 jal-2024.4.1/jal/net/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/net/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    30150 2024-04-06 22:22:24.000000 jal-2024.4.1/jal/net/downloader.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3420 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/net/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2173 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/pypi_description.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.852598 jal-2024.4.1/jal/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4921 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/reports/account_balance.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6179 2024-03-08 09:55:09.000000 jal-2024.4.1/jal/reports/assets_payments.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4756 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/reports/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2369 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/reports/deals.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17589 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/reports/income_spending.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1900 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/reports/operations_base.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4563 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/reports/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6615 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/reports/portfolio.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8772 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/reports/profit_loss.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4077 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/reports/reports.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4594 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/reports/tag.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6399 2024-04-01 22:26:18.000000 jal-2024.4.1/jal/reports/term_deposits.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.855932 jal-2024.4.1/jal/ui/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/ui/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.855932 jal-2024.4.1/jal/ui/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/ui/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3849 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/reports/ui_account_balance_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4959 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/reports/ui_assets_payments_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5880 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/reports/ui_category_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4480 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/reports/ui_deals_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4968 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/reports/ui_income_spending_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6093 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/reports/ui_peer_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5032 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/reports/ui_portfolio_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4701 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/reports/ui_profit_loss_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6063 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/reports/ui_tag_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4833 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/reports/ui_tax_estimation.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4431 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/reports/ui_term_deposits_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12854 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_asset_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4084 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_flow_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14824 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_login_fns_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3687 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_login_lidl_plus_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5249 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_login_pingo_doce_dlg.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9657 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14091 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_operations_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5735 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_rebuild_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12161 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_receipt_import_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7330 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_reference_data_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2917 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_select_account_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3281 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_select_reference_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9730 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_tax_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/ui_update_quotes_window.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.855932 jal-2024.4.1/jal/ui/widgets/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/ui/widgets/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9867 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/widgets/ui_asset_payment_operation.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8395 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/widgets/ui_corporate_action_operation.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8013 2024-04-01 21:48:03.000000 jal-2024.4.1/jal/ui/widgets/ui_income_spending_operation.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5888 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/widgets/ui_term_deposit_operation.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8943 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/widgets/ui_trade_operation.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10962 2024-04-01 21:48:04.000000 jal-2024.4.1/jal/ui/widgets/ui_transfer_operation.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.862598 jal-2024.4.1/jal/updates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_29.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_30.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_31.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_32.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_33.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_34.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_35.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_36.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_37.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_38.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_39.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_40.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_41.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_42.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_43.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_44.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      534 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_45.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      839 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_46.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      786 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_47.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2235 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_48.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1789 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_49.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1280 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_50.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1903 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_51.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3390 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/updates/jal_delta_52.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7714 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/updates/jal_delta_53.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      340 2024-03-26 22:04:52.000000 jal-2024.4.1/jal/updates/jal_delta_54.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1561 2024-04-08 17:32:39.000000 jal-2024.4.1/jal/updates/jal_delta_55.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.865932 jal-2024.4.1/jal/widgets/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3706 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/abstract_operation_details.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8179 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/account_select.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15881 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/widgets/asset_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6439 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/widgets/asset_payment_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9085 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/corporate_action_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.865932 jal-2024.4.1/jal/widgets/custom/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/custom/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4703 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/custom/date_range_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2068 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/custom/db_lookup_combobox.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6622 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/custom/log_viewer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3661 2024-04-01 22:26:12.000000 jal-2024.4.1/jal/widgets/custom/table_footer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1619 2024-03-07 10:48:10.000000 jal-2024.4.1/jal/widgets/custom/tableview_with_footer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1606 2024-03-07 10:47:34.000000 jal-2024.4.1/jal/widgets/custom/treeview_with_footer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14280 2024-02-12 11:52:33.000000 jal-2024.4.1/jal/widgets/delegates.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11104 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5248 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/widgets/icons.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11982 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/income_spending_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    14669 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/widgets/main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3386 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/mdi.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3014 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/widgets/operations_tabs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9646 2024-03-04 22:10:29.000000 jal-2024.4.1/jal/widgets/operations_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8563 2024-03-24 14:22:23.000000 jal-2024.4.1/jal/widgets/price_chart.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10731 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/qr_scanner.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11491 2024-04-08 17:32:39.000000 jal-2024.4.1/jal/widgets/reference_data.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    23849 2024-04-08 17:32:39.000000 jal-2024.4.1/jal/widgets/reference_dialogs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6037 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/reference_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3575 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/selection_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8311 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/tax_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7870 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/term_deposit_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3514 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/trade_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8145 2024-02-09 22:49:30.000000 jal-2024.4.1/jal/widgets/transfer_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-09 11:13:21.869265 jal-2024.4.1/jal.egg-info/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3127 2024-04-09 11:13:21.000000 jal-2024.4.1/jal.egg-info/PKG-INFO
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7158 2024-04-09 11:13:21.000000 jal-2024.4.1/jal.egg-info/SOURCES.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2024-04-09 11:13:21.000000 jal-2024.4.1/jal.egg-info/dependency_links.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2024-04-09 11:13:21.000000 jal-2024.4.1/jal.egg-info/entry_points.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      118 2024-04-09 11:13:21.000000 jal-2024.4.1/jal.egg-info/requires.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2024-04-09 11:13:21.000000 jal-2024.4.1/jal.egg-info/top_level.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2024-04-09 11:13:21.869265 jal-2024.4.1/setup.cfg
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1816 2024-02-09 22:49:30.000000 jal-2024.4.1/setup.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.885083 jal-2024.4.2/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2024-02-09 22:49:30.000000 jal-2024.4.2/MANIFEST.in
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3127 2024-04-21 14:43:55.881749 jal-2024.4.2/PKG-INFO
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.811748 jal-2024.4.2/docs/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6563 2024-02-09 22:49:30.000000 jal-2024.4.2/docs/README.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.811748 jal-2024.4.2/jal/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2024-04-21 14:40:59.000000 jal-2024.4.2/jal/__init__.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     7465 2024-04-08 17:32:39.000000 jal-2024.4.2/jal/constants.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.815082 jal-2024.4.2/jal/data_export/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21391 2024-04-01 21:45:52.000000 jal-2024.4.2/jal/data_export/dlsg.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.815082 jal-2024.4.2/jal/data_export/tax_reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/tax_reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1998 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/tax_reports/portugal.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7223 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/data_export/tax_reports/portugal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1808 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/tax_reports/russia.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35270 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/data_export/tax_reports/russia.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7465 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/data_export/taxes.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5484 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/taxes_flow.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.818415 jal-2024.4.2/jal/data_export/templates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/tax_prt_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/tax_prt_shares.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/tax_rus_bonds.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/tax_rus_corporate_actions.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/tax_rus_crypto.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5131 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/tax_rus_derivatives.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/tax_rus_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/tax_rus_fees.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1248 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/tax_rus_flow.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/tax_rus_interests.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5292 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_export/templates/tax_rus_trades.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10769 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/data_export/xlsx.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.821748 jal-2024.4.2/jal/data_import/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.821748 jal-2024.4.2/jal/data_import/broker_statements/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/broker_statements/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    72693 2024-04-09 10:20:42.000000 jal-2024.4.2/jal/data_import/broker_statements/ibkr.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20223 2024-04-14 21:06:50.000000 jal-2024.4.2/jal/data_import/broker_statements/just2trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9524 2024-04-14 21:06:49.000000 jal-2024.4.2/jal/data_import/broker_statements/kit.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33578 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/broker_statements/openbroker.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15514 2024-04-14 21:06:50.000000 jal-2024.4.2/jal/data_import/broker_statements/psb.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3687 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/broker_statements/revolut_crypto.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    28122 2024-04-14 21:45:25.000000 jal-2024.4.2/jal/data_import/broker_statements/tvoy.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21685 2024-04-21 14:34:23.000000 jal-2024.4.2/jal/data_import/broker_statements/vtb.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/category_recognizer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/import_schema.json
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.825082 jal-2024.4.2/jal/data_import/receipt_api/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/receipt_api/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12505 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/receipt_api/eu_lidl_plus.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12586 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/receipt_api/pt_pingo_doce.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1951 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/receipt_api/receipt_api.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2855 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/receipt_api/receipts.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16972 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/receipt_api/ru_fns.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16059 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/shop_receipt.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38724 2024-04-14 15:57:20.000000 jal-2024.4.2/jal/data_import/statement.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11616 2024-04-14 21:06:50.000000 jal-2024.4.2/jal/data_import/statement_xls.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6625 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/data_import/statement_xml.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4202 2024-04-14 22:08:38.000000 jal-2024.4.2/jal/data_import/statements.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.831749 jal-2024.4.2/jal/db/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/db/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20620 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/db/account.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    22515 2024-03-26 21:53:39.000000 jal-2024.4.2/jal/db/asset.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6139 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/db/backup_restore.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10566 2024-03-07 13:08:38.000000 jal-2024.4.2/jal/db/balances_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/db/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6299 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/db/closed_trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/db/country.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20303 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/db/db.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4585 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/db/deposit.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4109 2024-04-06 22:22:24.000000 jal-2024.4.2/jal/db/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16837 2024-03-24 14:22:32.000000 jal-2024.4.2/jal/db/holdings_model.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16683 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/db/ledger.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    67562 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/db/operations.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9859 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/db/operations_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/db/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    18453 2024-04-08 17:32:39.000000 jal-2024.4.2/jal/db/reference_models.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2989 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/db/settings.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2279 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/db/tag.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6762 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/db/tax_estimator.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10752 2024-02-11 21:17:50.000000 jal-2024.4.2/jal/db/trades_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5882 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/db/tree_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1642 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/db/view_model.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.855082 jal-2024.4.2/jal/img/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/aux_ibkr.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/aux_j2t.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/aux_kit.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/aux_openbroker.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/aux_psb.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      958 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/aux_revolut.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      348 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/aux_tvoy.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33310 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/aux_vtb.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/flag_en.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      704 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/flag_pt.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/flag_ru.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/img/tag_bank.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/img/tag_card.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/img/tag_cash.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/img/tag_investing.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_add.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-12 22:14:19.000000 jal-2024.4.2/jal/img/ui_add_child.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_amortization.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_buy.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_cancel.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_chart.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_clean.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_copy.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_coupon.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_delisting.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/img/ui_deposit_account.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_deposit_close.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_deposit_open.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_details.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_dividend.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_dividend_stock.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_fee.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_interest.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_jal.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_list.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_merger.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_minus.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_ok.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_plus.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_remove.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_renaming.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_sell.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_spinoff.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_split.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_tag.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_tax.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/img/ui_total.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_transfer_asset_in.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_transfer_asset_out.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_transfer_in.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_transfer_out.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    33350 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/img/ui_vesting.ico
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1740 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/jal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    95194 2024-04-08 17:32:39.000000 jal-2024.4.2/jal/jal_init.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.855082 jal-2024.4.2/jal/languages/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/languages/en.qm
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)   114655 2024-04-01 21:49:59.000000 jal-2024.4.2/jal/languages/ru.qm
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.855082 jal-2024.4.2/jal/net/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/net/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    30207 2024-04-19 16:51:15.000000 jal-2024.4.2/jal/net/downloader.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3420 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/net/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2173 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/pypi_description.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.858415 jal-2024.4.2/jal/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4921 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/reports/account_balance.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6179 2024-03-08 09:55:09.000000 jal-2024.4.2/jal/reports/assets_payments.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4756 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/reports/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2369 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/reports/deals.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17589 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/reports/income_spending.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1900 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/reports/operations_base.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4563 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/reports/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6615 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/reports/portfolio.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8772 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/reports/profit_loss.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4077 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/reports/reports.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4594 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/reports/tag.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6399 2024-04-01 22:26:18.000000 jal-2024.4.2/jal/reports/term_deposits.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.861749 jal-2024.4.2/jal/ui/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/ui/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.861749 jal-2024.4.2/jal/ui/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/ui/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3849 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/reports/ui_account_balance_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4959 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/reports/ui_assets_payments_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5880 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/reports/ui_category_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4480 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/reports/ui_deals_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4968 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/reports/ui_income_spending_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6093 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/reports/ui_peer_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5032 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/reports/ui_portfolio_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4701 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/reports/ui_profit_loss_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6063 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/reports/ui_tag_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4833 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/reports/ui_tax_estimation.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4431 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/reports/ui_term_deposits_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12854 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_asset_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4084 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_flow_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14824 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_login_fns_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3687 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_login_lidl_plus_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5249 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_login_pingo_doce_dlg.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9657 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14091 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_operations_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5735 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_rebuild_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12161 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_receipt_import_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7330 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_reference_data_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2917 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_select_account_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3281 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_select_reference_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9730 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_tax_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/ui_update_quotes_window.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.865082 jal-2024.4.2/jal/ui/widgets/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/ui/widgets/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9867 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/widgets/ui_asset_payment_operation.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8395 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/widgets/ui_corporate_action_operation.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8013 2024-04-01 21:48:03.000000 jal-2024.4.2/jal/ui/widgets/ui_income_spending_operation.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5888 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/widgets/ui_term_deposit_operation.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8943 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/widgets/ui_trade_operation.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10962 2024-04-01 21:48:04.000000 jal-2024.4.2/jal/ui/widgets/ui_transfer_operation.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.875082 jal-2024.4.2/jal/updates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_29.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_30.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_31.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_32.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_33.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_34.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_35.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_36.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_37.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_38.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_39.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_40.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_41.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_42.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_43.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_44.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      534 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_45.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      839 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_46.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      786 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_47.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2235 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_48.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1789 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_49.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1280 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_50.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1903 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_51.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3390 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/updates/jal_delta_52.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7714 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/updates/jal_delta_53.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      340 2024-03-26 22:04:52.000000 jal-2024.4.2/jal/updates/jal_delta_54.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1561 2024-04-08 17:32:39.000000 jal-2024.4.2/jal/updates/jal_delta_55.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.881749 jal-2024.4.2/jal/widgets/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3706 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/abstract_operation_details.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8179 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/account_select.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15881 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/widgets/asset_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6439 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/widgets/asset_payment_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9085 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/corporate_action_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.881749 jal-2024.4.2/jal/widgets/custom/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/custom/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4703 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/custom/date_range_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2068 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/custom/db_lookup_combobox.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6622 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/custom/log_viewer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3661 2024-04-01 22:26:12.000000 jal-2024.4.2/jal/widgets/custom/table_footer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1619 2024-03-07 10:48:10.000000 jal-2024.4.2/jal/widgets/custom/tableview_with_footer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1606 2024-03-07 10:47:34.000000 jal-2024.4.2/jal/widgets/custom/treeview_with_footer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14280 2024-02-12 11:52:33.000000 jal-2024.4.2/jal/widgets/delegates.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11104 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5248 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/widgets/icons.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11982 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/income_spending_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    14669 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/widgets/main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3386 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/mdi.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3014 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/widgets/operations_tabs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9646 2024-03-04 22:10:29.000000 jal-2024.4.2/jal/widgets/operations_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8563 2024-03-24 14:22:23.000000 jal-2024.4.2/jal/widgets/price_chart.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10731 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/qr_scanner.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11491 2024-04-08 17:32:39.000000 jal-2024.4.2/jal/widgets/reference_data.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    23849 2024-04-08 17:32:39.000000 jal-2024.4.2/jal/widgets/reference_dialogs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6037 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/reference_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3575 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/selection_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8311 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/tax_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7870 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/term_deposit_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3514 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/trade_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8145 2024-02-09 22:49:30.000000 jal-2024.4.2/jal/widgets/transfer_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2024-04-21 14:43:55.881749 jal-2024.4.2/jal.egg-info/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3127 2024-04-21 14:43:55.000000 jal-2024.4.2/jal.egg-info/PKG-INFO
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7158 2024-04-21 14:43:55.000000 jal-2024.4.2/jal.egg-info/SOURCES.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2024-04-21 14:43:55.000000 jal-2024.4.2/jal.egg-info/dependency_links.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2024-04-21 14:43:55.000000 jal-2024.4.2/jal.egg-info/entry_points.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      118 2024-04-21 14:43:55.000000 jal-2024.4.2/jal.egg-info/requires.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2024-04-21 14:43:55.000000 jal-2024.4.2/jal.egg-info/top_level.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2024-04-21 14:43:55.885083 jal-2024.4.2/setup.cfg
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1816 2024-02-09 22:49:30.000000 jal-2024.4.2/setup.py
```

### Comparing `jal-2024.4.1/PKG-INFO` & `jal-2024.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2024.4.1/docs/README.md` & `jal-2024.4.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/constants.py` & `jal-2024.4.2/jal/constants.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/dlsg.py` & `jal-2024.4.2/jal/data_export/dlsg.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/tax_reports/portugal.json` & `jal-2024.4.2/jal/data_export/tax_reports/portugal.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/tax_reports/portugal.py` & `jal-2024.4.2/jal/data_export/tax_reports/portugal.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/tax_reports/russia.json` & `jal-2024.4.2/jal/data_export/tax_reports/russia.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/tax_reports/russia.py` & `jal-2024.4.2/jal/data_export/tax_reports/russia.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/taxes.py` & `jal-2024.4.2/jal/data_export/taxes.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/taxes_flow.py` & `jal-2024.4.2/jal/data_export/taxes_flow.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/templates/tax_prt_dividends.json` & `jal-2024.4.2/jal/data_export/templates/tax_prt_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/templates/tax_prt_shares.json` & `jal-2024.4.2/jal/data_export/templates/tax_prt_shares.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/templates/tax_rus_bonds.json` & `jal-2024.4.2/jal/data_export/templates/tax_rus_bonds.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/templates/tax_rus_corporate_actions.json` & `jal-2024.4.2/jal/data_export/templates/tax_rus_corporate_actions.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/templates/tax_rus_crypto.json` & `jal-2024.4.2/jal/data_export/templates/tax_rus_crypto.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/templates/tax_rus_derivatives.json` & `jal-2024.4.2/jal/data_export/templates/tax_rus_derivatives.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/templates/tax_rus_dividends.json` & `jal-2024.4.2/jal/data_export/templates/tax_rus_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/templates/tax_rus_fees.json` & `jal-2024.4.2/jal/data_export/templates/tax_rus_fees.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/templates/tax_rus_flow.json` & `jal-2024.4.2/jal/data_export/templates/tax_rus_flow.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/templates/tax_rus_interests.json` & `jal-2024.4.2/jal/data_export/templates/tax_rus_interests.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/templates/tax_rus_trades.json` & `jal-2024.4.2/jal/data_export/templates/tax_rus_trades.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_export/xlsx.py` & `jal-2024.4.2/jal/data_export/xlsx.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/broker_statements/ibkr.py` & `jal-2024.4.2/jal/data_import/broker_statements/ibkr.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/broker_statements/just2trade.py` & `jal-2024.4.2/jal/data_import/broker_statements/just2trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,14 +193,17 @@
             trade = {"id": new_id, "number": deal_number, "timestamp": timestamp, "settlement": settlement,
                      "account": account_id, "asset": asset_id, "quantity": qty, "price": price, "fee": fee}
             self._data[FOF.TRADES].append(trade)
             cnt += 1
             row += 1
         logging.info(self.tr("Crypto trades loaded: ") + f"{cnt}")
 
+    def _load_asset_transactions(self):
+        pass
+
     def _load_cash_transactions(self):
         self._load_money_table()
         self._load_fees()
 
     def _load_money_table(self):
         columns = {
             "date": "Дата",
```

### Comparing `jal-2024.4.1/jal/data_import/broker_statements/kit.py` & `jal-2024.4.2/jal/data_import/broker_statements/kit.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,17 @@
                 payment = {"id": new_id, "type": FOF.PAYMENT_INTEREST, "account": account_id, "timestamp": timestamp,
                            "number": str(number), "asset": asset_id, "amount": bond_interest, "description": "НКД"}
                 self._data[FOF.ASSET_PAYMENTS].append(payment)
             cnt += 1
             row += 1
         logging.info(self.tr("Trades loaded: ") + f"{cnt}")
 
+    def _load_asset_transactions(self):
+        pass
+
     def _load_cash_transactions(self):
         cnt = 0
         columns = {
             "date": "Дата",
             "operation": "Тип операции",
             "amount": "Сумма",
             "currency": " Валюта",
```

### Comparing `jal-2024.4.1/jal/data_import/broker_statements/openbroker.py` & `jal-2024.4.2/jal/data_import/broker_statements/openbroker.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/broker_statements/psb.py` & `jal-2024.4.2/jal/data_import/broker_statements/psb.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,14 +118,17 @@
                                "timestamp": timestamp,
                                "number": deal_number, "asset": asset_id, "amount": bond_interest, "description": "НКД"}
                     self._data[FOF.ASSET_PAYMENTS].append(payment)
                 cnt += 1
                 row += 1
         logging.info(self.tr("Trades loaded: ") + f"{cnt}")
 
+    def _load_asset_transactions(self):
+        pass
+
     def _load_cash_transactions(self):
         self.load_cash_transactions()
         self.load_coupons()
         self.load_dividends()
 
     def load_cash_transactions(self):
         cnt = 0
```

### Comparing `jal-2024.4.1/jal/data_import/broker_statements/revolut_crypto.py` & `jal-2024.4.2/jal/data_import/broker_statements/revolut_crypto.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/broker_statements/tvoy.py` & `jal-2024.4.2/jal/data_import/broker_statements/tvoy.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,21 +447,18 @@
         if parts is None:
             logging.error(self.tr("Can't parse bond repayment description ") + f"'{description}'")
             return
         interest_data = parts.groupdict()
         asset_id = self.asset_id({'symbol': interest_data['NAME'], 'should_exist': True})
         match = [x for x in self.asset_withdrawal if x['asset'] == asset_id and x['timestamp'] == timestamp]
         if not match:
-            logging.error(self.tr("Can't find asset cancellation record for ") + f"'{description}'")
-            return
+            raise Statement_ImportError(self.tr("Can't find asset cancellation record for ") + f"'{description}'")
         if len(match) != 1:
-            logging.error(self.tr("Multiple asset cancellation match for ") + f"'{description}'")
-            return
+            raise Statement_ImportError(self.tr("Multiple asset cancellation match for ") + f"'{description}'")
         asset_cancel = match[0]
-
         qty = asset_cancel['quantity']
         price = abs(amount / qty)   # Price is always positive
         note = description + ", " + asset_cancel['note']
         new_id = max([0] + [x['id'] for x in self._data[FOF.TRADES]]) + 1
         trade = {"id": new_id, "number": asset_cancel['number'], "timestamp": timestamp, "settlement": timestamp,
                  "account": account_id, "asset": asset_id, "quantity": qty, "price": price, "fee": 0.0, "note": note}
         self._data[FOF.TRADES].append(trade)
@@ -474,10 +471,13 @@
 
     def fee(self, timestamp, _number, account_id, amount, description):
         new_id = max([0] + [x['id'] for x in self._data[FOF.INCOME_SPENDING]]) + 1
         fee = {"id": new_id, "timestamp": timestamp, "account": account_id, "peer": 0,
                "lines": [{"amount": amount, "category": -PredefinedCategory.Fees, "description": description}]}
         self._data[FOF.INCOME_SPENDING].append(fee)
 
+    def _load_asset_transactions(self):
+        pass
+
     def _strip_unused_data(self):
         for asset in self._data[FOF.ASSETS]:
             self.drop_extra_fields(asset, ['issuer', 'broker_name'])
```

### Comparing `jal-2024.4.1/jal/data_import/category_recognizer.py` & `jal-2024.4.2/jal/data_import/category_recognizer.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/import_schema.json` & `jal-2024.4.2/jal/data_import/import_schema.json`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/receipt_api/eu_lidl_plus.py` & `jal-2024.4.2/jal/data_import/receipt_api/eu_lidl_plus.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/receipt_api/pt_pingo_doce.py` & `jal-2024.4.2/jal/data_import/receipt_api/pt_pingo_doce.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/receipt_api/receipt_api.py` & `jal-2024.4.2/jal/data_import/receipt_api/receipt_api.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/receipt_api/receipts.py` & `jal-2024.4.2/jal/data_import/receipt_api/receipts.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/receipt_api/ru_fns.py` & `jal-2024.4.2/jal/data_import/receipt_api/ru_fns.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/shop_receipt.py` & `jal-2024.4.2/jal/data_import/shop_receipt.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/statement.py` & `jal-2024.4.2/jal/data_import/statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -634,14 +634,18 @@
             db_asset = JalAsset(data=asset_info, search=True, create=False)
             if db_asset.id():
                 asset = {'id': -db_asset.id(), 'type': FOF.convert_predefined_asset_type(db_asset.type()), 'name': db_asset.name(), 'isin': db_asset.isin()}
                 self._data[FOF.ASSETS].append(asset)
                 symbol_id = max([0] + [x['id'] for x in self._data[FOF.SYMBOLS]]) + 1
                 symbol = {"id": symbol_id, "asset": -db_asset.id(), 'symbol': db_asset.symbol(asset_info['currency']), 'currency': asset_info['currency']}
                 self._data[FOF.SYMBOLS].append(symbol)
+                if 'reg_number' in asset_info:
+                    data_id = max([0] + [x['id'] for x in self._data[FOF.ASSETS_DATA]]) + 1
+                    reg_number = {"id": data_id, "asset": -db_asset.id(), "reg_number": asset_info['reg_number']}
+                    self._data[FOF.ASSETS_DATA].append(reg_number)
                 return asset['id']
         if asset is None and 'search_online' in asset_info:
             if asset_info['search_online'] == "MOEX":
                 search_data = {}
                 self._uppend_keys_from(search_data, asset_info, ['isin', 'reg_number'])
                 if 'symbol' in asset_info:
                     search_data['name'] = asset_info['symbol']   # Search as by name as it is more flexible
```

### Comparing `jal-2024.4.1/jal/data_import/statement_xls.py` & `jal-2024.4.2/jal/data_import/statement_xls.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
         self._validate()
         self._load_currencies()
         self._load_accounts()
         self._load_money()
         self._load_assets()
         self._load_deals()
+        self._load_asset_transactions()
         self._load_cash_transactions()
         self._strip_unused_data()
 
         logging.info(self.tr("Statement loaded successfully: ") + f"{self.StatementName}")
 
     # Finds a row with header in column self.HeaderCol starting with 'header' and returns its index.
     # Return -1 if header isn't found
@@ -113,33 +114,33 @@
 
     def _check_statement_header(self):
         if self._statement[self.Header[0]][self.Header[1]] != self.Header[2]:
             raise Statement_ImportError(
                 self.tr("Can't find expected report header: ") + f"'{self.Header[2]}'")
 
     def _get_statement_period(self):
-        parts = re.match(self.PeriodPattern[2],
-                         self._statement[self.PeriodPattern[0]][self.PeriodPattern[1]], re.IGNORECASE)
+        parts = re.match(self.PeriodPattern[2], self._statement[self.PeriodPattern[0]][self.PeriodPattern[1]], re.IGNORECASE)
         if parts is None:
             raise Statement_ImportError(self.tr("Can't read report period"))
         statement_dates = parts.groupdict()
         start_day = int(datetime.strptime(statement_dates['S'], "%d.%m.%Y").replace(tzinfo=timezone.utc).timestamp())
         end_day = int(datetime.strptime(statement_dates['E'], "%d.%m.%Y").replace(tzinfo=timezone.utc).timestamp())
         self._data[FOF.PERIOD] = [start_day, self._end_of_date(end_day)]
 
     def _get_account_number(self):
         if self.AccountPattern[2] is None:
             self._account_number = str(self._statement[self.AccountPattern[0]][self.AccountPattern[1]])
-            return
-        parts = re.match(self.AccountPattern[2],
-                         self._statement[self.AccountPattern[0]][self.AccountPattern[1]], re.IGNORECASE)
-        if parts is None:
-            self._account_number = self._statement[self.AccountPattern[0]][self.AccountPattern[1]]
         else:
-            self._account_number = parts.groupdict()['ACCOUNT']
+            parts = re.match(self.AccountPattern[2], self._statement[self.AccountPattern[0]][self.AccountPattern[1]], re.IGNORECASE)
+            if parts is None:
+                self._account_number = self._statement[self.AccountPattern[0]][self.AccountPattern[1]]
+            else:
+                self._account_number = parts.groupdict()['ACCOUNT']
+        if not self._account_number:
+            raise Statement_ImportError(self.tr("Empty account number"))
 
     def _load_currencies(self):
         amounts = {}
         currency_col = {}
         _header_row = self.find_row(self.SummaryHeader)
         _start_row = self.find_row("входящ")
         _end_row = self.find_row("исходящ")
@@ -241,12 +242,15 @@
         new_account = {"id": new_id, "number": number, 'currency': currency_id}
         self._data[FOF.ACCOUNTS].append(new_account)
         return new_id
 
     def _load_deals(self):
         raise NotImplementedError("load_deals() method is not defined in subclass of StatementXLS")
 
+    def _load_asset_transactions(self):
+        raise NotImplementedError("load_deals() method is not defined in subclass of StatementXLS")
+
     def _load_cash_transactions(self):
         raise NotImplementedError("load_cash_transactions() method is not defined in subclass of StatementXLS")
 
     def _strip_unused_data(self):
         pass
```

### Comparing `jal-2024.4.1/jal/data_import/statement_xml.py` & `jal-2024.4.2/jal/data_import/statement_xml.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/data_import/statements.py` & `jal-2024.4.2/jal/data_import/statements.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/account.py` & `jal-2024.4.2/jal/db/account.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/asset.py` & `jal-2024.4.2/jal/db/asset.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/backup_restore.py` & `jal-2024.4.2/jal/db/backup_restore.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/balances_model.py` & `jal-2024.4.2/jal/db/balances_model.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/category.py` & `jal-2024.4.2/jal/db/category.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/closed_trade.py` & `jal-2024.4.2/jal/db/closed_trade.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/country.py` & `jal-2024.4.2/jal/db/country.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/db.py` & `jal-2024.4.2/jal/db/db.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/deposit.py` & `jal-2024.4.2/jal/db/deposit.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/helpers.py` & `jal-2024.4.2/jal/db/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/holdings_model.py` & `jal-2024.4.2/jal/db/holdings_model.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/ledger.py` & `jal-2024.4.2/jal/db/ledger.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/operations.py` & `jal-2024.4.2/jal/db/operations.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/operations_model.py` & `jal-2024.4.2/jal/db/operations_model.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/peer.py` & `jal-2024.4.2/jal/db/peer.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/reference_models.py` & `jal-2024.4.2/jal/db/reference_models.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/settings.py` & `jal-2024.4.2/jal/db/settings.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/tag.py` & `jal-2024.4.2/jal/db/tag.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/tax_estimator.py` & `jal-2024.4.2/jal/db/tax_estimator.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/trades_model.py` & `jal-2024.4.2/jal/db/trades_model.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/tree_model.py` & `jal-2024.4.2/jal/db/tree_model.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/db/view_model.py` & `jal-2024.4.2/jal/db/view_model.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/aux_ibkr.png` & `jal-2024.4.2/jal/img/aux_ibkr.png`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/aux_j2t.png` & `jal-2024.4.2/jal/img/aux_j2t.png`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/aux_kit.png` & `jal-2024.4.2/jal/img/aux_kit.png`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/aux_openbroker.ico` & `jal-2024.4.2/jal/img/aux_openbroker.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/aux_psb.ico` & `jal-2024.4.2/jal/img/aux_psb.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/aux_revolut.png` & `jal-2024.4.2/jal/img/aux_revolut.png`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/aux_vtb.ico` & `jal-2024.4.2/jal/img/aux_vtb.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/flag_pt.png` & `jal-2024.4.2/jal/img/flag_pt.png`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/tag_bank.ico` & `jal-2024.4.2/jal/img/tag_bank.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/tag_card.ico` & `jal-2024.4.2/jal/img/tag_card.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/tag_cash.ico` & `jal-2024.4.2/jal/img/tag_cash.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/tag_investing.ico` & `jal-2024.4.2/jal/img/tag_investing.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_add.ico` & `jal-2024.4.2/jal/img/ui_add.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_add_child.ico` & `jal-2024.4.2/jal/img/ui_add_child.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_amortization.ico` & `jal-2024.4.2/jal/img/ui_amortization.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_buy.ico` & `jal-2024.4.2/jal/img/ui_buy.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_cancel.ico` & `jal-2024.4.2/jal/img/ui_cancel.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_chart.ico` & `jal-2024.4.2/jal/img/ui_chart.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_clean.ico` & `jal-2024.4.2/jal/img/ui_clean.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_copy.ico` & `jal-2024.4.2/jal/img/ui_copy.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_coupon.ico` & `jal-2024.4.2/jal/img/ui_coupon.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_delisting.ico` & `jal-2024.4.2/jal/img/ui_delisting.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_deposit_account.ico` & `jal-2024.4.2/jal/img/ui_deposit_account.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_deposit_close.ico` & `jal-2024.4.2/jal/img/ui_deposit_close.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_deposit_open.ico` & `jal-2024.4.2/jal/img/ui_deposit_open.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_details.ico` & `jal-2024.4.2/jal/img/ui_details.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_dividend.ico` & `jal-2024.4.2/jal/img/ui_dividend.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_dividend_stock.ico` & `jal-2024.4.2/jal/img/ui_dividend_stock.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_fee.ico` & `jal-2024.4.2/jal/img/ui_fee.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_interest.ico` & `jal-2024.4.2/jal/img/ui_interest.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_jal.png` & `jal-2024.4.2/jal/img/ui_jal.png`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_list.ico` & `jal-2024.4.2/jal/img/ui_list.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_merger.ico` & `jal-2024.4.2/jal/img/ui_merger.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_minus.ico` & `jal-2024.4.2/jal/img/ui_minus.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_ok.ico` & `jal-2024.4.2/jal/img/ui_ok.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_plus.ico` & `jal-2024.4.2/jal/img/ui_plus.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_remove.ico` & `jal-2024.4.2/jal/img/ui_remove.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_renaming.ico` & `jal-2024.4.2/jal/img/ui_renaming.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_sell.ico` & `jal-2024.4.2/jal/img/ui_sell.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_spinoff.ico` & `jal-2024.4.2/jal/img/ui_spinoff.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_split.ico` & `jal-2024.4.2/jal/img/ui_split.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_tag.ico` & `jal-2024.4.2/jal/img/ui_tag.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_tax.ico` & `jal-2024.4.2/jal/img/ui_tax.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_total.ico` & `jal-2024.4.2/jal/img/ui_total.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_transfer_asset_in.ico` & `jal-2024.4.2/jal/img/ui_transfer_asset_in.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_transfer_asset_out.ico` & `jal-2024.4.2/jal/img/ui_transfer_asset_out.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_transfer_in.ico` & `jal-2024.4.2/jal/img/ui_transfer_in.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_transfer_out.ico` & `jal-2024.4.2/jal/img/ui_transfer_out.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/img/ui_vesting.ico` & `jal-2024.4.2/jal/img/ui_vesting.ico`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/jal.py` & `jal-2024.4.2/jal/jal.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/jal_init.sql` & `jal-2024.4.2/jal/jal_init.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/languages/en.qm` & `jal-2024.4.2/jal/languages/en.qm`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/languages/ru.qm` & `jal-2024.4.2/jal/languages/ru.qm`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/net/downloader.py` & `jal-2024.4.2/jal/net/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,16 @@
         }
         asset_type = {
             'stock_shares': PredefinedAsset.Stock,
             'stock_dr': PredefinedAsset.Stock,
             'stock_bonds': PredefinedAsset.Bond,
             'stock_etf': PredefinedAsset.ETF,
             'stock_ppif': PredefinedAsset.ETF,
-            'futures_forts': PredefinedAsset.Derivative
+            'futures_forts': PredefinedAsset.Derivative,
+            'currency_metal': PredefinedAsset.Commodity
         }
         asset = {}
         if not asset_code:
             return asset
         url = f"http://iss.moex.com/iss/securities/{asset_code}.xml"
         xml_root = xml_tree.fromstring(get_web_data(url))
         info_rows = xml_root.findall("data[@id='description']/rows/*")
```

### Comparing `jal-2024.4.1/jal/net/helpers.py` & `jal-2024.4.2/jal/net/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/pypi_description.md` & `jal-2024.4.2/jal/pypi_description.md`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/account_balance.py` & `jal-2024.4.2/jal/reports/account_balance.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/assets_payments.py` & `jal-2024.4.2/jal/reports/assets_payments.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/category.py` & `jal-2024.4.2/jal/reports/category.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/deals.py` & `jal-2024.4.2/jal/reports/deals.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/income_spending.py` & `jal-2024.4.2/jal/reports/income_spending.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/operations_base.py` & `jal-2024.4.2/jal/reports/operations_base.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/peer.py` & `jal-2024.4.2/jal/reports/peer.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/portfolio.py` & `jal-2024.4.2/jal/reports/portfolio.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/profit_loss.py` & `jal-2024.4.2/jal/reports/profit_loss.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/reports.py` & `jal-2024.4.2/jal/reports/reports.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/tag.py` & `jal-2024.4.2/jal/reports/tag.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/reports/term_deposits.py` & `jal-2024.4.2/jal/reports/term_deposits.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/reports/ui_account_balance_report.py` & `jal-2024.4.2/jal/ui/reports/ui_account_balance_report.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/reports/ui_assets_payments_report.py` & `jal-2024.4.2/jal/ui/reports/ui_assets_payments_report.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/reports/ui_category_report.py` & `jal-2024.4.2/jal/ui/reports/ui_category_report.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/reports/ui_deals_report.py` & `jal-2024.4.2/jal/ui/reports/ui_deals_report.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/reports/ui_income_spending_report.py` & `jal-2024.4.2/jal/ui/reports/ui_income_spending_report.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/reports/ui_peer_report.py` & `jal-2024.4.2/jal/ui/reports/ui_peer_report.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/reports/ui_portfolio_report.py` & `jal-2024.4.2/jal/ui/reports/ui_portfolio_report.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/reports/ui_profit_loss_report.py` & `jal-2024.4.2/jal/ui/reports/ui_profit_loss_report.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/reports/ui_tag_report.py` & `jal-2024.4.2/jal/ui/reports/ui_tag_report.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/reports/ui_tax_estimation.py` & `jal-2024.4.2/jal/ui/reports/ui_tax_estimation.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/reports/ui_term_deposits_report.py` & `jal-2024.4.2/jal/ui/reports/ui_term_deposits_report.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_asset_dlg.py` & `jal-2024.4.2/jal/ui/ui_asset_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_flow_export_widget.py` & `jal-2024.4.2/jal/ui/ui_flow_export_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_login_fns_dlg.py` & `jal-2024.4.2/jal/ui/ui_login_fns_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_login_lidl_plus_dlg.py` & `jal-2024.4.2/jal/ui/ui_login_lidl_plus_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_login_pingo_doce_dlg.py` & `jal-2024.4.2/jal/ui/ui_login_pingo_doce_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_main_window.py` & `jal-2024.4.2/jal/ui/ui_main_window.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_operations_widget.py` & `jal-2024.4.2/jal/ui/ui_operations_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_rebuild_window.py` & `jal-2024.4.2/jal/ui/ui_rebuild_window.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_receipt_import_dlg.py` & `jal-2024.4.2/jal/ui/ui_receipt_import_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_reference_data_dlg.py` & `jal-2024.4.2/jal/ui/ui_reference_data_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_select_account_dlg.py` & `jal-2024.4.2/jal/ui/ui_select_account_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_select_reference_dlg.py` & `jal-2024.4.2/jal/ui/ui_select_reference_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_tax_export_widget.py` & `jal-2024.4.2/jal/ui/ui_tax_export_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/ui_update_quotes_window.py` & `jal-2024.4.2/jal/ui/ui_update_quotes_window.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/widgets/ui_asset_payment_operation.py` & `jal-2024.4.2/jal/ui/widgets/ui_asset_payment_operation.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/widgets/ui_corporate_action_operation.py` & `jal-2024.4.2/jal/ui/widgets/ui_corporate_action_operation.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/widgets/ui_income_spending_operation.py` & `jal-2024.4.2/jal/ui/widgets/ui_income_spending_operation.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/widgets/ui_term_deposit_operation.py` & `jal-2024.4.2/jal/ui/widgets/ui_term_deposit_operation.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/widgets/ui_trade_operation.py` & `jal-2024.4.2/jal/ui/widgets/ui_trade_operation.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/ui/widgets/ui_transfer_operation.py` & `jal-2024.4.2/jal/ui/widgets/ui_transfer_operation.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_29.sql` & `jal-2024.4.2/jal/updates/jal_delta_29.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_30.sql` & `jal-2024.4.2/jal/updates/jal_delta_30.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_31.sql` & `jal-2024.4.2/jal/updates/jal_delta_31.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_32.sql` & `jal-2024.4.2/jal/updates/jal_delta_32.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_33.sql` & `jal-2024.4.2/jal/updates/jal_delta_33.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_34.sql` & `jal-2024.4.2/jal/updates/jal_delta_34.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_35.sql` & `jal-2024.4.2/jal/updates/jal_delta_35.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_36.sql` & `jal-2024.4.2/jal/updates/jal_delta_36.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_37.sql` & `jal-2024.4.2/jal/updates/jal_delta_37.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_38.sql` & `jal-2024.4.2/jal/updates/jal_delta_38.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_40.sql` & `jal-2024.4.2/jal/updates/jal_delta_40.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_41.sql` & `jal-2024.4.2/jal/updates/jal_delta_41.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_42.sql` & `jal-2024.4.2/jal/updates/jal_delta_42.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_43.sql` & `jal-2024.4.2/jal/updates/jal_delta_43.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_44.sql` & `jal-2024.4.2/jal/updates/jal_delta_44.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_45.sql` & `jal-2024.4.2/jal/updates/jal_delta_45.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_46.sql` & `jal-2024.4.2/jal/updates/jal_delta_46.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_47.sql` & `jal-2024.4.2/jal/updates/jal_delta_47.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_48.sql` & `jal-2024.4.2/jal/updates/jal_delta_48.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_49.sql` & `jal-2024.4.2/jal/updates/jal_delta_49.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_50.sql` & `jal-2024.4.2/jal/updates/jal_delta_50.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_51.sql` & `jal-2024.4.2/jal/updates/jal_delta_51.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_52.sql` & `jal-2024.4.2/jal/updates/jal_delta_52.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_53.sql` & `jal-2024.4.2/jal/updates/jal_delta_53.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/updates/jal_delta_55.sql` & `jal-2024.4.2/jal/updates/jal_delta_55.sql`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/abstract_operation_details.py` & `jal-2024.4.2/jal/widgets/abstract_operation_details.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/account_select.py` & `jal-2024.4.2/jal/widgets/account_select.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/asset_dialog.py` & `jal-2024.4.2/jal/widgets/asset_dialog.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/asset_payment_widget.py` & `jal-2024.4.2/jal/widgets/asset_payment_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/corporate_action_widget.py` & `jal-2024.4.2/jal/widgets/corporate_action_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/custom/date_range_selector.py` & `jal-2024.4.2/jal/widgets/custom/date_range_selector.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/custom/db_lookup_combobox.py` & `jal-2024.4.2/jal/widgets/custom/db_lookup_combobox.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/custom/log_viewer.py` & `jal-2024.4.2/jal/widgets/custom/log_viewer.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/custom/table_footer.py` & `jal-2024.4.2/jal/widgets/custom/table_footer.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/custom/tableview_with_footer.py` & `jal-2024.4.2/jal/widgets/custom/tableview_with_footer.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/custom/treeview_with_footer.py` & `jal-2024.4.2/jal/widgets/custom/treeview_with_footer.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/delegates.py` & `jal-2024.4.2/jal/widgets/delegates.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/helpers.py` & `jal-2024.4.2/jal/widgets/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/icons.py` & `jal-2024.4.2/jal/widgets/icons.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/income_spending_widget.py` & `jal-2024.4.2/jal/widgets/income_spending_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/main_window.py` & `jal-2024.4.2/jal/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/mdi.py` & `jal-2024.4.2/jal/widgets/mdi.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/operations_tabs.py` & `jal-2024.4.2/jal/widgets/operations_tabs.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/operations_widget.py` & `jal-2024.4.2/jal/widgets/operations_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/price_chart.py` & `jal-2024.4.2/jal/widgets/price_chart.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/qr_scanner.py` & `jal-2024.4.2/jal/widgets/qr_scanner.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/reference_data.py` & `jal-2024.4.2/jal/widgets/reference_data.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/reference_dialogs.py` & `jal-2024.4.2/jal/widgets/reference_dialogs.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/reference_selector.py` & `jal-2024.4.2/jal/widgets/reference_selector.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/selection_dialog.py` & `jal-2024.4.2/jal/widgets/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/tax_widget.py` & `jal-2024.4.2/jal/widgets/tax_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/term_deposit_widget.py` & `jal-2024.4.2/jal/widgets/term_deposit_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/trade_widget.py` & `jal-2024.4.2/jal/widgets/trade_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal/widgets/transfer_widget.py` & `jal-2024.4.2/jal/widgets/transfer_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/jal.egg-info/PKG-INFO` & `jal-2024.4.2/jal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2024.4.1/jal.egg-info/SOURCES.txt` & `jal-2024.4.2/jal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jal-2024.4.1/setup.py` & `jal-2024.4.2/setup.py`

 * *Files identical despite different names*

