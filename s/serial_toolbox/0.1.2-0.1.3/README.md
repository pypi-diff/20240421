# Comparing `tmp/serial_toolbox-0.1.2.tar.gz` & `tmp/serial_toolbox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serial_toolbox-0.1.2.tar", max compression
+gzip compressed data, was "serial_toolbox-0.1.3.tar", max compression
```

## Comparing `serial_toolbox-0.1.2.tar` & `serial_toolbox-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35184 2024-04-17 14:00:19.176430 serial_toolbox-0.1.2/LICENSE
--rw-r--r--   0        0        0      681 2024-04-18 02:16:08.296407 serial_toolbox-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      692 2024-04-17 14:01:35.426512 serial_toolbox-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-17 14:00:19.230977 serial_toolbox-0.1.2/serial_toolbox/__init__.py
--rw-r--r--   0        0        0     4854 2024-04-17 15:06:16.439508 serial_toolbox-0.1.2/serial_toolbox/connect.py
--rw-r--r--   0        0        0     5476 2024-04-18 02:15:25.200680 serial_toolbox-0.1.2/serial_toolbox/gui.py
--rw-r--r--   0        0        0     4539 2024-04-17 15:06:16.454508 serial_toolbox-0.1.2/serial_toolbox/interface_core.py
--rw-r--r--   0        0        0      911 2024-04-17 14:00:19.232977 serial_toolbox-0.1.2/serial_toolbox/log_init.py
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 serial_toolbox-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11546 2024-04-21 08:58:03.446600 serial_toolbox-0.1.3/LICENSE
+-rw-r--r--   0        0        0      683 2024-04-21 08:58:22.960172 serial_toolbox-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      692 2024-04-17 14:01:35.426512 serial_toolbox-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 14:00:19.230977 serial_toolbox-0.1.3/serial_toolbox/__init__.py
+-rw-r--r--   0        0        0     4884 2024-04-21 08:58:03.549409 serial_toolbox-0.1.3/serial_toolbox/connect.py
+-rw-r--r--   0        0        0     6538 2024-04-21 08:58:03.549409 serial_toolbox-0.1.3/serial_toolbox/gui.py
+-rw-r--r--   0        0        0     5359 2024-04-21 08:58:03.549909 serial_toolbox-0.1.3/serial_toolbox/interface_core.py
+-rw-r--r--   0        0        0      911 2024-04-17 14:00:19.232977 serial_toolbox-0.1.3/serial_toolbox/log_init.py
+-rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 serial_toolbox-0.1.3/PKG-INFO
```

### Comparing `serial_toolbox-0.1.2/pyproject.toml` & `serial_toolbox-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "serial_toolbox"
-version = "0.1.2"
+version = "0.1.3"
 description = "Utility functions for pySerial"
 authors = ["Takuya Sasatani <33111879+t-sasatani@users.noreply.github.com>"]
-license = "AGPL-3.0"
+license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 pyserial = "^3.5"
```

### Comparing `serial_toolbox-0.1.2/README.md` & `serial_toolbox-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `serial_toolbox-0.1.2/serial_toolbox/connect.py` & `serial_toolbox-0.1.3/serial_toolbox/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class port_manager:
     """
     A utility class for managing asynchronous communication over serial ports.
     """
     
     @classmethod
-    def select_port(cls, interactive: bool=False, portname: str=None, baudrate: int=115200, timeout: float=0.1,
+    def select_port(cls, interactive: bool=False, portname: str=None, baudrate: int=9600, timeout: float=0.1,
                     logger: logging.Logger=None) -> serial.Serial:
         """
         Class method for selecting the port for serial communication.
         
         Parameters
         ----------
         interactive : bool, optional
@@ -41,18 +41,18 @@
         
         if portname:
             print("Setup port (" + portname + "). [] is default value.")
         else:
             print("Setup port. [] is default value.")
 
         if interactive:
-            baudrate_input = input("baudrate [115200] >> ")
+            baudrate_input = input("baudrate [" + str(baudrate) + "] >> ")
             if baudrate_input.strip():
                 baudrate = int(baudrate_input)
-            timeout_input = input("timeout [0.1] >> ")
+            timeout_input = input("timeout [" + str(timeout) + "] >> ")
             if timeout_input.strip():
                 timeout = float(timeout_input)  # convert input to float
             print("======================")
                 
         ser.baudrate = baudrate
         ser.timeout = timeout
```

