# Comparing `tmp/moat-mqtt-0.40.1.tar.gz` & `tmp/moat-mqtt-0.40.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moat-mqtt-0.40.1.tar", last modified: Mon Feb 19 16:01:15 2024, max compression
+gzip compressed data, was "moat-mqtt-0.40.2.tar", last modified: Sun Apr 21 20:05:59 2024, max compression
```

## Comparing `moat-mqtt-0.40.1.tar` & `moat-mqtt-0.40.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.334602 moat-mqtt-0.40.1/
--rw-r--r--   0 smurf      (501) smurf      (501)      436 2024-02-19 16:01:11.000000 moat-mqtt-0.40.1/.gitignore
--rw-r--r--   0 smurf      (501) smurf      (501)      200 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/.pylintrc
--rw-r--r--   0 smurf      (501) smurf      (501)      307 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/.travis.yml
--rw-r--r--   0 smurf      (501) smurf      (501)      420 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/MANIFEST.in
--rw-r--r--   0 smurf      (501) smurf      (501)      513 2023-11-15 20:59:10.000000 moat-mqtt-0.40.1/Makefile
--rw-r--r--   0 smurf      (501) smurf      (501)      687 2024-02-19 16:01:15.334602 moat-mqtt-0.40.1/PKG-INFO
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.306599 moat-mqtt-0.40.1/docs/
--rw-r--r--   0 smurf      (501) smurf      (501)     7417 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/docs/Makefile
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.306599 moat-mqtt-0.40.1/docs/_static/
--rw-r--r--   0 smurf      (501) smurf      (501)       41 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/docs/_static/theme_overrides.css
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.306599 moat-mqtt-0.40.1/docs/_templates/
--rw-r--r--   0 smurf      (501) smurf      (501)      705 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/docs/_templates/layout.html
--rw-r--r--   0 smurf      (501) smurf      (501)     1862 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/docs/changelog.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    10355 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/docs/conf.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2198 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/docs/index.rst
--rw-r--r--   0 smurf      (501) smurf      (501)       52 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/docs/license.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     4958 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/docs/quickstart.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.310600 moat-mqtt-0.40.1/docs/references/
--rw-r--r--   0 smurf      (501) smurf      (501)     5654 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/docs/references/broker.rst
--rw-r--r--   0 smurf      (501) smurf      (501)      422 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/docs/references/common.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     4124 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/docs/references/distmqtt.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     5544 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/docs/references/distmqtt_pub.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     4526 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/docs/references/distmqtt_sub.rst
--rw-r--r--   0 smurf      (501) smurf      (501)      629 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/docs/references/index.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     8250 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/docs/references/mqttclient.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     1082 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/license.txt
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.310600 moat-mqtt-0.40.1/moat/
--rw-r--r--   0 smurf      (501) smurf      (501)      105 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/__init__.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.314600 moat-mqtt-0.40.1/moat/mqtt/
--rw-r--r--   0 smurf      (501) smurf      (501)       65 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/mqtt/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)      654 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/mqtt/_config.yaml
--rw-r--r--   0 smurf      (501) smurf      (501)     9968 2023-11-15 20:53:30.000000 moat-mqtt-0.40.1/moat/mqtt/_main.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4811 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/adapters.py
--rw-r--r--   0 smurf      (501) smurf      (501)    40344 2024-02-19 16:00:36.000000 moat-mqtt-0.40.1/moat/mqtt/broker.py
--rw-r--r--   0 smurf      (501) smurf      (501)    31552 2024-02-19 16:00:36.000000 moat-mqtt-0.40.1/moat/mqtt/client.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8540 2023-11-15 20:32:20.000000 moat-mqtt-0.40.1/moat/mqtt/codecs.py
--rw-r--r--   0 smurf      (501) smurf      (501)      635 2022-09-06 18:25:59.000000 moat-mqtt-0.40.1/moat/mqtt/errors.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6445 2023-11-16 11:16:31.000000 moat-mqtt-0.40.1/moat/mqtt/moat_kv_broker.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.314600 moat-mqtt-0.40.1/moat/mqtt/mqtt/
--rw-r--r--   0 smurf      (501) smurf      (501)     1580 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2793 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/connack.py
--rw-r--r--   0 smurf      (501) smurf      (501)    10900 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/connect.py
--rw-r--r--   0 smurf      (501) smurf      (501)      130 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/constants.py
--rw-r--r--   0 smurf      (501) smurf      (501)      752 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/disconnect.py
--rw-r--r--   0 smurf      (501) smurf      (501)     7214 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/packet.py
--rw-r--r--   0 smurf      (501) smurf      (501)      737 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/pingreq.py
--rw-r--r--   0 smurf      (501) smurf      (501)      801 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/pingresp.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.314600 moat-mqtt-0.40.1/moat/mqtt/mqtt/protocol/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/protocol/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8456 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/protocol/broker_handler.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6189 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/protocol/client_handler.py
--rw-r--r--   0 smurf      (501) smurf      (501)    29389 2024-02-19 16:00:36.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/protocol/handler.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1238 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/puback.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1244 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/pubcomp.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5326 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/publish.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1238 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/pubrec.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1241 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/pubrel.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2553 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/suback.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2583 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/subscribe.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1061 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/unsuback.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2295 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/mqtt/mqtt/unsubscribe.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.318601 moat-mqtt-0.40.1/moat/mqtt/plugins/
--rw-r--r--   0 smurf      (501) smurf      (501)       90 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/moat/mqtt/plugins/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3577 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/plugins/authentication.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1349 2022-09-16 17:01:50.000000 moat-mqtt-0.40.1/moat/mqtt/plugins/logging.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6851 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/plugins/manager.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2486 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/plugins/persistence.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.318601 moat-mqtt-0.40.1/moat/mqtt/plugins/sys/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/moat/mqtt/plugins/sys/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     7760 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/mqtt/plugins/sys/broker.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2823 2022-09-16 17:01:50.000000 moat-mqtt-0.40.1/moat/mqtt/plugins/topic_checking.py
--rw-r--r--   0 smurf      (501) smurf      (501)    11777 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/moat/mqtt/session.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2432 2023-11-15 20:32:20.000000 moat-mqtt-0.40.1/moat/mqtt/test.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3124 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/moat/mqtt/utils.py
--rw-r--r--   0 smurf      (501) smurf      (501)      108 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/moat/mqtt/version.py
--rw-r--r--   0 smurf      (501) smurf      (501)      535 2023-11-15 20:32:20.000000 moat-mqtt-0.40.1/moat-mqtt.cfg.sample
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.318601 moat-mqtt-0.40.1/moat_mqtt.egg-info/
--rw-r--r--   0 smurf      (501) smurf      (501)      687 2024-02-19 16:01:15.000000 moat-mqtt-0.40.1/moat_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)     2894 2024-02-19 16:01:15.000000 moat-mqtt-0.40.1/moat_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        1 2024-02-19 16:01:15.000000 moat-mqtt-0.40.1/moat_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 smurf      (501) smurf      (501)      146 2024-02-19 16:01:15.000000 moat-mqtt-0.40.1/moat_mqtt.egg-info/requires.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        5 2024-02-19 16:01:15.000000 moat-mqtt-0.40.1/moat_mqtt.egg-info/top_level.txt
--rw-r--r--   0 smurf      (501) smurf      (501)     2235 2024-02-19 16:00:36.000000 moat-mqtt-0.40.1/pyproject.toml
--rw-r--r--   0 smurf      (501) smurf      (501)     2551 2023-11-15 20:32:20.000000 moat-mqtt-0.40.1/readme.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.322601 moat-mqtt-0.40.1/samples/
--rw-r--r--   0 smurf      (501) smurf      (501)     1197 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/samples/broker_acl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1106 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/samples/broker_start.py
--rw-r--r--   0 smurf      (501) smurf      (501)      974 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/samples/broker_taboo.py
--rw-r--r--   0 smurf      (501) smurf      (501)      640 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/samples/client_keepalive.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1672 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/samples/client_publish.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1228 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/samples/client_publish_acl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1126 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/samples/client_publish_ssl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1149 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/samples/client_publish_ws.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1631 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/samples/client_retained.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1384 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/samples/client_subscribe.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1740 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/samples/client_subscribe_acl.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1078 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/samples/mosquitto.org.crt
--rw-r--r--   0 smurf      (501) smurf      (501)      167 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/samples/passwd
--rw-r--r--   0 smurf      (501) smurf      (501)       38 2024-02-19 16:01:15.334602 moat-mqtt-0.40.1/setup.cfg
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.322601 moat-mqtt-0.40.1/systemd/
--rw-r--r--   0 smurf      (501) smurf      (501)      328 2023-11-15 20:53:30.000000 moat-mqtt-0.40.1/systemd/moat-mqtt.service
--rw-r--r--   0 smurf      (501) smurf      (501)       86 2023-11-15 20:53:30.000000 moat-mqtt-0.40.1/systemd/sysusers
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.326601 moat-mqtt-0.40.1/tests/
--rw-r--r--   0 smurf      (501) smurf      (501)      153 2022-09-16 17:02:22.000000 moat-mqtt-0.40.1/tests/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)       71 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/tests/conftest.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1078 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/tests/mosquitto.org.crt
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.330602 moat-mqtt-0.40.1/tests/mqtt/
--rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/tests/mqtt/__init__.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.330602 moat-mqtt-0.40.1/tests/mqtt/protocol/
--rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/tests/mqtt/protocol/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)    14469 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/protocol/test_handler.py
--rw-r--r--   0 smurf      (501) smurf      (501)     6647 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/test_connect.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1766 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/test_packet.py
--rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/test_puback.py
--rw-r--r--   0 smurf      (501) smurf      (501)      760 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/test_pubcomp.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5166 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/test_publish.py
--rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/test_pubrec.py
--rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/test_pubrel.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1394 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/test_suback.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1204 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/test_subscribe.py
--rw-r--r--   0 smurf      (501) smurf      (501)      799 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/test_unsuback.py
--rw-r--r--   0 smurf      (501) smurf      (501)      996 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/mqtt/test_unsubscribe.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-02-19 16:01:15.334602 moat-mqtt-0.40.1/tests/plugins/
--rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/tests/plugins/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)      244 2022-09-06 09:13:47.000000 moat-mqtt-0.40.1/tests/plugins/passwd
--rw-r--r--   0 smurf      (501) smurf      (501)     3797 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/plugins/test_authentication.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3922 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/plugins/test_manager.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1812 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/plugins/test_persistence.py
--rw-r--r--   0 smurf      (501) smurf      (501)    26028 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/tests/test_broker.py
--rw-r--r--   0 smurf      (501) smurf      (501)     7707 2024-02-19 16:00:36.000000 moat-mqtt-0.40.1/tests/test_client.py
--rw-r--r--   0 smurf      (501) smurf      (501)     7648 2024-02-19 16:00:36.000000 moat-mqtt-0.40.1/tests/test_client_kv.py
--rw-r--r--   0 smurf      (501) smurf      (501)      957 2022-09-19 16:02:02.000000 moat-mqtt-0.40.1/tests/test_codecs.py
--rw-r--r--   0 smurf      (501) smurf      (501)      751 2023-05-18 12:50:18.000000 moat-mqtt-0.40.1/tests/test_tester.py
--rw-r--r--   0 smurf      (501) smurf      (501)      771 2022-09-06 09:53:33.000000 moat-mqtt-0.40.1/tox.ini
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.437508 moat-mqtt-0.40.2/
+-rw-r--r--   0 smurf      (501) smurf      (501)      436 2024-04-21 20:05:55.000000 moat-mqtt-0.40.2/.gitignore
+-rw-r--r--   0 smurf      (501) smurf      (501)      200 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/.pylintrc
+-rw-r--r--   0 smurf      (501) smurf      (501)      307 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/.travis.yml
+-rw-r--r--   0 smurf      (501) smurf      (501)      420 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/MANIFEST.in
+-rw-r--r--   0 smurf      (501) smurf      (501)      513 2023-11-15 20:59:10.000000 moat-mqtt-0.40.2/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)      687 2024-04-21 20:05:59.437508 moat-mqtt-0.40.2/PKG-INFO
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.405507 moat-mqtt-0.40.2/docs/
+-rw-r--r--   0 smurf      (501) smurf      (501)     7417 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/docs/Makefile
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.405507 moat-mqtt-0.40.2/docs/_static/
+-rw-r--r--   0 smurf      (501) smurf      (501)       41 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/docs/_static/theme_overrides.css
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.405507 moat-mqtt-0.40.2/docs/_templates/
+-rw-r--r--   0 smurf      (501) smurf      (501)      705 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/docs/_templates/layout.html
+-rw-r--r--   0 smurf      (501) smurf      (501)     1862 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/docs/changelog.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    10355 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/docs/conf.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2198 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/docs/index.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)       52 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/docs/license.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     4958 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/docs/quickstart.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.409507 moat-mqtt-0.40.2/docs/references/
+-rw-r--r--   0 smurf      (501) smurf      (501)     5654 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/docs/references/broker.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)      422 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/docs/references/common.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     4124 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/docs/references/distmqtt.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     5544 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/docs/references/distmqtt_pub.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     4526 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/docs/references/distmqtt_sub.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)      629 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/docs/references/index.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     8250 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/docs/references/mqttclient.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     1082 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/license.txt
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.409507 moat-mqtt-0.40.2/moat/
+-rw-r--r--   0 smurf      (501) smurf      (501)      105 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/__init__.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.413508 moat-mqtt-0.40.2/moat/mqtt/
+-rw-r--r--   0 smurf      (501) smurf      (501)       65 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/mqtt/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      654 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/mqtt/_config.yaml
+-rw-r--r--   0 smurf      (501) smurf      (501)     9968 2023-11-15 20:53:30.000000 moat-mqtt-0.40.2/moat/mqtt/_main.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4811 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/adapters.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    40344 2024-02-19 16:00:36.000000 moat-mqtt-0.40.2/moat/mqtt/broker.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    31552 2024-02-19 16:00:36.000000 moat-mqtt-0.40.2/moat/mqtt/client.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8540 2023-11-15 20:32:20.000000 moat-mqtt-0.40.2/moat/mqtt/codecs.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      635 2022-09-06 18:25:59.000000 moat-mqtt-0.40.2/moat/mqtt/errors.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6445 2023-11-16 11:16:31.000000 moat-mqtt-0.40.2/moat/mqtt/moat_kv_broker.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.413508 moat-mqtt-0.40.2/moat/mqtt/mqtt/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1580 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2793 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/connack.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    10900 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/connect.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      130 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/constants.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      752 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/disconnect.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     7214 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/packet.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      737 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/pingreq.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      801 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/pingresp.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.413508 moat-mqtt-0.40.2/moat/mqtt/mqtt/protocol/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/protocol/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8456 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/protocol/broker_handler.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6189 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/protocol/client_handler.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    29389 2024-02-19 16:00:36.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/protocol/handler.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1238 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/puback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1244 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/pubcomp.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5326 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/publish.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1238 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/pubrec.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1241 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/pubrel.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2553 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/suback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2583 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/subscribe.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1061 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/unsuback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2295 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/mqtt/mqtt/unsubscribe.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.417508 moat-mqtt-0.40.2/moat/mqtt/plugins/
+-rw-r--r--   0 smurf      (501) smurf      (501)       90 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/moat/mqtt/plugins/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3577 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/plugins/authentication.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1349 2022-09-16 17:01:50.000000 moat-mqtt-0.40.2/moat/mqtt/plugins/logging.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6851 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/plugins/manager.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2486 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/plugins/persistence.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.417508 moat-mqtt-0.40.2/moat/mqtt/plugins/sys/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/moat/mqtt/plugins/sys/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     7760 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/mqtt/plugins/sys/broker.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2823 2022-09-16 17:01:50.000000 moat-mqtt-0.40.2/moat/mqtt/plugins/topic_checking.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    11777 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/moat/mqtt/session.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2432 2023-11-15 20:32:20.000000 moat-mqtt-0.40.2/moat/mqtt/test.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3124 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/moat/mqtt/utils.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      108 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/moat/mqtt/version.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      535 2023-11-15 20:32:20.000000 moat-mqtt-0.40.2/moat-mqtt.cfg.sample
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.417508 moat-mqtt-0.40.2/moat_mqtt.egg-info/
+-rw-r--r--   0 smurf      (501) smurf      (501)      687 2024-04-21 20:05:59.000000 moat-mqtt-0.40.2/moat_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)     2894 2024-04-21 20:05:59.000000 moat-mqtt-0.40.2/moat_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2024-04-21 20:05:59.000000 moat-mqtt-0.40.2/moat_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)      144 2024-04-21 20:05:59.000000 moat-mqtt-0.40.2/moat_mqtt.egg-info/requires.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        5 2024-04-21 20:05:59.000000 moat-mqtt-0.40.2/moat_mqtt.egg-info/top_level.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)     2233 2024-04-21 20:05:22.000000 moat-mqtt-0.40.2/pyproject.toml
+-rw-r--r--   0 smurf      (501) smurf      (501)     2551 2023-11-15 20:32:20.000000 moat-mqtt-0.40.2/readme.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.425508 moat-mqtt-0.40.2/samples/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1197 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/samples/broker_acl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1106 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/samples/broker_start.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      974 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/samples/broker_taboo.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      640 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/samples/client_keepalive.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1672 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/samples/client_publish.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1228 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/samples/client_publish_acl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1126 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/samples/client_publish_ssl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1149 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/samples/client_publish_ws.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1631 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/samples/client_retained.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1384 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/samples/client_subscribe.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1740 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/samples/client_subscribe_acl.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1078 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/samples/mosquitto.org.crt
+-rw-r--r--   0 smurf      (501) smurf      (501)      167 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/samples/passwd
+-rw-r--r--   0 smurf      (501) smurf      (501)       38 2024-04-21 20:05:59.437508 moat-mqtt-0.40.2/setup.cfg
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.425508 moat-mqtt-0.40.2/systemd/
+-rw-r--r--   0 smurf      (501) smurf      (501)      328 2023-11-15 20:53:30.000000 moat-mqtt-0.40.2/systemd/moat-mqtt.service
+-rw-r--r--   0 smurf      (501) smurf      (501)       86 2023-11-15 20:53:30.000000 moat-mqtt-0.40.2/systemd/sysusers
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.429508 moat-mqtt-0.40.2/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)      153 2022-09-16 17:02:22.000000 moat-mqtt-0.40.2/tests/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)       71 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/tests/conftest.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1078 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/tests/mosquitto.org.crt
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.433508 moat-mqtt-0.40.2/tests/mqtt/
+-rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/tests/mqtt/__init__.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.437508 moat-mqtt-0.40.2/tests/mqtt/protocol/
+-rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/tests/mqtt/protocol/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    14469 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/protocol/test_handler.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     6647 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/test_connect.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1766 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/test_packet.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/test_puback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      760 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/test_pubcomp.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5166 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/test_publish.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/test_pubrec.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      755 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/test_pubrel.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1394 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/test_suback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1204 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/test_subscribe.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      799 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/test_unsuback.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      996 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/mqtt/test_unsubscribe.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2024-04-21 20:05:59.437508 moat-mqtt-0.40.2/tests/plugins/
+-rw-r--r--   0 smurf      (501) smurf      (501)       20 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/tests/plugins/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      244 2022-09-06 09:13:47.000000 moat-mqtt-0.40.2/tests/plugins/passwd
+-rw-r--r--   0 smurf      (501) smurf      (501)     3797 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/plugins/test_authentication.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3922 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/plugins/test_manager.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1812 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/plugins/test_persistence.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    26028 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/tests/test_broker.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     7707 2024-02-19 16:00:36.000000 moat-mqtt-0.40.2/tests/test_client.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     7648 2024-02-19 16:00:36.000000 moat-mqtt-0.40.2/tests/test_client_kv.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      957 2022-09-19 16:02:02.000000 moat-mqtt-0.40.2/tests/test_codecs.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      751 2023-05-18 12:50:18.000000 moat-mqtt-0.40.2/tests/test_tester.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      771 2022-09-06 09:53:33.000000 moat-mqtt-0.40.2/tox.ini
```

### Comparing `moat-mqtt-0.40.1/Makefile` & `moat-mqtt-0.40.2/Makefile`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/PKG-INFO` & `moat-mqtt-0.40.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moat-mqtt
-Version: 0.40.1
+Version: 0.40.2
 Summary: Async MQTT broker and client, with optional MoaT-KV support
 Author-email: Matthias Urlichs <matthias@urlichs.de>
 Project-URL: homepage, https://m-o-a-t.org
 Project-URL: repository, https://github.com/M-o-a-T/moat-mqtt
 Keywords: MoaT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moat-mqtt-0.40.1/docs/Makefile` & `moat-mqtt-0.40.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/docs/_templates/layout.html` & `moat-mqtt-0.40.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/docs/changelog.rst` & `moat-mqtt-0.40.2/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/docs/conf.py` & `moat-mqtt-0.40.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/docs/index.rst` & `moat-mqtt-0.40.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/docs/quickstart.rst` & `moat-mqtt-0.40.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/docs/references/broker.rst` & `moat-mqtt-0.40.2/docs/references/broker.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/docs/references/distmqtt.rst` & `moat-mqtt-0.40.2/docs/references/distmqtt.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/docs/references/distmqtt_pub.rst` & `moat-mqtt-0.40.2/docs/references/distmqtt_pub.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/docs/references/distmqtt_sub.rst` & `moat-mqtt-0.40.2/docs/references/distmqtt_sub.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/docs/references/index.rst` & `moat-mqtt-0.40.2/docs/references/index.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/docs/references/mqttclient.rst` & `moat-mqtt-0.40.2/docs/references/mqttclient.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/license.txt` & `moat-mqtt-0.40.2/license.txt`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/_config.yaml` & `moat-mqtt-0.40.2/moat/mqtt/_config.yaml`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/_main.py` & `moat-mqtt-0.40.2/moat/mqtt/_main.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/adapters.py` & `moat-mqtt-0.40.2/moat/mqtt/adapters.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/broker.py` & `moat-mqtt-0.40.2/moat/mqtt/broker.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/client.py` & `moat-mqtt-0.40.2/moat/mqtt/client.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/codecs.py` & `moat-mqtt-0.40.2/moat/mqtt/codecs.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/errors.py` & `moat-mqtt-0.40.2/moat/mqtt/errors.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/moat_kv_broker.py` & `moat-mqtt-0.40.2/moat/mqtt/moat_kv_broker.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/__init__.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/connack.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/connack.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/connect.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/connect.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/disconnect.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/disconnect.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/packet.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/packet.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/pingreq.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/pingreq.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/pingresp.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/pingresp.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/protocol/broker_handler.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/protocol/broker_handler.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/protocol/client_handler.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/protocol/client_handler.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/protocol/handler.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/protocol/handler.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/puback.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/puback.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/pubcomp.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/pubcomp.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/publish.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/publish.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/pubrec.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/pubrec.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/pubrel.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/pubrel.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/suback.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/suback.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/subscribe.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/subscribe.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/unsuback.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/unsuback.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/mqtt/unsubscribe.py` & `moat-mqtt-0.40.2/moat/mqtt/mqtt/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/plugins/authentication.py` & `moat-mqtt-0.40.2/moat/mqtt/plugins/authentication.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/plugins/logging.py` & `moat-mqtt-0.40.2/moat/mqtt/plugins/logging.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/plugins/manager.py` & `moat-mqtt-0.40.2/moat/mqtt/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/plugins/persistence.py` & `moat-mqtt-0.40.2/moat/mqtt/plugins/persistence.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/plugins/sys/broker.py` & `moat-mqtt-0.40.2/moat/mqtt/plugins/sys/broker.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/plugins/topic_checking.py` & `moat-mqtt-0.40.2/moat/mqtt/plugins/topic_checking.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/session.py` & `moat-mqtt-0.40.2/moat/mqtt/session.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/test.py` & `moat-mqtt-0.40.2/moat/mqtt/test.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat/mqtt/utils.py` & `moat-mqtt-0.40.2/moat/mqtt/utils.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat-mqtt.cfg.sample` & `moat-mqtt-0.40.2/moat-mqtt.cfg.sample`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/moat_mqtt.egg-info/PKG-INFO` & `moat-mqtt-0.40.2/moat_mqtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moat-mqtt
