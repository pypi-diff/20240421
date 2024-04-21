# Comparing `tmp/psp_liquids_daq_parser-0.0.6.tar.gz` & `tmp/psp_liquids_daq_parser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psp_liquids_daq_parser-0.0.6.tar", last modified: Tue Apr  9 07:42:17 2024, max compression
+gzip compressed data, was "psp_liquids_daq_parser-0.0.7.tar", last modified: Sun Apr 21 05:21:47 2024, max compression
```

## Comparing `psp_liquids_daq_parser-0.0.6.tar` & `psp_liquids_daq_parser-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:42:17.835251 psp_liquids_daq_parser-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35821 2024-04-09 07:42:11.000000 psp_liquids_daq_parser-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-04-09 07:42:17.835251 psp_liquids_daq_parser-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8269 2024-04-09 07:42:11.000000 psp_liquids_daq_parser-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-09 07:42:11.000000 psp_liquids_daq_parser-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:42:17.835251 psp_liquids_daq_parser-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:42:17.831251 psp_liquids_daq_parser-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 07:42:15.000000 psp_liquids_daq_parser-0.0.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-09 07:42:11.000000 psp_liquids_daq_parser-0.0.6/src/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-09 07:42:11.000000 psp_liquids_daq_parser-0.0.6/src/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:42:17.835251 psp_liquids_daq_parser-0.0.6/src/psp_liquids_daq_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-04-09 07:42:17.000000 psp_liquids_daq_parser-0.0.6/src/psp_liquids_daq_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-09 07:42:17.000000 psp_liquids_daq_parser-0.0.6/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:42:17.000000 psp_liquids_daq_parser-0.0.6/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 07:42:17.000000 psp_liquids_daq_parser-0.0.6/src/psp_liquids_daq_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 07:42:17.000000 psp_liquids_daq_parser-0.0.6/src/psp_liquids_daq_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-09 07:42:11.000000 psp_liquids_daq_parser-0.0.6/src/psp_liquids_daq_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:21:47.303653 psp_liquids_daq_parser-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35821 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-21 05:21:47.303653 psp_liquids_daq_parser-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 05:21:47.303653 psp_liquids_daq_parser-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:21:47.303653 psp_liquids_daq_parser-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 05:21:45.000000 psp_liquids_daq_parser-0.0.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/src/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/src/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/src/plotly_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:21:47.303653 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-21 05:21:47.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-21 05:21:47.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 05:21:47.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-21 05:21:47.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-21 05:21:47.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.py
```

### Comparing `psp_liquids_daq_parser-0.0.6/LICENSE` & `psp_liquids_daq_parser-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.6/PKG-INFO` & `psp_liquids_daq_parser-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psp_liquids_daq_parser
-Version: 0.0.6
+Version: 0.0.7
 Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
 Author-email: Rajan Phadnis <rajansd28@gmail.com>
 Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
 Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,18 @@
 
 ## Use
 
 There are two functions and two classes that come with this package:
 
 ### Function: `parseTDMS`:
 
+`start_time_unix_ms` defines the start time of the TDMS file in milliseconds since the UNIX epoch. This is a required argument, and offsets the TDMS time data with the given start time converted to seconds.
+
 If `file_path_custom` isn't specified, the file picker dialog comes up to select a tdms file. Then, we check to see if there's an equivalent pickle file in the same directory as the chosen tdms file.
+
 If there's a pickle file, we parse that. Otherwise, we parse the TDMS file and save the resulting object to a pickle file for later.
 
 ### Function: `extendDatasets`
 
 Basically makes all the datasets of all the channel the same length. Uses the numpy "edge" method for the time dataset. Uses constant values for channel data (o for analog data, 0.5 for binary data)
 
 For example, if you had:
```

### Comparing `psp_liquids_daq_parser-0.0.6/README.md` & `psp_liquids_daq_parser-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 
 ## Use
 
 There are two functions and two classes that come with this package:
 
 ### Function: `parseTDMS`:
 
+`start_time_unix_ms` defines the start time of the TDMS file in milliseconds since the UNIX epoch. This is a required argument, and offsets the TDMS time data with the given start time converted to seconds.
+
 If `file_path_custom` isn't specified, the file picker dialog comes up to select a tdms file. Then, we check to see if there's an equivalent pickle file in the same directory as the chosen tdms file.
+
 If there's a pickle file, we parse that. Otherwise, we parse the TDMS file and save the resulting object to a pickle file for later.
 
 ### Function: `extendDatasets`
 
 Basically makes all the datasets of all the channel the same length. Uses the numpy "edge" method for the time dataset. Uses constant values for channel data (o for analog data, 0.5 for binary data)
 
 For example, if you had:
```

### Comparing `psp_liquids_daq_parser-0.0.6/pyproject.toml` & `psp_liquids_daq_parser-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.6/src/classes.py` & `psp_liquids_daq_parser-0.0.7/src/classes.py`

 * *Files 9% similar despite different names*

```diff
@@ -126,7 +126,23 @@
     @property
     def min_v(self) -> float:
         return self._min_v
 
     @property
     def max_v(self) -> float:
         return self._max_v
