# Comparing `tmp/yoto_api-1.3.1.tar.gz` & `tmp/yoto_api-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.3.1.tar", last modified: Sat Apr 20 02:01:36 2024, max compression
+gzip compressed data, was "yoto_api-1.4.0.tar", last modified: Sun Apr 21 18:47:49 2024, max compression
```

## Comparing `yoto_api-1.3.1.tar` & `yoto_api-1.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:36.466202 yoto_api-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 02:01:09.000000 yoto_api-1.3.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-20 02:01:09.000000 yoto_api-1.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 02:01:09.000000 yoto_api-1.3.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 02:01:09.000000 yoto_api-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 02:01:09.000000 yoto_api-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-20 02:01:36.466202 yoto_api-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-20 02:01:09.000000 yoto_api-1.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 02:01:09.000000 yoto_api-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 02:01:36.466202 yoto_api-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-20 02:01:28.000000 yoto_api-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:36.462202 yoto_api-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:09.000000 yoto_api-1.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-20 02:01:09.000000 yoto_api-1.3.1/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:36.462202 yoto_api-1.3.1/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    21095 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 02:01:09.000000 yoto_api-1.3.1/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:01:36.466202 yoto_api-1.3.1/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 02:01:36.000000 yoto_api-1.3.1/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:47:49.891564 yoto_api-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-21 18:47:26.000000 yoto_api-1.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-21 18:47:26.000000 yoto_api-1.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 18:47:26.000000 yoto_api-1.4.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 18:47:26.000000 yoto_api-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-21 18:47:26.000000 yoto_api-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-21 18:47:49.891564 yoto_api-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-21 18:47:26.000000 yoto_api-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 18:47:26.000000 yoto_api-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:47:49.891564 yoto_api-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-21 18:47:42.000000 yoto_api-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:47:49.887564 yoto_api-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:47:26.000000 yoto_api-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-21 18:47:26.000000 yoto_api-1.4.0/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:47:49.891564 yoto_api-1.4.0/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-21 18:47:26.000000 yoto_api-1.4.0/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-21 18:47:26.000000 yoto_api-1.4.0/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23227 2024-04-21 18:47:26.000000 yoto_api-1.4.0/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-21 18:47:26.000000 yoto_api-1.4.0/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-21 18:47:26.000000 yoto_api-1.4.0/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-21 18:47:26.000000 yoto_api-1.4.0/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-21 18:47:26.000000 yoto_api-1.4.0/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:47:49.891564 yoto_api-1.4.0/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-21 18:47:49.000000 yoto_api-1.4.0/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-21 18:47:49.000000 yoto_api-1.4.0/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:47:49.000000 yoto_api-1.4.0/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:47:49.000000 yoto_api-1.4.0/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 18:47:49.000000 yoto_api-1.4.0/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 18:47:49.000000 yoto_api-1.4.0/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.3.1/CONTRIBUTING.rst` & `yoto_api-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.3.1/LICENSE` & `yoto_api-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.3.1/setup.py` & `yoto_api-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.3.1",
+    version="1.4.0",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.3.1/yoto_api/Card.py` & `yoto_api-1.4.0/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.3.1/yoto_api/YotoAPI.py` & `yoto_api-1.4.0/yoto_api/YotoAPI.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """API Methods"""
 
 import requests
 import logging
 import datetime
+import paho.mqtt.client as mqtt
+
 from datetime import timedelta
 import pytz
 from .const import DOMAIN
 from .Token import Token
 from .Card import Card
 from .YotoPlayer import YotoPlayer
 
@@ -16,16 +18,16 @@
 class YotoAPI:
     def __init__(self) -> None:
         self.BASE_URL: str = "https://api.yotoplay.com"
         self.CLIENT_ID: str = "4P2do5RhHDXvCDZDZ6oti27Ft2XdRrzr"
         self.LOGIN_URL: str = "login.yotoplay.com"
         self.TOKEN_URL: str = "https://api.yotoplay.com/auth/token"
         self.SCOPE: str = "YOUR_SCOPE"
-        # self.MQTT_AUTH_NAME: str = "JwtAuthorizer_mGDDmvLsocFY"
-        # self.MQTT_URL: str = "wss://aqrphjqbp3u2z-ats.iot.eu-west-2.amazonaws.com"
+        self.MQTT_AUTH_NAME: str = "JwtAuthorizer_mGDDmvLsocFY"
+        self.MQTT_URL: str = "aqrphjqbp3u2z-ats.iot.eu-west-2.amazonaws.com"
 
     def login(self, username: str, password: str) -> Token:
         url = self.TOKEN_URL
         payload = {}
         payload["audience"] = self.BASE_URL
         payload["client_id"] = self.CLIENT_ID
         payload["grant_type"] = "password"
@@ -74,15 +76,15 @@
             if self.get_child_value(item, "deviceId") not in players:
                 player: YotoPlayer = YotoPlayer(
                     id=self.get_child_value(item, "deviceId"),
                 )
                 players[player.id] = player
             deviceId = self.get_child_value(item, "deviceId")
             players[deviceId].name = self.get_child_value(item, "name")
