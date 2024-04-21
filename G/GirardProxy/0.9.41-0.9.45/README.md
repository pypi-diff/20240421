# Comparing `tmp/girardproxy-0.9.41.tar.gz` & `tmp/girardproxy-0.9.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girardproxy-0.9.41.tar", last modified: Sun Apr 21 10:18:03 2024, max compression
+gzip compressed data, was "girardproxy-0.9.45.tar", last modified: Sun Apr 21 12:03:42 2024, max compression
```

## Comparing `girardproxy-0.9.41.tar` & `girardproxy-0.9.45.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:18:03.718453 girardproxy-0.9.41/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:18:03.718453 girardproxy-0.9.41/GirardProxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-21 10:18:03.000000 girardproxy-0.9.41/GirardProxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-21 10:18:03.000000 girardproxy-0.9.41/GirardProxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:18:03.000000 girardproxy-0.9.41/GirardProxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 10:18:03.000000 girardproxy-0.9.41/GirardProxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-21 10:18:03.000000 girardproxy-0.9.41/GirardProxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 10:17:58.000000 girardproxy-0.9.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-21 10:18:03.718453 girardproxy-0.9.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 10:18:03.718453 girardproxy-0.9.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-21 10:17:58.000000 girardproxy-0.9.41/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:18:03.718453 girardproxy-0.9.41/src/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:17:58.000000 girardproxy-0.9.41/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-21 10:17:58.000000 girardproxy-0.9.41/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:03:42.909198 girardproxy-0.9.45/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:03:42.909198 girardproxy-0.9.45/GirardProxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-21 12:03:42.000000 girardproxy-0.9.45/GirardProxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-21 12:03:42.000000 girardproxy-0.9.45/GirardProxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:03:42.000000 girardproxy-0.9.45/GirardProxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 12:03:42.000000 girardproxy-0.9.45/GirardProxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 12:03:42.000000 girardproxy-0.9.45/GirardProxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 12:03:38.000000 girardproxy-0.9.45/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-21 12:03:42.909198 girardproxy-0.9.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 12:03:42.909198 girardproxy-0.9.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-21 12:03:38.000000 girardproxy-0.9.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:03:42.909198 girardproxy-0.9.45/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-21 12:03:38.000000 girardproxy-0.9.45/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-21 12:03:38.000000 girardproxy-0.9.45/src/proxy.py
```

### Comparing `girardproxy-0.9.41/GirardProxy.egg-info/PKG-INFO` & `girardproxy-0.9.45/GirardProxy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GirardProxy
-Version: 0.9.41
+Version: 0.9.45
 Summary: Python module that scrape and retrive working proxy addresses
 Author: Girard
 Author-email: girardhappy.it@gmail.com
 License: MIT
 Keywords: proxy scraper
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
```

### Comparing `girardproxy-0.9.41/LICENSE` & `girardproxy-0.9.45/LICENSE`

 * *Files identical despite different names*

### Comparing `girardproxy-0.9.41/PKG-INFO` & `girardproxy-0.9.45/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GirardProxy
-Version: 0.9.41
+Version: 0.9.45
 Summary: Python module that scrape and retrive working proxy addresses
 Author: Girard
 Author-email: girardhappy.it@gmail.com
 License: MIT
 Keywords: proxy scraper
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
```

### Comparing `girardproxy-0.9.41/setup.py` & `girardproxy-0.9.45/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "GirardProxy",
-    version = "0.9.41",
+    version = "0.9.45",
     author = "Girard",
     author_email = "girardhappy.it@gmail.com",
     description = ("Python module that scrape and retrive working proxy addresses"),
     license = "MIT",
     keywords = "proxy scraper",