### Comparing `serial_toolbox-0.1.2/serial_toolbox/gui.py` & `serial_toolbox-0.1.3/serial_toolbox/gui.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         The Figure object for the plot in the right frame. This object is what actually contains the graphical representation of the data.
     plot : AxesSubplot
         The subplot in the figure. This is where the data from the serial interface gets plotted.
     canvas : FigureCanvasTkAgg
         The canvas on which the figure is drawn. This is a tkinter-compatible canvas that the Figure object draws onto.
     """
 
-    def __init__(self, interface):
+    def __init__(self, interface, plotting : bool = True):
         """Initialize the Application."""
         super().__init__()
         self.interface = interface
 
         ctk.set_appearance_mode("Dark")
 
         self.left_frame = ctk.CTkFrame(self)
@@ -53,76 +53,98 @@
 
         self.send_button = ctk.CTkButton(self.left_frame, text="Send", command=self.send_command)
         self.send_button.pack(side=ctk.TOP, fill=ctk.X)
 
         self.data_text = ctk.CTkTextbox(self.left_frame, height=10, width=50)
         self.data_text.pack(side=ctk.TOP, fill=ctk.BOTH, expand=True)
 
+        self.plotting = plotting
+
         self.figure = Figure(figsize=(5, 4), dpi=100)
         self.plot = self.figure.add_subplot(1, 1, 1)
 
         self.canvas = FigureCanvasTkAgg(self.figure, self.right_frame)
         self.canvas.get_tk_widget().pack(fill=ctk.BOTH, expand=True)
-        
+        self.data_list = []
+        self.plot_queue = queue.Queue()
         self.rowconfigure(0, weight=1)
         self.columnconfigure(1, weight=1)
         self.right_frame.rowconfigure(0, weight=1)
         self.right_frame.columnconfigure(0, weight=1)
 
-        self.data_list = []
-        self.plot_queue = queue.Queue()
-
-        self.update_plot()
+        self.rxd_update()
 
     def send_command(self):
         """
         Fetch the command, send it via the serial interface and update the textbox.
         Clear the command entry field after sending the command.
         This function is connected to the 'Send' button and the 'Return' key while typing into the data_entry field.
         """
         command = self.entry_text.get()
-        self.data_text.insert(0., "CMD: " + command + "\n")
+        if self.interface.format == 'STR':        
+            self.data_text.insert(0., "TXD: " + command + "\n")
+        elif self.interface.format == 'HEX':
+            try:
+                _ = bytes.fromhex(command)
+            except ValueError:
+                print('\'' + command + '\' includes non-hexadecimal number')
+                self.data_text.insert(0., 'ERR: non-hex cmd')
+                self.entry_text.set("")
+                return
+            self.data_text.insert(0., "TXD: 0x" + command + "\n")
         self.interface.write_to_port(command)
         self.entry_text.set("")
 
-    def update_plot(self):
+    def rxd_update(self):
         """
         Update the plot with the data from the interface. 
         This function re-plots the data from the serial interface, then schedules itself to be called again after 100 ms.
         This function is automatically triggered in the initialization of the Application class, implementing a regular update of the plot.
         """
         data_queue_size = self.interface.data_queue.qsize()
         if data_queue_size > 0:
             self.plot.clear()
             self.data_list = []  # Clear data_list in every iteration of update_plot
 
             for _ in range(data_queue_size):
                 data_dict = self.interface.data_queue.get()
-                if data_dict['data'].isdigit():
-                    self.plot_queue.put(data_dict) # pass down numbers to plot_queue
-                else:
-                    self.data_text.insert(0., data_dict['data'] + "\n")
-            
+
+                if self.interface.format == 'HEX':
+                    self.data_text.insert(0., "RXD: 0x" + data_dict['data'].hex() + "\n")
+                elif self.interface.format == 'STR':
+                    data_dict['data'] = data_dict['data'].decode('utf-8').strip()
+                    if data_dict['data'].decode('utf-8').strip().isdigit() and self.plotting == True:
+                        self.plot_queue.put(data_dict) # pass down numbers to plot_queue
+                    else:
+                        self.data_text.insert(0., data_dict['data'] + "\n")
+
             plot_queue_size = self.plot_queue.qsize()
             for _ in range(plot_queue_size):
                 data_dict = self.plot_queue.get()
                 self.data_list.append(float(data_dict['data']))  # Store individual data-points
                 self.plot_queue.put(data_dict)
             
             # Outside of the loop, plot the entire data_list
             self.plot.plot(self.data_list)
             self.canvas.draw()
 
-        self.after(100, self.update_plot)
+        self.after(100, self.rxd_update)
         
 
 def serial_monitor_gui():
     """
     Start and run the customtkinter application. 
     This is the main entry point of the application that creates an instance of the Application class and executes the main loop.
     """
     port_interface = port_manager.select_port(interactive=True, portname="serial monitor")
+    format_input = input("format ('STR', 'HEX') ['STR'] >> ")
+    if format_input.strip():
+        format = format_input
+    else:
+        format = 'STR'
+
     if not port_interface:
         return
-    target_serial_interface = serial_interface(port_interface, terminal=False, max_queue_size=200)
-    app = Application(target_serial_interface)
+    
+    target_serial_interface = serial_interface(port_interface, terminal=False, max_queue_size=200, format=format)
+    app = Application(target_serial_interface, plotting = (format == 'STR'))
     app.mainloop()
```

### Comparing `serial_toolbox-0.1.2/serial_toolbox/interface_core.py` & `serial_toolbox-0.1.3/serial_toolbox/interface_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,49 +30,56 @@
         Continuously reads data from the serial port.
     process_data(data)
         Processes incoming data and add to the queue.
     write_to_port(data)
         Writes data to the serial port.
     """
 
