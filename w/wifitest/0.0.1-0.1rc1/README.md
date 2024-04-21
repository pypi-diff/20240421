# Comparing `tmp/wifitest-0.0.1.tar.gz` & `tmp/wifitest-0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wifitest-0.0.1.tar", last modified: Sun Apr 21 18:09:49 2024, max compression
+gzip compressed data, was "wifitest-0.1rc1.tar", last modified: Sun Apr 21 02:08:13 2024, max compression
```

## Comparing `wifitest-0.0.1.tar` & `wifitest-0.1rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-21 18:09:49.211013 wifitest-0.0.1/
--rw-rw-r--   0 juan      (1000) juan      (1000)    18092 2024-04-21 18:04:01.000000 wifitest-0.0.1/LICENSE
--rw-r--r--   0 juan      (1000) juan      (1000)     2076 2024-04-21 18:09:49.211013 wifitest-0.0.1/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)      752 2024-04-21 18:04:01.000000 wifitest-0.0.1/README.md
--rw-rw-r--   0 juan      (1000) juan      (1000)     1462 2024-04-21 18:08:43.000000 wifitest-0.0.1/pyproject.toml
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-21 18:09:49.211013 wifitest-0.0.1/setup.cfg
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-21 18:09:49.207013 wifitest-0.0.1/wifitest/
--rw-rw-r--   0 juan      (1000) juan      (1000)      203 2024-04-21 18:04:01.000000 wifitest-0.0.1/wifitest/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2009 2024-04-21 18:04:01.000000 wifitest-0.0.1/wifitest/__main__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1742 2024-04-21 18:04:01.000000 wifitest-0.0.1/wifitest/bruteforce.py
--rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-04-21 18:04:01.000000 wifitest-0.0.1/wifitest/cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      871 2024-04-21 18:04:01.000000 wifitest-0.0.1/wifitest/events.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1772 2024-04-21 18:04:01.000000 wifitest-0.0.1/wifitest/scan.py
--rw-rw-r--   0 juan      (1000) juan      (1000)       72 2024-04-21 18:07:05.000000 wifitest-0.0.1/wifitest/version.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-21 18:09:49.211013 wifitest-0.0.1/wifitest.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     2076 2024-04-21 18:09:49.000000 wifitest-0.0.1/wifitest.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)      363 2024-04-21 18:09:49.000000 wifitest-0.0.1/wifitest.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-21 18:09:49.000000 wifitest-0.0.1/wifitest.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       51 2024-04-21 18:09:49.000000 wifitest-0.0.1/wifitest.egg-info/entry_points.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        7 2024-04-21 18:09:49.000000 wifitest-0.0.1/wifitest.egg-info/requires.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        9 2024-04-21 18:09:49.000000 wifitest-0.0.1/wifitest.egg-info/top_level.txt
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-21 02:08:13.909643 wifitest-0.1rc1/
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18092 2024-04-21 00:01:50.000000 wifitest-0.1rc1/LICENSE
+-rw-r--r--   0 juan      (1000) juan      (1000)     1570 2024-04-21 02:08:13.909643 wifitest-0.1rc1/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)      245 2024-04-21 02:06:52.000000 wifitest-0.1rc1/README.md
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1464 2024-04-21 02:06:21.000000 wifitest-0.1rc1/pyproject.toml
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-21 02:08:13.909643 wifitest-0.1rc1/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-21 02:08:13.905643 wifitest-0.1rc1/wifitest/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      203 2024-04-21 02:03:00.000000 wifitest-0.1rc1/wifitest/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1394 2024-04-21 02:02:59.000000 wifitest-0.1rc1/wifitest/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1742 2024-04-21 02:02:58.000000 wifitest-0.1rc1/wifitest/bruteforce.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-04-21 02:02:57.000000 wifitest-0.1rc1/wifitest/cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      871 2024-04-21 02:02:56.000000 wifitest-0.1rc1/wifitest/events.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1125 2024-04-21 02:02:55.000000 wifitest-0.1rc1/wifitest/scan.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       74 2024-04-21 02:02:54.000000 wifitest-0.1rc1/wifitest/version.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-21 02:08:13.909643 wifitest-0.1rc1/wifitest.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     1570 2024-04-21 02:08:13.000000 wifitest-0.1rc1/wifitest.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)      363 2024-04-21 02:08:13.000000 wifitest-0.1rc1/wifitest.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-21 02:08:13.000000 wifitest-0.1rc1/wifitest.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       51 2024-04-21 02:08:13.000000 wifitest-0.1rc1/wifitest.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        7 2024-04-21 02:08:13.000000 wifitest-0.1rc1/wifitest.egg-info/requires.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        9 2024-04-21 02:08:13.000000 wifitest-0.1rc1/wifitest.egg-info/top_level.txt
```

### Comparing `wifitest-0.0.1/LICENSE` & `wifitest-0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `wifitest-0.0.1/PKG-INFO` & `wifitest-0.1rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,99 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7769 6669  : 2.1.Name: wifi
 00000020: 7465 7374 0a56 6572 7369 6f6e 3a20 302e  test.Version: 0.
-00000030: 302e 310a 5375 6d6d 6172 793a 2050 7974  0.1.Summary: Pyt
-00000040: 686f 6e20 3320 6c69 6272 6172 7920 666f  hon 3 library fo
-00000050: 7220 7769 6669 2074 6573 7469 6e67 2e0a  r wifi testing..
-00000060: 4175 7468 6f72 2d65 6d61 696c 3a20 4a75  Author-email: Ju
-00000070: 616e 2042 696e 6465 7a20 3c6a 7561 6e62  an Bindez <juanb
-00000080: 696e 6465 7a37 3830 4067 6d61 696c 2e63  indez780@gmail.c
-00000090: 6f6d 3e0a 4c69 6365 6e73 653a 2047 504c  om>.License: GPL
-000000a0: 7632 206c 6963 656e 7365 0a50 726f 6a65  v2 license.Proje
-000000b0: 6374 2d55 524c 3a20 486f 6d65 7061 6765  ct-URL: Homepage
-000000c0: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-000000d0: 2e63 6f6d 2f6a 7561 6e62 696e 6465 7a2f  .com/juanbindez/
-000000e0: 7769 6669 7465 7374 0a50 726f 6a65 6374  wifitest.Project
-000000f0: 2d55 524c 3a20 4275 6720 5265 706f 7274  -URL: Bug Report
-00000100: 732c 2068 7474 7073 3a2f 2f67 6974 6875  s, https://githu
-00000110: 622e 636f 6d2f 6a75 616e 6269 6e64 657a  b.com/juanbindez
-00000120: 2f77 6966 6974 6573 742f 6973 7375 6573  /wifitest/issues
-00000130: 0a50 726f 6a65 6374 2d55 524c 3a20 5265  .Project-URL: Re
-00000140: 6164 2074 6865 2044 6f63 732c 2068 7474  ad the Docs, htt
-00000150: 703a 2f2f 7769 6669 7465 7374 2e72 6561  p://wifitest.rea
-00000160: 6474 6865 646f 6373 2e69 6f2f 0a4b 6579  dthedocs.io/.Key
-00000170: 776f 7264 733a 2062 7275 7465 666f 7263  words: bruteforc
-00000180: 652c 7769 6669 2c74 6f6f 6c73 2c63 6c69  e,wifi,tools,cli
-00000190: 2c73 6361 6e0a 436c 6173 7369 6669 6572  ,scan.Classifier
-000001a0: 3a20 4465 7665 6c6f 706d 656e 7420 5374  : Development St
-000001b0: 6174 7573 203a 3a20 3520 2d20 5072 6f64  atus :: 5 - Prod
-000001c0: 7563 7469 6f6e 2f53 7461 626c 650a 436c  uction/Stable.Cl
-000001d0: 6173 7369 6669 6572 3a20 456e 7669 726f  assifier: Enviro
-000001e0: 6e6d 656e 7420 3a3a 2043 6f6e 736f 6c65  nment :: Console
-000001f0: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
-00000200: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000210: 3a20 4465 7665 6c6f 7065 7273 0a43 6c61  : Developers.Cla
-00000220: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-00000230: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000240: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
-00000250: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
-00000260: 3220 2847 504c 7632 290a 436c 6173 7369  2 (GPLv2).Classi
-00000270: 6669 6572 3a20 4e61 7475 7261 6c20 4c61  fier: Natural La
-00000280: 6e67 7561 6765 203a 3a20 456e 676c 6973  nguage :: Englis
-00000290: 680a 436c 6173 7369 6669 6572 3a20 4f70  h.Classifier: Op
-000002a0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000002b0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-000002c0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000002d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002f0: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
-00000300: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000310: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000320: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
-00000330: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000340: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000350: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
-00000360: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000370: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000380: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
-00000390: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000003a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000003b0: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
-000003c0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000003d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000003e0: 2050 7974 686f 6e20 3a3a 2033 2e31 320a   Python :: 3.12.
-000003f0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000400: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000410: 203a 3a20 5079 7468 6f6e 0a43 6c61 7373   :: Python.Class
-00000420: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
-00000430: 496e 7465 726e 6574 0a43 6c61 7373 6966  Internet.Classif
-00000440: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
-00000450: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
-00000460: 6e74 203a 3a20 4c69 6272 6172 6965 7320  nt :: Libraries 
-00000470: 3a3a 2050 7974 686f 6e20 4d6f 6475 6c65  :: Python Module
-00000480: 730a 436c 6173 7369 6669 6572 3a20 546f  s.Classifier: To
-00000490: 7069 6320 3a3a 2054 6572 6d69 6e61 6c73  pic :: Terminals
-000004a0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
-000004b0: 6963 203a 3a20 5574 696c 6974 6965 730a  ic :: Utilities.
-000004c0: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
-000004d0: 203e 3d33 2e37 0a44 6573 6372 6970 7469   >=3.7.Descripti
-000004e0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-000004f0: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
-00000500: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
-00000510: 454e 5345 0a52 6571 7569 7265 732d 4469  ENSE.Requires-Di
-00000520: 7374 3a20 7079 7769 6669 0a0a 2320 7769  st: pywifi..# wi
-00000530: 6669 7465 7374 0a0a 215b 5079 5049 202d  fitest..![PyPI -
-00000540: 2044 6f77 6e6c 6f61 6473 5d28 6874 7470   Downloads](http
-00000550: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000560: 696f 2f70 7970 692f 646d 2f77 6966 6974  io/pypi/dm/wifit
-00000570: 6573 7429 0a21 5b50 7950 4920 2d20 4c69  est).![PyPI - Li
-00000580: 6365 6e73 655d 2868 7474 7073 3a2f 2f69  cense](https://i
-00000590: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000005a0: 7069 2f6c 2f77 6966 6974 6573 7429 0a21  pi/l/wifitest).!
-000005b0: 5b52 6561 6420 7468 6520 446f 6373 5d28  [Read the Docs](
-000005c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000005d0: 6c64 732e 696f 2f72 6561 6474 6865 646f  lds.io/readthedo
-000005e0: 6373 2f77 6966 6974 6573 7429 0a21 5b47  cs/wifitest).![G
-000005f0: 6974 4875 6220 5461 675d 2868 7474 7073  itHub Tag](https
-00000600: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000610: 6f2f 6769 7468 7562 2f76 2f74 6167 2f4a  o/github/v/tag/J
-00000620: 7561 6e42 696e 6465 7a2f 7769 6669 7465  uanBindez/wifite
-00000630: 7374 3f69 6e63 6c75 6465 5f70 7265 7265  st?include_prere
-00000640: 6c65 6173 6573 290a 3c61 2068 7265 663d  leases).<a href=
-00000650: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
-00000660: 672f 7072 6f6a 6563 742f 7769 6669 7465  g/project/wifite
-00000670: 7374 2f22 3e3c 696d 6720 7372 633d 2268  st/"><img src="h
-00000680: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000690: 6473 2e69 6f2f 7079 7069 2f76 2f77 6966  ds.io/pypi/v/wif
-000006a0: 6974 6573 7422 202f 3e3c 2f61 3e0a 0a23  itest" /></a>..#
-000006b0: 2320 5079 7468 6f6e 2033 206c 6962 7261  # Python 3 libra
-000006c0: 7279 2066 6f72 2077 6966 6920 7465 7374  ry for wifi test
-000006d0: 696e 672e 0a0a 2323 2320 496e 7374 616c  ing...### Instal
-000006e0: 6c0a 0a20 2020 2073 7564 6f20 7069 7020  l..    sudo pip 
-000006f0: 696e 7374 616c 6c20 7769 6669 7465 7374  install wifitest
-00000700: 0a0a 0a23 2323 2075 7361 6765 3a0a 0a23  ...### usage:..#
-00000710: 2323 2320 696d 706f 7274 0a0a 6060 6070  ### import..```p
-00000720: 7974 686f 6e0a 6672 6f6d 2077 6966 6974  ython.from wifit
-00000730: 6573 7420 696d 706f 7274 2057 6966 6954  est import WifiT
-00000740: 6573 740a 6060 600a 2323 2323 2073 6361  est.```.#### sca
-00000750: 6e20 6176 6169 6c61 626c 6520 7769 6669  n available wifi
-00000760: 206e 6574 776f 726b 730a 0a60 6060 7079   networks..```py
-00000770: 7468 6f6e 0a73 203d 2057 6966 6954 6573  thon.s = WifiTes
-00000780: 7428 290a 732e 7363 616e 2829 0a60 6060  t().s.scan().```
-00000790: 0a23 2323 2320 6272 7574 6566 6f72 6365  .#### bruteforce
-000007a0: 206f 6e20 7769 6669 206e 6574 776f 726b   on wifi network
-000007b0: 0a0a 6060 6070 7974 686f 6e0a 5353 4944  ..```python.SSID
-000007c0: 203d 2022 7769 6669 220a 574f 5244 4c49   = "wifi".WORDLI
-000007d0: 5354 203d 2022 776f 7264 6c69 7374 2e74  ST = "wordlist.t
-000007e0: 7874 220a 0a77 6966 6920 3d20 5769 6669  xt"..wifi = Wifi
-000007f0: 5465 7374 2829 0a77 6966 692e 6272 7574  Test().wifi.brut
-00000800: 6566 6f72 6365 2853 5349 442c 2057 4f52  eforce(SSID, WOR
-00000810: 444c 4953 5429 0a0a 6060 600a            DLIST)..```.
+00000030: 3172 6331 0a53 756d 6d61 7279 3a20 5079  1rc1.Summary: Py
+00000040: 7468 6f6e 2033 206c 6962 7261 7279 2066  thon 3 library f
+00000050: 6f72 2077 6966 6920 7465 7374 696e 672e  or wifi testing.
+00000060: 0a41 7574 686f 722d 656d 6169 6c3a 204a  .Author-email: J
+00000070: 7561 6e20 4269 6e64 657a 203c 6a75 616e  uan Bindez <juan
+00000080: 6269 6e64 657a 3738 3040 676d 6169 6c2e  bindez780@gmail.
+00000090: 636f 6d3e 0a4c 6963 656e 7365 3a20 4750  com>.License: GP
+000000a0: 4c76 3220 6c69 6365 6e73 650a 5072 6f6a  Lv2 license.Proj
+000000b0: 6563 742d 5552 4c3a 2048 6f6d 6570 6167  ect-URL: Homepag
+000000c0: 652c 2068 7474 7073 3a2f 2f67 6974 6875  e, https://githu
+000000d0: 622e 636f 6d2f 6a75 616e 6269 6e64 657a  b.com/juanbindez
+000000e0: 2f77 6966 6974 6573 740a 5072 6f6a 6563  /wifitest.Projec
+000000f0: 742d 5552 4c3a 2042 7567 2052 6570 6f72  t-URL: Bug Repor
+00000100: 7473 2c20 6874 7470 733a 2f2f 6769 7468  ts, https://gith
+00000110: 7562 2e63 6f6d 2f6a 7561 6e62 696e 6465  ub.com/juanbinde
+00000120: 7a2f 7769 6669 7465 7374 2f69 7373 7565  z/wifitest/issue
+00000130: 730a 5072 6f6a 6563 742d 5552 4c3a 2052  s.Project-URL: R
+00000140: 6561 6420 7468 6520 446f 6373 2c20 6874  ead the Docs, ht
+00000150: 7470 3a2f 2f77 6966 6974 6573 742e 7265  tp://wifitest.re
+00000160: 6164 7468 6564 6f63 732e 696f 2f0a 4b65  adthedocs.io/.Ke
+00000170: 7977 6f72 6473 3a20 6272 7574 6566 6f72  ywords: brutefor
+00000180: 6365 2c77 6966 692c 746f 6f6c 732c 636c  ce,wifi,tools,cl
+00000190: 692c 7363 616e 0a43 6c61 7373 6966 6965  i,scan.Classifie
+000001a0: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+000001b0: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
+000001c0: 6475 6374 696f 6e2f 5374 6162 6c65 0a43  duction/Stable.C
+000001d0: 6c61 7373 6966 6965 723a 2045 6e76 6972  lassifier: Envir
+000001e0: 6f6e 6d65 6e74 203a 3a20 436f 6e73 6f6c  onment :: Consol
+000001f0: 650a 436c 6173 7369 6669 6572 3a20 496e  e.Classifier: In
+00000200: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000210: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
+00000220: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+00000230: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000240: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
+00000250: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+00000260: 7632 2028 4750 4c76 3229 0a43 6c61 7373  v2 (GPLv2).Class
+00000270: 6966 6965 723a 204e 6174 7572 616c 204c  ifier: Natural L
+00000280: 616e 6775 6167 6520 3a3a 2045 6e67 6c69  anguage :: Engli
+00000290: 7368 0a43 6c61 7373 6966 6965 723a 204f  sh.Classifier: O
+000002a0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000002b0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000002c0: 740a 436c 6173 7369 6669 6572 3a20 5072  t.Classifier: Pr
+000002d0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000002e0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000002f0: 332e 370a 436c 6173 7369 6669 6572 3a20  3.7.Classifier: 
+00000300: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000310: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000320: 3a20 332e 380a 436c 6173 7369 6669 6572  : 3.8.Classifier
+00000330: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000340: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000350: 203a 3a20 332e 390a 436c 6173 7369 6669   :: 3.9.Classifi
+00000360: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000370: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000380: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
+00000390: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000003a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000003b0: 7974 686f 6e20 3a3a 2033 2e31 310a 436c  ython :: 3.11.Cl
+000003c0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000003d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000003e0: 3a20 5079 7468 6f6e 203a 3a20 332e 3132  : Python :: 3.12
+000003f0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000400: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000410: 6520 3a3a 2050 7974 686f 6e0a 436c 6173  e :: Python.Clas
+00000420: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00000430: 2049 6e74 6572 6e65 740a 436c 6173 7369   Internet.Classi
+00000440: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+00000450: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+00000460: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
+00000470: 203a 3a20 5079 7468 6f6e 204d 6f64 756c   :: Python Modul
+00000480: 6573 0a43 6c61 7373 6966 6965 723a 2054  es.Classifier: T
+00000490: 6f70 6963 203a 3a20 5465 726d 696e 616c  opic :: Terminal
+000004a0: 730a 436c 6173 7369 6669 6572 3a20 546f  s.Classifier: To
+000004b0: 7069 6320 3a3a 2055 7469 6c69 7469 6573  pic :: Utilities
+000004c0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
+000004d0: 3a20 3e3d 332e 370a 4465 7363 7269 7074  : >=3.7.Descript
+000004e0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
+000004f0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
+00000500: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+00000510: 4345 4e53 450a 5265 7175 6972 6573 2d44  CENSE.Requires-D
+00000520: 6973 743a 2070 7977 6966 690a 0a23 2077  ist: pywifi..# w
+00000530: 6966 6974 6573 740a 0a23 2320 5079 7468  ifitest..## Pyth
+00000540: 6f6e 2033 206c 6962 7261 7279 2066 6f72  on 3 library for
+00000550: 2077 6966 6920 7465 7374 696e 672e 0a0a   wifi testing...
+00000560: 2323 2320 496e 7374 616c 6c0a 0a20 2020  ### Install..   
+00000570: 2073 7564 6f20 7069 7020 696e 7374 616c   sudo pip instal
+00000580: 6c20 7769 6669 7465 7374 0a0a 0a23 2323  l wifitest...###
+00000590: 2075 7361 6765 0a0a 6060 6070 7974 686f   usage..```pytho
+000005a0: 6e0a 0a66 726f 6d20 7769 6669 7465 7374  n..from wifitest
+000005b0: 2069 6d70 6f72 7420 5769 6669 5465 7374   import WifiTest
+000005c0: 0a0a 5353 4944 203d 2022 7769 6669 220a  ..SSID = "wifi".
+000005d0: 574f 5244 4c49 5354 203d 2022 776f 7264  WORDLIST = "word
+000005e0: 6c69 7374 2e74 7874 220a 0a77 6966 6920  list.txt"..wifi 
+000005f0: 3d20 5769 6669 5465 7374 2829 0a77 6966  = WifiTest().wif
+00000600: 692e 6272 7574 6566 6f72 6365 2853 5349  i.bruteforce(SSI
+00000610: 442c 2057 4f52 444c 4953 5429 0a0a 6060  D, WORDLIST)..``
+00000620: 600a                                     `.
```

