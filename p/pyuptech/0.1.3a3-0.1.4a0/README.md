# Comparing `tmp/pyuptech-0.1.3a3.tar.gz` & `tmp/pyuptech-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.3a3.tar", last modified: Sat Apr 20 15:56:01 2024, max compression
+gzip compressed data, was "pyuptech-0.1.4a0.tar", last modified: Sun Apr 21 09:30:44 2024, max compression
```

## Comparing `pyuptech-0.1.3a3.tar` & `pyuptech-0.1.4a0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     7052 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/README.md
--rw-r--r--   0        0        0      462 2024-04-20 15:56:01.263247 pyuptech-0.1.3a3/pyproject.toml
--rw-r--r--   0        0        0     1095 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/__init__.py
--rw-r--r--   0        0        0   219512 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/lib/libuptech.so
--rw-r--r--   0        0        0      110 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     1096 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      577 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0     1725 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/pins.py
--rw-r--r--   0        0        0    10454 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0     9833 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0     4912 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/src/pyuptech/tools/display.py
--rw-r--r--   0        0        0        0 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/tests/__init__.py
--rw-r--r--   0        0        0     1105 2024-04-20 15:55:42.335341 pyuptech-0.1.3a3/tests/perf_tests.py
--rw-r--r--   0        0        0     7369 1970-01-01 00:00:00.000000 pyuptech-0.1.3a3/PKG-INFO
+-rw-r--r--   0        0        0     8297 2024-04-21 09:30:25.579958 pyuptech-0.1.4a0/README.md
+-rw-r--r--   0        0        0      547 2024-04-21 09:30:44.336152 pyuptech-0.1.4a0/pyproject.toml
+-rw-r--r--   0        0        0     1280 2024-04-21 09:30:25.579958 pyuptech-0.1.4a0/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0   219512 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/lib/libuptech.so
+-rw-r--r--   0        0        0      110 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     1933 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/emulation.py
+-rw-r--r--   0        0        0     1096 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1761 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    10454 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0    10681 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0     6040 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/src/pyuptech/tools/display.py
+-rw-r--r--   0        0        0      252 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/tests/__init__.py
+-rw-r--r--   0        0        0      386 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/tests/display_tests.py
+-rw-r--r--   0        0        0     1036 2024-04-21 09:30:25.583958 pyuptech-0.1.4a0/tests/perf_tests.py
+-rw-r--r--   0        0        0     8614 1970-01-01 00:00:00.000000 pyuptech-0.1.4a0/PKG-INFO
```

### Comparing `pyuptech-0.1.3a3/README.md` & `pyuptech-0.1.4a0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -49,20 +49,23 @@
 ```python
 from pyuptech import OnBoardSensors
 from ctypes import c_uint8, Array
 
 # 创建OnBoardSensors对象，设置模拟量传感器最小采样间隔为5ms
 sensor_controller = OnBoardSensors(adc_min_sample_interval_ms=5)
 
+# 初始化ADC,设置所有GPIO引脚为输入，设置初始电平为高
+sensor_controller.adc_io_open().set_all_io_mode(0).set_all_io_level(1)
+
 # 设置ADC最小采样间隔为10ms，防止请求堵塞STM32从机
 sensor_controller.adc_min_sample_interval_ms = 10
 
 # 获取所有GPIO引脚当前电平
 gpio_levels: c_uint8 = sensor_controller.io_all_channels()
-print(gpio_levels)
+print(gpio_levels.value)
 
 # 初始化并读取MPU6500加速度数据
 sensor_controller.MPU6500_Open()
 acceleration_data: Array = sensor_controller.acc_all()
 
 # 设置第3号GPIO引脚为输出并设置电平为低
 sensor_controller.set_io_mode(2, 1)
@@ -176,19 +179,23 @@
 
 ## 调试
 
 通过 `tools.display` 可以将传感器数据打印到终端或者主板板载LCD屏幕上
 
 ```python
 from pyuptech import (
+    set_emulation_mode,
     mpu_display_on_lcd,
     mpu_display_on_console,
     adc_io_display_on_lcd,
     adc_io_display_on_console)
 
