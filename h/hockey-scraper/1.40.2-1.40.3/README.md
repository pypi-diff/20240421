# Comparing `tmp/hockey_scraper-1.40.2-py3-none-any.whl.zip` & `tmp/hockey_scraper-1.40.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 86409 bytes, number of entries: 44
+Zip file size: 86424 bytes, number of entries: 44
 -rw-r--r--  2.0 unx      288 b- defN 21-Jan-23 14:38 hockey_scraper/__init__.py
 -rw-r--r--  2.0 unx     4112 b- defN 21-Jan-01 13:56 hockey_scraper/cli.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Aug-04 17:20 hockey_scraper/nhl/__init__.py
 -rw-r--r--  2.0 unx    14030 b- defN 23-Dec-31 04:00 hockey_scraper/nhl/game_scraper.py
 -rw-r--r--  2.0 unx     5827 b- defN 24-Jan-03 05:41 hockey_scraper/nhl/json_schedule.py
 -rw-r--r--  2.0 unx    15946 b- defN 21-Mar-06 02:47 hockey_scraper/nhl/live_scrape.py
 -rw-r--r--  2.0 unx     4865 b- defN 20-Dec-22 20:23 hockey_scraper/nhl/playing_roster.py
 -rw-r--r--  2.0 unx    10719 b- defN 23-Dec-26 04:07 hockey_scraper/nhl/scrape_functions.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Aug-04 17:20 hockey_scraper/nhl/pbp/__init__.py
 -rw-r--r--  2.0 unx     7411 b- defN 22-Oct-08 23:26 hockey_scraper/nhl/pbp/espn_pbp.py
 -rw-r--r--  2.0 unx    28248 b- defN 22-Mar-17 23:46 hockey_scraper/nhl/pbp/html_pbp.py
--rw-r--r--  2.0 unx     5089 b- defN 23-Dec-31 04:01 hockey_scraper/nhl/pbp/json_pbp.py
+-rw-r--r--  2.0 unx     5109 b- defN 24-Apr-21 00:29 hockey_scraper/nhl/pbp/json_pbp.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Aug-04 17:20 hockey_scraper/nhl/shifts/__init__.py
 -rw-r--r--  2.0 unx     6464 b- defN 22-Oct-08 22:56 hockey_scraper/nhl/shifts/html_shifts.py
 -rw-r--r--  2.0 unx     3359 b- defN 21-Jan-20 14:06 hockey_scraper/nhl/shifts/json_shifts.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Aug-04 17:20 hockey_scraper/nwhl/__init__.py
 -rw-r--r--  2.0 unx     6384 b- defN 20-Aug-04 17:20 hockey_scraper/nwhl/game_pbp.py
 -rw-r--r--  2.0 unx     5726 b- defN 21-Jan-23 13:48 hockey_scraper/nwhl/scrape_functions.py
 -rw-r--r--  2.0 unx     5861 b- defN 21-Jan-23 14:40 hockey_scraper/nwhl/scrape_schedule.py
@@ -34,13 +34,13 @@
 -rw-r--r--  2.0 unx     2395 b- defN 23-Oct-30 08:35 tests/test_json_pbp.py
 -rw-r--r--  2.0 unx     2889 b- defN 24-Jan-03 05:57 tests/test_json_schedule.py
 -rw-r--r--  2.0 unx     1650 b- defN 20-Aug-04 17:20 tests/test_json_shifts.py
 -rw-r--r--  2.0 unx       37 b- defN 20-Aug-04 17:20 tests/test_nwhl.py
 -rw-r--r--  2.0 unx     3585 b- defN 20-Aug-04 17:20 tests/test_playing_roster.py
 -rw-r--r--  2.0 unx     1234 b- defN 20-Aug-04 17:20 tests/test_scrape_functions.py
 -rw-r--r--  2.0 unx     3011 b- defN 23-Dec-26 05:30 tests/test_shared.py