### Comparing `wifitest-0.0.1/pyproject.toml` & `wifitest-0.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wifitest"
-version = "0.0.1"
+version = "0.1-rc1"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for wifi testing."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

### Comparing `wifitest-0.0.1/wifitest/__main__.py` & `wifitest-0.1rc1/wifitest/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,39 +19,21 @@
 
 from wifitest.bruteforce import BruteForce
 from wifitest.events import WifiEvents
 from wifitest.scan import WifiScan
 
 
 class WifiTest:
-    """
-    Class to perform tests related to Wi-Fi networks, such as scanning, brute-forcing, and event monitoring.
-    """
-    
     def scan(self):
-        """
-        Performs a scan of available Wi-Fi networks and prints their details.
-        """
         wifi_scan = WifiScan()
         print("Scanning for Wi-Fi networks...")
         print("Wi-Fi networks found:")
-        
         networks = wifi_scan.scan_wifi_networks()
         wifi_scan.print_wifi_details(networks)
 
     def bruteforce(self, ssid: str, wordlist: str):
-        """
-        Performs a brute-force attack on a specified Wi-Fi network using a wordlist.
-
-        Args:
-            ssid (str): The SSID of the target Wi-Fi network.
-            wordlist (str): The path to the wordlist file.
-        """
         bf = BruteForce()
         bf.brute_force_attack(ssid, wordlist)
 
     def events(self):