+
+class SensorNetData:
+    def __init__(self, name: str, rawTime: NDArray[float64], rawData: NDArray[float64]):
+        self._rawData = rawData
+        self._name = name
+        self._rawTime = rawTime
+    @property
+    def data(self) -> NDArray[float64]:
+        return self._rawData
+    @property
+    def time(self) -> NDArray[float64]:
+        return self._rawTime
+    @property
+    def name(self) -> str:
+        return self._name
+
```

### Comparing `psp_liquids_daq_parser-0.0.6/src/helpers.py` & `psp_liquids_daq_parser-0.0.7/src/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,16 +43,17 @@
             toReturn_DI[channel_data_obj.name] = channel_data_obj
 
         print("parsed " + channel_data_obj.name + " as " + parsed_as)
     return (toReturn_AI, toReturn_DI)
 
 
 def getTime(
-    channel_data: dict[str, AnalogChannelData | DigitalChannelData], group_name: str
+    channel_data: dict[str, AnalogChannelData | DigitalChannelData], group_name: str, start_time_unix_ms: int
 ) -> list[float]:
     samples: int = channel_data[next(iter(channel_data))].rawData.size
     pattern: str = r"\(([^()]+)\)"
     match: re.Match = re.search(pattern, group_name)
     sample_rate: float = float(match.group(1)[:-3])
     dt: float = 1 / sample_rate
-    time: list[float] = np.arange(0, samples * dt, dt).tolist()
+    addedtime = np.arange(0, samples * dt, dt) + (start_time_unix_ms/1000)
+    time: list[float] = addedtime.tolist()
     return time
```

### Comparing `psp_liquids_daq_parser-0.0.6/src/psp_liquids_daq_parser.egg-info/PKG-INFO` & `psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psp_liquids_daq_parser
-Version: 0.0.6
+Version: 0.0.7
 Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
 Author-email: Rajan Phadnis <rajansd28@gmail.com>
 Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
 Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,18 @@
 
 ## Use
 
 There are two functions and two classes that come with this package:
 
 ### Function: `parseTDMS`:
 
+`start_time_unix_ms` defines the start time of the TDMS file in milliseconds since the UNIX epoch. This is a required argument, and offsets the TDMS time data with the given start time converted to seconds.
+
 If `file_path_custom` isn't specified, the file picker dialog comes up to select a tdms file. Then, we check to see if there's an equivalent pickle file in the same directory as the chosen tdms file.
+
 If there's a pickle file, we parse that. Otherwise, we parse the TDMS file and save the resulting object to a pickle file for later.
 
 ### Function: `extendDatasets`
 
 Basically makes all the datasets of all the channel the same length. Uses the numpy "edge" method for the time dataset. Uses constant values for channel data (o for analog data, 0.5 for binary data)
 
 For example, if you had:
```

### Comparing `psp_liquids_daq_parser-0.0.6/src/psp_liquids_daq_parser.py` & `psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+from numpy import float64
+from numpy.typing import NDArray
 from nptdms import TdmsFile, TdmsGroup
 import pickle
 import numpy as np
 import tkinter as tk
 from tkinter import filedialog
 import os
-from classes import AnalogChannelData, DigitalChannelData
+
+import pandas as pd
+from classes import AnalogChannelData, DigitalChannelData, SensorNetData
 from helpers import compileChannels, getTime
 
 def parseTDMS(
-    dev_num: int, file_path_custom: str = "", dev_group: str = "Data (1000.000000 Hz)"
-) -> dict[str, AnalogChannelData | DigitalChannelData | list[float]]:
+    dev_num: int, start_time_unix_ms: int, file_path_custom: str = "", dev_group: str = "Data (1000.000000 Hz)"
+) -> dict[str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]]:
     """## Parse a TDMS file (or an equivalent pickle file)
     ### Arguments:
     - `dev_num` (Type: `int`): dev box number (i.e: the `5` or `6` in dev5 or dev6)
+    - `start_time_unix_ms` (Type: `int`): unix timestamp in milliseconds indicating recording start time. Only required if not reading from a pickle file.
     - (Optional) `file_path_custom` (Type: `str`): the dynamic file path to a `.TDMS` file (use this in case you don't want to keep selecting the tdms file to parse every time you run the script)
     - (Optional) `dev_group` (Type: `str`): the TDMS group header. You usually don't have to touch this unless the data isn't high frequency sampling data
     ### Description
     If `file_path_custom` isn't specified, the file picker dialog comes up to select a tdms file. Then, we check to see if there's an equivalent pickle file in the same directory as the chosen tdms file.
     If there's a pickle file, we parse that. Otherwise, we parse the TDMS file and save the resulting object to a pickle file for later.
     """
     if file_path_custom == "":
