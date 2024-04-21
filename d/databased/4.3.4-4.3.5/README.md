# Comparing `tmp/databased-4.3.4.tar.gz` & `tmp/databased-4.3.5.tar.gz`

## Comparing `databased-4.3.4.tar` & `databased-4.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 databased-4.3.4/src/databased/__init__.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 databased-4.3.4/src/databased/create_shell.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 databased-4.3.4/src/databased/customshell.py
--rw-r--r--   0        0        0    21640 2020-02-02 00:00:00.000000 databased-4.3.4/src/databased/databased.py
--rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 databased-4.3.4/src/databased/dbparsers.py
--rw-r--r--   0        0        0    18728 2020-02-02 00:00:00.000000 databased-4.3.4/src/databased/dbshell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databased-4.3.4/src/databased/py.typed
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 databased-4.3.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-4.3.4/LICENSE.txt
--rw-r--r--   0        0        0    22832 2020-02-02 00:00:00.000000 databased-4.3.4/README.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 databased-4.3.4/pyproject.toml
--rw-r--r--   0        0        0    23346 2020-02-02 00:00:00.000000 databased-4.3.4/PKG-INFO
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 databased-4.3.5/src/databased/__init__.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 databased-4.3.5/src/databased/create_shell.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 databased-4.3.5/src/databased/customshell.py
+-rw-r--r--   0        0        0    21640 2020-02-02 00:00:00.000000 databased-4.3.5/src/databased/databased.py
+-rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 databased-4.3.5/src/databased/dbparsers.py
+-rw-r--r--   0        0        0    18728 2020-02-02 00:00:00.000000 databased-4.3.5/src/databased/dbshell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databased-4.3.5/src/databased/py.typed
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 databased-4.3.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-4.3.5/LICENSE.txt
+-rw-r--r--   0        0        0    22876 2020-02-02 00:00:00.000000 databased-4.3.5/README.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 databased-4.3.5/pyproject.toml
+-rw-r--r--   0        0        0    23365 2020-02-02 00:00:00.000000 databased-4.3.5/PKG-INFO
```

### Comparing `databased-4.3.4/src/databased/create_shell.py` & `databased-4.3.5/src/databased/create_shell.py`

 * *Files identical despite different names*

### Comparing `databased-4.3.4/src/databased/customshell.py` & `databased-4.3.5/src/databased/customshell.py`

 * *Files identical despite different names*

### Comparing `databased-4.3.4/src/databased/databased.py` & `databased-4.3.5/src/databased/databased.py`

 * *Files identical despite different names*

### Comparing `databased-4.3.4/src/databased/dbparsers.py` & `databased-4.3.5/src/databased/dbparsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 
 def add_where_argument(parser: argshell.ArgShellParser) -> argshell.ArgShellParser:
     """Add an optional `where` argument to the parser and return it.
 
     The added argument has a default value of `None` and has `nargs="?"`"""
     parser.add_argument(
-        "where",
+        "-w",
+        "--where",
         type=str,
         default=None,
         nargs="?",
         help=""" The `WHERE` clause to use, if any. Don't include "WHERE" keyword in argument string. """,
     )
     return parser
```

### Comparing `databased-4.3.4/src/databased/dbshell.py` & `databased-4.3.5/src/databased/dbshell.py`

 * *Files identical despite different names*

### Comparing `databased-4.3.4/LICENSE.txt` & `databased-4.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databased-4.3.4/README.md` & `databased-4.3.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,96 +1,110 @@
 # Databased
-Databased is a module that wraps the standard library SQLite3 module to streamline integrating a database into a project.<br>
 
-Install with:
-<pre>pip install databased</pre>
+Databased is a module that wraps the standard library SQLite3 module to streamline integrating a database into a project.  
 
+Install with:
+```pip install databased```
 
-## Usage:
+## Usage
 
 ### Creation and Connections
-<pre>
+
+```python
 from databased import Databased
 
 # for reference, "chi.db" is database of Chicago food inspections and business licenses
 db = Databased("chi.db") # The file will be created if it doesn't exist
-</pre>
+```
 
-You can call `db.connect()` manually, but generally you shouldn't need to.<br>
-All database functions are built on the `db.query()` function, which will open a connection if one isn't already established.<br>
+You can call `db.connect()` manually, but generally you shouldn't need to.  
+All database functions are built on the `db.query()` function, which will open a connection if one isn't already established.  
 e.g. Accessing the `db.tables` property uses the `db.query()` function and opens a connection for you