-Version: 0.40.1
+Version: 0.40.2
 Summary: Async MQTT broker and client, with optional MoaT-KV support
 Author-email: Matthias Urlichs <matthias@urlichs.de>
 Project-URL: homepage, https://m-o-a-t.org
 Project-URL: repository, https://github.com/M-o-a-T/moat-mqtt
 Keywords: MoaT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moat-mqtt-0.40.1/moat_mqtt.egg-info/SOURCES.txt` & `moat-mqtt-0.40.2/moat_mqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/pyproject.toml` & `moat-mqtt-0.40.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 	"Framework :: AnyIO",
 	"License :: OSI Approved",
 	"Development Status :: 4 - Beta",
 	"Topic :: Communications",
 	"Topic :: Internet",
 	]
 dependencies = [
-	"anyio ~= 4.0",
+	"anyio ~= 4.2",
 	"transitions",
 	"asyncwebsockets >= 0.9.2",
 	"passlib",
 	"pyyaml",
 	"attrs >= 19",
 	"simplejson",
 	"msgpack",
-	"moat-util ~= 0.35.0",
+	"moat-util ~= 0.35",
 	"transitions",
 	"wsproto",
 	"asyncscope >= 0.6.0",
 	]
 dynamic = [ "version",]
 keywords = [ "MoaT",]
 requires-python = ">=3.8"
