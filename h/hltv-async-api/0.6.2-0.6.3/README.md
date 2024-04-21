# Comparing `tmp/hltv_async_api-0.6.2.tar.gz` & `tmp/hltv_async_api-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.6.2.tar", max compression
+gzip compressed data, was "hltv_async_api-0.6.3.tar", max compression
```

## Comparing `hltv_async_api-0.6.2.tar` & `hltv_async_api-0.6.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      124 2024-04-18 21:30:05.353310 hltv_async_api-0.6.2/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    38547 2024-04-20 14:54:15.471310 hltv_async_api-0.6.2/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.6.2/LICENSE
--rw-r--r--   0        0        0      648 2024-04-20 14:55:02.780232 hltv_async_api-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    15314 2024-04-18 21:50:02.092187 hltv_async_api-0.6.2/README.md
--rw-r--r--   0        0        0    15827 1970-01-01 00:00:00.000000 hltv_async_api-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      124 2024-04-21 18:39:28.954429 hltv_async_api-0.6.3/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    39828 2024-04-21 18:37:13.661717 hltv_async_api-0.6.3/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.6.3/LICENSE
+-rw-r--r--   0        0        0      648 2024-04-21 18:39:28.939349 hltv_async_api-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    15314 2024-04-18 21:50:02.092187 hltv_async_api-0.6.3/README.md
+-rw-r--r--   0        0        0    15827 1970-01-01 00:00:00.000000 hltv_async_api-0.6.3/PKG-INFO
```

### Comparing `hltv_async_api-0.6.2/hltv_async_api/aiohltv.py` & `hltv_async_api-0.6.3/hltv_async_api/aiohltv.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,19 @@
                  timeout: int = 5,
                  proxy_path: str | None = None,
                  proxy_list: list | None = None,
                  debug: bool = False,
                  max_retries: int = 0,
                  proxy_protocol: str | None = None,
                  proxy_one_time: bool = False,
-                 one_time_session: bool = True,
                  ):
         self.headers = {
             "referer": "https://www.hltv.org/stats",
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)",
-            "hltvTimeZone": "UTC"
+            "hltvTimeZone": "Europe/Copenhagen"     # TODO Timezone settings???
         }
         self.MAX_DELAY = max_delay
         self.timeout = timeout
         self.max_retries = max_retries
         self.DEBUG = debug
         self._configure_logging()
         self.logger = logging.getLogger(__name__)
@@ -356,20 +355,46 @@
     async def get_match_info(self, match_id: str | int, team1: str, team2: str, event_title: str, stats: bool = True):
         r = await self._fetch(f"https://www.hltv.org/matches/{str(match_id)}/"
                               f"{team1.replace(' ', '-')}-vs-"
                               f"{team2.replace(' ', '-')}-"
                               f"{event_title.replace(' ', '-')}")
         if not r:
             return
+        status_ = {'Match over': 0, 'LIVE': 1}
 
         status = r.find('div', {'class': 'countdown'}).text
 
+        status_int = status_[status] if status in status_ else 2
+
+        if status_int == 2:
+            components = status.split(" : ")
+
+            days, hours, minutes, seconds = 0, 0, 0, 0
+
+            for component in components:
+                if 'd' in component:
+                    days = int(component.replace("d", ""))
+                elif 'h' in component:
+                    hours = int(component.replace("h", ""))
+                elif 'm' in component:
+                    minutes = int(component.replace("m", ""))
+                elif 's' in component:
+                    seconds = int(component.replace("s", ""))
+
+            date_ = datetime.now(tz=pytz.timezone('Europe/Copenhagen')) + timedelta(days=days,
+                                                                                         hours=hours,
+                                                                                         minutes=minutes,
+                                                                                         seconds=seconds)
+
+            status = date_.strftime('%d-%m-%Y-%H-%M')
+
+
         score1, score2 = 0, 0
 
-        if status == 'Match over':
+        if status_int == 0:
             scores = r.find_all('div', class_='team')
             score1 = scores[0].get_text().replace('\n', '')[-1]
             score2 = scores[1].get_text().replace('\n', '')[-1]
 
         maps = []
         for map_div in r.find_all('div', {'class': 'mapholder'}):
 
@@ -380,15 +405,15 @@
                 r_team2 = r_teams[1].text
             except (AttributeError, IndexError):
                 r_team1 = '0'
                 r_team2 = '0'
             maps.append({'mapname': mapname, 'r_team1': r_team1, 'r_team2': r_team2})
 
         stats_ = []
-        if stats and status == 'Match over':
+        if stats and status_int == 0:
             for table_div in r.find_all('table', {'class': 'table totalstats'})[:2]:
                 for player in table_div.find_all('tr')[1:]:
                     player_id = player.find('a', class_='flagAlign')['href'].split('/')[2]
                     player_name = player.find('div', class_='statsPlayerName').text.strip()
                     nickname = re.findall(r"'(.*?)'", player_name)[0]
 
                     kd = player.find('td', class_='kd').text.strip()
@@ -398,25 +423,26 @@
                         'id': player_id,
                         'nickname': nickname,
                         'kd': kd,
                         'adr': adr,
                         'rating': rating
                     })
 
-        if status == "LIVE":
+        if status_int == 1:
             for map in maps:
+                len_ = len(map)
                 if map["r_team1"] == '13':
-                    if len(map) != 1:
+                    if len_ != 1:
                         score1 += 1
                     else:
                         score1 = 13
                         score2 = int(map["r_team2"])
 
                 elif map["r_team1"] == '13':
-                    if len(map) != 1:
+                    if len_ != 1:
                         score2 += 1
                     else:
                         score2 = 13
                         score1 = int(map["r_team1"])
 
         return {'id': match_id, 'score1': score1, 'score2': score2, 'status': status, 'maps': maps, 'stats': stats_}
 
@@ -638,15 +664,15 @@
                     'end_date': event_end_date,
                 })
         except AttributeError:
             pass
 
         return events
 
-    async def get_events(self, featured=True, outgoing=True, future=True, max_events=10):
+    async def get_events(self, outgoing=True, future=True, max_events=10):
         """Returns events
         :params:
         outgoing - include live tournaments
         future - include future tournamets
         max_events - use only if future=True
         :return:
         [('id', 'title', 'startdate', 'enddate')]
@@ -957,11 +983,12 @@
                 break
 
         return news
 
 
 async def main():
     hltv = Hltv()
-    print(await hltv.get_matches())
+    print(await hltv.get_matches(live=False))
+    print(await hltv.get_match_info(2371706, 'Guild Eagles', 'sangal', 'CCT Season 2 Europe Series 1'))
 
 if __name__ == '__main__':
     asyncio.run(main())
```

### Comparing `hltv_async_api-0.6.2/LICENSE` & `hltv_async_api-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.6.2/pyproject.toml` & `hltv_async_api-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.6.2"
+version = "0.6.3"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `hltv_async_api-0.6.2/README.md` & `hltv_async_api-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.6.2/PKG-INFO` & `hltv_async_api-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.6.2
+Version: 0.6.3
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Author: Akim Slys
 Author-email: akimslys2003@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