@@ -31,38 +36,38 @@
     else:
         filepath = file_path_custom
     pickle_filepath: str = filepath[:-5] + ".pickle"
     if os.path.exists(pickle_filepath):
         print("unpickling...")
         with open(pickle_filepath, "rb") as f:
             unpickledData: dict[
-                str, AnalogChannelData | DigitalChannelData | list[float]
+                str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]
             ] = pickle.loads(f.read())
             print("unpickled data")
             return unpickledData
     else:
         channel_data_map: dict[
-            str, AnalogChannelData | DigitalChannelData | list[float]
+            str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]
         ] = {}
         tdms_file: TdmsFile = TdmsFile.read(filepath)
         group: TdmsGroup = tdms_file[dev_group]
         dev5_channels = compileChannels(group.channels())
         channel_data_map.update(dev5_channels[0])
         channel_data_map.update(dev5_channels[1])
-        channel_data_map["time"] = getTime(channel_data_map, dev_group)
+        channel_data_map["time"] = getTime(channel_data_map, dev_group, start_time_unix_ms)
         with open(pickle_filepath, "wb") as f:
             pickle.dump(channel_data_map, f, pickle.HIGHEST_PROTOCOL)
         print(
             f'conversion done!\n\n\nNext time you want to run the converter, consider calling the function with: "parseTDMS({dev_num}, file_path_custom={pickle_filepath[:-7] + ".tdms"})"'
         )
         return channel_data_map
 
 def extendDatasets(
-    channel_data: dict[str, AnalogChannelData | DigitalChannelData | list[float]], binary_channel_prefixes: tuple[str] = ("pi-", "reed-")
-) -> tuple[list[str], dict[str, AnalogChannelData | DigitalChannelData | list[float]]]:
+    channel_data: dict[str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]], binary_channel_prefixes: tuple[str] = ("pi-", "reed-")
+) -> tuple[list[str], dict[str, list[float]]]:
     """## Extend combined datasets
     Basically makes all the datasets of all the channel the same length. Uses the numpy "edge" method for the time dataset. Uses constant values for channel data (o for analog data, 0.5 for binary data)
 
     For example, if you had:
     ```
     {
     "channel1": [0, 1, 2],
@@ -126,7 +131,61 @@
                         "constant",
                         constant_values=(0, 0),
                     )
                 }
             )
 
     return (available_channels, df_list_constant)
+
+def parseCSV(
+    start_time_unix_ms: int, file_path_custom: str = ""
+) -> dict[str, SensorNetData]:
+    """## Parse a CSV file (or an equivalent pickle file)
+    ### Arguments:
+    - `start_time_unix_ms` (Type: `int`): unix timestamp in milliseconds indicating recording start time. Only required if not reading from a pickle file.
+    - (Optional) `file_path_custom` (Type: `str`): the dynamic file path to a `.TDMS` file (use this in case you don't want to keep selecting the tdms file to parse every time you run the script)
+    ### Description
+    If `file_path_custom` isn't specified, the file picker dialog comes up to select a reduced csv file from sensornet. Then, we check to see if there's an equivalent pickle file in the same directory as the chosen csv file.
+    If there's a pickle file, we parse that. Otherwise, we parse the csv file and save the resulting object to a pickle file for later.
+    """
+    if file_path_custom == "":
+        root = tk.Tk()
+        root.withdraw()
+        filepath: str = filedialog.askopenfilename(
+            initialdir="./", title="Choose Reduced Sensornet CSV file"
+        )
+        print(
+            f'to skip the filepicker, use "parseCSV(file_path_custom=\"{filepath}\")"'
+        )
+    else:
+        filepath = file_path_custom
+    pickle_filepath: str = filepath[:-4] + ".pickle"
+    if os.path.exists(pickle_filepath):
+        print("unpickling...")
+        with open(pickle_filepath, "rb") as f:
+            unpickledData: dict[
+                str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]
+            ] = pickle.loads(f.read())
+            print("unpickled data")
+            return unpickledData
+    else:
+        channel_data_map: dict[
+            str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]
+        ] = {}
+
+        df: pd.DataFrame = pd.read_csv(filepath)
+        channel_names: list[str] = df.columns.to_list()
+        df[channel_names] = df[channel_names].astype('float64')
+        for i in range(1,len(channel_names),2):
+            channel: str = channel_names[i]
+            timeArray: NDArray[float64] = df.iloc[:,i-1].to_numpy() + (start_time_unix_ms/1000)
+            dataArray: NDArray[float64] = df.iloc[:,i].to_numpy()
+            channel_data_map[channel] = SensorNetData(channel, timeArray, dataArray)
+
+        # channel_data_map["time"] = getTime(channel_data_map, dev_group)
+        with open(pickle_filepath, "wb") as f:
+            pickle.dump(channel_data_map, f, pickle.HIGHEST_PROTOCOL)
+        print(
+            f'conversion done!\n\n\nNext time you want to run the converter, consider calling the function with: "parseCSV(file_path_custom=\"{pickle_filepath[:-7] + ".tdms"}\")"'
+        )
+        return channel_data_map
+
```