-        """
-        Initiates monitoring of events related to Wi-Fi networks, such as connection and disconnection.
-        """
         events = WifiEvents()
-        events.monitor_wifi_events()
+        events.monitor_wifi_events()
```

### Comparing `wifitest-0.0.1/wifitest/bruteforce.py` & `wifitest-0.1rc1/wifitest/bruteforce.py`

 * *Files identical despite different names*

### Comparing `wifitest-0.0.1/wifitest/events.py` & `wifitest-0.1rc1/wifitest/events.py`

 * *Files identical despite different names*

### Comparing `wifitest-0.0.1/wifitest/scan.py` & `wifitest-0.1rc1/wifitest/scan.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,32 @@
 import pywifi
 from pywifi import const
 
 
 class WifiScan():
-    """
-    Class to perform Wi-Fi network scanning and print details of the scanned networks.
-    """    
-    
     def scan_wifi_networks(self):
-        """
-        Scan for Wi-Fi networks and return the scan results.
-
-        Returns:
-            list: A list of network scan results.
-        """
         wifi = pywifi.PyWiFi()
         iface = wifi.interfaces()[0]  # obtém a primeira interface Wi-Fi disponível
         iface.scan()
         return iface.scan_results()
 
     def print_wifi_details(self, networks):
-        """
-        Print details of the scanned Wi-Fi networks.
-
-        Args:
-            networks (list): A list of network scan results.
-        """
         for network in networks:
             print("SSID:", network.ssid)
             print("BSSID:", network.bssid)
             print("Signal Strength (dBm):", network.signal)
             print("Security:", self.translate_encryption_type(network.akm))
             print("----------------------------------")
 
     def translate_encryption_type(self, encryption_type):
