# Comparing `tmp/ansi-string-0.1.3.tar.gz` & `tmp/ansi-string-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansi-string-0.1.3.tar", last modified: Sat Apr 20 15:52:48 2024, max compression
+gzip compressed data, was "ansi-string-1.0.0.tar", last modified: Sun Apr 21 19:18:06 2024, max compression
```

## Comparing `ansi-string-0.1.3.tar` & `ansi-string-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:52:48.534259 ansi-string-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 15:52:40.000000 ansi-string-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-20 15:52:40.000000 ansi-string-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-20 15:52:48.534259 ansi-string-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-20 15:52:40.000000 ansi-string-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-20 15:52:40.000000 ansi-string-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-20 15:52:48.534259 ansi-string-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-20 15:52:40.000000 ansi-string-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:52:48.534259 ansi-string-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:52:48.534259 ansi-string-0.1.3/src/ansi_string/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-20 15:52:40.000000 ansi-string-0.1.3/src/ansi_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59771 2024-04-20 15:52:40.000000 ansi-string-0.1.3/src/ansi_string/ansi_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:52:48.534259 ansi-string-0.1.3/src/ansi_string.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-20 15:52:48.000000 ansi-string-0.1.3/src/ansi_string.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-20 15:52:48.000000 ansi-string-0.1.3/src/ansi_string.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 15:52:48.000000 ansi-string-0.1.3/src/ansi_string.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 15:52:48.000000 ansi-string-0.1.3/src/ansi_string.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 15:52:48.000000 ansi-string-0.1.3/src/ansi_string.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:18:06.539337 ansi-string-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 19:17:55.000000 ansi-string-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-21 19:17:55.000000 ansi-string-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-21 19:18:06.539337 ansi-string-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-21 19:17:55.000000 ansi-string-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 19:17:55.000000 ansi-string-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 19:18:06.539337 ansi-string-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-21 19:17:55.000000 ansi-string-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:18:06.535338 ansi-string-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:18:06.535338 ansi-string-1.0.0/src/ansi_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-21 19:17:55.000000 ansi-string-1.0.0/src/ansi_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71474 2024-04-21 19:17:55.000000 ansi-string-1.0.0/src/ansi_string/ansi_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:18:06.539337 ansi-string-1.0.0/src/ansi_string.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-21 19:18:06.000000 ansi-string-1.0.0/src/ansi_string.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-21 19:18:06.000000 ansi-string-1.0.0/src/ansi_string.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:18:06.000000 ansi-string-1.0.0/src/ansi_string.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 19:18:06.000000 ansi-string-1.0.0/src/ansi_string.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 19:18:06.000000 ansi-string-1.0.0/src/ansi_string.egg-info/top_level.txt
```

### Comparing `ansi-string-0.1.3/LICENSE` & `ansi-string-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansi-string-0.1.3/setup.py` & `ansi-string-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `ansi-string-0.1.3/src/ansi_string/ansi_string.py` & `ansi-string-1.0.0/src/ansi_string/ansi_string.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 # SOFTWARE.
 
 import sys
 import re
 import math
 from enum import Enum, auto as enum_auto
 import io
-from typing import Any, Union, List
+from typing import Any, Union, List, Dict, Tuple
 
-__version__ = '0.1.3'
+__version__ = '1.0.0'
 PACKAGE_NAME = 'ansi-string'
 
 WHITESPACE_CHARS = ' \t\n\r\v\f'
 
 IS_WINDOWS = sys.platform.lower().startswith('win')
 
 if IS_WINDOWS:
@@ -89,15 +89,15 @@
 
 ColourComponentType = ColorComponentType  # Alias for my British English friends
 
 class AnsiFormat(Enum):
     '''
     Formatting which may be supplied to AnsiString.
     '''
-    RESET='0'
+    # Never use RESET
     BOLD='1'
     FAINT='2'
     ITALIC='3'
     ITALICS=ITALIC # Alias
     UNDERLINE='4'
     SLOW_BLINK='5'
     RAPID_BLINK='6'
@@ -735,15 +735,20 @@
     UL_GREY=UL_GRAY # Alias for my British English friends
     UL_DIM_GRAY=f'{UNDERLINE};{SET_UNDERLINE_COLOR_RGB};105;105;105'
     UL_LIGHT_SLATE_GRAY=f'{UNDERLINE};{SET_UNDERLINE_COLOR_RGB};119;136;153'
     UL_SLATE_GRAY=f'{UNDERLINE};{SET_UNDERLINE_COLOR_RGB};112;128;144'
     UL_DARK_SLATE_GRAY=f'{UNDERLINE};{SET_UNDERLINE_COLOR_RGB};47;79;79'
 
     @staticmethod
-    def rgb(r_or_rgb:int, g:Union[int,None]=None, b:Union[int,None]=None, component:ColorComponentType=ColorComponentType.FOREGROUND):
+    def rgb(
+        r_or_rgb:int,
+        g:Union[int,None]=None,
+        b:Union[int,None]=None,
+        component:ColorComponentType=ColorComponentType.FOREGROUND
+    ) -> str:
         '''
         Generates a FG or BG ANSI sequence for the given RGB values.
         r_or_rgb: Either an 8-bit red component or the full 24-bit RGB value
         g: An 8-bit green component (b must also be specified when set)
         b: An 8-bit blue component (g must also be specified when set)
         component: The component to set color of (background, foreground, or underline)
         '''
@@ -804,49 +809,61 @@
     '''
 
     # The escape sequence that needs to be formatted with command str
     ANSI_ESCAPE_FORMAT = '\x1b[{}m'
     # The escape sequence which will clear all previous formatting (empty command is same as 0)
     ANSI_ESCAPE_CLEAR = ANSI_ESCAPE_FORMAT.format('')
 
-    # Number of elements in each value of _color_settings dict
-    SETTINGS_ITEM_LIST_LEN = 2
-    # Index of _color_settings value list which contains settings to apply
-    SETTINGS_APPLY_IDX = 0
-    # Index of _color_settings value list which contains settings to remove
-    SETTINGS_REMOVE_IDX = 1
+    # This isn't in AnsiFormat because it shouldn't be used externally
+    RESET = '0'
 
-    class Settings:
+    class Setting:
         '''
         Internal use only - mainly used to create a unique objects which may contain same strings
         '''
-        def __init__(self, setting_or_settings:Union[List[str], str, List[AnsiFormat], AnsiFormat]):
-            if not isinstance(setting_or_settings, list):
-                settings = [setting_or_settings]
-            else:
-                settings = setting_or_settings
+        def __init__(self, setting:Union[str, int, AnsiFormat]):
+            if isinstance(setting, int):
+                setting = str(setting)
+            elif hasattr(setting, 'value') and isinstance(setting.value, str):
+                # Likely an enumeration - use the value
+                setting = setting.value
+            elif not isinstance(setting, str):
+                raise TypeError('Unsupported type for setting_or_settings: {}'.format(type(setting)))
 
-            for i, item in enumerate(settings):
-                if isinstance(item, str):
-                    settings[i] = __class__._scrub_ansi_format_string(item)
-                elif hasattr(item, 'value') and isinstance(item.value, str):
-                    # Likely an enumeration - use the value
-                    settings[i] = item.value
-                else:
-                    raise TypeError('Unsupported type for setting_or_settings: {}'.format(type(setting_or_settings)))
+            self._str = setting
+
+        def __eq__(self, value) -> bool:
+            if isinstance(value, str):
+                return self._str == value
+            elif isinstance(value, AnsiString.Setting):
+                return self._str == value._str
+            return False
+
+        def __str__(self) -> str:
+            return self._str
 
-            self._str = ';'.join(settings)
+    class SettingPoint:
+        def __init__(
+            self,
+            add:Union[List['AnsiString.Setting'],None]=None,
+            rem:Union[List['AnsiString.Setting'],None]=None
+        ):
+            self.add:List[AnsiString.Setting] = add or []
+            self.rem:List[AnsiString.Setting] = rem or []
 
         def __eq__(self, value) -> bool:
-            if not isinstance(value, AnsiString.Settings):
-                return False
-            return self._str == value._str
+            if isinstance(value, AnsiString.SettingPoint):
+                return value.add == self.add and value.rem == self.rem
+            return False
+
+        def __bool__(self) -> bool:
+            return bool(self.add) or bool(self.rem)
 
         @staticmethod
-        def _parse_rgb_string(s:str):
+        def _parse_rgb_string(s:str) -> str:
             component_dict = {
                 'ul_': ColorComponentType.UNDERLINE,
                 'bg_': ColorComponentType.BACKGROUND,
                 'fg_': ColorComponentType.FOREGROUND
             }
 
             # rgb(), fg_rgb(), bg_rgb(), or ul_rgb() with 3 distinct values as decimal or hex
@@ -867,18 +884,18 @@
                     rgb = int(match.group(3), 16 if match.group(2) else 10)
                 except ValueError:
                     raise ValueError('Invalid rgb value')
                 return AnsiFormat.rgb(rgb, component=component_dict.get(match.group(1), ColorComponentType.FOREGROUND))
             return None
 
         @staticmethod
-        def _scrub_ansi_format_string(ansi_format):
+        def _scrub_ansi_format_string(ansi_format:str) -> List[str]:
             if ansi_format.startswith("["):
                 # Use the rest of the string as-is for settings
-                return ansi_format[1:]
+                return [ansi_format[1:]]
             else:
                 # The format string contains names within AnsiFormat or integers, separated by semicolon
                 formats = ansi_format.split(';')
                 format_settings_strs = []
                 for format in formats:
                     ansi_fmt_enum = None
                     try:
@@ -888,113 +905,160 @@
                     else:
                         format_settings_strs.append(ansi_fmt_enum.value)
 
                     if ansi_fmt_enum is None:
                         rgb_format = __class__._parse_rgb_string(format)
                         if not rgb_format:
                             try:
-                                _ = int(format)
+                                int_value = int(format)
+                                # 0 should never be used because it will mess with internal assumptions
+                                # Negative values are invalid
+                                if int_value <= 0:
+                                    raise ValueError(f'Invalid value [{int_value}]; must be greater than 0')
                             except ValueError:
                                 raise ValueError(
                                     'AnsiString.__format__ failed to parse format ({}); invalid name: {}'
                                     .format(ansi_format, format)
                                 )
                             else:
                                 # Value is an integer - use the format verbatim
                                 format_settings_strs.append(format)
                         else:
                             format_settings_strs.append(rgb_format)
-                return ';'.join(format_settings_strs)
+                return format_settings_strs
 
-        def __str__(self):
-            return self._str
+        def insert_setting(self, apply:bool, setting:'AnsiString.Setting', topmost:bool=True):
+            lst = self.add if apply else self.rem
+            if topmost:
+                lst.append(setting)
+            else:
+                lst.insert(0, setting)
 
-    def __init__(self, s:str='', setting_or_settings:Union[List[str], str, List[AnsiFormat], AnsiFormat]=None):
+        def insert_settings(
+            self,
+            apply:bool,
+            settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiString.Setting'], 'AnsiString.Setting'],
+            topmost:bool=True
+        ) -> List['AnsiString.Setting']:
+            if not isinstance(settings, list) and not isinstance(settings, tuple):
+                settings = [settings]
+
+            settings_to_insert = []
+            for setting in settings:
+                if isinstance(setting, AnsiString.Setting):
+                    settings_to_insert.append(setting)
+                elif isinstance(setting, str) or isinstance(setting, int):
+                    settings_to_insert.extend([AnsiString.Setting(s) for s in __class__._scrub_ansi_format_string(str(setting))])
+                elif hasattr(setting, "value") and isinstance(setting.value, str):
+                    settings_to_insert.append(AnsiString.Setting(setting.value))
+
+            lst = self.add if apply else self.rem
+            if topmost:
+                lst.extend(settings_to_insert)
+            else:
+                lst[:0] = settings_to_insert
+
+            return settings_to_insert
+
+    def __init__(self, s:str='', *setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat]):
         self._s = s
         # Key is the string index to make a color change at
         # Each value element is a list of 2 lists
         #   index 0: the settings to apply at this string index
         #   index 1: the settings to remove at this string index
-        self._color_settings = {}
-        if setting_or_settings:
-            self.apply_formatting(setting_or_settings)
+        # TODO: it likely makes sense to create a separate class to maintain setting lists. This map of lists gets
+        #       really difficult to read!
+        self._fmts:Dict[int,'AnsiString.SettingPoint'] = {}
+
+        # Unpack settings
+        settings = []
+        for sos in setting_or_settings:
+            if not isinstance(sos, list) and not isinstance(sos, tuple):
+                settings.append(sos)
+            else:
+                settings += sos
 
-    def assign_str(self, s):
+        if settings:
+            self.apply_formatting(settings)
+
+    def assign_str(self, s:str):
         '''
-        Assigns the base string.
+        Assigns the base string and adjusts the ANSI settings based on the new length.
         '''
+        if len(s) > len(self._s):
+            if len(self._s) in self._fmts:
+                self._fmts[len(s)] = self._fmts.pop(len(self._s))
+        elif len(s) < len(self._s):
+            # This may erase some settings that will no longer apply
+            self.clip(end=len(s), inplace=True)
         self._s = s
 
     @property
     def base_str(self) -> str:
         '''
         Returns the base string without any formatting set.
         '''
         return self._s
 
-    def copy(self):
+    def copy(self) -> 'AnsiString':
         return self[:]
 
     @staticmethod
-    def _insert_settings_to_dict(settings_dict:dict, idx:int, apply:bool, settings:Settings, topmost:bool=True):
-        if idx not in settings_dict:
-            settings_dict[idx] = [[] for _ in range(__class__.SETTINGS_ITEM_LIST_LEN)]
-        list_idx = __class__.SETTINGS_APPLY_IDX if apply else __class__.SETTINGS_REMOVE_IDX
-        if topmost:
-            settings_dict[idx][list_idx].append(settings)
-        else:
-            settings_dict[idx][list_idx].insert(0, settings)
-
-    @staticmethod
-    def _shift_settings_idx(settings_dict:dict, num:int, keep_origin:bool):
+    def _shift_settings_idx(settings_dict:Dict[int,'AnsiString.SettingPoint'], num:int, keep_origin:bool):
         '''
         Not fully supported for when num is negative
         '''
         for key in sorted(settings_dict.keys(), reverse=(num > 0)):
             if not keep_origin or key != 0:
                 new_key = max(key + num, 0)
                 # new_key could be negative when num is negative - TODO: either handle or raise exception
                 settings_dict[new_key] = settings_dict.pop(key)
 
-    def _insert_settings(self, idx:int, apply:bool, settings:Settings, topmost:bool=True):
-        __class__._insert_settings_to_dict(self._color_settings, idx, apply, settings, topmost)
+    def _insert_settings(
+        self,
+        idx:int,
+        apply:bool,
+        settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiString.Setting'], 'AnsiString.Setting'],
+        topmost:bool=True
+    ) -> List['AnsiString.Setting']:
+        if idx not in self._fmts:
+            self._fmts[idx] = __class__.SettingPoint()
+        return self._fmts[idx].insert_settings(apply, settings, topmost)
 
     def apply_formatting(
             self,
-            setting_or_settings:Union[List[str], str, List[AnsiFormat], AnsiFormat],
+            setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiString.Setting'], 'AnsiString.Setting'],
             start:int=0,
             end:Union[int,None]=None,
-            topmost=True
+            topmost:bool=True
     ):
         '''
         Sets the formatting for a given range of characters.
         Inputs: setting_or_settings - Can either be a single item or list of items;
                                       each item can either be a string or AnsiFormat type
                 start - The string start index where setting(s) are to be applied
                 end - The string index where the setting(s) should be removed
                 topmost - When true, this setting is placed at the end of the set for the given
                         start_index meaning it is applied last; when false, setting is applied first
 
         Note: The desired effect may not be achieved if the same setting is applied over an
               overlapping range of characters.
         '''
-        if not setting_or_settings or start >= len(self._s):
+        start = self._slice_val_to_idx(start, 0)
+        end = self._slice_val_to_idx(end, len(self._s))
+
+        if not setting_or_settings or start >= len(self._s) or end <= start:
             # Ignore - nothing to apply
             return
 
-        if end is None:
-            end = len(self._s)
-
-        settings = __class__.Settings(setting_or_settings)
-
         # Apply settings
-        self._insert_settings(start, True, settings, topmost)
+        inserted_settings = self._insert_settings(start, True, setting_or_settings, topmost)
 
         # Remove settings
-        self._insert_settings(end, False, settings, topmost)
+        self._insert_settings(end, False, inserted_settings, topmost)
 
     def apply_formatting_for_match(
             self,
             setting_or_settings:Union[List[str], str, List[AnsiFormat], AnsiFormat],
             match_object,
             group:int=0
     ):
@@ -1005,53 +1069,89 @@
         e = match_object.end(group)
         self.apply_formatting(setting_or_settings, s, e)
 
     def clear_formatting(self):
         '''
         Clears all internal formatting.
         '''
-        self._color_settings = {}
+        self._fmts = {}
+
+    @staticmethod
+    def _find_setting_reference(find:Setting, in_list:List[Setting]) -> int:
+        for i, s in enumerate(in_list):
+            if s is find:
+                return i
+        return -1
+
+    @staticmethod
+    def _find_settings_references(find_list:List[Setting], in_list:List[Setting]) -> List[Tuple]:
+        matches = []
+        for i, s in enumerate(find_list):
+            for i2, s2 in enumerate(in_list):
+                if s is s2:
+                    matches.append((i, i2))
+        return matches
 
     class SettingsIterator:
-        def __init__(self, settings_dict:dict):
-            self.settings_dict = settings_dict
-            self.current_settings = []
+        def __init__(self, settings_dict:Dict[int,'AnsiString.SettingPoint']):
+            self.settings_dict:Dict[int,AnsiString.SettingPoint] = settings_dict
+            self.current_settings:List[AnsiString.Setting] = []
             self.dict_iter = iter(sorted(self.settings_dict))
 
         def __iter__(self):
             return self
 
-        def __next__(self) -> tuple:
+        def __next__(self) -> Tuple[int,'AnsiString.SettingPoint',List['AnsiString.Setting']]:
             # Will raise StopIteration when complete
             idx = next(self.dict_iter)
             settings = self.settings_dict[idx]
             # Remove settings that it is time to remove
-            for setting in settings[AnsiString.SETTINGS_REMOVE_IDX]:
+            for setting in settings.rem:
                 # setting object will only be matched and removed if it is the same reference to one
                 # previously added - will raise exception otherwise which should not happen if the
                 # settings dictionary and this method were setup correctly.
-                self.current_settings.remove(setting)
+                remove_idx = AnsiString._find_setting_reference(setting, self.current_settings)
+                if remove_idx >= 0:
+                    del self.current_settings[remove_idx]
+                else:
+                    raise ValueError('could not remove setting: not in list')
             # Apply settings that it is time to add
-            self.current_settings += settings[AnsiString.SETTINGS_APPLY_IDX]
+            self.current_settings += settings.add
             return (idx, settings, self.current_settings)
 
+    class CharIterator:
+        def __init__(self, s:'AnsiString'):
+            self.current_idx:int = -1
+            self.s:AnsiString = s
+
+        def __iter__(self):
+            return self
+
+        def __next__(self) -> 'AnsiString':
+            self.current_idx += 1
+            if self.current_idx >= len(self.s):
+                raise StopIteration
+            return self.s[self.current_idx]
+
     def _slice_val_to_idx(self, val:int, default:int) -> int:
         if val is None:
             return default
         elif val < 0:
             ret_val = len(self._s) + val
             if ret_val < 0:
                 ret_val = 0
             return ret_val
         else:
             return val
 
-    def __getitem__(self, val:Union[int, slice]):
+    def __getitem__(self, val:Union[int, slice]) -> 'AnsiString':
         '''
-        Returns a new AnsiString object which represents a substring of self
+        Returns a new AnsiString object which represents a substring of self.
+        Note: the new copy may contain some references to settings in the origin. This is ok since the value of each
+              setting is not internally modified after creation.
         '''
         if isinstance(val, int):
             st = val
             en = val + 1
         elif isinstance(val, slice):
             if val.step is not None and val.step != 1:
                 raise ValueError('Step other than 1 not supported')
@@ -1062,50 +1162,61 @@
 
         new_s = AnsiString(self._s[val])
 
         if not new_s._s:
             # Special case - string is now empty
             return new_s
 
-        last_settings = []
+        # String cannot be empty from this point on, so that will be assumed going forward
+
+        previous_settings = None
         settings_initialized = False
-        for idx, settings, current_settings in __class__.SettingsIterator(self._color_settings):
+        for idx, settings, current_settings in __class__.SettingsIterator(self._fmts):
             if idx > len(self._s) or idx > en:
-                if not settings_initialized and len(new_s) > 0 and last_settings:
-                    # Substring was between settings
-                    new_s._color_settings[0] = [last_settings, []]
-                # Because this class supports concatenation, it's necessary to remove all settings before ending
-                if last_settings:
-                    new_len = len(new_s._s)
-                    if new_len in new_s._color_settings:
-                        new_s._color_settings[new_len][1].extend(last_settings)
-                    else:
-                        new_s._color_settings[new_len] = [[], last_settings]
                 # Complete
                 break
-            if idx == st:
+            elif idx == en:
+                if settings.rem:
+                    new_s._fmts[idx - st] = __class__.SettingPoint(rem=list(settings.rem))
+                # Complete
+                break
+            elif idx == st:
                 if current_settings:
-                    new_s._color_settings[0] = [list(current_settings), []]
+                    new_s._fmts[0] = __class__.SettingPoint(add=list(current_settings))
                 settings_initialized = True
             elif idx > st:
-                if not settings_initialized and idx - st != 0 and last_settings:
-                    new_s._color_settings[0] = [last_settings, []]
-                    settings_initialized = True
-                new_s._color_settings[idx - st] = [list(settings[0]), list(settings[1])]
-            # It's unfortunately necessary to copy since current_settings ref will change
-            last_settings = list(current_settings)
+                if not settings_initialized and previous_settings:
+                    new_s._fmts[0] = __class__.SettingPoint(add=previous_settings)
+                settings_initialized = True
+                new_s._fmts[idx - st] = __class__.SettingPoint(settings.add, settings.rem)
+
+            # It's necessary to copy (i.e. call list()) since current_settings ref will change on next loop
+            previous_settings = list(current_settings)
+
+        if not settings_initialized and previous_settings:
+            # Substring was between settings
+            new_s._fmts[0] = __class__.SettingPoint(add=previous_settings)
+
+        # Because this class supports concatenation, it's necessary to remove all settings before ending
+        if previous_settings:
+            new_len = len(new_s._s)
+            if new_len not in new_s._fmts:
+                new_s._fmts[new_len] = __class__.SettingPoint()
+            settings_to_remove = [s for s in previous_settings if s not in new_s._fmts[new_len].rem]
+            new_s._fmts[new_len].rem.extend(settings_to_remove)
+
         return new_s
 
     def __str__(self) -> str:
         '''
         Returns an ANSI format string with only internal formatting set.
         '''
         return self.__format__(None)
 
-    def _apply_string_format(self, string_format):
+    def _apply_string_format(self, string_format:str):
         match = re.search(r'^(.?)<([0-9]*)$', string_format)
         if match:
             # Left justify
             num = match.group(2)
             if num:
                 self.ljust(int(num), match.group(1) or ' ', inplace=True)
             return
@@ -1141,15 +1252,15 @@
         '''
         Returns an ANSI format string with both internal and given formatting spec set.
         __format_spec: must be in the format "[string_format][:ansi_format]" where string_format is the standard
                        string format specifier and ansi_format contains 0 or more ansi directives separated by
                        semicolons (;)
                        ex: ">10:bold;fg_red" to make output right justify with width of 10, bold and red formatting
         '''
-        if not __format_spec and not self._color_settings:
+        if not __format_spec and not self._fmts:
             # No formatting
             return self._s
 
         if __format_spec:
             # Make a copy
             obj = self.copy()
 
@@ -1165,51 +1276,54 @@
         else:
             # No changes - just copy the reference
             obj = self
 
         out_str = ''
         last_idx = 0
         clear_needed = False
-        for idx, settings, current_settings in __class__.SettingsIterator(obj._color_settings):
+        for idx, settings, current_settings in __class__.SettingsIterator(obj._fmts):
             if idx >= len(obj):
                 # Invalid
                 break
             # Catch up output to current index
             out_str += obj._s[last_idx:idx]
             last_idx = idx
 
             settings_to_apply = [str(s) for s in current_settings]
-            if settings[__class__.SETTINGS_REMOVE_IDX] and settings_to_apply:
+            if settings.rem and settings_to_apply:
                 # Settings were removed and there are settings to be applied -
                 # need to reset before applying current settings
-                settings_to_apply = [AnsiFormat.RESET.value] + settings_to_apply
+                settings_to_apply = [__class__.RESET] + settings_to_apply
             # Apply these settings
             out_str += __class__.ANSI_ESCAPE_FORMAT.format(';'.join(settings_to_apply))
             # Save this flag in case this is the last loop
             clear_needed = bool(current_settings)
 
         # Final catch up
         out_str += obj._s[last_idx:]
         if clear_needed:
             # Clear settings
             out_str += __class__.ANSI_ESCAPE_CLEAR
 
         return out_str
 
-    def capitalize(self):
+    def __iter__(self):
+        return iter(__class__.CharIterator(self))
+
+    def capitalize(self) -> 'AnsiString':
         cpy = self.copy()
         cpy._s = cpy._s.capitalize()
         return cpy
 
-    def casefold(self):
+    def casefold(self) -> 'AnsiString':
         cpy = self.copy()
         cpy._s = cpy._s.casefold()
         return cpy
 
-    def center(self, width:int, fillchar:str=' ', inplace:bool=False):
+    def center(self, width:int, fillchar:str=' ', inplace:bool=False) -> 'AnsiString':
         '''
         Center justification.
         inplace: True to execute in-place; False to return a copy
         '''
         if inplace:
             obj = self
         else:
@@ -1218,73 +1332,71 @@
         old_len = len(obj._s)
         num = width - old_len
         if num > 0:
             left_spaces = math.floor((num) / 2)
             right_spaces = num - left_spaces
             obj._s = fillchar * left_spaces + obj._s + fillchar * right_spaces
             # Move the removal settings from previous end to new end (formats the right fillchars with same as last char)
-            if old_len in obj._color_settings:
-                obj._color_settings[len(obj._s)] = obj._color_settings.pop(old_len)
+            if old_len in obj._fmts:
+                obj._fmts[len(obj._s)] = obj._fmts.pop(old_len)
             # Shift all indices except for the origin (formats the left fillchars with same as first char)
-            __class__._shift_settings_idx(obj._color_settings, left_spaces, True)
+            __class__._shift_settings_idx(obj._fmts, left_spaces, True)
 
         return obj
 
-    def ljust(self, width:int, fillchar:str=' ', inplace:bool=False):
+    def ljust(self, width:int, fillchar:str=' ', inplace:bool=False) -> 'AnsiString':
         '''
         Left justification.
         inplace: True to execute in-place; False to return a copy
         '''
         if inplace:
             obj = self
         else:
             obj = self.copy()
 
         old_len = len(obj._s)
         num = width - old_len
         if num > 0:
             obj._s += fillchar * num
             # Move the removal settings from previous end to new end (formats the right fillchars with same as last char)
-            if old_len in obj._color_settings:
-                obj._color_settings[len(obj._s)] = obj._color_settings.pop(old_len)
+            if old_len in obj._fmts:
+                obj._fmts[len(obj._s)] = obj._fmts.pop(old_len)
 
         return obj
 
-    def rjust(self, width:int, fillchar:str=' ', inplace:bool=False):
+    def rjust(self, width:int, fillchar:str=' ', inplace:bool=False) -> 'AnsiString':
         '''
         Right justification.
         inplace: True to execute in-place; False to return a copy
         '''
         if inplace:
             obj = self
         else:
             obj = self.copy()
 
         old_len = len(obj._s)
         num = width - old_len
         if num > 0:
             obj._s = fillchar * num + obj._s
             # Shift all indices except for the origin (formats the left fillchars with same as first char)
-            __class__._shift_settings_idx(obj._color_settings, num, True)
+            __class__._shift_settings_idx(obj._fmts, num, True)
 
         return obj
 
     def count(self, sub:str, start:int, end:int) -> int:
         return self._s.count(sub, start, end)
 
     def encode(self, encoding:str="utf-8", errors:str="strict") -> bytes:
         return str(self).encode(encoding, errors)
 
     def endswith(self, suffix:str, start:int=None, end:int=None) -> bool:
         return self._s.endswith(suffix, start, end)
 
-    def expandtabs(self, tabsize:int=8):
-        cpy = self.copy()
-        cpy._s = cpy._s.expandtabs(tabsize)
-        return cpy
+    def expandtabs(self, tabsize:int=8, inplace:bool=False) -> 'AnsiString':
+        return self.replace('\t', ' ' * tabsize, inplace=inplace)
 
     def find(self, sub:str, start:int=None, end:int=None) -> int:
         return self._s.find(sub, start, end)
 
     def index(self, sub:str, start:int=None, end:int=None) -> int:
         return self._s.index(sub, start, end)
 
@@ -1320,117 +1432,157 @@
 
     def istitle(self) -> bool:
         return self._s.istitle()
 
     def isupper(self) -> bool:
         return self._s.isupper()
 
-    def __add__(self, value):
+    def __add__(self, value:Union[str,'AnsiString']) -> 'AnsiString':
         cpy = self.copy()
         cpy += value
         return cpy
 
-    def __iadd__(self, value):
+    def __iadd__(self, value:Union[str,'AnsiString']) -> 'AnsiString':
         if isinstance(value, str):
             self._s += value
         elif isinstance(value, AnsiString):
-            value_cpy = value.copy()
-            settings_cpy = value_cpy._color_settings
-            __class__._shift_settings_idx(settings_cpy, len(self._s), False)
+            shift = len(self._s)
             self._s += value._s
-            for key, value in settings_cpy.items():
-                if key in self._color_settings:
-                    self._color_settings[key][0].extend(value[0])
-                    self._color_settings[key][1].extend(value[1])
+            find_settings = []
+            replace_settings = []
+            for key, settings in value._fmts.items():
+                key += shift
+                if key in self._fmts:
+                    if (
+                        key == shift
+                        and settings.add
+                        and self._fmts[key].rem[:len(settings.add)] == settings.add
+                    ):
+                        # Special case - the string being added contains same formatting as end of my string.
+                        # Because the settings work based on references instead of values, the settings not only
+                        # need to be removed here but changed where they are removed in the added string.
+                        find_settings = settings.add
+                        replace_settings = self._fmts[key].rem[:len(settings.add)]
+                        self._fmts[key].rem = self._fmts[key].rem[len(settings.add):]
+                        settings.add = []
+                        if not self._fmts[key] and not settings:
+                            del self._fmts[key]
+                            continue
+
+                    self._fmts[key].add.extend(settings.add)
+                    self._fmts[key].rem.extend(settings.rem)
+
                 else:
-                    self._color_settings[key] = value
+                    self._fmts[key] = __class__.SettingPoint(list(settings.add), list(settings.rem))
+
+                    finds = __class__._find_settings_references(find_settings, settings.rem)
+                    if finds:
+                        for find_idx, add_idx in reversed(finds):
+                            self._fmts[key].rem[add_idx] = replace_settings[find_idx]
+                            # Note: find_idx will always be sorted in ascending order and this is iterating in reverse
+                            del find_settings[find_idx]
+                            del replace_settings[find_idx]
+
         else:
             raise ValueError(f'value is invalid type: {type(value)}')
         return self
 
-    def __eq__(self, value) -> bool:
+    def __eq__(self, value:'AnsiString') -> bool:
         if not isinstance(value, AnsiString):
             return False
-        return self._s == value._s and self._color_settings == value._color_settings
+        return self._s == value._s and self._fmts == value._fmts
 
-    def __contains__(self, value) -> bool:
+    def __contains__(self, value:Union[str,'AnsiString',Any]) -> bool:
         if isinstance(value, str):
             return value in self._s
         elif isinstance(value, AnsiString):
             return value._s in self._s
         return False
 
     def __len__(self) -> int:
         return len(self._s)
 
     @staticmethod
-    def join(*args):
+    def join(*args:Union[str,'AnsiString']) -> 'AnsiString':
         if not args:
             return AnsiString()
         args = list(args)
         first_arg = args[0]
         if isinstance(first_arg, str):
             joint = AnsiString(first_arg)
         elif isinstance(first_arg, AnsiString):
             joint = first_arg.copy()
         else:
             raise ValueError(f'value is invalid type: {type(first_arg)}')
         for arg in args[1:]:
             joint += arg
         return joint
 
-    def lower(self, inplace:bool=False):
+    def lower(self, inplace:bool=False) -> 'AnsiString':
         '''
         Convert to lowercase.
         inplace: True to execute in-place; False to return a copy
         '''
         if inplace:
             obj = self
         else:
             obj = self.copy()
         obj._s = obj._s.lower()
         return obj
 
-    def upper(self, inplace:bool=False):
+    def upper(self, inplace:bool=False) -> 'AnsiString':
         '''
         Convert to uppercase.
         inplace: True to execute in-place; False to return a copy
         '''
         if inplace:
             obj = self
         else:
             obj = self.copy()
         obj._s = obj._s.lower()
         return obj
 
-    def lstrip(self, chars:str=None, inplace:bool=False):
+    def lstrip(self, chars:str=None, inplace:bool=False) -> 'AnsiString':
         '''
         Remove leading whitespace
         chars: If not None, remove characters in chars instead
         inplace: True to execute in-place; False to return a copy
         '''
         return self._strip(chars=chars, inplace=inplace, do_lstrip=True, do_rstrip=False)
 
-    def rstrip(self, chars:str=None, inplace:bool=False):
+    def clip(self, start:int=None, end:int=None, inplace:bool=False) -> 'AnsiString':
+        '''
+        Calls [] operator and optionally assigns in-place
+        '''
+        obj = self[start:end]
+        if inplace:
+            self._s = obj._s
+            self._fmts = obj._fmts
+            del obj
+            return self
+        else:
+            return obj
+
+    def rstrip(self, chars:str=None, inplace:bool=False) -> 'AnsiString':
         '''
         Remove trailing whitespace
         chars: If not None, remove characters in chars instead
         inplace: True to execute in-place; False to return a copy
         '''
         return self._strip(chars=chars, inplace=inplace, do_lstrip=False, do_rstrip=True)
 
-    def strip(self, chars:str=None, inplace:bool=False):
+    def strip(self, chars:str=None, inplace:bool=False) -> 'AnsiString':
         '''
         Remove leading and trailing whitespace
         chars: If not None, remove characters in chars instead
         inplace: True to execute in-place; False to return a copy
         '''
         return self._strip(chars=chars, inplace=inplace, do_lstrip=True, do_rstrip=True)
 
-    def _strip(self, chars:str=None, inplace:bool=False, do_lstrip:bool=True, do_rstrip:bool=True):
+    def _strip(self, chars:str=None, inplace:bool=False, do_lstrip:bool=True, do_rstrip:bool=True) -> 'AnsiString':
         '''
         Remove leading and trailing whitespace
         chars: If not None, remove characters in chars instead
         inplace: True to execute in-place; False to return a copy
         '''
         if chars is None:
             chars = WHITESPACE_CHARS
@@ -1454,15 +1606,158 @@
             if rcount == 0:
                 rcount = None
 
         if inplace and lcount == 0 and rcount is None:
             return self
 
         # This is always going to create a copy - no good way to modify settings while iterating over it
-        obj = self[lcount:rcount]
+        return self.clip(lcount, rcount, inplace)
+
+    def partition(self, sep:str) -> Tuple['AnsiString','AnsiString','AnsiString']:
+        '''
+        Partition the string into three parts using the given separator.
+
+        This will search for the separator in the string. If the separator is found, returns a 3-tuple containing the
+        part before the separator, the separator itself, and the part after it.
+
+        If the separator is not found, returns a 3-tuple containing the original string and two empty strings.
+        '''
+        idx = self._s.find(sep)
+        if idx >= 0:
+            sep_len = len(sep)
+            idx_end = idx + sep_len
+            return (self[0:idx], self[idx:idx_end], self[idx_end:])
+        else:
+            return (self.copy(), AnsiString(), AnsiString())
+
+    def rpartition(self, sep:str) -> Tuple['AnsiString','AnsiString','AnsiString']:
+        '''
+        Partition the string into three parts using the given separator, searching from right to left.
+
+        This will search for the separator in the string. If the separator is found, returns a 3-tuple containing the
+        part before the separator, the separator itself, and the part after it.
+
+        If the separator is not found, returns a 3-tuple containing the original string and two empty strings.
+        '''
+        idx = self._s.rfind(sep)
+        if idx >= 0:
+            sep_len = len(sep)
+            idx_end = idx + sep_len
+            return (self[0:idx], self[idx:idx_end], self[idx_end:])
+        else:
+            return (self.copy(), AnsiString(), AnsiString())
+
+    def settings_at(self, idx:int) -> str:
+        '''
+        Returns a string which represents the settings being used at the given index
+        '''
+        if idx >= 0 and idx < len(self._s):
+            previous_settings = []
+            for sidx, _, current_settings in __class__.SettingsIterator(self._fmts):
+                if sidx > idx:
+                    break
+                previous_settings = list(current_settings)
+            return ';'.join(str(s) for s in previous_settings)
+        else:
+            return ''
+
+    def removeprefix(self, prefix:str, inplace:bool=False) -> 'AnsiString':
+        if not self._s.startswith(prefix):
+            if inplace:
+                return self
+            else:
+                return self.copy()
+        else:
+            return self.clip(start=len(prefix), inplace=inplace)
+
+    def removesuffix(self, suffix:str, inplace:bool=False) -> 'AnsiString':
+        if not self._s.endswith(suffix):
+            if inplace:
+                return self
+            else:
+                return self.copy()
+        else:
+            return self.clip(end=-len(suffix), inplace=inplace)
+
+    def replace(self, old:str, new:Union[str,'AnsiString'], count:int=-1, inplace:bool=False) -> 'AnsiString':
+        obj = self
+        idx = self._s.find(old)
+        while (count < 0 or count > 0) and idx >= 0:
+            obj = self[:idx] + new + self[idx+len(new):]
+            if count > 0:
+                count -= 1
+            idx = self._s.find(old, idx + len(old))
 
         if inplace:
             self._s = obj._s
-            self._color_settings = obj._color_settings
+            self._fmts = obj._fmts
             return self
         else:
             return obj
+
+    def rfind(self, sub:str, start:int=None, end:int=None) -> int:
+        return self._s.rfind(sub, start, end)
+
+    def rindex(self, sub:str, start:int=None, end:int=None) -> int:
+        return self._s.rindex(sub, start, end)
+
+    def _split(self, sep:Union[str,None]=None, maxsplit:int=-1, r:bool=False) -> List['AnsiString']:
+        if r:
+            str_splits = self._s.rsplit(sep, maxsplit)
+        else:
+            str_splits = self._s.split(sep, maxsplit)
+        split_idx_len = []
+        idx = 0
+        for s in str_splits:
+            idx = self._s.find(s, idx)
+            split_idx_len.append((idx, len(s)))
+            idx += len(s)
+
+        ansi_str_splits = []
+        for idx, length in split_idx_len:
+            ansi_str_splits.append(self[idx:idx+length])
+
+        return ansi_str_splits
+
+    def split(self, sep:Union[str,None]=None, maxsplit:int=-1) -> List['AnsiString']:
+        return self._split(sep, maxsplit, False)
+
+    def rsplit(self, sep:Union[str,None]=None, maxsplit:int=-1) -> List['AnsiString']:
+        return self._split(sep, maxsplit, True)
+
+    def splitlines(self, keepends:bool=False) -> List['AnsiString']:
+        str_splits = self._s.splitlines(keepends)
+        split_idx_len = []
+        idx = 0
+        for s in str_splits:
+            idx = self._s.find(s, idx)
+            split_idx_len.append((idx, len(s)))
+            idx += len(s)
+
+        ansi_str_splits = []
+        for idx, length in split_idx_len:
+            ansi_str_splits.append(self[idx:idx+length])
+
+        return ansi_str_splits
+
+    def swapcase(self, inplace:bool=False) -> 'AnsiString':
+        if inplace:
+            obj = self
+        else:
+            obj = self.copy()
+
+        obj._s = obj._s.swapcase()
+
+        return obj
+
+    def title(self, inplace:bool=False) -> 'AnsiString':
+        if inplace:
+            obj = self
+        else:
+            obj = self.copy()
+
+        obj._s = obj._s.title()
+
+        return obj
+
+    def zfill(self, width:int, inplace:bool=False) -> 'AnsiString':
+        return self.rjust(width, "0", inplace)
```