-    packages=['src'],
+    package_dir={'GirardProxy': 'src'},
     long_description="""A module that offer you the possibility to create an object that continuosly request proxies addresses, verify if they work using multithreading and retrive to you one of them <3""",
     install_requires=[
           'requests[socks]'
       ],
     classifiers=[
         'Development Status :: 4 - Beta',
         "Topic :: Utilities",
```

### Comparing `girardproxy-0.9.41/src/main.py` & `girardproxy-0.9.45/src/proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests,threading,time
 
-class ProxyScraper():
+class Proxy():
     __country_list = ['all','AF', 'AX', 'AL', 'DZ', 'AS', 'AD', 'AO', 'AI', 'AQ', 'AG', 'AR', 'AM', 'AW', 'AU', 'AT', 'AZ', 'BS', 'BH', 'BD', 'BB', 'BY', 'BE', 'BZ', 'BJ', 'BM', 'BT', 'BO', 'BA', 'BW', 'BV', 'BR', 'IO', 'BN', 'BG', 'BF', 'BI', 'KH', 'CM', 'CA', 'CV', 'KY', 'CF', 'TD', 'CL', 'CN', 'CX', 'CC', 'CO', 'KM', 'CG', 'CD', 'CK', 'CR', 'CI', 'HR', 'CU', 'CY', 'CZ', 'DK', 'DJ', 'DM', 'DO', 'EC', 'EG', 'SV', 'GQ', 'ER', 'EE', 'ET', 'FK', 'FO', 'FJ', 'FI', 'FR', 'GF', 'PF', 'TF', 'GA', 'GM', 'GE', 'DE', 'GH', 'GI', 'GR', 'GL', 'GD', 'GP', 'GU', 'GT', 'GG', 'GN', 'GW', 'GY', 'HT', 'HM', 'VA', 'HN', 'HK', 'HU', 'IS', 'IN', 'ID', 'IR', 'IQ', 'IE', 'IM', 'IL', 'IT', 'JM', 'JP', 'JE', 'JO', 'KZ', 'KE', 'KI', 'KR', 'KP', 'KW', 'KG', 'LA', 'LV', 'LB', 'LS', 'LR', 'LY', 'LI', 'LT', 'LU', 'MO', 'MK', 'MG', 'MW', 'MY', 'MV', 'ML', 'MT', 'MH', 'MQ', 'MR', 'MU', 'YT', 'MX', 'FM', 'MD', 'MC', 'MN', 'ME', 'MS', 'MA', 'MZ', 'MM', 'NA', 'NR', 'NP', 'NL', 'AN', 'NC', 'NZ', 'NI', 'NE', 'NG', 'NU', 'NF', 'MP', 'NO', 'OM', 'PK', 'PW', 'PS', 'PA', 'PG', 'PY', 'PE', 'PH', 'PN', 'PL', 'PT', 'PR', 'QA', 'RE', 'RO', 'RU', 'RW', 'BL', 'SH', 'KN', 'LC', 'MF', 'PM', 'VC', 'WS', 'SM', 'ST', 'SA', 'SN', 'RS', 'SC', 'SL', 'SG', 'SK', 'SI', 'SB', 'SO', 'ZA', 'GS', 'ES', 'LK', 'SD', 'SR', 'SJ', 'SZ', 'SE', 'CH', 'SY', 'TW', 'TJ', 'TZ', 'TH', 'TL', 'TG', 'TK', 'TO', 'TT', 'TN', 'TR', 'TM', 'TC', 'TV', 'UG', 'UA', 'AE', 'GB', 'US', 'UM', 'UY', 'UZ', 'VU', 'VE', 'VN', 'VG', 'VI', 'WF', 'EH', 'YE', 'ZM', 'ZW']
     
     def __init__(self,scraper_timeout=60,protocol="socks5",timeout=1000,country=['all'],ssl='all',anonimity="elite",start=True):
-        """Create setup and run the ProxyScraper\n
+        """Create setup and run the Proxy Scraper\n
         ``scraper_timeout`` int
         ``protocol`` ['all','http','socks4','socks5']\n
         ``timeout`` int\n
         ``country`` array containing iso alpha 2 countries or 'all'\n
         ``ssl`` ['all','yes','no']\n
         ``anonimity`` ['elite','anonymous','transparent','all']\n
         ``start`` bool
@@ -52,54 +52,54 @@
         """set the proxy request option\n
         ``protocol`` ['all','http','socks4','socks5']\n
         ``timeout`` int\n
         ``country`` array containing iso alpha 2 countries or 'all'\n
         ``ssl`` ['all','yes','no']\n
         ``anonimity`` ['elite','anonymous','transparent','all']\n
         """    
-        ProxyScraper.__checkParams(protocol,timeout,country,ssl,anonimity)
+        Proxy.__checkParams(protocol,timeout,country,ssl,anonimity)
         self.__options = {}
         self.__options['url'] = f"https://api.proxyscrape.com/v3/free-proxy-list/get?request=displayproxies&protocol={protocol}&format=json&anonymity={anonimity}&timeout={timeout}&ssl={ssl}&country={','.join(country)}"
         self.__options['protocol'] = protocol
         self.__options['timeout'] = timeout
         self.__options['country'] = country
         self.__options['ssl'] = ssl
         self.__options['anonimity'] = anonimity
 
     def __checkParams(protocol,timeout,country,ssl,anonimity):
         if not protocol in ['all','http','socks4','socks5']:
-            raise ProxyScraper.ProxyError("protocol must be ['all','http','socks4','socks5']")
+            raise Proxy.ProxyError("protocol must be ['all','http','socks4','socks5']")
 
         if not type(timeout) is int:
-            raise ProxyScraper.ProxyError("timout must be an int")
+            raise Proxy.ProxyError("timout must be an int")
 
         if not type(country) is list:
-            raise ProxyScraper.ProxyError("country must be an array of iso alpha 2 countries or ['all']")
+            raise Proxy.ProxyError("country must be an array of iso alpha 2 countries or ['all']")
 
         for c in country:
-            if not c in ProxyScraper.__country_list:
-                raise ProxyScraper.ProxyError("country must be an iso alpha 2 countries or 'all'")
+            if not c in Proxy.__country_list:
+                raise Proxy.ProxyError("country must be an iso alpha 2 countries or 'all'")
 
         if not ssl in ['all','yes','no']:
-            raise ProxyScraper.ProxyError("ssl must be ['all','yes','no']")
+            raise Proxy.ProxyError("ssl must be ['all','yes','no']")
 
         if not anonimity in ['elite','anonymous','transparent','all']:
-            raise ProxyScraper.ProxyError("anonimity must be ['elite','anonymous','transparent','all']")
+            raise Proxy.ProxyError("anonimity must be ['elite','anonymous','transparent','all']")
     
     def __proxywork(host,port,ip_data):
         try:
             requests.get('https://api.ipify.org', proxies=dict(http=f'socks5://{host}:{port}',https=f'socks5://{host}:{port}'),timeout=0.5)
             return host,port,ip_data,False
         except:
             return None,None,None,True
 
     def __requestProxy(self):
         r = requests.get(self.__options.get('url')).json()
         for prox in r.get('proxies'):
-            t = ProxyScraper.__ReturnValueThread(target=ProxyScraper.__proxywork,args=(prox.get('ip'),prox.get('port'),prox.get('ip_data')))
+            t = Proxy.__ReturnValueThread(target=Proxy.__proxywork,args=(prox.get('ip'),prox.get('port'),prox.get('ip_data')))
             t.start()
             self.__threads.append(t)
         while len(self.__threads)>0:
             for t in self.__threads:
                 if not t.is_alive():
                     host,port,ip_data,error = t.join()
                     if not error:
@@ -127,17 +127,12 @@
 
         def run(self):
             if self._target is None:
                 return
             try:
                 self.result = self._target(*self._args, **self._kwargs)
             except Exception as exc:
-                ProxyScraper.ProxyError(f'ReturnValueThread Error => {type(exc).__name__}: {exc}')
+                Proxy.ProxyError(f'ReturnValueThread Error => {type(exc).__name__}: {exc}')
 
         def join(self, *args, **kwargs):
             super().join(*args, **kwargs)
             return self.result
-
-start = time.time()
-proxy = ProxyScraper()
-print(proxy)
-proxy.stop()
```

