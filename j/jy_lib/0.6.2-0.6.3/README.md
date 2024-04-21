# Comparing `tmp/jy_lib-0.6.2.tar.gz` & `tmp/jy_lib-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy_lib-0.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jy_lib-0.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jy_lib-0.6.2.tar` & `jy_lib-0.6.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.6.2/.gitignore
--rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.6.2/.pypirc
--rw-r--r--   0        0        0      466 2023-10-19 02:20:46.582059 jy_lib-0.6.2/.vscode/launch.json
--rw-r--r--   0        0        0     1615 2023-10-19 02:20:46.582499 jy_lib-0.6.2/.vscode/settings.json
--rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.6.2/LICENSE
--rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.6.2/Pipfile
--rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.6.2/Pipfile.lock
--rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.6.2/README.md
--rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.6.2/README_Project.md
--rw-r--r--   0        0        0      518 2024-04-18 00:57:34.004921 jy_lib-0.6.2/jy_lib/__init__.py
--rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.6.2/jy_lib/auth_client.py
--rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.6.2/jy_lib/bank.py
--rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.6.2/jy_lib/base.py
--rw-r--r--   0        0        0     2972 2024-04-18 00:57:02.602284 jy_lib-0.6.2/jy_lib/cache.py
--rw-r--r--   0        0        0     3356 2024-04-15 08:39:28.625202 jy_lib-0.6.2/jy_lib/clickhouse.py
--rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.6.2/jy_lib/compressor.py
--rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.6.2/jy_lib/country.py
--rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.6.2/jy_lib/currency.py
--rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.6.2/jy_lib/date.py
--rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.6.2/jy_lib/decorator.py
--rw-r--r--   0        0        0     4230 2023-10-25 08:34:10.094139 jy_lib-0.6.2/jy_lib/exchange.py
--rw-r--r--   0        0        0      602 2024-03-26 02:17:46.967953 jy_lib-0.6.2/jy_lib/interrupt_protect.py
--rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.6.2/jy_lib/lock.py
--rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.6.2/jy_lib/math.py
--rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.6.2/jy_lib/nav.py
--rw-r--r--   0        0        0    18478 2024-04-17 00:51:09.235795 jy_lib-0.6.2/jy_lib/smb_client.py
--rw-r--r--   0        0        0     4385 2024-01-16 08:18:48.686163 jy_lib-0.6.2/jy_lib/symbol.py
--rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.6.2/jy_lib/symbol_em.py
--rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.6.2/jy_lib/time.py
--rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.6.2/publish-jypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.6.2/publish-pypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.6.2/publish-test.sh
--rw-r--r--   0        0        0      639 2024-04-11 07:52:56.404049 jy_lib-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-15 07:06:48.431549 jy_lib-0.6.2/requirements.txt
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     2083 2024-01-01 02:29:02.554641 jy_lib-0.6.3/.gitignore
+-rw-r--r--   0        0        0      285 2024-01-01 02:29:02.554755 jy_lib-0.6.3/.pypirc
+-rw-r--r--   0        0        0      466 2024-01-01 02:29:02.554898 jy_lib-0.6.3/.vscode/launch.json
+-rw-r--r--   0        0        0     1615 2024-01-01 02:29:02.554993 jy_lib-0.6.3/.vscode/settings.json
+-rw-r--r--   0        0        0     1073 2024-01-01 02:29:02.555085 jy_lib-0.6.3/LICENSE
+-rw-r--r--   0        0        0      573 2024-04-21 14:22:14.414420 jy_lib-0.6.3/Pipfile
+-rw-r--r--   0        0        0    40838 2024-01-01 02:29:02.555480 jy_lib-0.6.3/Pipfile.lock
+-rw-r--r--   0        0        0       10 2024-01-01 02:29:02.555572 jy_lib-0.6.3/README.md
+-rw-r--r--   0        0        0      469 2024-01-01 02:29:02.555665 jy_lib-0.6.3/README_Project.md
+-rw-r--r--   0        0        0      518 2024-04-21 14:22:38.760916 jy_lib-0.6.3/jy_lib/__init__.py
+-rw-r--r--   0        0        0     7230 2024-01-01 02:29:02.555927 jy_lib-0.6.3/jy_lib/auth_client.py
+-rw-r--r--   0        0        0    10531 2024-01-01 02:29:02.556043 jy_lib-0.6.3/jy_lib/bank.py
+-rw-r--r--   0        0        0      809 2024-01-01 02:29:02.556135 jy_lib-0.6.3/jy_lib/base.py
+-rw-r--r--   0        0        0     3549 2024-04-21 14:22:14.414940 jy_lib-0.6.3/jy_lib/cache.py
+-rw-r--r--   0        0        0     3356 2024-04-21 14:22:14.415034 jy_lib-0.6.3/jy_lib/clickhouse.py
+-rw-r--r--   0        0        0     4411 2024-04-21 14:22:14.415174 jy_lib-0.6.3/jy_lib/compressor.py
+-rw-r--r--   0        0        0    21765 2024-01-01 02:29:02.556414 jy_lib-0.6.3/jy_lib/country.py
+-rw-r--r--   0        0        0    10928 2024-01-01 02:29:02.556554 jy_lib-0.6.3/jy_lib/currency.py
+-rw-r--r--   0        0        0     2399 2024-04-21 14:22:14.416027 jy_lib-0.6.3/jy_lib/date.py
+-rw-r--r--   0        0        0      931 2024-01-01 02:29:02.556726 jy_lib-0.6.3/jy_lib/decorator.py
+-rw-r--r--   0        0        0     4230 2024-01-01 02:29:02.556837 jy_lib-0.6.3/jy_lib/exchange.py
+-rw-r--r--   0        0        0      602 2024-04-21 14:22:14.416177 jy_lib-0.6.3/jy_lib/interrupt_protect.py
+-rw-r--r--   0        0        0     2151 2024-01-01 02:29:02.556936 jy_lib-0.6.3/jy_lib/lock.py
+-rw-r--r--   0        0        0      707 2024-04-21 14:22:14.416596 jy_lib-0.6.3/jy_lib/math.py
+-rw-r--r--   0        0        0     5926 2024-01-01 02:29:02.557127 jy_lib-0.6.3/jy_lib/nav.py
+-rw-r--r--   0        0        0    18478 2024-04-21 14:22:14.416811 jy_lib-0.6.3/jy_lib/smb_client.py
+-rw-r--r--   0        0        0     4385 2024-04-21 14:22:14.417137 jy_lib-0.6.3/jy_lib/symbol.py
+-rw-r--r--   0        0        0    20726 2024-04-21 14:22:14.417332 jy_lib-0.6.3/jy_lib/symbol_em.py
+-rw-r--r--   0        0        0      577 2024-01-01 02:29:02.557631 jy_lib-0.6.3/jy_lib/time.py
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557712 jy_lib-0.6.3/publish-jypi.sh
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557791 jy_lib-0.6.3/publish-pypi.sh
+-rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557873 jy_lib-0.6.3/publish-test.sh
+-rw-r--r--   0        0        0      639 2024-04-21 14:22:14.417488 jy_lib-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-21 14:22:14.417721 jy_lib-0.6.3/requirements.txt
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.6.3/PKG-INFO
```

### Comparing `jy_lib-0.6.2/.gitignore` & `jy_lib-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/.vscode/settings.json` & `jy_lib-0.6.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/LICENSE` & `jy_lib-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/Pipfile` & `jy_lib-0.6.3/Pipfile`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/Pipfile.lock` & `jy_lib-0.6.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/__init__.py` & `jy_lib-0.6.3/jy_lib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 Python SDK for jyfund
 """
 # 枚举类
 from .bank import Bank
 from .country import CountryA2, CountryA3
 from .currency import Currency
 from .exchange import Exchange
-from .lock import SyncRWLock, AsyncRWLock
-from .symbol_em import KLineRecord, TrendRecord, EMParser
+from .lock import AsyncRWLock, SyncRWLock
 from .symbol import (
-    SymbolSubType,
-    StockType,
-    FundType,
+    BlockType,
     BondType,
-    OptionsType,
     DrType,
-    IndexType,
+    FundType,
     FuturesType,
-    WarrantsType,
-    BlockType,
+    IndexType,
+    OptionsType,
     SpotType,
-    SymbolType,
+    StockType,
     SymbolFlag,
+    SymbolSubType,
+    SymbolType,
+    WarrantsType,
 )
+from .symbol_em import EMParser, KLineRecord, TrendRecord
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
```

