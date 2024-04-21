# Comparing `tmp/aiopioneer-0.6.0b1.tar.gz` & `tmp/aiopioneer-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopioneer-0.6.0b1.tar", last modified: Mon Apr  8 07:52:57 2024, max compression
+gzip compressed data, was "aiopioneer-0.6.0rc1.tar", last modified: Sun Apr 21 10:58:26 2024, max compression
```

## Comparing `aiopioneer-0.6.0b1.tar` & `aiopioneer-0.6.0rc1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwx---   0 root         (0) adm          (4)        0 2024-04-08 07:52:57.905947 aiopioneer-0.6.0b1/
--rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.6.0b1/LICENSE
--rw-rw----   0 root         (0) adm          (4)    15367 2024-04-08 07:52:57.913423 aiopioneer-0.6.0b1/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)    14715 2024-03-13 09:14:43.000000 aiopioneer-0.6.0b1/README.md
-drwxrwx---   0 root         (0) adm          (4)        0 2024-04-08 07:52:57.675950 aiopioneer-0.6.0b1/aiopioneer/
--rw-rw----   0 root         (0) adm          (4)       68 2024-03-27 20:16:44.000000 aiopioneer-0.6.0b1/aiopioneer/__init__.py
--rw-rw----   0 root         (0) adm          (4)    11031 2024-04-01 16:54:34.000000 aiopioneer-0.6.0b1/aiopioneer/cli.py
--rw-rw----   0 root         (0) adm          (4)    13805 2024-04-01 19:37:10.000000 aiopioneer-0.6.0b1/aiopioneer/commands.py
--rw-rw----   0 root         (0) adm          (4)    15083 2024-04-08 07:52:18.000000 aiopioneer-0.6.0b1/aiopioneer/const.py
--rw-rw----   0 root         (0) adm          (4)    18687 2024-03-27 20:47:07.000000 aiopioneer-0.6.0b1/aiopioneer/param.py
-drwxrwx---   0 root         (0) adm          (4)        0 2024-04-08 07:52:57.875947 aiopioneer-0.6.0b1/aiopioneer/parsers/
--rw-rw----   0 root         (0) adm          (4)     8175 2024-04-03 07:47:01.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/__init__.py
--rw-rw----   0 root         (0) adm          (4)     3419 2024-03-13 09:14:44.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/audio.py
--rw-rw----   0 root         (0) adm          (4)    19209 2024-03-13 09:14:44.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/dsp.py
--rw-rw----   0 root         (0) adm          (4)    25466 2024-03-31 11:50:52.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/information.py
--rw-rw----   0 root         (0) adm          (4)      599 2024-03-13 09:14:44.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/response.py
--rw-rw----   0 root         (0) adm          (4)    23416 2024-03-13 09:14:44.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/settings.py
--rw-rw----   0 root         (0) adm          (4)    15910 2024-04-03 07:56:23.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/system.py
--rw-rw----   0 root         (0) adm          (4)     6987 2024-04-03 07:20:56.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/tuner.py
--rw-rw----   0 root         (0) adm          (4)     8405 2024-03-13 09:14:44.000000 aiopioneer-0.6.0b1/aiopioneer/parsers/video.py
--rw-rw----   0 root         (0) adm          (4)    87240 2024-04-05 20:17:20.000000 aiopioneer-0.6.0b1/aiopioneer/pioneer_avr.py
--rw-rw----   0 root         (0) adm          (4)     5266 2024-04-05 20:12:40.000000 aiopioneer-0.6.0b1/aiopioneer/util.py
-drwxrwx---   0 root         (0) adm          (4)        0 2024-04-08 07:52:57.885947 aiopioneer-0.6.0b1/aiopioneer.egg-info/
--rw-rw----   0 root         (0) adm          (4)    15367 2024-04-08 07:52:56.000000 aiopioneer-0.6.0b1/aiopioneer.egg-info/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)      614 2024-04-08 07:52:57.000000 aiopioneer-0.6.0b1/aiopioneer.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) adm          (4)        1 2024-04-08 07:52:57.000000 aiopioneer-0.6.0b1/aiopioneer.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) adm          (4)       51 2024-04-08 07:52:57.000000 aiopioneer-0.6.0b1/aiopioneer.egg-info/entry_points.txt
--rw-rw----   0 root         (0) adm          (4)       11 2024-04-08 07:52:57.000000 aiopioneer-0.6.0b1/aiopioneer.egg-info/top_level.txt
--rw-rw----   0 root         (0) adm          (4)       38 2024-04-08 07:52:57.918339 aiopioneer-0.6.0b1/setup.cfg
--rw-rw----   0 root         (0) adm          (4)     1101 2024-03-31 08:50:09.000000 aiopioneer-0.6.0b1/setup.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-21 10:58:26.599502 aiopioneer-0.6.0rc1/
+-rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.6.0rc1/LICENSE
+-rw-rw----   0 root         (0) adm          (4)    29883 2024-04-21 10:58:26.603877 aiopioneer-0.6.0rc1/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)    29230 2024-04-20 12:22:03.000000 aiopioneer-0.6.0rc1/README.md
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-21 10:58:26.409504 aiopioneer-0.6.0rc1/aiopioneer/
+-rw-rw----   0 root         (0) adm          (4)       68 2024-03-27 20:16:44.000000 aiopioneer-0.6.0rc1/aiopioneer/__init__.py
+-rw-rw----   0 root         (0) adm          (4)    11211 2024-04-20 12:17:48.000000 aiopioneer-0.6.0rc1/aiopioneer/cli.py
+-rw-rw----   0 root         (0) adm          (4)    13805 2024-04-01 19:37:10.000000 aiopioneer-0.6.0rc1/aiopioneer/commands.py
+-rw-rw----   0 root         (0) adm          (4)    15131 2024-04-20 09:58:15.000000 aiopioneer-0.6.0rc1/aiopioneer/const.py
+-rw-rw----   0 root         (0) adm          (4)    18687 2024-03-27 20:47:07.000000 aiopioneer-0.6.0rc1/aiopioneer/param.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-21 10:58:26.569502 aiopioneer-0.6.0rc1/aiopioneer/parsers/
+-rw-rw----   0 root         (0) adm          (4)     8175 2024-04-03 07:47:01.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/__init__.py
+-rw-rw----   0 root         (0) adm          (4)     3419 2024-03-13 09:14:44.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/audio.py
+-rw-rw----   0 root         (0) adm          (4)    19209 2024-03-13 09:14:44.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/dsp.py
+-rw-rw----   0 root         (0) adm          (4)    25466 2024-03-31 11:50:52.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/information.py
+-rw-rw----   0 root         (0) adm          (4)      599 2024-03-13 09:14:44.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/response.py
+-rw-rw----   0 root         (0) adm          (4)    23416 2024-03-13 09:14:44.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/settings.py
+-rw-rw----   0 root         (0) adm          (4)    15910 2024-04-03 07:56:23.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/system.py
+-rw-rw----   0 root         (0) adm          (4)     6987 2024-04-03 07:20:56.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/tuner.py
+-rw-rw----   0 root         (0) adm          (4)     8405 2024-03-13 09:14:44.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/video.py
+-rw-rw----   0 root         (0) adm          (4)    86948 2024-04-20 12:17:45.000000 aiopioneer-0.6.0rc1/aiopioneer/pioneer_avr.py
+-rw-rw----   0 root         (0) adm          (4)     5266 2024-04-05 20:12:40.000000 aiopioneer-0.6.0rc1/aiopioneer/util.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-21 10:58:26.579502 aiopioneer-0.6.0rc1/aiopioneer.egg-info/
+-rw-rw----   0 root         (0) adm          (4)    29883 2024-04-21 10:58:25.000000 aiopioneer-0.6.0rc1/aiopioneer.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)      614 2024-04-21 10:58:26.000000 aiopioneer-0.6.0rc1/aiopioneer.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) adm          (4)        1 2024-04-21 10:58:25.000000 aiopioneer-0.6.0rc1/aiopioneer.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) adm          (4)       51 2024-04-21 10:58:25.000000 aiopioneer-0.6.0rc1/aiopioneer.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) adm          (4)       11 2024-04-21 10:58:25.000000 aiopioneer-0.6.0rc1/aiopioneer.egg-info/top_level.txt
+-rw-rw----   0 root         (0) adm          (4)       38 2024-04-21 10:58:26.610801 aiopioneer-0.6.0rc1/setup.cfg
+-rw-rw----   0 root         (0) adm          (4)     1101 2024-03-31 08:50:09.000000 aiopioneer-0.6.0rc1/setup.py
```

### Comparing `aiopioneer-0.6.0b1/LICENSE` & `aiopioneer-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/cli.py` & `aiopioneer-0.6.0rc1/aiopioneer/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                 pioneer.set_source_dict(source_dict)
             except json.JSONDecodeError:
                 print(f'ERROR: Invalid JSON source dict: "{arg}""')
         elif cmd == "get_source_list":
             print(f"Source list: {json.dumps(pioneer.get_source_list())}")
         elif cmd == "get_zone_listening_modes":
             print(
-                f"Available listening modes: {json.dumps(pioneer.get_zone_listening_modes())}"
+                f"Available listening modes: {json.dumps(pioneer.get_listening_modes())}"
             )
         elif cmd == "get_params":
             print(f"Params: {json.dumps(pioneer.get_params())}")
         elif cmd == "get_user_params":
             print(f"User Params: {json.dumps(pioneer.get_user_params())}")
         elif cmd == "set_user_params":
             try:
@@ -205,25 +205,29 @@
             except Exception as exc:  # pylint: disable=broad-except
                 print(f'ERROR: Invalid volume level "{arg}": {exc}')
         elif cmd == "select_source":
             source = arg if arg else ""
             await pioneer.select_source(source, zone=zone)
         elif cmd == "set_listening_mode":
             listening_mode = arg if arg else ""
-            await pioneer.set_listening_mode(listening_mode)
+            await pioneer.select_listening_mode(listening_mode)
         elif cmd == "set_tuner_frequency":
             subargs = arg.split(" ", maxsplit=1)
             try:
                 band = subargs[0]
                 frequency = float(subargs[1]) if len(subargs) > 1 else None
                 await pioneer.set_tuner_frequency(band, frequency)
             except Exception as exc:  # pylint: disable=broad-except
                 print(
                     f'ERROR: Invalid parameters for set_tuner_frequency "{arg}": {exc}'
                 )
+        elif cmd == "tuner_previous_preset":
+            await pioneer.tuner_previous_preset()
+        elif cmd == "tuner_next_preset":
+            await pioneer.tuner_next_preset()
         elif cmd in ["send_raw_command", ">"]:
             if arg:
                 print(f"Sending raw command {arg}")
                 await pioneer.send_raw_command(arg)
             else:
                 print("ERROR: No raw command specified")
         elif cmd in PIONEER_COMMANDS:
```

### Comparing `aiopioneer-0.6.0b1/aiopioneer/commands.py` & `aiopioneer-0.6.0rc1/aiopioneer/commands.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/const.py` & `aiopioneer-0.6.0rc1/aiopioneer/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Constants for aiopioneer."""
 
 from enum import StrEnum
 
+VERSION = "0.6.0rc1"
+DEFAULT_TIMEOUT = 2
+DEFAULT_SCAN_INTERVAL = 60
 DEFAULT_PORT = 8102
-VERSION = "0.6.0b1"
 
 
 class Zones(StrEnum):
     """Valid aiopioneer zones."""
 
     ALL = "ALL"
     Z1 = "1"
```

### Comparing `aiopioneer-0.6.0b1/aiopioneer/param.py` & `aiopioneer-0.6.0rc1/aiopioneer/param.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/parsers/__init__.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/parsers/audio.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/parsers/dsp.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/dsp.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/parsers/information.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/information.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/parsers/response.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/response.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/parsers/settings.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/settings.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/parsers/system.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/system.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/parsers/tuner.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/tuner.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/parsers/video.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/video.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer/pioneer_avr.py` & `aiopioneer-0.6.0rc1/aiopioneer/pioneer_avr.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,18 @@
     get_backoff_delay,
     cancel_task,
     safe_wait_for,
 )
 from .const import (
     Zones,
     TunerBand,
-    DEFAULT_PORT,
     VERSION,
+    DEFAULT_PORT,
+    DEFAULT_TIMEOUT,
+    DEFAULT_SCAN_INTERVAL,
     SOURCE_TUNER,
     LISTENING_MODES,
     DIMMER_MODES,
     TONE_MODES,
     TONE_DB_VALUES,
     SPEAKER_MODES,
     HDMI_OUT_MODES,
@@ -89,19 +91,19 @@
 
 
 class PioneerAVR:
     """Pioneer AVR interface."""
 
     def __init__(
         self,
-        host,
-        port=DEFAULT_PORT,
-        timeout=2,
-        scan_interval=60,
-        params=None,
+        host: str,
+        port: int = DEFAULT_PORT,
+        timeout: float = DEFAULT_TIMEOUT,
+        scan_interval: int = DEFAULT_SCAN_INTERVAL,
+        params: dict[str, str] = None,
     ):
         """Initialise the Pioneer AVR interface."""
         _LOGGER.info("Starting aiopioneer %s", VERSION)
         _LOGGER.debug(
             '>> PioneerAVR.__init__(host="%s", port=%s, timeout=%s, params=%s)',
             host,
             port,
@@ -207,15 +209,15 @@
             and PARAM_TUNER_AM_FREQ_STEP in self._system_params
         ):
             ## defer PARAM_TUNER_AM_FREQ_STEP to _user_params if specified
             del self._system_params[PARAM_TUNER_AM_FREQ_STEP]
         merge(self._params, self._system_params)
 
     def set_user_params(self, params: dict[str, Any] = None) -> None:
-        """Set parameters and merge with defaults."""
+        """Set user parameters and update current parameters."""
         _LOGGER.debug(">> PioneerAVR.set_user_params(%s)", params)
         self._user_params = copy.deepcopy(params) if params is not None else {}
         self._update_params()
         self._update_listening_modes()
 
     def _set_default_params_model(self) -> None:
         """Set default parameters based on device model."""
@@ -229,16 +231,16 @@
                         model,
                         model_regex,
                     )
                     merge(self._default_params, model_params, force_overwrite=True)
         self._update_params()
 
     def get_param(self, param_name: str) -> Any:
-        """Get a copy of all current parameters."""
-        return self._params[param_name]
+        """Get the value of the specified parameter."""
+        return self._params.get(param_name)
 
     def get_params(self) -> dict[str, Any]:
         """Get a copy of all current parameters."""
         ## NOTE: can't use MappingProxyTypeType because of mutable dict values
         return copy.deepcopy(self._params)
 
     def get_user_params(self) -> dict[str, Any]:
@@ -455,16 +457,15 @@
                             "volume_down", skip_if_queued=False, insert_at=1
                         )
                 self._power_zone_1 = self.power.get(Zones.Z1)  # cache value
 
                 # Implement a command queue so that we can queue commands if we
                 # need to update attributes that only get updated when we
                 # request them to change.
-                if len(self._command_queue) > 0:
-                    self._command_queue_schedule()
+                self.command_queue_schedule()
 
                 # NOTE: to avoid deadlocks, do not run any operations that
                 # depend on further responses (returned by the listener) within
                 # the listener loop.
 
                 if updated_zones:
                     action = f" while calling zone callbacks for {updated_zones}"
@@ -670,18 +671,18 @@
             return response
 
     async def send_command(
         self,
         command: str,
         zone: Zones = Zones.Z1,
         prefix: str = "",
+        suffix: str = "",
         ignore_error: bool | None = None,
         rate_limit: bool = True,
-        suffix: str = "",
-    ) -> bool | None:
+    ) -> str | bool | None:
         """Send a command or request to the device."""
         # pylint: disable=unidiomatic-typecheck disable=logging-not-lazy
         debug_command = self._params[PARAM_DEBUG_COMMAND]
         if debug_command:
             _LOGGER.debug(
                 '>> PioneerAVR.send_command("%s", zone="%s", prefix="%s", '
                 + "ignore_error=%s, rate_limit=%s, suffix=%s)",
@@ -709,17 +710,16 @@
                     if debug_command:
                         _LOGGER.debug("send_command received response: %s", response)
                     return response
                 else:
                     _LOGGER.error("invalid request %s for zone %s", raw_command, zone)
                     return None
             elif type(raw_command) is str:
-                return await self.send_raw_command(
-                    prefix + raw_command + suffix, rate_limit
-                )
+                await self.send_raw_command(prefix + raw_command + suffix, rate_limit)
+                return True
             else:
                 _LOGGER.warning("invalid command %s for zone %s", command, zone)
                 return None
         except RuntimeError as exc:
             _LOGGER.error("cannot execute %s command: %s", command, exc)
             return False
 
@@ -870,28 +870,25 @@
         source_name = None
         if source_id in self._source_id_to_name:
             source_name = self._source_id_to_name[source_id]
             self._source_id_to_name.pop(source_id)
         if source_name in self._source_name_to_id:
             self._source_name_to_id.pop(source_name)
 
-    def get_zone_listening_modes(self, zone: Zones = Zones.Z1) -> dict[str, str] | None:
-        """Return dict of valid listening modes and names for zone."""
-        ## Listening modes only supported on main zone
-        if zone == Zones.Z1:
-            multichannel = self.audio.get("input_multichannel")
-            listening_modes = self._params.get(PARAM_AVAILABLE_LISTENING_MODES, {})
-            zone_listening_modes = {}
-            for mode_id, mode_details in listening_modes.items():
-                if (multichannel and mode_details[2]) or (
-                    not multichannel and mode_details[1]
-                ):
-                    zone_listening_modes |= {mode_id: mode_details[0]}
-            return zone_listening_modes
-        return None
+    def get_listening_modes(self) -> dict[str, str] | None:
+        """Return dict of valid listening modes and names for Zone 1."""
+        multichannel = self.audio.get("input_multichannel")
+        listening_modes = self._params.get(PARAM_AVAILABLE_LISTENING_MODES, {})
+        zone_listening_modes = {}
+        for mode_id, mode_details in listening_modes.items():
+            if (multichannel and mode_details[2]) or (
+                not multichannel and mode_details[1]
+            ):
+                zone_listening_modes |= {mode_id: mode_details[0]}
+        return zone_listening_modes
 
     def _update_listening_modes(self) -> None:
         """Update list of valid listening modes for AVR."""
         all_listening_modes = LISTENING_MODES | self._params.get(
             PARAM_EXTRA_LISTENING_MODES, {}
         )
         disabled_listening_modes = self._params.get(PARAM_DISABLED_LISTENING_MODES)
@@ -983,15 +980,15 @@
         if zone in self.zones or zone == Zones.ALL:
             if callback:
                 self._zone_callback[zone] = callback
             else:
                 self._zone_callback.pop(zone)
 
     def clear_zone_callbacks(self) -> None:
-        """Clear all callbacks for a zone."""
+        """Clear callbacks for all zones."""
         self._zone_callback = {}
 
     def _call_zone_callbacks(self, zones: list[Zones] | None = None) -> None:
         """Call callbacks to signal updated zone(s)."""
         if not zones:
             zones = self.zones + [Zones.ALL]
         for zone in zones:
@@ -1157,15 +1154,15 @@
 
     async def _updater_cancel(self) -> None:
         """Cancel the updater task."""
         debug_updater = self._params[PARAM_DEBUG_UPDATER]
         await cancel_task(self._updater_task, "updater", debug=debug_updater)
         self._updater_task = None
 
-    async def _update_zone(self, zone: Zones | str) -> None:
+    async def _update_zone(self, zone: Zones) -> None:
         """Update an AVR zone."""
         # Check for timeouts, but ignore errors (eg. ?V will
         # return E02 immediately after power on)
 
         query_commands = []
         if not self._params.get(PARAM_DISABLE_AUTO_QUERY):
             query_commands = [
@@ -1185,43 +1182,46 @@
         ):
             # Timeout occurred, indicates AVR disconnected
             raise TimeoutError("Timeout waiting for data")
 
         # Zone 1 updates only, we loop through this to allow us to add commands
         # to read without needing to add it here, also only do this if the zone
         # is powered on
-        if Zones(zone) is Zones.Z1 and bool(self.power.get(Zones.Z1)):
+        if zone == Zones.Z1 and bool(self.power.get(Zones.Z1)):
             for comm in query_commands:
                 if PIONEER_COMMANDS.get(comm).get(Zones.Z1):
                     await self.send_command(comm, zone, ignore_error=True)
 
         # Zone 2 updates only, only available if zone 2 is on
-        if Zones(zone) is Zones.Z2 and bool(self.power.get(Zones.Z2)):
+        if zone == Zones.Z2 and bool(self.power.get(Zones.Z2)):
             for comm in query_commands:
                 if PIONEER_COMMANDS.get(comm).get(Zones.Z2):
                     await self.send_command(comm, zone, ignore_error=True)
 
         # CHANNEL updates are handled differently as it requires more complex
         # logic to send the commands we use the set_channel_levels command
         # and prefix the query to it.
         # Only run this if the main zone is on
         # HDZone does not have any channels
         if ("channels" in self._params.get(PARAM_ENABLED_FUNCTIONS)) and (
             not self._params.get(PARAM_DISABLE_AUTO_QUERY)
         ):
-            if bool(self.power.get(Zones.Z1)) and Zones(zone) is not Zones.HDZ:
+            if bool(self.power.get(Zones.Z1)) and zone != Zones.HDZ:
                 for k in CHANNEL_LEVELS_OBJ:
                     if len(k) == 1:
                         # Add two underscores
                         k = k + "__"
                     elif len(k) == 2:
                         # Add one underscore
                         k = k + "_"
                     await self.send_command(
-                        "set_channel_levels", zone, "?" + str(k), ignore_error=True
+                        "set_channel_levels",
+                        zone,
+                        prefix="?" + str(k),
+                        ignore_error=True,
                     )
 
     async def _updater_update(self) -> bool | None:
         """Update AVR cached status."""
         debug_updater = self._params[PARAM_DEBUG_UPDATER]
         if debug_updater:
             _LOGGER.debug(">> PioneerAVR._updater_update() started")
@@ -1333,20 +1333,20 @@
     def _check_zone(self, zone: Zones) -> Zones:
         """Check that specified zone is valid."""
         if zone not in self.zones:
             raise ValueError(f"zone {zone} does not exist on AVR")
         return zone
 
     async def turn_on(self, zone: Zones = Zones.Z1) -> bool | None:
-        """Turn on the Pioneer AVR."""
+        """Turn on the Pioneer AVR zone."""
         zone = self._check_zone(zone)
         return await self.send_command("turn_on", zone)
 
     async def turn_off(self, zone: Zones = Zones.Z1) -> bool | None:
-        """Turn off the Pioneer AVR."""
+        """Turn off the Pioneer AVR zone."""
         zone = self._check_zone(zone)
         return await self.send_command("turn_off", zone)
 
     async def select_source(self, source: str, zone: Zones = Zones.Z1) -> bool | None:
         """Select input source."""
         zone = self._check_zone(zone)
         source_id = self._source_name_to_id.get(source)
@@ -1433,18 +1433,21 @@
         debug_command = self._params[PARAM_DEBUG_COMMAND]
         await cancel_task(
             self._command_queue_task, "command_queue", debug=debug_command
         )
         self._command_queue_task = None
         self._command_queue = []
 
-    def _command_queue_schedule(self) -> None:
+    def command_queue_schedule(self) -> None:
         """Schedule commands to queue."""
         if self._params[PARAM_DEBUG_COMMAND]:
             _LOGGER.debug(">> PioneerAVR._command_queue_schedule()")
+        if len(self._command_queue) == 0:
+            return
+
         ## NOTE: does not create new task if one already exists
         if self._command_queue_task is None or self._command_queue_task.done():
             self._command_queue_task = asyncio.create_task(
                 self._execute_command_queue()
             )
 
     def queue_command(
@@ -1461,15 +1464,15 @@
             self._full_update = True
         if insert_at >= 0:
             self._command_queue.insert(insert_at, command)
         else:
             self._command_queue.append(command)
 
     async def set_volume_level(
-        self, target_volume: int, zone: Zones | str = Zones.Z1
+        self, target_volume: int, zone: Zones = Zones.Z1
     ) -> bool:
         """Set volume level (0..185 for Zone 1, 0..81 for other Zones)."""
         zone = self._check_zone(zone)
         current_volume = self.volume.get(zone.value)
         max_volume = self.max_volume[zone.value]
         if target_volume < 0 or target_volume > max_volume:
             raise ValueError(f"volume {target_volume} out of range for zone {zone}")
@@ -1520,56 +1523,48 @@
         return await self.send_command("mute_on", zone, ignore_error=False)
 
     async def mute_off(self, zone: Zones = Zones.Z1) -> bool:
         """Unmute AVR."""
         zone = self._check_zone(zone)
         return await self.send_command("mute_off", zone, ignore_error=False)
 
-    async def set_listening_mode(self, listening_mode: str) -> bool:
+    async def select_listening_mode(self, listening_mode: str) -> bool:
         """Set the listening mode using the predefined list of options in params."""
-        zone = Zones.Z1
-        listening_modes = self.get_zone_listening_modes(zone)
+        listening_modes = self.get_listening_modes()
         if listening_modes:
             for mode_id, mode_name in listening_modes.items():
                 if mode_name == listening_mode:
                     return await self.send_command(
                         "set_listening_mode",
-                        zone,
                         prefix=mode_id,
                         ignore_error=False,
                     )
         raise ValueError(f"listening mode {listening_mode} not available")
 
-    async def set_panel_lock(self, panel_lock: str, zone: Zones = Zones.Z1) -> bool:
+    async def set_panel_lock(self, panel_lock: str) -> bool:
         """Set the panel lock."""
-        zone = self._check_zone(zone)
         return await self.send_command(
             "set_amp_panel_lock",
-            zone,
-            self._get_parameter_key_from_value(panel_lock, PANEL_LOCK),
+            prefix=self._get_parameter_key_from_value(panel_lock, PANEL_LOCK),
             ignore_error=False,
         )
 
-    async def set_remote_lock(self, remote_lock: bool, zone: Zones = Zones.Z1) -> bool:
+    async def set_remote_lock(self, remote_lock: bool) -> bool:
         """Set the remote lock."""
-        zone = self._check_zone(zone)
         return await self.send_command(
             "set_amp_remote_lock",
-            zone,
-            ignore_error=False,
             prefix=str(int(remote_lock)),
+            ignore_error=False,
         )
 
-    async def set_dimmer(self, dimmer: str, zone: Zones = Zones.Z1) -> bool:
+    async def set_dimmer(self, dimmer: str) -> bool:
         """Set the display dimmer."""
-        zone = self._check_zone(zone)
         return await self.send_command(
             "set_amp_dimmer",
-            zone,
-            self._get_parameter_key_from_value(dimmer, DIMMER_MODES),
+            prefix=self._get_parameter_key_from_value(dimmer, DIMMER_MODES),
             ignore_error=False,
         )
 
     async def set_tone_settings(
         self,
         tone: str = None,
         treble: int = None,
@@ -1587,33 +1582,35 @@
         if not -6 <= bass <= 6:
             raise ValueError(f"invalid bass value: {bass}")
 
         if tone is not None:
             rc = await self.send_command(
                 "set_tone_mode",
                 zone,
-                self._get_parameter_key_from_value(tone, TONE_MODES),
+                prefix=self._get_parameter_key_from_value(tone, TONE_MODES),
                 ignore_error=False,
             )
         ## Set treble and bass only if zone tone status is set to "On"
         if rc and self.tone.get(zone.value, {}).get("status") == "On":
             treble_str = f"{str(treble)}dB"
             bass_str = f"{str(bass)}dB"
             if treble is not None:
                 rc = await self.send_command(
                     "set_tone_treble",
                     zone,
-                    self._get_parameter_key_from_value(treble_str, TONE_DB_VALUES),
+                    prefix=self._get_parameter_key_from_value(
+                        treble_str, TONE_DB_VALUES
+                    ),
                     ignore_error=False,
                 )
             if rc and bass is not None:
                 rc = await self.send_command(
                     "set_tone_bass",
                     zone,
-                    self._get_parameter_key_from_value(bass_str, TONE_DB_VALUES),
+                    prefix=self._get_parameter_key_from_value(bass_str, TONE_DB_VALUES),
                     ignore_error=False,
                 )
         return bool(rc)
 
     async def set_amp_settings(
         self,
         speaker_config: str = None,
@@ -1628,72 +1625,74 @@
         rc = True
 
         # FUNC: SPEAKERS (use PARAM_SPEAKER_MODES)
         if self.amp.get("speakers") is not None and speaker_config is not None:
             rc = await self.send_command(
                 "set_amp_speaker_status",
                 zone,
-                self._get_parameter_key_from_value(speaker_config, SPEAKER_MODES),
+                prefix=self._get_parameter_key_from_value(
+                    speaker_config, SPEAKER_MODES
+                ),
                 ignore_error=False,
             )
 
         # FUNC: HDMI OUTPUT SELECT (use PARAM_HDMI_OUT_MODES)
         if rc and self.amp.get("hdmi_out") is not None and hdmi_out is not None:
             rc = await self.send_command(
                 "set_amp_hdmi_out_status",
                 zone,
-                self._get_parameter_key_from_value(hdmi_out, HDMI_OUT_MODES),
+                prefix=self._get_parameter_key_from_value(hdmi_out, HDMI_OUT_MODES),
                 ignore_error=False,
             )
 
         # FUNC: HDMI AUDIO (simple bool, True is on, otherwise audio only goes to amp)
         if (
             rc
             and self.amp.get("hdmi_audio") is not None
             and hdmi_audio_output is not None
         ):
             rc = await self.send_command(
                 "set_amp_hdmi_audio_status",
                 zone,
-                str(int(hdmi_audio_output)),
+                prefix=str(int(hdmi_audio_output)),
                 ignore_error=False,
             )
 
         # FUNC: PQLS (simple bool, True is auto, False is off)
         if rc and self.amp.get("pqls") is not None and pqls is not None:
             rc = await self.send_command(
-                "set_amp_pqls_status", zone, str(int(pqls)), ignore_error=False
+                "set_amp_pqls_status", zone, prefix=str(int(pqls)), ignore_error=False
             )
 
         # FUNC: AMP (use PARAM_AMP_MODES)
         if rc and self.amp.get("status") is not None and amp is not None:
             rc = await self.send_command(
                 "set_amp_status",
                 zone,
-                self._get_parameter_key_from_value(amp, AMP_MODES),
+                prefix=self._get_parameter_key_from_value(amp, AMP_MODES),
                 ignore_error=False,
             )
 
         return rc
 
     async def select_tuner_band(self, band: TunerBand = TunerBand.FM) -> bool:
         """Set the tuner band."""
-        zone = Zones.Z1
-        band = TunerBand(band)
+        if not isinstance(band, TunerBand):
+            raise ValueError(f"invalid TunerBand specified: {band}")
         if self.tuner.get("band") is None or SOURCE_TUNER not in self.source.values():
             raise SystemError("tuner is unavailable")
 
         ## Set the tuner band
         if band == self.tuner.get("band"):
             return True
         tuner_commands = {
             TunerBand.AM: "set_tuner_band_am",
             TunerBand.FM: "set_tuner_band_fm",
         }
-        return await self.send_command(tuner_commands[band], zone, ignore_error=False)
+        return await self.send_command(tuner_commands[band], ignore_error=False)
 
     async def _calculate_am_frequency_step(self) -> None:
         """
         Automatically calculate the AM frequency step by stepping the frequency
         up and then down.
         """
         debug_command = self._params[PARAM_DEBUG_COMMAND]
@@ -1780,63 +1779,53 @@
             rc = False
         return rc
 
     async def set_tuner_frequency(
         self, band: TunerBand, frequency: float = None
     ) -> bool:
         """Set the tuner frequency and band."""
-        zone = Zones.Z1
-        band = TunerBand(band)
         if not await self.select_tuner_band(band):
             return False
         await self._command_queue_wait()  ## wait for AM step to be calculated
 
         if frequency is None:
             return True
         elif not isinstance(frequency, float):
             raise ValueError(f"invalid frequency {frequency}")
         elif (band == TunerBand.AM and not 530 <= frequency <= 1700) or (
             band == TunerBand.FM and not 87.5 <= frequency <= 108.0
         ):
             raise ValueError(f"frequency {frequency} out of range for band {band}")
 
-        if await self.send_command("operation_direct_access", zone, ignore_error=True):
+        if await self.send_command("operation_direct_access", ignore_error=True):
             ## Set tuner frequency directly if command is supported
             freq_str = str(int(frequency * (100 if band == TunerBand.FM else 1)))
             for digit in freq_str:
                 if not await self.send_command(
-                    "operation_tuner_digit", zone, prefix=digit, ignore_error=False
+                    "operation_tuner_digit", prefix=digit, ignore_error=False
                 ):
                     raise SystemError(f"AVR rejected frequency set to {frequency}")
         else:
             return await self._step_tuner_frequency(band, frequency)
 
     async def select_tuner_preset(self, tuner_class: str, preset: int) -> bool:
         """Select the tuner preset."""
-        zone = Zones.Z1
         return await self.send_command(
             "select_tuner_preset",
-            zone,
-            str(tuner_class).upper() + str(preset).upper().zfill(2),
+            prefix=str(tuner_class).upper() + str(preset).upper().zfill(2),
             ignore_error=False,
         )
 
     async def tuner_previous_preset(self) -> bool:
-        """Select the tuner preset."""
-        zone = Zones.Z1
-        return await self.send_command(
-            "decrease_tuner_preset", zone, ignore_error=False
-        )
+        """Select the previous tuner preset."""
+        return await self.send_command("decrease_tuner_preset", ignore_error=False)
 
     async def tuner_next_preset(self) -> bool:
-        """Select the tuner preset."""
-        zone = Zones.Z1
-        return await self.send_command(
-            "increase_tuner_preset", zone, ignore_error=False
-        )
+        """Select the next tuner preset."""
+        return await self.send_command("increase_tuner_preset", ignore_error=False)
 
     async def set_channel_levels(
         self, channel: str, level: float, zone: Zones = Zones.Z1
     ) -> bool:
         """Set the level (gain) for amplifier channel in zone."""
         zone = self._check_zone(zone)
         if self.channel_levels.get(zone.value) is None:
@@ -1851,21 +1840,20 @@
             channel = channel + "__"
         elif len(channel) == 2:
             channel = channel + "_"
 
         # convert the float to correct int
         level = int((level * 2) + 50)
         return await self.send_command(
-            "set_channel_levels", zone, channel + str(level), ignore_error=False
+            "set_channel_levels", zone, prefix=channel + str(level), ignore_error=False
         )
 
     async def set_video_settings(self, **arguments) -> bool:
         """Set video settings for a given zone."""
-        zone = Zones(arguments.get("zone"))
-        zone = self._check_zone(zone)
+        zone = self._check_zone(arguments.get("zone"))
 
         # This function is only valid for zone 1, no video settings are
         # available for zone 2, 3, 4 and HDZone
         if zone != Zones.Z1:
             raise ValueError(f"Invalid zone {zone}")
 
         # This is a complex function and supports handles requests to update any
@@ -1920,25 +1908,24 @@
                                 arguments[arg] += 50
                             elif arg == "mnr":
                                 arguments[arg] += 50
 
                         await self.send_command(
                             "set_video_" + arg,
                             zone,
-                            str(arguments.get(arg)),
+                            prefix=str(arguments.get(arg)),
                             ignore_error=False,
                         )
 
         ## TODO: check command rc, refactor to use match
         return True
 
     async def set_dsp_settings(self, **arguments) -> bool:
         """Set the DSP settings for the amplifier."""
-        zone = Zones(arguments.get("zone"))
-        zone = self._check_zone(zone)
+        zone = self._check_zone(arguments.get("zone"))
         if zone != Zones.Z1:
             raise ValueError(f"Invalid zone {zone}")
 
         for arg in arguments:
             if arg != "zone":
                 if arguments.get(arg) is not None:
                     if self.dsp.get(arg) is not arguments.get(arg):
@@ -1998,15 +1985,15 @@
                                 arguments[arg] = str(arguments.get(arg)).zfill(2)
                             elif arg == "center_width":
                                 arguments[arg] = str(arguments.get(arg)).zfill(2)
 
                         await self.send_command(
                             "set_dsp_" + arg,
                             zone,
-                            str(arguments.get(arg)),
+                            prefix=str(arguments.get(arg)),
                             ignore_error=False,
                         )
 
         ## TODO: check command rc, refactor to use match
         return True
 
     async def media_control(self, action: str, zone: Zones = Zones.Z1) -> bool:
```

### Comparing `aiopioneer-0.6.0b1/aiopioneer/util.py` & `aiopioneer-0.6.0rc1/aiopioneer/util.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/aiopioneer.egg-info/SOURCES.txt` & `aiopioneer-0.6.0rc1/aiopioneer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0b1/setup.py` & `aiopioneer-0.6.0rc1/setup.py`

 * *Files identical despite different names*

