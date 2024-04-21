# Comparing `tmp/s3i-0.7.0-py3-none-any.whl.zip` & `tmp/s3i-0.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 25253 bytes, number of entries: 19
+Zip file size: 25282 bytes, number of entries: 19
 -rw-r--r--  2.0 unx     1106 b- defN 24-Apr-19 12:32 s3i/__init__.py
--rw-r--r--  2.0 unx    10786 b- defN 24-Apr-19 12:32 s3i/broker.py
+-rw-r--r--  2.0 unx    11194 b- defN 24-Apr-21 14:43 s3i/broker.py
 -rw-r--r--  2.0 unx    23600 b- defN 24-Apr-10 15:48 s3i/broker_message.py
 -rw-r--r--  2.0 unx     6627 b- defN 24-Apr-10 15:48 s3i/callback_manager.py
 -rw-r--r--  2.0 unx     7206 b- defN 24-Apr-10 15:48 s3i/config.py
 -rw-r--r--  2.0 unx     3028 b- defN 24-Apr-10 17:26 s3i/directory.py
 -rw-r--r--  2.0 unx     5324 b- defN 24-Apr-10 17:26 s3i/ditto_manager.py
 -rw-r--r--  2.0 unx    14682 b- defN 24-Apr-19 12:32 s3i/event_system.py
 -rw-r--r--  2.0 unx    15645 b- defN 24-Apr-10 15:48 s3i/exception.py
 -rw-r--r--  2.0 unx     2361 b- defN 24-Apr-19 12:32 s3i/identity_provider.py
 -rw-r--r--  2.0 unx     4567 b- defN 21-Nov-09 20:20 s3i/key_pgp.py
 -rw-r--r--  2.0 unx     1008 b- defN 21-Nov-09 20:20 s3i/logger.py
 -rw-r--r--  2.0 unx      455 b- defN 21-Nov-09 20:20 s3i/repository.py
 -rw-r--r--  2.0 unx     1110 b- defN 24-Apr-10 17:26 s3i/tools.py
--rw-rw-rw-  2.0 unx     7651 b- defN 24-Apr-19 12:37 s3i-0.7.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1469 b- defN 24-Apr-19 12:37 s3i-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 12:37 s3i-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-19 12:37 s3i-0.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1406 b- defN 24-Apr-19 12:37 s3i-0.7.0.dist-info/RECORD
-19 files, 108127 bytes uncompressed, 23029 bytes compressed:  78.7%
+-rw-rw-rw-  2.0 unx     7651 b- defN 24-Apr-21 16:18 s3i-0.7.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1436 b- defN 24-Apr-21 16:18 s3i-0.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 16:18 s3i-0.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-21 16:18 s3i-0.7.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1406 b- defN 24-Apr-21 16:18 s3i-0.7.1.dist-info/RECORD
+19 files, 108502 bytes uncompressed, 23058 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: s3i/repository.py
 Comment: 
 
 Filename: s3i/tools.py
 Comment: 
 
-Filename: s3i-0.7.0.dist-info/LICENSE.txt
+Filename: s3i-0.7.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: s3i-0.7.0.dist-info/METADATA
+Filename: s3i-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: s3i-0.7.0.dist-info/WHEEL
+Filename: s3i-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: s3i-0.7.0.dist-info/top_level.txt
+Filename: s3i-0.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: s3i-0.7.0.dist-info/RECORD
+Filename: s3i-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## s3i/broker.py

```diff
@@ -99,14 +99,15 @@
         raise_error_from_broker_api_response(response, S3IBrokerRESTError, 200)
         return response.json()
 
 
 class BrokerAMQP:
     _ON_CONNECTION_OPEN = "_on_connection_open"
     _ON_CONNECTION_CLOSED = "_on_connection_closed"
+    _ON_CONNECTION_ERROR = "_on_connection_error"
     _ON_CHANNEL_OPEN = "_on_channel_open"
     _ON_CHANNEL_CLOSED = "_on_channel_closed"
 
     def __init__(self, token, loop=asyncio.get_event_loop(), logger=logging.getLogger()):
         self.__token = token
 
         self.__connection = None
@@ -143,15 +144,15 @@
             password=self.__token,
             erase_on_connect=True
         )
         connection_parameters = pika.ConnectionParameters(
             host=HOST,
             virtual_host=VIRTUAL_HOST,
             credentials=credentials,
-            heartbeat=10,
+            heartbeat=5,
             port=5671,
             ssl_options=pika.SSLOptions(ssl.SSLContext())
         )
         AsyncioConnection(
             parameters=connection_parameters,
             on_open_callback=self.on_connection_open,
             on_open_error_callback=self.on_connection_open_error,
@@ -174,14 +175,15 @@
         self.__callback_manager.process(
             self._ON_CONNECTION_OPEN,
             self.__loop
         )
 
     def on_connection_open_error(self, _unused_connection, err):
         self.__logger.error("[S3I]: Opening broker connection failed: {}".format(err))
+        self.__callback_manager.process(self._ON_CONNECTION_ERROR, self.__loop)
 
     def on_connection_closed(self, _unused_connection, err):
         self.__logger.info("[S3I]: Current Broker connection closed: {}".format(err))
 
     def on_channel_open(self, _unused_channel):
         self.__logger.info("[S3I]: Opening broker channel succeed")
         self.__channel = _unused_channel
@@ -235,14 +237,24 @@
             self._ON_CONNECTION_CLOSED,
             callback,
             one_shot,
             False,
             *args,
             **kwargs
         )
+    
+    def add_on_connection_error_callback(self, callback, one_shot, *args, **kwargs):
+        self.__callback_manager.add(
+            self._ON_CONNECTION_ERROR,
+            callback,
+            one_shot,
+            False,
+            *args,
+            **kwargs
+        )
 
     def start_consuming(self, endpoint, on_message):
         self.__consumer_tag = self.__channel.basic_consume(
             auto_ack=True,
             exclusive=True,
             queue=endpoint,
             on_message_callback=on_message
```