### Comparing `jy_lib-0.6.2/jy_lib/auth_client.py` & `jy_lib-0.6.3/jy_lib/auth_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/bank.py` & `jy_lib-0.6.3/jy_lib/bank.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/base.py` & `jy_lib-0.6.3/jy_lib/base.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/cache.py` & `jy_lib-0.6.3/jy_lib/cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,54 +9,62 @@
 import time
 from typing import Any, Set, List
 
 
 class Cache:
     """持久化TTL缓存"""
 
-    def __init__(self, path: str):
+    def __init__(self, path: str = None):
         current_frame = inspect.currentframe()
         caller_frame = current_frame.f_back
         caller_file = caller_frame.f_code.co_filename
+        if not path:
+            path: str = f'_{os.path.splitext(os.path.basename(caller_file))[0]}.db3'
         self.path: str = os.path.join(os.path.dirname(caller_file), path)
+
         self.conn = sqlite3.connect(self.path)
         self.datasets: Set[str] = self.get_tables()
 
     def get_tables(self) -> Set[str]:
+        """获取所有数据集"""
         cursor = self.conn.cursor()
         r = cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
         return {row[0] for row in r.fetchall()}
 
     def create_table(self, dataset: str) -> None:
+        """创建数据集"""
         assert not re.findall(r'\s', dataset)
         self.conn.execute(f"""CREATE TABLE IF NOT EXISTS `{dataset}` (
             `key` TEXT PRIMARY KEY NOT NULL,
             `value` BLOB NOT NULL,
             `expired_at` REAL NOT NULL
         )""")
         self.conn.execute(f"""CREATE INDEX IF NOT EXISTS expired_at ON `{dataset}` (`expired_at`)""")
         self.conn.commit()
 
     def set(self, dataset: str, key: str, value: Any, expire: float = math.inf) -> None:
+        """设置键值"""
         if dataset not in self.datasets:
             self.create_table(dataset=dataset)
             self.datasets.clear()
             self.datasets.update(self.get_tables())
         payload: bytes = lz4.frame.compress(pickle.dumps(value))
         sql: str = f"""REPLACE INTO `{dataset}` (`key`, `value`, `expired_at`) VALUES(?,?,?)"""
         self.conn.execute(sql, (key, payload, time.time() + expire))
         self.conn.commit()
 
     def delete(self, dataset: str, key: str) -> None:
+        """删除键值对"""
         if dataset in self.datasets:
             sql: str = f"""DELETE FROM `{dataset}` WHERE `key`=?"""
             self.conn.execute(sql, (key, ))
             self.conn.commit()
 
     def get(self, dataset: str, key: str) -> Any | None:
+        """获取键值"""
         if dataset in self.datasets:
             cursor = self.conn.cursor()
             sql: str = f"""SELECT `value`, `expired_at` FROM `{dataset}` WHERE `key`=?"""
             r = cursor.execute(sql, (key, ))
             r = r.fetchone()
             if r is None:
                 return r
@@ -65,16 +73,25 @@
                 if expired_at > time.time():
                     return pickle.loads(lz4.frame.decompress(value))
                 else:
                     self.delete(dataset=dataset, key=key)
                     return None
 
     def keys(self, dataset: str) -> List[str] | None:
+        """列出所有键名"""
         if dataset in self.datasets:
             cursor = self.conn.cursor()
             sql: str = f"""SELECT `key` FROM `{dataset}` WHERE `expired_at`>?"""
             r = cursor.execute(sql, (time.time(), ))
             return [r[0] for r in r.fetchall()]
 
+    def drop_table(self, dataset: str):
+        """删除数据集"""
+        if dataset in self.datasets:
+            sql: str = f"""DROP TABLE IF EXISTS `{dataset}`"""
+            self.conn.execute(sql)
+            self.conn.commit()
+            self.datasets.discard(dataset)
+
     def close(self):
         self.conn.commit()
         self.conn.close()
```

### Comparing `jy_lib-0.6.2/jy_lib/clickhouse.py` & `jy_lib-0.6.3/jy_lib/clickhouse.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/compressor.py` & `jy_lib-0.6.3/jy_lib/compressor.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/country.py` & `jy_lib-0.6.3/jy_lib/country.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/currency.py` & `jy_lib-0.6.3/jy_lib/currency.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/date.py` & `jy_lib-0.6.3/jy_lib/date.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/decorator.py` & `jy_lib-0.6.3/jy_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/exchange.py` & `jy_lib-0.6.3/jy_lib/exchange.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/interrupt_protect.py` & `jy_lib-0.6.3/jy_lib/interrupt_protect.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/lock.py` & `jy_lib-0.6.3/jy_lib/lock.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/math.py` & `jy_lib-0.6.3/jy_lib/math.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/nav.py` & `jy_lib-0.6.3/jy_lib/nav.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/smb_client.py` & `jy_lib-0.6.3/jy_lib/smb_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/symbol.py` & `jy_lib-0.6.3/jy_lib/symbol.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/symbol_em.py` & `jy_lib-0.6.3/jy_lib/symbol_em.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/jy_lib/time.py` & `jy_lib-0.6.3/jy_lib/time.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.2/pyproject.toml` & `jy_lib-0.6.3/pyproject.toml`

 * *Files identical despite different names*