-<pre>
+
+```python
 print(*db.tables, sep="\n")
-</pre>
+```
+
 Output:
-<pre>
+
+```console
 business_addresses
 businesses
 license_codes
 license_statuses
 licenses
 facility_types
 risk_levels
 facility_addresses
 inspected_businesses
 inspection_types
 result_types
 inspections
 violation_types
 violations
-</pre>
+```
 
 `db.query()` executes SQL strings and returns the results as a list of dictionaries
-<pre>
+
+```python
 print(
     *db.query("SELECT * FROM businesses WHERE legal_name LIKE 'z%' LIMIT 5;"), sep="\n"
 )
-</pre>
+```
+
 Output:
-<pre>
+
+```json
 {'account_number': 106, 'legal_name': 'Zaven, Inc.', 'dba': 'Zaven / Lepetit Paris', 'address_id': 6880}
 {'account_number': 113, 'legal_name': 'Zanies Comedy Clubs, Inc.', 'dba': 'Zanies Comedy Club', 'address_id': 5702}
 {'account_number': 122, 'legal_name': 'Ziemek Corporation, Inc.', 'dba': 'The Thirsty Tavern', 'address_id': 146144}
 {'account_number': 1918, 'legal_name': 'Zimmies Inc #8', 'dba': 'Original Pancake House', 'address_id': 143541}
 {'account_number': 3007, 'legal_name': 'Zikainan Nursing Home Inc', 'dba': 'All American Nursing Home', 'address_id': 155957}
-</pre>
+```
 
 When a connection is no longer needed, it will need to be manually closed.
-<pre>
+
+```python
 db.close()
-</pre>
-By default the database will be committed when db.close() is called.<br>
-This can be prevented by setting `commit_on_close` to `False` in either the Databased constructor or through the property `db.commit_on_close`.<br>
-<pre>
+```
+
+By default the database will be committed when db.close() is called.  
+This can be prevented by setting `commit_on_close` to `False` in either the Databased constructor or through the property `db.commit_on_close`.  
+
+```python
 db = Databased("chi.db", commit_on_close=False)
 # or
 db.commit_on_close = False
-</pre>
+```
+
+The database can always be committed manually with `db.commit()`.  
 
-The database can always be committed manually with `db.commit()`.<br>
+Using Databased with a context manager will call the close() method for you (and commit the database if `commit_on_close` is `True`)  
 
-Using Databased with a context manager will call the close() method for you (and commit the database if `commit_on_close` is `True`)<br>
-<pre>
+```python
 with Databased("chi.db") as db:
     print(f"{db.connected=}")
     print(*db.get_columns("businesses"), sep="\n")
 print(f"{db.connected=}")
-</pre>
+```
+
 Output:
-<pre>
+
+```python
 db.connected=True
 account_number
 legal_name
 dba
 address_id
 db.connected=False
-</pre>
+```
 
 ### Tables and Columns
-<pre>
+
+```python
 with Databased("chi.db") as db:
     db.create_table(
         "inspectors",
         "id INTEGER PRIMARY KEY AUTOINCREMENT",
         "first_name TEXT",
         "last_name TEXT",
         "ward INTEGER",
@@ -109,17 +123,19 @@
     print()
     # ---------------------------------------------------------
     db.drop_column("employees", "title")
     db.rename_table("employees", "inspectors")
     print(db.to_grid(db.select("inspectors")))
     print()
     db.drop_table("inspectors")
-</pre>
+```
+
 Output:
-<pre>
+
+```console
 +------+--------------+-------------+--------+
 | id   | first_name   | last_name   | ward   |
 +======+==============+=============+========+
 | 1    | Billy        | Bob         | 1      |
 +------+--------------+-------------+--------+
 | 2    | Jenna        | Jones       | 33     |
 +------+--------------+-------------+--------+
@@ -141,21 +157,23 @@
 +======+==============+=============+========+
 | 1    | Billy        | Bob         | 1      |
 +------+--------------+-------------+--------+
 | 2    | Jenna        | Jones       | 33     |
 +------+--------------+-------------+--------+
 | 3    | Tiny         | Tim         | 25     |
 +------+--------------+-------------+--------+
-</pre>
+```
 
 ### Select
-Moderately complex queries can be executed with `db.select()`.<br>
-More advanced queries will need to be written out and executed directly with `db.query()`.<br>
+
+Moderately complex queries can be executed with `db.select()`.  
+More advanced queries will need to be written out and executed directly with `db.query()`.  
 Example using all available `db.select()` parameters:
-<pre>
+
+```python
 with Databased("chi.db") as db:
     print(
         db.to_grid(
             db.select(
                 table="inspections",
                 columns=[
                     "inspections.license_number",
@@ -197,17 +215,19 @@
             GROUP BY inspections.license_number
             HAVING num_inspections > 10
             ORDER BY num_inspections DESC
             LIMIT 5;
             """
             )
         )
-</pre>
+```
+
 Output:
-<pre>
+
+```console
 +------------------+-------------------------+------+--------------------+--------+-------------------+
 | license_number   | legal_name              | id   | description        | ward   | num_inspections   |
 +==================+=========================+======+====================+========+===================+
 | 2583423          | Meadowflour Llc         | 7    | Pass W/ Conditions | 40     | 18                |
 +------------------+-------------------------+------+--------------------+--------+-------------------+
 | 2594606          | Hz Ops Holdings Inc     | 4    | Not Ready          | 6      | 17                |
 +------------------+-------------------------+------+--------------------+--------+-------------------+
@@ -227,28 +247,31 @@
 +------------------+-------------------------+------+--------------------+--------+-------------------+
 | 2405951          | Wendy's Properties, Llc | 7    | Pass W/ Conditions | 10     | 17                |
 +------------------+-------------------------+------+--------------------+--------+-------------------+
 | 833              | Steve Ziemek            | 7    | Pass W/ Conditions | 10     | 17                |
 +------------------+-------------------------+------+--------------------+--------+-------------------+
 | 55418            | 2053 W. Division Inc.   | 5    | Out Of Business    | 1      | 16                |
 +------------------+-------------------------+------+--------------------+--------+-------------------+
-</pre>
+```
 
 ### Update
-<pre>
+
+```python
 with Databased("chi.db", commit_on_close=False) as db:
     print(db.to_grid(db.select("businesses", where="dba LIKE 'deli %'")))
     num_rows = db.update(
         "businesses", "dba", "deli BreadMeat City", "dba LIKE 'deli %'"
     )
     print(f"num rows updated: {num_rows}")
     print(db.to_grid(db.select("businesses", where="dba LIKE 'deli %'")))
-</pre>
+```
+
 Output:
-<pre>
+
+```console
 +------------------+-------------------------+---------------------------------+--------------+
 | account_number   | legal_name              | dba                             | address_id   |
 +==================+=========================+=================================+==============+
 | 17214            | Emil Korpacki, Inc.     | Deli On Rice                    | 110271       |
 +------------------+-------------------------+---------------------------------+--------------+
 | 348935           | Deli King Inc.          | Deli King Inc.                  | 17090        |
 +------------------+-------------------------+---------------------------------+--------------+
@@ -268,36 +291,40 @@
 +------------------+-------------------------+---------------------+--------------+
 | 389169           | Pheidias, Inc.          | deli BreadMeat City | 138721       |
 +------------------+-------------------------+---------------------+--------------+
 | 391766           | Ted's Deli & More, Inc. | deli BreadMeat City | 142080       |
 +------------------+-------------------------+---------------------+--------------+
 | 421955           | Deli Flavor, Inc.       | deli BreadMeat City | 5057         |
 +------------------+-------------------------+---------------------+--------------+
-</pre>
+```
 
 ### Delete
-<pre>
+
+```python
 with Databased("chi.db", commit_on_close=False) as db:
     num_rows = db.delete("businesses", "dba LIKE 'deli %' AND address_id > 6000")
     print(f"num rows deleted: {num_rows}")
     print(db.to_grid(db.select("businesses", where="dba LIKE 'deli %'")))
-</pre>
+```
+
 Output:
-<pre>
+
+```console
 num rows deleted: 4
 +------------------+-------------------+-------------+--------------+
 | account_number   | legal_name        | dba         | address_id   |
 +==================+===================+=============+==============+
 | 421955           | Deli Flavor, Inc. | Deli Flavor | 5057         |
 +------------------+-------------------+-------------+--------------+
-</pre>
+```
 
