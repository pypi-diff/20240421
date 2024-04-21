# Comparing `tmp/autocar_automate_po-0.3.8.tar.gz` & `tmp/autocar_automate_po-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocar_automate_po-0.3.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "autocar_automate_po-0.3.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `autocar_automate_po-0.3.8.tar` & `autocar_automate_po-0.3.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1920 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/.gitignore
--rw-r--r--   0        0        0     1068 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/LICENSE
--rw-r--r--   0        0        0       21 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/README.md
--rw-r--r--   0        0        0       51 2024-04-17 16:34:25.891431 autocar_automate_po-0.3.8/autocar_automate_po/__init__.py
--rw-r--r--   0        0        0    27865 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/autocar_automate_po/automate_po_process.py
--rw-r--r--   0        0        0     2262 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/autocar_automate_po/print_po.py
--rw-r--r--   0        0        0      436 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/pyproject.toml
--rw-r--r--   0        0        0       78 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.8/requirements.txt
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 autocar_automate_po-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1920 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1068 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.9/LICENSE
+-rw-r--r--   0        0        0       21 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.9/README.md
+-rw-r--r--   0        0        0       51 2024-04-17 16:41:35.427411 autocar_automate_po-0.3.9/autocar_automate_po/__init__.py
+-rw-r--r--   0        0        0    27922 2024-04-17 16:41:35.431411 autocar_automate_po-0.3.9/autocar_automate_po/automate_po_process.py
+-rw-r--r--   0        0        0     2262 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.9/autocar_automate_po/print_po.py
+-rw-r--r--   0        0        0      436 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-17 16:32:52.907436 autocar_automate_po-0.3.9/requirements.txt
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 autocar_automate_po-0.3.9/PKG-INFO
```

### Comparing `autocar_automate_po-0.3.8/.gitignore` & `autocar_automate_po-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `autocar_automate_po-0.3.8/LICENSE` & `autocar_automate_po-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autocar_automate_po-0.3.8/autocar_automate_po/automate_po_process.py` & `autocar_automate_po-0.3.9/autocar_automate_po/automate_po_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,15 +563,16 @@
             'Cost_Center': '',
             'Line_Comments': line_comments,
             'Ship_To': ship_to_nr,
             'Header_Comments': 'Please reference this Purchase Order on the Invoice. Email the Invoice to ap@autocartruck.com',
             'Supplier_Number': supplier_nr,
             'Supplier_Name': supplier_name
         }
-        df = pd.concat([df, data_to_df], ignore_index=True)
+        data_to_df_series = pd.Series(data_to_df)
+        df = pd.concat([df, data_to_df_series], ignore_index=True)
     return df
 
 
 def populate_export(check_filename, time_identifier):
     def df_check_read_excel():
         df_check = pd.read_excel(check_filename, converters={
             'Supplier_Number': str,
```

### Comparing `autocar_automate_po-0.3.8/autocar_automate_po/print_po.py` & `autocar_automate_po-0.3.9/autocar_automate_po/print_po.py`

 * *Files identical despite different names*