--rw-r--r--  2.0 unx    35150 b- defN 24-Jan-03 06:14 hockey_scraper-1.40.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     8297 b- defN 24-Jan-03 06:14 hockey_scraper-1.40.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-03 06:14 hockey_scraper-1.40.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 24-Jan-03 06:14 hockey_scraper-1.40.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3859 b- defN 24-Jan-03 06:14 hockey_scraper-1.40.2.dist-info/RECORD
-44 files, 249757 bytes uncompressed, 80195 bytes compressed:  67.9%
+-rw-r--r--  2.0 unx    35150 b- defN 24-Apr-21 00:30 hockey_scraper-1.40.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     8297 b- defN 24-Apr-21 00:30 hockey_scraper-1.40.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 00:30 hockey_scraper-1.40.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 24-Apr-21 00:30 hockey_scraper-1.40.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3859 b- defN 24-Apr-21 00:30 hockey_scraper-1.40.3.dist-info/RECORD
+44 files, 249777 bytes uncompressed, 80210 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -111,23 +111,23 @@
 
 Filename: tests/test_scrape_functions.py
 Comment: 
 
 Filename: tests/test_shared.py
 Comment: 
 
-Filename: hockey_scraper-1.40.2.dist-info/LICENSE.txt
+Filename: hockey_scraper-1.40.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hockey_scraper-1.40.2.dist-info/METADATA
+Filename: hockey_scraper-1.40.3.dist-info/METADATA
 Comment: 
 
-Filename: hockey_scraper-1.40.2.dist-info/WHEEL
+Filename: hockey_scraper-1.40.3.dist-info/WHEEL
 Comment: 
 
-Filename: hockey_scraper-1.40.2.dist-info/top_level.txt
+Filename: hockey_scraper-1.40.3.dist-info/top_level.txt
 Comment: 
 
-Filename: hockey_scraper-1.40.2.dist-info/RECORD
+Filename: hockey_scraper-1.40.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hockey_scraper/nhl/pbp/json_pbp.py

```diff
@@ -85,15 +85,15 @@
     :param event: json of event 
     
     :return: dictionary with the info
     """
     play = dict()
 
     play['event_id'] = event['eventId']
-    play['period'] = event['period']
+    play['period'] = event['periodDescriptor']['number']
     play['event'] = str(change_event_name(event['typeDescKey'].upper()))
     play['seconds_elapsed'] = shared.convert_to_seconds(event['timeInPeriod'])
     
     play['p1_name'], play['p2_name'], play['p3_name'] = '', '', ''
     if 'details' in event.keys():
         details = event['details'].keys()
         # If there's a players key that means an event occurred on the play.
```