-`databased` also comes with an interactive shell called `dbshell`, which is built from the [argshell](https://github.com/matt-manes/argshell) package.<br>
+`databased` also comes with an interactive shell called `dbshell`, which is built from the [argshell](https://github.com/matt-manes/argshell) package.  
 It can be launched from the terminal by entering `dbshell`
-<pre>
+
+```console
 >dbshell
 Searching for database...
 Could not find a .db file in e:/1vsCode/python/databased.
 Enter path to .db file to use or press enter to search again recursively:
 Searching recursively...
 DB options:
 (1) shelltesting/chi.db (2) shelltesting/chi_backup.db (3) shelltesting/chi_backup_09-21-2023-12_06_37_PM.db
@@ -389,13 +416,11 @@
 +------+----------------------------------------------------+
 | 62   | Compliance With Clean Indoor Air Ordinance         |
 +------+----------------------------------------------------+
 | 61   | Summary Report Displayed And Visible To The Public |
 +------+----------------------------------------------------+
 | 60   | Previous Core Violation Corrected                  |
 +------+----------------------------------------------------+
-</pre>
-The `customize` command or the `custom_shell` script can be used to generate a template file in the current directory that subclasses `DBManager`.<br>
-This allows for project specific additional commands as well as modifications of available commands.
-
-
+```
 
+The `customize` command or the `custom_shell` script can be used to generate a template file in the current directory that subclasses `DBManager`.  
+This allows for project specific additional commands as well as modifications of available commands.
```

### Comparing `databased-4.3.4/pyproject.toml` & `databased-4.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "databased"
 description = "Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier."
-version = "4.3.4"
+version = "4.3.5"
 dependencies = ["tabulate", "argshell", "pathier", "griddle", "loggi", "noiftimer", "printbuddies", "rich"]
 readme = "README.md"
 keywords = ["database", "sqlite", "sqlite3"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 requires-python = ">=3.10, <=3.12"
 
 [[project.authors]]
```

### Comparing `databased-4.3.4/PKG-INFO` & `databased-4.3.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: databased
-Version: 4.3.4
+Version: 4.3.5
 Summary: Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier.
 Project-URL: Homepage, https://github.com/matt-manes/databased
 Project-URL: Documentation, https://github.com/matt-manes/databased/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/databased/tree/main/src/databased
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: database,sqlite,sqlite3
@@ -19,102 +19,116 @@
 Requires-Dist: pathier
 Requires-Dist: printbuddies
 Requires-Dist: rich
 Requires-Dist: tabulate
 Description-Content-Type: text/markdown
 
 # Databased
-Databased is a module that wraps the standard library SQLite3 module to streamline integrating a database into a project.<br>
 
-Install with:
-<pre>pip install databased</pre>
+Databased is a module that wraps the standard library SQLite3 module to streamline integrating a database into a project.  
 
+Install with:
+```pip install databased```
 
-## Usage:
+## Usage
 
 ### Creation and Connections
-<pre>
+
+```python
 from databased import Databased
 
 # for reference, "chi.db" is database of Chicago food inspections and business licenses
 db = Databased("chi.db") # The file will be created if it doesn't exist
-</pre>
+```
 
-You can call `db.connect()` manually, but generally you shouldn't need to.<br>
-All database functions are built on the `db.query()` function, which will open a connection if one isn't already established.<br>
+You can call `db.connect()` manually, but generally you shouldn't need to.  
+All database functions are built on the `db.query()` function, which will open a connection if one isn't already established.  
 e.g. Accessing the `db.tables` property uses the `db.query()` function and opens a connection for you
-<pre>
+
+```python
 print(*db.tables, sep="\n")
-</pre>
+```
+
 Output:
-<pre>
+
+```console
 business_addresses
 businesses
 license_codes
 license_statuses
 licenses
 facility_types
 risk_levels
 facility_addresses
 inspected_businesses
 inspection_types
 result_types
 inspections
 violation_types
 violations
-</pre>
+```
 
 `db.query()` executes SQL strings and returns the results as a list of dictionaries
-<pre>
+
+```python
 print(
     *db.query("SELECT * FROM businesses WHERE legal_name LIKE 'z%' LIMIT 5;"), sep="\n"
 )
-</pre>
+```
+
 Output:
-<pre>
+
+```json
 {'account_number': 106, 'legal_name': 'Zaven, Inc.', 'dba': 'Zaven / Lepetit Paris', 'address_id': 6880}
 {'account_number': 113, 'legal_name': 'Zanies Comedy Clubs, Inc.', 'dba': 'Zanies Comedy Club', 'address_id': 5702}
 {'account_number': 122, 'legal_name': 'Ziemek Corporation, Inc.', 'dba': 'The Thirsty Tavern', 'address_id': 146144}
 {'account_number': 1918, 'legal_name': 'Zimmies Inc #8', 'dba': 'Original Pancake House', 'address_id': 143541}
 {'account_number': 3007, 'legal_name': 'Zikainan Nursing Home Inc', 'dba': 'All American Nursing Home', 'address_id': 155957}
-</pre>
+```
 
 When a connection is no longer needed, it will need to be manually closed.
-<pre>
+
+```python
 db.close()
-</pre>
-By default the database will be committed when db.close() is called.<br>
-This can be prevented by setting `commit_on_close` to `False` in either the Databased constructor or through the property `db.commit_on_close`.<br>
-<pre>
+```
+
+By default the database will be committed when db.close() is called.  
+This can be prevented by setting `commit_on_close` to `False` in either the Databased constructor or through the property `db.commit_on_close`.  
+
+```python
 db = Databased("chi.db", commit_on_close=False)
 # or
 db.commit_on_close = False
-</pre>
+```
+
+The database can always be committed manually with `db.commit()`.  
 
-The database can always be committed manually with `db.commit()`.<br>
+Using Databased with a context manager will call the close() method for you (and commit the database if `commit_on_close` is `True`)  
 
-Using Databased with a context manager will call the close() method for you (and commit the database if `commit_on_close` is `True`)<br>
-<pre>
+```python
 with Databased("chi.db") as db:
     print(f"{db.connected=}")
     print(*db.get_columns("businesses"), sep="\n")
 print(f"{db.connected=}")
-</pre>
+```
+
 Output:
-<pre>
+
+```python
 db.connected=True
 account_number
 legal_name
 dba
 address_id
 db.connected=False
-</pre>
+```
 
 ### Tables and Columns
-<pre>
+
+```python
 with Databased("chi.db") as db:
     db.create_table(
         "inspectors",
         "id INTEGER PRIMARY KEY AUTOINCREMENT",
         "first_name TEXT",
         "last_name TEXT",
         "ward INTEGER",
@@ -133,17 +147,19 @@
     print()
     # ---------------------------------------------------------
     db.drop_column("employees", "title")
     db.rename_table("employees", "inspectors")
     print(db.to_grid(db.select("inspectors")))
     print()
     db.drop_table("inspectors")
-</pre>
+```
+
 Output:
-<pre>
+
+```console
 +------+--------------+-------------+--------+
 | id   | first_name   | last_name   | ward   |
 +======+==============+=============+========+
 | 1    | Billy        | Bob         | 1      |
 +------+--------------+-------------+--------+
 | 2    | Jenna        | Jones       | 33     |
 +------+--------------+-------------+--------+
@@ -165,21 +181,23 @@
 +======+==============+=============+========+
 | 1    | Billy        | Bob         | 1      |
 +------+--------------+-------------+--------+
 | 2    | Jenna        | Jones       | 33     |
 +------+--------------+-------------+--------+
 | 3    | Tiny         | Tim         | 25     |
 +------+--------------+-------------+--------+
-</pre>
+```
 
 ### Select
-Moderately complex queries can be executed with `db.select()`.<br>
-More advanced queries will need to be written out and executed directly with `db.query()`.<br>
+
+Moderately complex queries can be executed with `db.select()`.  
+More advanced queries will need to be written out and executed directly with `db.query()`.  
 Example using all available `db.select()` parameters:
-<pre>
+
+```python
 with Databased("chi.db") as db:
     print(
         db.to_grid(
             db.select(
                 table="inspections",
                 columns=[
                     "inspections.license_number",
@@ -221,17 +239,19 @@
             GROUP BY inspections.license_number
             HAVING num_inspections > 10
             ORDER BY num_inspections DESC
             LIMIT 5;
             """
             )
         )
-</pre>
+```
+
 Output:
-<pre>
+
+```console
 +------------------+-------------------------+------+--------------------+--------+-------------------+
 | license_number   | legal_name              | id   | description        | ward   | num_inspections   |
 +==================+=========================+======+====================+========+===================+
 | 2583423          | Meadowflour Llc         | 7    | Pass W/ Conditions | 40     | 18                |
 +------------------+-------------------------+------+--------------------+--------+-------------------+
 | 2594606          | Hz Ops Holdings Inc     | 4    | Not Ready          | 6      | 17                |
 +------------------+-------------------------+------+--------------------+--------+-------------------+
@@ -251,28 +271,31 @@
 +------------------+-------------------------+------+--------------------+--------+-------------------+
 | 2405951          | Wendy's Properties, Llc | 7    | Pass W/ Conditions | 10     | 17                |
 +------------------+-------------------------+------+--------------------+--------+-------------------+
 | 833              | Steve Ziemek            | 7    | Pass W/ Conditions | 10     | 17                |
 +------------------+-------------------------+------+--------------------+--------+-------------------+
 | 55418            | 2053 W. Division Inc.   | 5    | Out Of Business    | 1      | 16                |
 +------------------+-------------------------+------+--------------------+--------+-------------------+
-</pre>
+```
 
 ### Update
-<pre>
+
+```python
 with Databased("chi.db", commit_on_close=False) as db:
     print(db.to_grid(db.select("businesses", where="dba LIKE 'deli %'")))
     num_rows = db.update(
         "businesses", "dba", "deli BreadMeat City", "dba LIKE 'deli %'"
     )
     print(f"num rows updated: {num_rows}")
     print(db.to_grid(db.select("businesses", where="dba LIKE 'deli %'")))
-</pre>
+```
+
 Output:
-<pre>
+
+```console
 +------------------+-------------------------+---------------------------------+--------------+
 | account_number   | legal_name              | dba                             | address_id   |
 +==================+=========================+=================================+==============+
 | 17214            | Emil Korpacki, Inc.     | Deli On Rice                    | 110271       |
 +------------------+-------------------------+---------------------------------+--------------+
 | 348935           | Deli King Inc.          | Deli King Inc.                  | 17090        |
 +------------------+-------------------------+---------------------------------+--------------+
@@ -292,36 +315,40 @@
 +------------------+-------------------------+---------------------+--------------+
 | 389169           | Pheidias, Inc.          | deli BreadMeat City | 138721       |
 +------------------+-------------------------+---------------------+--------------+
 | 391766           | Ted's Deli & More, Inc. | deli BreadMeat City | 142080       |
 +------------------+-------------------------+---------------------+--------------+
 | 421955           | Deli Flavor, Inc.       | deli BreadMeat City | 5057         |
 +------------------+-------------------------+---------------------+--------------+
-</pre>
+```
 
 ### Delete
-<pre>
+
+```python
 with Databased("chi.db", commit_on_close=False) as db:
     num_rows = db.delete("businesses", "dba LIKE 'deli %' AND address_id > 6000")
     print(f"num rows deleted: {num_rows}")
     print(db.to_grid(db.select("businesses", where="dba LIKE 'deli %'")))
-</pre>
+```
+
 Output:
-<pre>
+
+```console
 num rows deleted: 4
 +------------------+-------------------+-------------+--------------+
 | account_number   | legal_name        | dba         | address_id   |
 +==================+===================+=============+==============+
 | 421955           | Deli Flavor, Inc. | Deli Flavor | 5057         |
 +------------------+-------------------+-------------+--------------+
-</pre>
+```
 
-`databased` also comes with an interactive shell called `dbshell`, which is built from the [argshell](https://github.com/matt-manes/argshell) package.<br>
+`databased` also comes with an interactive shell called `dbshell`, which is built from the [argshell](https://github.com/matt-manes/argshell) package.  
 It can be launched from the terminal by entering `dbshell`
-<pre>
+
+```console
 >dbshell
 Searching for database...
 Could not find a .db file in e:/1vsCode/python/databased.
 Enter path to .db file to use or press enter to search again recursively:
 Searching recursively...
 DB options:
 (1) shelltesting/chi.db (2) shelltesting/chi_backup.db (3) shelltesting/chi_backup_09-21-2023-12_06_37_PM.db
@@ -413,13 +440,11 @@
 +------+----------------------------------------------------+
 | 62   | Compliance With Clean Indoor Air Ordinance         |
 +------+----------------------------------------------------+
 | 61   | Summary Report Displayed And Visible To The Public |
 +------+----------------------------------------------------+
 | 60   | Previous Core Violation Corrected                  |
 +------+----------------------------------------------------+
-</pre>
-The `customize` command or the `custom_shell` script can be used to generate a template file in the current directory that subclasses `DBManager`.<br>
-This allows for project specific additional commands as well as modifications of available commands.
-
-
+```
 
+The `customize` command or the `custom_shell` script can be used to generate a template file in the current directory that subclasses `DBManager`.  
+This allows for project specific additional commands as well as modifications of available commands.
```