## Comparing `s3i-0.7.0.dist-info/LICENSE.txt` & `s3i-0.7.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `s3i-0.7.0.dist-info/METADATA` & `s3i-0.7.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3i
-Version: 0.7.0
+Version: 0.7.1
 Home-page: https://www.kwh40.de/
 Author: Kompetenzzentrum Wald und Holz 4.0
 Author-email: s3i@kwh40.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 License-File: LICENSE.txt
@@ -31,15 +31,14 @@
 Requires-Dist: pyparsing ==2.4.5
 Requires-Dist: pytz ==2019.3
 Requires-Dist: pyrql ==0.6.0
 Requires-Dist: python-keycloak ==3.9.0
 Requires-Dist: requests ==2.25.1
 Requires-Dist: six ==1.13.0
 Requires-Dist: snowballstemmer ==2.0.0
-Requires-Dist: typed-ast ==1.4.0
 Requires-Dist: wrapt ==1.11.2
 Requires-Dist: pgpy
 Requires-Dist: python-gnupg
 Requires-Dist: websocket-client
 Requires-Dist: schema ==0.7.1
 Requires-Dist: pynput
 Requires-Dist: urllib3 ==1.26.5
```

## Comparing `s3i-0.7.0.dist-info/RECORD` & `s3i-0.7.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 s3i/__init__.py,sha256=Sfd_rF3kYzXkXrGKupuyJBvMPibiWZA-xNZ3gPlVbZo,1106
-s3i/broker.py,sha256=Zr7TTpQqdnH24zywDFTfoU1ImtcaSe_PEzpiW_FcSE8,10786
+s3i/broker.py,sha256=457tfSelqOI8r37uqio3JWVXtCNSTyrxQ4fZdgDSqDM,11194
 s3i/broker_message.py,sha256=xIVE6Ku6T6yBih8NcVoweVU3vpCkTrRZsI7oZEEUhCI,23600
 s3i/callback_manager.py,sha256=5lTs4h-pNfExBtFUEfHsKVXVrQOl5EwRg-vw_wQUFZI,6627
 s3i/config.py,sha256=aoLSe6W-B4o5eW6onabsLJTutkXvlrpGNWXVoxG_CNI,7206
 s3i/directory.py,sha256=taOw4SrxIwzoDEBUMP_nsr57COi_LMtGG0Tkb6ozDb0,3028
 s3i/ditto_manager.py,sha256=tskSKozUZ6UMdtofj5zqWVTZQxATvShnv9g79XjrDos,5324
 s3i/event_system.py,sha256=I24OmyaKcHhYbgXEkflJLdxEW9KarYDfBk6IABKDKyI,14682
 s3i/exception.py,sha256=IgVQudVbCkSGe3Z_q2JMXMeF2blM0LpmVfXBYtdvBPk,15645
 s3i/identity_provider.py,sha256=q_DW5zhnmvydnuOGmT4nEqt6QM5iCEN67_-Q1Acfr18,2361
 s3i/key_pgp.py,sha256=1th7SmiLm7oQN5Qn-du8P3i24dvLvlFEFfPaHUH626c,4567
 s3i/logger.py,sha256=BjGtlc2_H_LfN9zH0q-I4lIilxglgUdXSkZHv3bk0r0,1008
 s3i/repository.py,sha256=SthJ_f55pl80USWr8aZnc6LB52igit4AfG6CbALVjpg,455
 s3i/tools.py,sha256=49mtYksygu_hqrwcKw_jJdcwwXHAfD662yrHAD4sq3w,1110
-s3i-0.7.0.dist-info/LICENSE.txt,sha256=pWgb-bBdsU2Gd2kwAXxketnm5W_2u8_fIeWEgojfrxs,7651
-s3i-0.7.0.dist-info/METADATA,sha256=n6v4H444v9VdgzW4DKPjGDcpgQM9oeyT6NY5kKtiRP4,1469
-s3i-0.7.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-s3i-0.7.0.dist-info/top_level.txt,sha256=_pR0bxLAE-quxyeIgilf0DVoaG-R7RpQlVArNNVes2I,4
-s3i-0.7.0.dist-info/RECORD,,
+s3i-0.7.1.dist-info/LICENSE.txt,sha256=pWgb-bBdsU2Gd2kwAXxketnm5W_2u8_fIeWEgojfrxs,7651
+s3i-0.7.1.dist-info/METADATA,sha256=H_ZjxmEoVLN30AzKXAExZvhNJyy0pV0NsAZZuDVsr9g,1436
+s3i-0.7.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+s3i-0.7.1.dist-info/top_level.txt,sha256=_pR0bxLAE-quxyeIgilf0DVoaG-R7RpQlVArNNVes2I,4
+s3i-0.7.1.dist-info/RECORD,,
```