+# 关闭模拟模式，不关闭将无法进行正常的实机运行
+set_emulation_mode("off")
+
 mpu_display_on_console()  # 将MPU6500数据打印到终端
 
 mpu_display_on_lcd(mode="acc")  # 将MPU6500加速度数据打印到LCD
 
 # 定义ADC标签索引字典，可以空缺部分键值
 adc_labels = {
     6: 'EDGE_FL',
@@ -211,12 +218,46 @@
 }
 
 adc_io_display_on_lcd(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到LCD 
 
 adc_io_display_on_console(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到终端 
 
 
+```
+
+## 使用传感器仿真器
+
+通过 `modules.emulation.SensorEmulator` 可以使用传感器仿真器
+
+```python
+
+# 传感器仿真器导入
+from pyuptech import SensorEmulator
+
+# SensorEmulator 通过继承 OnBoardSensors 类并重写与硬件的交互方法完成的一个仿真器，所以它具有的方法是和OnBoardSensors 基本一致
+# Note: 所有返回的数据都是随机生成的，只是用于演示
+sensor_emulator = SensorEmulator(adc_min_sample_interval_ms=10)
+
+print(sensor_emulator.adc_io_open())
+
+print(list(sensor_emulator.MPU6500_Open().acc_all()))
 
 
 ```
 
+配合 `modules.display` 使用
+
+```python
+from pyuptech import (
+    set_emulation_mode,
+    mpu_display_on_console,
+    adc_io_display_on_console)
+
+# 启动模拟模式，以便打印可以正常使用随机生成的数据进行工作
+set_emulation_mode("on")
+
+mpu_display_on_console()  # 将MPU6500数据打印到终端
+
+adc_io_display_on_console()  # 将ADC和GPIO数据打印到终端
+
+```
```

### Comparing `pyuptech-0.1.3a3/src/pyuptech/__init__.py` & `pyuptech-0.1.4a0/src/pyuptech/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,52 @@
+from .modules.emulation import SensorEmulator
 from .modules.loader import load_lib, TECHSTAR_LIB
 from .modules.logger import set_log_level
 from .modules.pins import (
     pin_setter_constructor,
     pin_getter_constructor,
     pin_mode_setter_constructor,
     multiple_pin_mode_setter_constructor,
     PinGetter,
     PinSetter,
     PinModeSetter,
     IndexedGetter,
     IndexedSetter,
 )
 from .modules.screen import Screen, Color, FontSize
-from .modules.sensors import OnBoardSensors
-
+from .modules.sensors import OnBoardSensors, ADCArrayType, MPUArrayType
 from .tools.display import (
+    set_emulation_mode,
     adc_io_display_on_lcd,
     adc_io_display_on_console,
     mpu_display_on_lcd,
     mpu_display_on_console,
 )
 
 __all__ = [
     "OnBoardSensors",
+    "SensorEmulator",
     "Screen",
     "Color",
     "FontSize",
     "TECHSTAR_LIB",
     "load_lib",
     "set_log_level",
     "pin_getter_constructor",
     "pin_setter_constructor",
     "multiple_pin_mode_setter_constructor",
     "pin_mode_setter_constructor",
     # typing
+    "ADCArrayType",
+    "MPUArrayType",
     "PinGetter",
     "PinSetter",
     "PinModeSetter",
     "IndexedGetter",
     "IndexedSetter",
     # tools
+    "set_emulation_mode",
     "adc_io_display_on_lcd",
     "adc_io_display_on_console",
     "mpu_display_on_lcd",
     "mpu_display_on_console",
 ]
```

### Comparing `pyuptech-0.1.3a3/src/pyuptech/lib/libuptech.so` & `pyuptech-0.1.4a0/src/pyuptech/lib/libuptech.so`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a3/src/pyuptech/modules/loader.py` & `pyuptech-0.1.4a0/src/pyuptech/modules/loader.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a3/src/pyuptech/modules/logger.py` & `pyuptech-0.1.4a0/src/pyuptech/modules/logger.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a3/src/pyuptech/modules/pins.py` & `pyuptech-0.1.4a0/src/pyuptech/modules/pins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Sequence, Callable, TypeAlias
+from typing import Sequence, Callable, TypeAlias, SupportsIndex
 
 PinSetter: TypeAlias = Callable[[int], None]
-IndexedSetter: TypeAlias = Callable[[int, int], None]
 PinGetter: TypeAlias = Callable[[], int]
-IndexedGetter: TypeAlias = Callable[[int], int]
+IndexedSetter: TypeAlias = Callable[[SupportsIndex, int], None]
+IndexedGetter: TypeAlias = Callable[[SupportsIndex], int]
+
 PinModeSetter: TypeAlias = Callable[[int], None]
 
 
 def pin_setter_constructor(indexed_setter: IndexedSetter, pin: int) -> PinSetter:
     """
 
     Args:
```

### Comparing `pyuptech-0.1.3a3/src/pyuptech/modules/screen.py` & `pyuptech-0.1.4a0/src/pyuptech/modules/screen.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.3a3/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.4a0/src/pyuptech/modules/sensors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,64 @@
 import ctypes
 from time import perf_counter_ns
-from typing import Self, Literal, Any
+from typing import Self, Literal, Any, Callable
 
 from .loader import TECHSTAR_LIB
 from .logger import _logger
 
 E6 = 1000000
 
 """
+Only For IO, mode and level
 OUTPUT = 1
 INPUT = 0
 HIGH = 1
 LOW = 0
 """
+# this will create a function that returns a C array, but it can't be recognized correctly by the pycharm
+ADCArrayType: Callable = ctypes.c_uint16 * 10  # type: ignore
+# on 32bit machine, this will create a C array of 3 floats with bit-width of 4 bytes
+MPUArrayType: Callable = ctypes.c_float * 3  # type: ignore
 
 
 class OnBoardSensors:
     """
     provides sealed methods accessing to the IOs and builtin sensors
-    """
 
-    __adc_data_list_type = ctypes.c_uint16 * 10
-    __mpu_data_list_type = ctypes.c_float * 3
+    Owns 10 ADC channels and 3 MPU channels  and 8 IO channels
+
+    ADC: 9 for normal use, 1 for power voltage measurement(the last element in the seq)
+    IO: all the 8 are for normal use
+    MPU: all the 3 are for normal use
+    """
 
     def __init__(self, adc_min_sample_interval_ms: int = 5):
+        """
+        Initializes an instance of the OnBoardSensors class.
+        init the ADC, IO and MPU data slots
+        init sample freq limiter
+
+        *Will NOT init the IO, ADC and MPU , you need to do it manually
+
 
-        success = self.adc_io_open()
-        self.set_all_io_mode(0)
-        self.set_all_io_level(1)
-        self._adc_all: ctypes.Array = self.__adc_data_list_type()
-        self._accel_all: ctypes.Array = self.__mpu_data_list_type()
-        self._gyro_all: ctypes.Array = self.__mpu_data_list_type()
-        self._atti_all: ctypes.Array = self.__mpu_data_list_type()
+        Parameters:
+            adc_min_sample_interval_ms (int): The minimum sample interval in milliseconds for the ADC channels. Defaults to 5.
+
+        Examples:
+            >>> on_board = OnBoardSensors().adc_io_open().set_all_io_mode(0).set_all_io_level(1).MPU6500_Open()
+        """
+
+        self._adc_all: ctypes.Array = ADCArrayType()
+        self._accel_all: ctypes.Array = MPUArrayType()
+        self._gyro_all: ctypes.Array = MPUArrayType()
+        self._atti_all: ctypes.Array = MPUArrayType()
 
         self.__adc_last_sample_timestamp: int = perf_counter_ns()
 
         self.__adc_min_sample_interval_ns: int = adc_min_sample_interval_ms * E6
-        _logger.debug(f"Sensor channel have inited [{success}] times")
 
     @property
     def last_sample_timestamp_ms(self) -> int:
         return int(self.__adc_last_sample_timestamp / E6)
 
     @property
     def adc_min_sample_interval_ms(self) -> int:
@@ -59,24 +77,26 @@
         self.__adc_min_sample_interval_ns = value * E6
 
     def adc_io_open(self) -> Self:
         """
         open the adc-io plug
         """
         _logger.info("Initializing ADC-IO")
-        if TECHSTAR_LIB.adc_io_open():
+        if open_times := TECHSTAR_LIB.adc_io_open() == -1:
             _logger.error("Failed to open ADC-IO")
+        else:
+            _logger.debug(f"ADC-IO open {open_times} times")
         return self
 
     def adc_io_close(self) -> Self:
         """
         close the adc-io plug
         """
         _logger.info("Closing ADC-IO")
-        if TECHSTAR_LIB.adc_io_close():
+        if TECHSTAR_LIB.adc_io_close() == -1:
             _logger.error("Failed to close ADC-IO")
         return self
 
     def adc_all_channels(self) -> ctypes.Array:
         """
         Get all the ADC channels. Length = 10
 
@@ -227,18 +247,17 @@
         """
         initialize the 6-axis enhancer MPU6500
         default settings:
             acceleration: -+8G
             gyro: -+2000 degree/s
             sampling rate: 1kHz
         """
+        _logger.info("Initializing MPU6500...")
         if TECHSTAR_LIB.mpu6500_dmp_init():
             _logger.warning("Failed to initialize MPU6500")
-        else:
-            _logger.info("MPU6500 successfully initialized")
         return self
 
     def acc_all(self) -> ctypes.Array:
         """
         Retrieves the acceleration data from the MPU6500 sensor.
 
         Returns:
```

### Comparing `pyuptech-0.1.3a3/src/pyuptech/tools/display.py` & `pyuptech-0.1.4a0/src/pyuptech/tools/display.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,51 @@
 import time
 from typing import Literal, Dict
 
+from ..modules.emulation import SensorEmulator
 from ..modules.screen import Screen, Color, FontSize
 from ..modules.sensors import OnBoardSensors
 
-sensors: OnBoardSensors = OnBoardSensors().adc_io_open()
-screen: Screen = (
-    Screen()
-    .open()
-    .fill_screen(Color.BLACK)
-    .refresh()
-    .set_led_color(0, Color.BROWN)
-    .set_led_color(1, Color.GRED)
-)
+sensors: OnBoardSensors | SensorEmulator | None = None
+screen: Screen | None = None
+
+
+def set_emulation_mode(mode: Literal["on", "off"]):
+    """
+    Sets the emulation mode of the sensors.
+
+    Args:
+        mode (Literal["on", "off"]): The emulation mode to set. Must be either "on" or "off".
+
+    Returns:
+        None
+
+    This function sets the emulation mode of the sensors. If the mode is "on", it creates a new instance of the SensorEmulator class and assigns it to the global variable "sensors". If the mode is "off", it creates a new instance of the OnBoardSensors class and assigns it to the global variable "sensors".
+
+    Raises:
+        None
+    """
+    global sensors, screen
+    match mode:
+        case "on":
+            #  仿真器不需要启动adc-io等硬件设备
+            sensors = SensorEmulator()
+            screen = None  # 仿真模式下，假设屏幕是脱机的
+        case "off":
+            sensors = (
+                OnBoardSensors().adc_io_open().set_all_io_mode(0).set_all_io_level(1)
+            )
+            screen = (
+                Screen()
+                .open()
+                .fill_screen(Color.BLACK)
+                .refresh()
+                .set_led_color(0, Color.BROWN)
+                .set_led_color(1, Color.GRED)
+            )
 
 
 def mpu_display_on_lcd(mode: Literal["atti", "acc", "gyro"]):
     """
     Display the specified mode on the screen.
 
     Parameters:
@@ -67,15 +96,15 @@
         combined_data.append(
             [
                 acc_names[i],
                 f"{sensors.acc_all()[i]:.2}",
                 gyro_names[i],
                 f"{sensors.gyro_all()[i]:.2}",
                 atti_names[i],
-                f"{atti_names[i]:.2}",
+                f"{sensors.atti_all()[i]:.2}",
             ]
         )
 
     # Create and print the table
     table = DoubleTable(combined_data)
     table.inner_row_border = True  # Add inner row borders for clarity
     print(table.table)
@@ -105,15 +134,15 @@
     io_labels = io_labels or {}
     adc = sensors.adc_all_channels()
     io = sensors.io_all_channels()
     rows = [
         ["Names"] + ([adc_labels.get(i, f"ADC{i}") for i in range(10)]),
         ["ADC"] + [f"{x}" for x in adc],
         ["Names"] + ([io_labels.get(i, f"IO{i}") for i in range(8)]),
-        ["IO"] + [int(bit) for bit in format(io, "08b")],
+        ["IO"] + [int(bit) for bit in f"{io.value:08b}"],
     ]
     table = DoubleTable(rows)
     table.inner_row_border = True
     print(table.table)
 
 
 def adc_io_display_on_lcd(
@@ -142,15 +171,15 @@
     adc = sensors.adc_all_channels()
     # 打印 ADC 通道值表格
     for i in range(9):
         label = adc_labels.get(i, f"[{i}]")
         value = adc[i]
         screen.put_string(0, i * 8, f"{label}:{value}")
 
-    io = [int(bit) for bit in format(sensors.io_all_channels(), "08b")]
+    io = [int(bit) for bit in f"{sensors.io_all_channels().value:08b}"]
     # 打印 IO 通道值表格
     for i in range(8):
         label = io_labels.get(i, f"[{i}]")
         value = io[i]
         screen.put_string(90, i * 8, f"{label}:{value}")
     screen.fill_screen(Color.BLACK).refresh()
     time.sleep(interval)
```

### Comparing `pyuptech-0.1.3a3/tests/perf_tests.py` & `pyuptech-0.1.4a0/tests/perf_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import unittest
 from time import sleep, perf_counter_ns
 
 
-class PerfTestCase(unittest.TestCase):
+def sample_freq_test(func):
+    """
+    Test the performance and frequency of the provided function.
+
+    Args:
+        func (Callable): The function to be tested.
+    """
+    res = []
+    ms = 10000  # Assuming you want to measure for 10 seconds
+    sleep(5)  # Allow some warm-up time before starting measurement
+    end = perf_counter_ns() + ms * 1000000
+    while perf_counter_ns() < end:
+        res.append(tuple(list(func())))
+
+    deduped_res = set(res)
+    print(f"Result list length: {len(res)}")
+    print(f"Average interval (including duplicates): {ms / len(res)}ms")
+    print(f"Deduplicated result count: {len(deduped_res)}")
+    print(f"Average actual interval: {ms / len(deduped_res)}ms")
 
-    def sample_freq_test(self, func):
-        """Test the performance and frequency of the provided function.
 
-        Args:
-            func (Callable): The function to be tested.
-        """
-        res = []
-        ms = 10000  # Assuming you want to measure for 10 seconds
-        sleep(5)  # Allow some warm-up time before starting measurement
-        end = perf_counter_ns() + ms * 1000000
-        while perf_counter_ns() < end:
-            res.append(tuple(list(func())))
-
-        deduped_res = set(res)
-        print(f"Result list length: {len(res)}")
-        print(f"Average interval (including duplicates): {ms / len(res)}ms")
-        print(f"Deduplicated result count: {len(deduped_res)}")
-        print(f"Average actual interval: {ms / len(deduped_res)}ms")
+class PerfTestCase(unittest.TestCase):
 
     def test_function_performance(self):
         # Replace this with your actual function
         def dummy_func():
             return [1, 2, 3]
 
-        self.sample_freq_test(dummy_func)
+        sample_freq_test(dummy_func)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pyuptech-0.1.3a3/PKG-INFO` & `pyuptech-0.1.4a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuptech
-Version: 0.1.3a3
+Version: 0.1.4a0
 Summary: A Python wrapper for the uptech binary lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: terminaltables>=3.1.10
 Description-Content-Type: text/markdown
@@ -60,20 +60,23 @@
 ```python
 from pyuptech import OnBoardSensors
 from ctypes import c_uint8, Array
 
 # 创建OnBoardSensors对象，设置模拟量传感器最小采样间隔为5ms
 sensor_controller = OnBoardSensors(adc_min_sample_interval_ms=5)
 
+# 初始化ADC,设置所有GPIO引脚为输入，设置初始电平为高
+sensor_controller.adc_io_open().set_all_io_mode(0).set_all_io_level(1)
+
 # 设置ADC最小采样间隔为10ms，防止请求堵塞STM32从机
 sensor_controller.adc_min_sample_interval_ms = 10
 
 # 获取所有GPIO引脚当前电平
 gpio_levels: c_uint8 = sensor_controller.io_all_channels()
-print(gpio_levels)
+print(gpio_levels.value)
 
 # 初始化并读取MPU6500加速度数据
 sensor_controller.MPU6500_Open()
 acceleration_data: Array = sensor_controller.acc_all()
 
 # 设置第3号GPIO引脚为输出并设置电平为低
 sensor_controller.set_io_mode(2, 1)
@@ -187,19 +190,23 @@
 
 ## 调试
 
 通过 `tools.display` 可以将传感器数据打印到终端或者主板板载LCD屏幕上
 
 ```python
 from pyuptech import (
+    set_emulation_mode,
     mpu_display_on_lcd,
     mpu_display_on_console,
     adc_io_display_on_lcd,
     adc_io_display_on_console)
 
+# 关闭模拟模式，不关闭将无法进行正常的实机运行
+set_emulation_mode("off")
+
 mpu_display_on_console()  # 将MPU6500数据打印到终端
 
 mpu_display_on_lcd(mode="acc")  # 将MPU6500加速度数据打印到LCD
 
 # 定义ADC标签索引字典，可以空缺部分键值
 adc_labels = {
     6: 'EDGE_FL',
@@ -222,12 +229,46 @@
 }
 
 adc_io_display_on_lcd(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到LCD 
 
 adc_io_display_on_console(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到终端 
 
 
+```
+
+## 使用传感器仿真器
+
+通过 `modules.emulation.SensorEmulator` 可以使用传感器仿真器
+
+```python
+
+# 传感器仿真器导入
+from pyuptech import SensorEmulator
+
+# SensorEmulator 通过继承 OnBoardSensors 类并重写与硬件的交互方法完成的一个仿真器，所以它具有的方法是和OnBoardSensors 基本一致
+# Note: 所有返回的数据都是随机生成的，只是用于演示
+sensor_emulator = SensorEmulator(adc_min_sample_interval_ms=10)
+
+print(sensor_emulator.adc_io_open())
+
+print(list(sensor_emulator.MPU6500_Open().acc_all()))
 
 
 ```
 
+配合 `modules.display` 使用
+
+```python
+from pyuptech import (
+    set_emulation_mode,
+    mpu_display_on_console,
+    adc_io_display_on_console)
+
+# 启动模拟模式，以便打印可以正常使用随机生成的数据进行工作
+set_emulation_mode("on")
+
+mpu_display_on_console()  # 将MPU6500数据打印到终端
+
+adc_io_display_on_console()  # 将ADC和GPIO数据打印到终端
+
+```
```