-            players[deviceId].deviceType = self.get_child_value(item, "deviceType")
+            players[deviceId].device_type = self.get_child_value(item, "deviceType")
             players[deviceId].online = self.get_child_value(item, "online")
             players[deviceId].last_updated_at = datetime.datetime.now(pytz.utc)
 
     def update_library(self, token: Token, library: dict[Card]) -> list[Card]:
         response = self._get_cards(token)
         for item in response["cards"]:
             if self.get_child_value(item, "cardId") not in library:
@@ -274,14 +276,62 @@
         #       "updatedAt": "2024-04-05T04:03:55.198Z",
         #       "createdAt": "2023-03-16T17:32:34.249Z",
         #       "lastPlayedAt": "2024-04-05T06:15:11.308Z",
         #       "masterUid": "04dedd46720000"
         #     }
         # }
 
+    def connect_mqtt(self, token: Token, deviceId: str):
+        def on_message(client, userdata, message):
+            # Process MQTT Message
+            _LOGGER.debug(
+                f"{DOMAIN} - MQTT Message: {str(message.payload.decode('utf-8'))}"
+            )
+            _LOGGER.debug(f"{DOMAIN} - MQTT Topic: {message.topic}")
+            _LOGGER.debug(f"{DOMAIN} - MQTT QOS: {message.qos}")
+            _LOGGER.debug(f"{DOMAIN} - MQTT Retain: {message.retain}")
+
+        client = mqtt.Client(
+            mqtt.CallbackAPIVersion.VERSION1,
+            client_id="DASH" + deviceId,
+            transport="websockets",
+        )
+        client.username_pw_set(
+            username=deviceId + "?x-amz-customauthorizer-name=" + self.MQTT_AUTH_NAME,
+            password=token.access_token,
+        )
+        # client.on_connect = on_message
+        client.on_message = on_message
+        client.tls_set()
+        client.connect(host=self.MQTT_URL, port=443)
+        client.loop_start()
+        client.subscribe("device/" + deviceId + "/events")
+        client.subscribe("device/" + deviceId + "/status")
+        client.subscribe("device/" + deviceId + "/response")
+        # Command not needed but helps sniffing traffic
+        client.subscribe("device/" + deviceId + "/command")
+
+        # time.sleep(60)
+        # client.loop_stop()
+        return client
+
+    def card_pause(self, client, deviceId):
+        topic = "device/" + deviceId + "/command/card-pause"
+        payload = ""
+        self._publish_command(client, topic, payload)
+        # MQTT Message: {"status":{"card-pause":"OK","req_body":""}}
+
+    def card_play(self, client, deviceId):
+        topic = "device/" + deviceId + "/command/card-play"
+        self._publish_command(self, client, topic, "card-play")
+        # MQTT Message: {"status":{"card-play":"OK","req_body":"{\"uri\":\"https://yoto.io/7JtVV\",\"secondsIn\":0,\"cutOff\":0,\"chapterKey\":\"01\",\"trackKey\":\"01\",\"requestId\":\"5385910e-f853-4f34-99a4-d2ed94f02f6d\"}"}}
+
+    def _publish_command(self, client, topic, payload):
+        client.publish(topic, payload)
+
     def _get_card_detail(self, token: Token, cardid: str) -> dict:
         ############## Details below from snooping JSON requests of the app ######################
 
         url = self.BASE_URL + "/card/details/" + cardid
         headers = self._get_authenticated_headers(token)
 
         response = requests.post(url, headers=headers).json()
```

### Comparing `yoto_api-1.3.1/yoto_api/YotoManager.py` & `yoto_api-1.4.0/yoto_api/YotoManager.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,29 +15,38 @@
     def __init__(self, username: str, password: str) -> None:
         self.username: str = username
         self.password: str = password
         self.api: YotoAPI = YotoAPI()
         self.players: dict = {}
         self.token: Token = None
         self.library: list = {}
+        self.mqtt_client = None
 
     def initialize(self) -> None:
         self.token: Token = self.api.login(self.username, self.password)
         self.update_players_status()
         self.update_cards()
 
     def update_players_status(self) -> None:
         # Updates the data with current player data.
         self.api.update_players(self.token, self.players)
 
+    def connect_to_events(self) -> None:
+        for player in self.players.values():
+            # Needs to be correct to handle multiple devices. 1 client per device
+            self.mqtt_client = self.api.connect_mqtt(self.token, player.id)
+
     def update_cards(self) -> None:
         # Updates library and all card data.  Typically only required on startup.
         # TODO: Should update the self.library object with a current dict of players. Should it do details for all cards too or separate?
         self.api.update_library(self.token, self.library)
 
+    def pause_player(self, player_id: str):
+        self.api.card_pause(client=self.mqtt_client, deviceId=player_id)
+
     def check_and_refresh_token(self) -> bool:
         if self.token is None:
             self.initialize()
             return True
         # Check if valid and correct if not
         if self.token.valid_until <= datetime.datetime.now(pytz.utc):
             _LOGGER.debug(f"{DOMAIN} - Refresh token expired")
```