-    def __init__(self, serial_port, terminal: bool = True, max_queue_size: int = 100):
+    def __init__(self, serial_port, terminal: bool = True, max_queue_size: int = 100, format: str = 'STR'):
         """
         Parameters
         ----------
         serial_port : serial.Serial
             Instance of the serial port to read from.
         terminal : bool, optional
             If True, print incoming data to console. Defaults to True.
         max_queue_size : int, optional
             Maximum size for data_queue. Older data will be discarded when max is reached. Defaults to 100.
+        format : str, optional
+            TBD
         """
         self.serial_port = serial_port
         self.thread = threading.Thread(target=self.read_from_port, args=(self.serial_port,))
         self.thread.daemon = True
         self.stop_flag = False
         self.data_queue = queue.Queue()
         self.terminal = terminal
         self.data_index = 0
         self.max_queue_size = max_queue_size
+        self.format = format
         self.thread.start()
 
     def read_from_port(self, serial_port):
         """
         Continuously reads data from the serial port until stop_flag is set to True.
 
         Parameters
         ----------
         serial_port : serial.Serial
             Instance of the serial port to read from.
         """
         try:
             while not self.stop_flag:
                 if serial_port.in_waiting:
-                    line = serial_port.readline().decode('utf-8').strip()
-                    self.process_data(line)
+                    if self.format == 'STR':
+                        line = serial_port.readline().decode('utf-8').strip()
+                        self.process_data(line)
+                    elif self.format == 'HEX':
+                        raw_data = serial_port.readline()
+                        self.process_data(raw_data)
         except Exception as e:
             print(e)
             return
         serial_port.close()
 
     def process_data(self, data):
         """
@@ -94,24 +101,32 @@
 
         self.data_queue.put(data_dict)
         self.data_index += 1
 
         if self.terminal:
             print(data)
 
-    def write_to_port(self, data):
+    def write_to_port(self, data_str):
         """
         Writes data to the serial port.
 
         Parameters
         ----------
         data : str
             The data to write to the serial port.
         """
-        self.serial_port.write((data+"\n").encode())
+        if self.format == 'STR':
+            self.serial_port.write((data_str+"\n").encode())
+            return
+        elif self.format == 'HEX':
+            try:
+                data_bin = bytes.fromhex(data_str)
+                self.serial_port.write(data_bin)
+            except ValueError:
+                print('\'' + data_str + '\' includes non-hexadecimal number')
 
 def serial_monitor_cli(interactive: bool = True):
     """
     Command-line interface for serial port monitor.
     
     Prompts the user to select a port, then starts the SerialReader on that port. 
     Reading operation can be stopped by a KeyboardInterrupt (Ctrl+C).
@@ -123,16 +138,22 @@
     
     The thread is closed properly by setting its stop_flag to True and waiting for
     the thread to finish execution before returning from the function.    
     """    
     port = port_manager.select_port(interactive, portname="serial monitor")
     if not port:
         return
-    interface = serial_interface(port)
     
+    format_input = input("format ('STR', 'HEX') ['STR'] >> ")
+    if format_input.strip():
+        format = format_input
+    else:
+        format = 'STR'
+    
+    interface = serial_interface(port, format)
 
     print("\nSerial port monitor started. Press Ctrl+C to stop.\n")
 
     try:
         while True: 
             pass
     except KeyboardInterrupt:
```

### Comparing `serial_toolbox-0.1.2/serial_toolbox/log_init.py` & `serial_toolbox-0.1.3/serial_toolbox/log_init.py`

 * *Files identical despite different names*

### Comparing `serial_toolbox-0.1.2/PKG-INFO` & `serial_toolbox-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: serial_toolbox
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utility functions for pySerial
-License: AGPL-3.0
+License: Apache-2.0
 Author: Takuya Sasatani
 Author-email: 33111879+t-sasatani@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: customtkinter (>=5.2.2,<6.0.0)
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: myst-parser (>=2.0.0,<3.0.0)
```