```

### Comparing `moat-mqtt-0.40.1/readme.rst` & `moat-mqtt-0.40.2/readme.rst`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/broker_acl.py` & `moat-mqtt-0.40.2/samples/broker_acl.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/broker_start.py` & `moat-mqtt-0.40.2/samples/broker_start.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/broker_taboo.py` & `moat-mqtt-0.40.2/samples/broker_taboo.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/client_keepalive.py` & `moat-mqtt-0.40.2/samples/client_keepalive.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/client_publish.py` & `moat-mqtt-0.40.2/samples/client_publish.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/client_publish_acl.py` & `moat-mqtt-0.40.2/samples/client_publish_acl.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/client_publish_ssl.py` & `moat-mqtt-0.40.2/samples/client_publish_ssl.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/client_publish_ws.py` & `moat-mqtt-0.40.2/samples/client_publish_ws.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/client_retained.py` & `moat-mqtt-0.40.2/samples/client_retained.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/client_subscribe.py` & `moat-mqtt-0.40.2/samples/client_subscribe.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/client_subscribe_acl.py` & `moat-mqtt-0.40.2/samples/client_subscribe_acl.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/samples/mosquitto.org.crt` & `moat-mqtt-0.40.2/samples/mosquitto.org.crt`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mosquitto.org.crt` & `moat-mqtt-0.40.2/tests/mosquitto.org.crt`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/protocol/test_handler.py` & `moat-mqtt-0.40.2/tests/mqtt/protocol/test_handler.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/test_connect.py` & `moat-mqtt-0.40.2/tests/mqtt/test_connect.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/test_packet.py` & `moat-mqtt-0.40.2/tests/mqtt/test_packet.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/test_puback.py` & `moat-mqtt-0.40.2/tests/mqtt/test_puback.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/test_pubcomp.py` & `moat-mqtt-0.40.2/tests/mqtt/test_pubcomp.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/test_publish.py` & `moat-mqtt-0.40.2/tests/mqtt/test_publish.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/test_pubrec.py` & `moat-mqtt-0.40.2/tests/mqtt/test_pubrec.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/test_pubrel.py` & `moat-mqtt-0.40.2/tests/mqtt/test_pubrel.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/test_suback.py` & `moat-mqtt-0.40.2/tests/mqtt/test_suback.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/test_subscribe.py` & `moat-mqtt-0.40.2/tests/mqtt/test_subscribe.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/test_unsuback.py` & `moat-mqtt-0.40.2/tests/mqtt/test_unsuback.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/mqtt/test_unsubscribe.py` & `moat-mqtt-0.40.2/tests/mqtt/test_unsubscribe.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/plugins/test_authentication.py` & `moat-mqtt-0.40.2/tests/plugins/test_authentication.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/plugins/test_manager.py` & `moat-mqtt-0.40.2/tests/plugins/test_manager.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/plugins/test_persistence.py` & `moat-mqtt-0.40.2/tests/plugins/test_persistence.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/test_broker.py` & `moat-mqtt-0.40.2/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/test_client.py` & `moat-mqtt-0.40.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/test_client_kv.py` & `moat-mqtt-0.40.2/tests/test_client_kv.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/test_codecs.py` & `moat-mqtt-0.40.2/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tests/test_tester.py` & `moat-mqtt-0.40.2/tests/test_tester.py`

 * *Files identical despite different names*

### Comparing `moat-mqtt-0.40.1/tox.ini` & `moat-mqtt-0.40.2/tox.ini`

 * *Files identical despite different names*