## Comparing `hockey_scraper-1.40.2.dist-info/LICENSE.txt` & `hockey_scraper-1.40.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hockey_scraper-1.40.2.dist-info/METADATA` & `hockey_scraper-1.40.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hockey-scraper
-Version: 1.40.2
+Version: 1.40.3
 Summary: Python Package for scraping NHL Play-by-Play and Shift data.
 Home-page: https://github.com/HarryShomer/Hockey-Scraper
 Author: Harry Shomer
 Author-email: Harryshomer@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: NHL
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `hockey_scraper-1.40.2.dist-info/RECORD` & `hockey_scraper-1.40.3.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 hockey_scraper/nhl/json_schedule.py,sha256=yTZ4bVdPWpHjZy-4JJloKHMVUaerr3ittdB6vavtYhY,5827
 hockey_scraper/nhl/live_scrape.py,sha256=BDbqPOI2Py4rhR0en16pmGdLi5n5Opu3JDb6yxSwRZI,15946
 hockey_scraper/nhl/playing_roster.py,sha256=j_5qt4fk3k9Ipa9FuRJNcFw6GvsxbbIr5IWDidR2f84,4865
 hockey_scraper/nhl/scrape_functions.py,sha256=x_x_ADtDSRNzOP3exmdqizVkUButs1GWL8V6SCWL9l4,10719
 hockey_scraper/nhl/pbp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hockey_scraper/nhl/pbp/espn_pbp.py,sha256=w0aqHrGT6gLFVPAqgI3KlXRyEnzXHo5HL1iltbUPUVk,7411
 hockey_scraper/nhl/pbp/html_pbp.py,sha256=5_cTJe0zlR54rxuwVTHckOSXt-umOQ6Vp0_Awr-6yO0,28248
-hockey_scraper/nhl/pbp/json_pbp.py,sha256=lTVhbaNVWDttjaCiaUvHbRF-SmH4LZ0OOx5MNMxycXY,5089
+hockey_scraper/nhl/pbp/json_pbp.py,sha256=aR6jOSfJjqxqGi7xVKPwnFXFmezZx6xPiaxujVbK8b8,5109
 hockey_scraper/nhl/shifts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hockey_scraper/nhl/shifts/html_shifts.py,sha256=eB2UMWbnb34RO9ndjL6zqHvezdgFVlPzhO0omFi3Up0,6464
 hockey_scraper/nhl/shifts/json_shifts.py,sha256=J8on4VqyY0safP6DYYgJmA1ws7afitmWMjBuYOj40es,3359
 hockey_scraper/nwhl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hockey_scraper/nwhl/game_pbp.py,sha256=lsd6DvdtWqmbZEBnMSQB5n6PqE9GBsBXYg41VUAmRPA,6384
 hockey_scraper/nwhl/scrape_functions.py,sha256=usHg7T4hT7dLkE287iqltAIU62OJ9saxPW-cjzOZnIQ,5726
 hockey_scraper/nwhl/scrape_schedule.py,sha256=J-FLgjW_lagwGKJJL7EzffBcGft26jI8v6arAMVYEJU,5861
@@ -33,12 +33,12 @@
 tests/test_json_pbp.py,sha256=0RRxBvBb9oHypln1ezeM6ur_GvsWpEsfzNb_ObOJamM,2395
 tests/test_json_schedule.py,sha256=pNFHlf0E8fJSwnD00BrbKwPcrOJKN_i1vPrI7x7AYH0,2889
 tests/test_json_shifts.py,sha256=xo5HSzOMoLI3igM-8ZYkKaHDE20sMkpjVRhXIfG-fV8,1650
 tests/test_nwhl.py,sha256=aVgLEXVyHDxELNJ9n8AlbPXR7yIrb-aC6Sn55qVjS6U,37
 tests/test_playing_roster.py,sha256=p7siNVT7QqXppYpcIk2dGRkm5PSROJqb4-TaGHCtbj8,3585
 tests/test_scrape_functions.py,sha256=Xl0chK2vopjnpfQscvU6QA89GR0vOdOt9wTGInAz6uo,1234
 tests/test_shared.py,sha256=6ciiJhAI9o29D86ECcT4SZokZ1m0Lc3NICBF0F2I-B4,3011
-hockey_scraper-1.40.2.dist-info/LICENSE.txt,sha256=5X8cMguM-HmKfS_4Om-eBqM6A1hfbgZf6pfx2G24QFI,35150
-hockey_scraper-1.40.2.dist-info/METADATA,sha256=HJnIW5wkY1yPwvZkGgxNqkdJaxksfCpMDkDSvLvYw84,8297
-hockey_scraper-1.40.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-hockey_scraper-1.40.2.dist-info/top_level.txt,sha256=DKqfVm305m1cR57HpSwJrVwHF69qVVk9oU8n_HnJ2EY,21
-hockey_scraper-1.40.2.dist-info/RECORD,,
+hockey_scraper-1.40.3.dist-info/LICENSE.txt,sha256=5X8cMguM-HmKfS_4Om-eBqM6A1hfbgZf6pfx2G24QFI,35150
+hockey_scraper-1.40.3.dist-info/METADATA,sha256=TUguN6s_FOp1-FMEKx2YGhjZ4Xo2zjekjueNmsMv-E4,8297
+hockey_scraper-1.40.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+hockey_scraper-1.40.3.dist-info/top_level.txt,sha256=DKqfVm305m1cR57HpSwJrVwHF69qVVk9oU8n_HnJ2EY,21
+hockey_scraper-1.40.3.dist-info/RECORD,,
```