-        """
-        Translate encryption type code to human-readable format.
-
-        Args:
-            encryption_type (int): Encryption type code.
-
-        Returns:
-            str: Human-readable encryption type.
-        """
         if encryption_type == const.AKM_TYPE_NONE:
             return "Open"
         elif encryption_type == const.AKM_TYPE_WPA:
             return "WPA"
         elif encryption_type == const.AKM_TYPE_WPAPSK:
             return "WPA-PSK"
         elif encryption_type == const.AKM_TYPE_WPA2:
             return "WPA2"
         elif encryption_type == const.AKM_TYPE_WPA2PSK:
             return "WPA2-PSK"
         else:
-            return "Unknown"
+            return "Unknown"
```

### Comparing `wifitest-0.0.1/wifitest.egg-info/PKG-INFO` & `wifitest-0.1rc1/wifitest.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,99 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7769 6669  : 2.1.Name: wifi
 00000020: 7465 7374 0a56 6572 7369 6f6e 3a20 302e  test.Version: 0.
-00000030: 302e 310a 5375 6d6d 6172 793a 2050 7974  0.1.Summary: Pyt
-00000040: 686f 6e20 3320 6c69 6272 6172 7920 666f  hon 3 library fo
-00000050: 7220 7769 6669 2074 6573 7469 6e67 2e0a  r wifi testing..
-00000060: 4175 7468 6f72 2d65 6d61 696c 3a20 4a75  Author-email: Ju
-00000070: 616e 2042 696e 6465 7a20 3c6a 7561 6e62  an Bindez <juanb
-00000080: 696e 6465 7a37 3830 4067 6d61 696c 2e63  indez780@gmail.c
-00000090: 6f6d 3e0a 4c69 6365 6e73 653a 2047 504c  om>.License: GPL
-000000a0: 7632 206c 6963 656e 7365 0a50 726f 6a65  v2 license.Proje
-000000b0: 6374 2d55 524c 3a20 486f 6d65 7061 6765  ct-URL: Homepage
-000000c0: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-000000d0: 2e63 6f6d 2f6a 7561 6e62 696e 6465 7a2f  .com/juanbindez/
-000000e0: 7769 6669 7465 7374 0a50 726f 6a65 6374  wifitest.Project
-000000f0: 2d55 524c 3a20 4275 6720 5265 706f 7274  -URL: Bug Report
-00000100: 732c 2068 7474 7073 3a2f 2f67 6974 6875  s, https://githu
-00000110: 622e 636f 6d2f 6a75 616e 6269 6e64 657a  b.com/juanbindez
-00000120: 2f77 6966 6974 6573 742f 6973 7375 6573  /wifitest/issues
-00000130: 0a50 726f 6a65 6374 2d55 524c 3a20 5265  .Project-URL: Re
-00000140: 6164 2074 6865 2044 6f63 732c 2068 7474  ad the Docs, htt
-00000150: 703a 2f2f 7769 6669 7465 7374 2e72 6561  p://wifitest.rea
-00000160: 6474 6865 646f 6373 2e69 6f2f 0a4b 6579  dthedocs.io/.Key
-00000170: 776f 7264 733a 2062 7275 7465 666f 7263  words: bruteforc
-00000180: 652c 7769 6669 2c74 6f6f 6c73 2c63 6c69  e,wifi,tools,cli
-00000190: 2c73 6361 6e0a 436c 6173 7369 6669 6572  ,scan.Classifier
-000001a0: 3a20 4465 7665 6c6f 706d 656e 7420 5374  : Development St
-000001b0: 6174 7573 203a 3a20 3520 2d20 5072 6f64  atus :: 5 - Prod
-000001c0: 7563 7469 6f6e 2f53 7461 626c 650a 436c  uction/Stable.Cl
-000001d0: 6173 7369 6669 6572 3a20 456e 7669 726f  assifier: Enviro
-000001e0: 6e6d 656e 7420 3a3a 2043 6f6e 736f 6c65  nment :: Console
-000001f0: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
-00000200: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000210: 3a20 4465 7665 6c6f 7065 7273 0a43 6c61  : Developers.Cla
-00000220: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-00000230: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000240: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
-00000250: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
-00000260: 3220 2847 504c 7632 290a 436c 6173 7369  2 (GPLv2).Classi
-00000270: 6669 6572 3a20 4e61 7475 7261 6c20 4c61  fier: Natural La
-00000280: 6e67 7561 6765 203a 3a20 456e 676c 6973  nguage :: Englis
-00000290: 680a 436c 6173 7369 6669 6572 3a20 4f70  h.Classifier: Op
-000002a0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000002b0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-000002c0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000002d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002f0: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
-00000300: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000310: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000320: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
-00000330: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000340: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000350: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
-00000360: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000370: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000380: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
-00000390: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000003a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000003b0: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
-000003c0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000003d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000003e0: 2050 7974 686f 6e20 3a3a 2033 2e31 320a   Python :: 3.12.
-000003f0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000400: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000410: 203a 3a20 5079 7468 6f6e 0a43 6c61 7373   :: Python.Class
-00000420: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
-00000430: 496e 7465 726e 6574 0a43 6c61 7373 6966  Internet.Classif
-00000440: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
-00000450: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
-00000460: 6e74 203a 3a20 4c69 6272 6172 6965 7320  nt :: Libraries 
-00000470: 3a3a 2050 7974 686f 6e20 4d6f 6475 6c65  :: Python Module
-00000480: 730a 436c 6173 7369 6669 6572 3a20 546f  s.Classifier: To
-00000490: 7069 6320 3a3a 2054 6572 6d69 6e61 6c73  pic :: Terminals
-000004a0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
-000004b0: 6963 203a 3a20 5574 696c 6974 6965 730a  ic :: Utilities.
-000004c0: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
-000004d0: 203e 3d33 2e37 0a44 6573 6372 6970 7469   >=3.7.Descripti
-000004e0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-000004f0: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
-00000500: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
-00000510: 454e 5345 0a52 6571 7569 7265 732d 4469  ENSE.Requires-Di
-00000520: 7374 3a20 7079 7769 6669 0a0a 2320 7769  st: pywifi..# wi
-00000530: 6669 7465 7374 0a0a 215b 5079 5049 202d  fitest..![PyPI -
-00000540: 2044 6f77 6e6c 6f61 6473 5d28 6874 7470   Downloads](http
-00000550: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000560: 696f 2f70 7970 692f 646d 2f77 6966 6974  io/pypi/dm/wifit
-00000570: 6573 7429 0a21 5b50 7950 4920 2d20 4c69  est).![PyPI - Li
-00000580: 6365 6e73 655d 2868 7474 7073 3a2f 2f69  cense](https://i
-00000590: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000005a0: 7069 2f6c 2f77 6966 6974 6573 7429 0a21  pi/l/wifitest).!
-000005b0: 5b52 6561 6420 7468 6520 446f 6373 5d28  [Read the Docs](
-000005c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000005d0: 6c64 732e 696f 2f72 6561 6474 6865 646f  lds.io/readthedo
-000005e0: 6373 2f77 6966 6974 6573 7429 0a21 5b47  cs/wifitest).![G
-000005f0: 6974 4875 6220 5461 675d 2868 7474 7073  itHub Tag](https
-00000600: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000610: 6f2f 6769 7468 7562 2f76 2f74 6167 2f4a  o/github/v/tag/J
-00000620: 7561 6e42 696e 6465 7a2f 7769 6669 7465  uanBindez/wifite
-00000630: 7374 3f69 6e63 6c75 6465 5f70 7265 7265  st?include_prere
-00000640: 6c65 6173 6573 290a 3c61 2068 7265 663d  leases).<a href=
-00000650: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
-00000660: 672f 7072 6f6a 6563 742f 7769 6669 7465  g/project/wifite
-00000670: 7374 2f22 3e3c 696d 6720 7372 633d 2268  st/"><img src="h
-00000680: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000690: 6473 2e69 6f2f 7079 7069 2f76 2f77 6966  ds.io/pypi/v/wif
-000006a0: 6974 6573 7422 202f 3e3c 2f61 3e0a 0a23  itest" /></a>..#
-000006b0: 2320 5079 7468 6f6e 2033 206c 6962 7261  # Python 3 libra
-000006c0: 7279 2066 6f72 2077 6966 6920 7465 7374  ry for wifi test
-000006d0: 696e 672e 0a0a 2323 2320 496e 7374 616c  ing...### Instal
-000006e0: 6c0a 0a20 2020 2073 7564 6f20 7069 7020  l..    sudo pip 
-000006f0: 696e 7374 616c 6c20 7769 6669 7465 7374  install wifitest
-00000700: 0a0a 0a23 2323 2075 7361 6765 3a0a 0a23  ...### usage:..#
-00000710: 2323 2320 696d 706f 7274 0a0a 6060 6070  ### import..```p
-00000720: 7974 686f 6e0a 6672 6f6d 2077 6966 6974  ython.from wifit
-00000730: 6573 7420 696d 706f 7274 2057 6966 6954  est import WifiT
-00000740: 6573 740a 6060 600a 2323 2323 2073 6361  est.```.#### sca
-00000750: 6e20 6176 6169 6c61 626c 6520 7769 6669  n available wifi
-00000760: 206e 6574 776f 726b 730a 0a60 6060 7079   networks..```py
-00000770: 7468 6f6e 0a73 203d 2057 6966 6954 6573  thon.s = WifiTes
-00000780: 7428 290a 732e 7363 616e 2829 0a60 6060  t().s.scan().```
-00000790: 0a23 2323 2320 6272 7574 6566 6f72 6365  .#### bruteforce
-000007a0: 206f 6e20 7769 6669 206e 6574 776f 726b   on wifi network
-000007b0: 0a0a 6060 6070 7974 686f 6e0a 5353 4944  ..```python.SSID
-000007c0: 203d 2022 7769 6669 220a 574f 5244 4c49   = "wifi".WORDLI
-000007d0: 5354 203d 2022 776f 7264 6c69 7374 2e74  ST = "wordlist.t
-000007e0: 7874 220a 0a77 6966 6920 3d20 5769 6669  xt"..wifi = Wifi
-000007f0: 5465 7374 2829 0a77 6966 692e 6272 7574  Test().wifi.brut
-00000800: 6566 6f72 6365 2853 5349 442c 2057 4f52  eforce(SSID, WOR
-00000810: 444c 4953 5429 0a0a 6060 600a            DLIST)..```.
+00000030: 3172 6331 0a53 756d 6d61 7279 3a20 5079  1rc1.Summary: Py
+00000040: 7468 6f6e 2033 206c 6962 7261 7279 2066  thon 3 library f
+00000050: 6f72 2077 6966 6920 7465 7374 696e 672e  or wifi testing.
+00000060: 0a41 7574 686f 722d 656d 6169 6c3a 204a  .Author-email: J
+00000070: 7561 6e20 4269 6e64 657a 203c 6a75 616e  uan Bindez <juan
+00000080: 6269 6e64 657a 3738 3040 676d 6169 6c2e  bindez780@gmail.
+00000090: 636f 6d3e 0a4c 6963 656e 7365 3a20 4750  com>.License: GP
+000000a0: 4c76 3220 6c69 6365 6e73 650a 5072 6f6a  Lv2 license.Proj
+000000b0: 6563 742d 5552 4c3a 2048 6f6d 6570 6167  ect-URL: Homepag
+000000c0: 652c 2068 7474 7073 3a2f 2f67 6974 6875  e, https://githu
+000000d0: 622e 636f 6d2f 6a75 616e 6269 6e64 657a  b.com/juanbindez
+000000e0: 2f77 6966 6974 6573 740a 5072 6f6a 6563  /wifitest.Projec
+000000f0: 742d 5552 4c3a 2042 7567 2052 6570 6f72  t-URL: Bug Repor
+00000100: 7473 2c20 6874 7470 733a 2f2f 6769 7468  ts, https://gith
+00000110: 7562 2e63 6f6d 2f6a 7561 6e62 696e 6465  ub.com/juanbinde
+00000120: 7a2f 7769 6669 7465 7374 2f69 7373 7565  z/wifitest/issue
+00000130: 730a 5072 6f6a 6563 742d 5552 4c3a 2052  s.Project-URL: R
+00000140: 6561 6420 7468 6520 446f 6373 2c20 6874  ead the Docs, ht
+00000150: 7470 3a2f 2f77 6966 6974 6573 742e 7265  tp://wifitest.re
+00000160: 6164 7468 6564 6f63 732e 696f 2f0a 4b65  adthedocs.io/.Ke
+00000170: 7977 6f72 6473 3a20 6272 7574 6566 6f72  ywords: brutefor
+00000180: 6365 2c77 6966 692c 746f 6f6c 732c 636c  ce,wifi,tools,cl
+00000190: 692c 7363 616e 0a43 6c61 7373 6966 6965  i,scan.Classifie
+000001a0: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+000001b0: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
+000001c0: 6475 6374 696f 6e2f 5374 6162 6c65 0a43  duction/Stable.C
+000001d0: 6c61 7373 6966 6965 723a 2045 6e76 6972  lassifier: Envir
+000001e0: 6f6e 6d65 6e74 203a 3a20 436f 6e73 6f6c  onment :: Consol
+000001f0: 650a 436c 6173 7369 6669 6572 3a20 496e  e.Classifier: In
+00000200: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000210: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
+00000220: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+00000230: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000240: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
+00000250: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+00000260: 7632 2028 4750 4c76 3229 0a43 6c61 7373  v2 (GPLv2).Class
+00000270: 6966 6965 723a 204e 6174 7572 616c 204c  ifier: Natural L
+00000280: 616e 6775 6167 6520 3a3a 2045 6e67 6c69  anguage :: Engli
+00000290: 7368 0a43 6c61 7373 6966 6965 723a 204f  sh.Classifier: O
+000002a0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000002b0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000002c0: 740a 436c 6173 7369 6669 6572 3a20 5072  t.Classifier: Pr
+000002d0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000002e0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000002f0: 332e 370a 436c 6173 7369 6669 6572 3a20  3.7.Classifier: 
+00000300: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000310: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000320: 3a20 332e 380a 436c 6173 7369 6669 6572  : 3.8.Classifier
+00000330: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000340: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000350: 203a 3a20 332e 390a 436c 6173 7369 6669   :: 3.9.Classifi
+00000360: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000370: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000380: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
+00000390: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000003a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000003b0: 7974 686f 6e20 3a3a 2033 2e31 310a 436c  ython :: 3.11.Cl
+000003c0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000003d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000003e0: 3a20 5079 7468 6f6e 203a 3a20 332e 3132  : Python :: 3.12
+000003f0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000400: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000410: 6520 3a3a 2050 7974 686f 6e0a 436c 6173  e :: Python.Clas
+00000420: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00000430: 2049 6e74 6572 6e65 740a 436c 6173 7369   Internet.Classi
+00000440: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+00000450: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+00000460: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
+00000470: 203a 3a20 5079 7468 6f6e 204d 6f64 756c   :: Python Modul
+00000480: 6573 0a43 6c61 7373 6966 6965 723a 2054  es.Classifier: T
+00000490: 6f70 6963 203a 3a20 5465 726d 696e 616c  opic :: Terminal
+000004a0: 730a 436c 6173 7369 6669 6572 3a20 546f  s.Classifier: To
+000004b0: 7069 6320 3a3a 2055 7469 6c69 7469 6573  pic :: Utilities
+000004c0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
+000004d0: 3a20 3e3d 332e 370a 4465 7363 7269 7074  : >=3.7.Descript
+000004e0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
+000004f0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
+00000500: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+00000510: 4345 4e53 450a 5265 7175 6972 6573 2d44  CENSE.Requires-D
+00000520: 6973 743a 2070 7977 6966 690a 0a23 2077  ist: pywifi..# w
+00000530: 6966 6974 6573 740a 0a23 2320 5079 7468  ifitest..## Pyth
+00000540: 6f6e 2033 206c 6962 7261 7279 2066 6f72  on 3 library for
+00000550: 2077 6966 6920 7465 7374 696e 672e 0a0a   wifi testing...
+00000560: 2323 2320 496e 7374 616c 6c0a 0a20 2020  ### Install..   
+00000570: 2073 7564 6f20 7069 7020 696e 7374 616c   sudo pip instal
+00000580: 6c20 7769 6669 7465 7374 0a0a 0a23 2323  l wifitest...###
+00000590: 2075 7361 6765 0a0a 6060 6070 7974 686f   usage..```pytho
+000005a0: 6e0a 0a66 726f 6d20 7769 6669 7465 7374  n..from wifitest
+000005b0: 2069 6d70 6f72 7420 5769 6669 5465 7374   import WifiTest
+000005c0: 0a0a 5353 4944 203d 2022 7769 6669 220a  ..SSID = "wifi".
+000005d0: 574f 5244 4c49 5354 203d 2022 776f 7264  WORDLIST = "word
+000005e0: 6c69 7374 2e74 7874 220a 0a77 6966 6920  list.txt"..wifi 
+000005f0: 3d20 5769 6669 5465 7374 2829 0a77 6966  = WifiTest().wif
+00000600: 692e 6272 7574 6566 6f72 6365 2853 5349  i.bruteforce(SSI
+00000610: 442c 2057 4f52 444c 4953 5429 0a0a 6060  D, WORDLIST)..``
+00000620: 600a                                     `.
```

