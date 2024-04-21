# Comparing `tmp/tkeasygui-0.2.49.tar.gz` & `tmp/tkeasygui-0.2.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkeasygui-0.2.49.tar", last modified: Thu Apr 18 02:06:34 2024, max compression
+gzip compressed data, was "tkeasygui-0.2.55.tar", last modified: Sun Apr 21 04:20:39 2024, max compression
```

## Comparing `tkeasygui-0.2.49.tar` & `tkeasygui-0.2.55.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-18 02:06:34.930151 tkeasygui-0.2.49/
--rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.49/LICENSE
--rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-18 02:06:34.929840 tkeasygui-0.2.49/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)     3578 2024-04-16 00:24:05.000000 tkeasygui-0.2.49/README.md
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-18 02:06:34.927708 tkeasygui-0.2.49/TkEasyGUI/
--rw-r--r--   0 kujirahand   (501) staff       (20)      329 2024-04-14 07:30:36.000000 tkeasygui-0.2.49/TkEasyGUI/__init__.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    17301 2024-04-17 16:08:20.000000 tkeasygui-0.2.49/TkEasyGUI/dialogs.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      882 2024-04-17 16:08:20.000000 tkeasygui-0.2.49/TkEasyGUI/utils.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-18 02:06:32.000000 tkeasygui-0.2.49/TkEasyGUI/version.py
--rw-r--r--   0 kujirahand   (501) staff       (20)   116242 2024-04-18 02:04:20.000000 tkeasygui-0.2.49/TkEasyGUI/widgets.py
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-18 02:06:34.929440 tkeasygui-0.2.49/TkEasyGUI.egg-info/
--rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-18 02:06:34.000000 tkeasygui-0.2.49/TkEasyGUI.egg-info/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)      300 2024-04-18 02:06:34.000000 tkeasygui-0.2.49/TkEasyGUI.egg-info/SOURCES.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-18 02:06:34.000000 tkeasygui-0.2.49/TkEasyGUI.egg-info/dependency_links.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-18 02:06:34.000000 tkeasygui-0.2.49/TkEasyGUI.egg-info/requires.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-18 02:06:34.000000 tkeasygui-0.2.49/TkEasyGUI.egg-info/top_level.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-18 02:06:27.000000 tkeasygui-0.2.49/pyproject.toml
--rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-18 02:06:34.930243 tkeasygui-0.2.49/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-21 04:20:39.237384 tkeasygui-0.2.55/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.55/LICENSE
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6433 2024-04-21 04:20:39.237101 tkeasygui-0.2.55/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)     4029 2024-04-19 15:10:50.000000 tkeasygui-0.2.55/README.md
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-21 04:20:39.234976 tkeasygui-0.2.55/TkEasyGUI/
+-rw-r--r--   0 kujirahand   (501) staff       (20)      376 2024-04-20 12:19:46.000000 tkeasygui-0.2.55/TkEasyGUI/__init__.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)    24899 2024-04-21 03:08:26.000000 tkeasygui-0.2.55/TkEasyGUI/dialogs.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1850 2024-04-20 22:49:53.000000 tkeasygui-0.2.55/TkEasyGUI/locale_easy.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6460 2024-04-20 04:43:52.000000 tkeasygui-0.2.55/TkEasyGUI/utils.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-21 04:20:37.000000 tkeasygui-0.2.55/TkEasyGUI/version.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)   114225 2024-04-21 03:08:33.000000 tkeasygui-0.2.55/TkEasyGUI/widgets.py
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-21 04:20:39.236667 tkeasygui-0.2.55/TkEasyGUI.egg-info/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6433 2024-04-21 04:20:39.000000 tkeasygui-0.2.55/TkEasyGUI.egg-info/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)      325 2024-04-21 04:20:39.000000 tkeasygui-0.2.55/TkEasyGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-21 04:20:39.000000 tkeasygui-0.2.55/TkEasyGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-21 04:20:39.000000 tkeasygui-0.2.55/TkEasyGUI.egg-info/requires.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-21 04:20:39.000000 tkeasygui-0.2.55/TkEasyGUI.egg-info/top_level.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-21 04:20:31.000000 tkeasygui-0.2.55/pyproject.toml
+-rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-21 04:20:39.237444 tkeasygui-0.2.55/setup.cfg
```

### Comparing `tkeasygui-0.2.49/LICENSE` & `tkeasygui-0.2.55/LICENSE`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.49/PKG-INFO` & `tkeasygui-0.2.55/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.49
+Version: 0.2.55
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -45,26 +45,30 @@
 License-File: LICENSE
 Requires-Dist: Pillow
 Requires-Dist: pyperclip
 
 # TkEasyGUI
 
 `TkEasyGUI` is a Python library that allows for the easy and simple creation of GUI applications.
-In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
 
-Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
+<img src="https://github.com/kujirahand/tkeasygui-python/raw/main/docs/image/logo-button.jpg" width="180" alt="TkEasyGUI Logo">
 
-This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
+- Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
+- In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
+- This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
 
 - [👉日本語](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md) / [👉中文](https://github.com/kujirahand/tkeasygui-python/blob/main/README-zh.md)
 
+
 ## Platform
 
 - Windows / macOS / Linux (Tkinter required)
 
+<img src="https://github.com/kujirahand/tkeasygui-python/raw/main/docs/image/tkeasygui-shot640.jpg" width="300" alt="TkEasyGUI">
+
 ## Install
 
 Install from pypi
 
 
 ```sh
 python -m pip install TkEasyGUI
@@ -77,14 +81,23 @@
 python -m pip install git+https://github.com/kujirahand/tkeasygui-python
 ```
 
 - (memo) Updating from older versions (less than 0.2.24) will fail. ([See the solution](https://github.com/kujirahand/tkeasygui-python/blob/main/docs/installation_trouble.md))
 
 ## How to use
 
+Using TkEasyGUI is simple. If you only want to display a dialog, it requires just two lines of code.
+
+```py
+import TkEasyGUI as eg
+eg.popup("A joyful heart is good medicine.")
+```
+
+###
+
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
 import TkEasyGUI as eg
 # define layout
 layout = [[eg.Text("Hello, World!")],
           [eg.Button("Exit")]]
```

### Comparing `tkeasygui-0.2.49/README.md` & `tkeasygui-0.2.55/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # TkEasyGUI
 
 `TkEasyGUI` is a Python library that allows for the easy and simple creation of GUI applications.
-In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
 
-Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
+<img src="https://github.com/kujirahand/tkeasygui-python/raw/main/docs/image/logo-button.jpg" width="180" alt="TkEasyGUI Logo">
 
-This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
+- Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
+- In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
+- This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
 
 - [👉日本語](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md) / [👉中文](https://github.com/kujirahand/tkeasygui-python/blob/main/README-zh.md)
 
+
 ## Platform
 
 - Windows / macOS / Linux (Tkinter required)
 
+<img src="https://github.com/kujirahand/tkeasygui-python/raw/main/docs/image/tkeasygui-shot640.jpg" width="300" alt="TkEasyGUI">
+
 ## Install
 
 Install from pypi
 
 
 ```sh
 python -m pip install TkEasyGUI
@@ -29,14 +33,23 @@
 python -m pip install git+https://github.com/kujirahand/tkeasygui-python
 ```
 
 - (memo) Updating from older versions (less than 0.2.24) will fail. ([See the solution](https://github.com/kujirahand/tkeasygui-python/blob/main/docs/installation_trouble.md))
 
 ## How to use
 
+Using TkEasyGUI is simple. If you only want to display a dialog, it requires just two lines of code.
+
+```py
+import TkEasyGUI as eg
+eg.popup("A joyful heart is good medicine.")
+```
+
+###
+
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
 import TkEasyGUI as eg
 # define layout
 layout = [[eg.Text("Hello, World!")],
           [eg.Button("Exit")]]
```

### Comparing `tkeasygui-0.2.49/TkEasyGUI/dialogs.py` & `tkeasygui-0.2.55/TkEasyGUI/dialogs.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,54 +2,70 @@
 TkEasyGUI dialogs
 """
 import subprocess
 import tkinter.filedialog as filedialog
 import tkinter.messagebox as messagebox
 from datetime import datetime, timedelta
 from tkinter import colorchooser
-from typing import Union
+from typing import Any, Union
 
+from . import locale_easy as le
 from . import widgets as eg
 from .utils import (
     FontType,
+    get_root_window,
+    is_mac,
+    is_win,
 )
 
 #------------------------------------------------------------------------------
 # Dialogs
 #------------------------------------------------------------------------------
 # like PySimpleGUI
 
-def popup_buttons(message: str, title: str = "Question", buttons: list[str] = ["OK", "Cancel"], 
-        auto_close_duration: int = -1, timeout_key: str="-TIMEOUT-", non_blocking: bool = False) -> str:
+def popup_buttons(
+        message: str,
+        title: Union[str,None] = None,
+        buttons: list[str] = ["OK", "Cancel"], 
+        auto_close_duration: int = -1, # auto close duration (msec)
+        timeout_key: str="-TIMEOUT-", # timeout key
+        non_blocking: bool = False
+    ) -> str:
     """
     Popup window with user defined buttons. Return button's label.
 
     #### Example:
     ```py
     color = eg.popup_buttons(
         "Which color do you like?", 
         "Question",
         buttons=["red","yellow","green"])
     print(color)
     ```
     """
+    if title is None:
+        title = le.get_text("Question")
     result = buttons[-1] if len(buttons) > 0 else None
+    
     # create window
     win = eg.Window(title, layout=[
         [eg.Text(message)],
         [eg.Button(s, width=9) for s in buttons],
     ], modal=True)
+    
     # event loop
     timer_id = eg.time_checker_start()
     autoclose_sec: int = auto_close_duration * 1000
     if non_blocking:
         # TODO: popup non blocking window
         pass
     while win.is_alive():
         event, _ = win.read(timeout=100, timeout_key=eg.WINDOW_TIMEOUT)
+        if event == eg.WINDOW_CLOSED:
+            result = eg.WINDOW_CLOSED
         if event in buttons:
             result = event
             break
         if event == eg.WINDOW_TIMEOUT:
             if auto_close_duration > 0 and eg.time_checker_end(timer_id) > autoclose_sec:
                 result = timeout_key # timeout_key only use result
                 break
@@ -69,93 +85,185 @@
     return popup_buttons(message=message, title=title, buttons=["OK"])
 
 def popup_non_blocking(message: str, title: str="", auto_close_duration: int = -1) -> str:
     """(TODO) Display a non blocking window"""
     return popup_buttons(message, title, buttons=["OK"], auto_close_duration=auto_close_duration, non_blocking=True)
 
 def popup_no_buttons(message: str, title: str="") -> None:
+    """Display a message in a popup window without buttons."""
     popup_buttons(message, title, buttons=[])
 
 def popup_auto_close(message: str, title: str="", auto_close_duration: int = 3, buttons: list[str] = ["OK", "Cancel"], timeout_key="-TIMEOUT-") -> str:
     """Display a message in a popup window that closes automatically after a specified time."""
     return popup_buttons(message, title, buttons=buttons, auto_close_duration=auto_close_duration, timeout_key=timeout_key)
 
 def popup_no_wait(message: str, title: str="", **kw) -> str:
     """Display a message in a popup window without waiting."""
     return popup_auto_close(message, title, auto_close_duration=0, **kw)
 
 def popup_ok(message: str, title: str="") -> str:
     """Display a message in a popup window.(Alias popup)"""
     return popup_buttons(message, title, buttons=["OK"])
 
-def popup_ok_cancel(message: str, title: str="") -> str:
-    """Display a message in a popup window with OK and Cancel buttons. Return "OK" or "Cancel"."""
-    return popup_buttons(message, title, buttons=["OK", "Cancel"])
-
-def popup_yes_no(message: str, title: str = "Question", yes_label: str="Yes", no_label: str="No") -> str:
+def popup_ok_cancel(
+        message: str,
+        title: Union[str,None] = None,
+        ok_label: Union[str, None] = None,
+        cancel_label: Union[str, None] = None,
+        ok_value: str = "OK",
+        cancel_value: str = "Cancel",
+        ) -> str:
+    """Display a message in a popup window with OK and Cancel buttons. Return "OK" or "Cancel" or eg.WINDOW_CLOSED."""
+    if ok_label is None:
+        ok_label = le.get_text("OK")
+    if cancel_label is None:
+        cancel_label = le.get_text("Cancel")
+    result = popup_buttons(message, title, buttons=[ok_label, cancel_label])
+    if result == ok_label:
+        return ok_value
+    if result == cancel_label:
+        return cancel_value
+    return result # pushed close button
+
+def popup_yes_no(
+                message: str, # question message
+                title: Union[str,None] = None, # window title
+                yes_label: Union[str,None]=None, # label for yes button
+                no_label: Union[str,None]=None, # label for no button
+                yes_value: str = "Yes", # return value for yes
+                no_value: str = "No" # return value for no
+                ) -> str:
     """
-    Display a message in a popup window with Yes and No buttons. Return "Yes" or "No".
-
-    #### Example:
-    Ask user question, [Yes] or [No]
+    Display a message in a popup window with Yes and No buttons. Return "Yes" or "No" (or eg.WINDOW_CLOSED).
+    @see [tests/localize_test.py](https://github.com/kujirahand/tkeasygui-python/blob/main/tests/localize_test.py)
+    #### Example - simple:
+    Ask user question, [Yes] or [No] buttons.
     ```py
-    a = eg.popup_yes_no("Do you like Sushi?", "Question")
-    print(a) # "Yes" or "No"
+    ans = eg.popup_yes_no("Do you like Sushi?", "Question")
+    print(ans) # "Yes" or "No"
     ```
-    Ask user question in Japanes [はい] or [いいえ]
+    #### Eample - custom label:
+    Ask user question in special button
     ```py
-    ja_a = eg.popup_yes_no("寿司は好き?", "質問", yes_label="はい", no_label="いいえ")
-    print(ja_a) # "はい" or "いいえ"
+    ans = eg.popup_yes_no("Do you eat Sushi?", yes_label="EAT", no_label="no")
+    print(ans) # "Yes" or "No"
     ```
+    #### Example - custom return value:
+    ans = eg.popup_yes_no("Can you speak Japanese?", yes_value="can", no_value="no")
+    print(ans) # "can" or "no"
     """
-    # return "Yes" if messagebox.askyesno(title, message) else "No"
-    return popup_buttons(message, title, buttons=[yes_label, no_label])
+    # get locale text
+    title = title if title is not None else le.get_text("Question")
+    yes_label = yes_label if yes_label is not None else le.get_text("Yes")
+    no_label = no_label if no_label is not None else le.get_text("No")
+    # ask yes or no
+    result = popup_buttons(message, title, buttons=[yes_label, no_label])
+    # get result
+    if result == yes_label:
+        return yes_value
+    if result == no_label:
+        return no_value
+    return result # pushed close button
 
-def popup_yes_no_cancel(message: str, title: str = "Question") -> str:
+def popup_yes_no_cancel(
+        message: str,
+        title: Union[str, None] = None,
+        yes_label: Union[str, None] = None,
+        no_label: Union[str, None] = None,
+        cancel_label: Union[str, None] = None,
+        yes_value: str = "Yes",
+        no_value: str = "No",
+        cancel_value: str = "Cancel"
+        ) -> str:
     """Display a message in a popup window with Yes and No buttons. Return "Yes" or "No" or "Cancel"."""
-    return popup_buttons(message, title, buttons=["Yes", "No", "Cancel"])
+    # return popup_buttons(message, title, buttons=["Yes", "No", "Cancel"])
+    # get locale text
+    title = title if title is not None else le.get_text("Question")
+    yes_label = yes_label if yes_label is not None else le.get_text("Yes")
+    no_label = no_label if no_label is not None else le.get_text("No")
+    cancel_label = cancel_label if cancel_label is not None else le.get_text("Cancel")
+    # ask yes or no
+    result = popup_buttons(message, title, buttons=[yes_label, no_label, cancel_label])
+    # get result
+    if result == yes_label:
+        return yes_value
+    if result == no_label:
+        return no_value
+    if result == cancel_label:
+        return cancel_value
+    return cancel_label
 
 def popup_cancel(message: str, title: str="") -> str:
-    """Display a message in a popup window with OK and Cancel buttons. Return "OK" or "Cancel"."""
-    return popup_buttons(message, title, buttons=["Cancel"])
+    """Display a message in a popup window with OK and Cancel buttons. Return "Cancel" or eg.WINDOW_CLOSED."""
+    cancel_label = le.get_text("Cancel")
+    result = popup_buttons(message, title, buttons=["Cancel"])
+    return cancel_label if result == cancel_label else result
 
-def popup_get_text(message: str, title: str = "", default: str = "", font: eg.FontType=None) -> Union[str, None]:
+def popup_get_text(
+        message: str,
+        title: Union[str,None] = None,
+        default: Union[str, None] = None,
+        default_text: Union[str, None] = None, # same as default for compatibility
+        font: FontType=None) -> Union[str, None]:
     """Display a message in a popup window with a text entry. Return the text entered."""
     # return simpledialog.askstring(title, message, initialvalue=default)
+    if default_text is not None:
+        default = default_text
     return popup_input(message, title, default, font=font)
 
-def popup_input(message: str, title: str = "", default: str = "", font: eg.FontType=None) -> Union[str, None]:
-    """Display a message in a popup window with a text entry. Return the text entered."""
-    result = None
+def popup_input(
+        message: str,
+        title: Union[str,None] = None,
+        default: str = "",
+        ok_label: Union[str, None] = None,
+        cancel_label: Union[str, None] = None,
+        cancel_value: Any = None,
+        font: FontType=None) -> Union[str, None]:
+    """Display a message in a popup window with a text entry. Return the text entered. if canceled, return cancel_value."""
+    result = cancel_value
+    if title is None:
+        title = le.get_text("Text input")
+    if ok_label is None:
+        ok_label = le.get_text("OK")
+    if cancel_label is None:
+        cancel_label = le.get_text("Cancel")
     win = eg.Window(title, layout=[
         [eg.Text(message)],
         [eg.Input(default, key="-user-", width=40)],
-        [eg.Button("OK", width=9), eg.Button("Cancel", width=9)]
+        [eg.Button(ok_label, width=11), eg.Button(cancel_label, width=9)]
     ], modal=True, font=font)
-    while win.is_alive():
+    while True:
         event, values = win.read()
-        if event == "OK":
+        if event == ok_label:
             result = values["-user-"]
             break
-        if event == "Cancel":
+        if event in [cancel_label, eg.WINDOW_CLOSED]:
+            # let result = cancel_value
             break
     win.close()
     return result
 
-def popup_error(message: str, title: str="Error") -> None:
+def popup_error(message: str, title: Union[str,None]=None) -> None:
     """Display a message in a popup window with an error icon."""
-    popup_buttons(message, title, buttons=["Error"])
+    if title is None:
+        title = le.get_text("Error")
+    error_label = le.get_text("Error")
+    popup_buttons(message, title, buttons=[error_label])
     # messagebox.showerror(title, message)
 
-def popup_warning(message: str, title: str="Warning") -> None:
+def popup_warning(message: str, title: Union[str,None]=None) -> None:
     """Display a message in a popup window with an warning icon."""
+    if title is None:
+        title = le.get_text("Warning")
     messagebox.showwarning(title, message)
 
-def popup_info(message: str, title: str="Warning") -> None:
+def popup_info(message: str, title: Union[str,None]=None) -> None:
     """Display a message in a popup window with an warning icon."""
+    if title is None:
+        title = le.get_text("Information")
     messagebox.showwarning(title, message)
 
 def popup_get_file(
         message: str="",
         title: Union[str, None] = None,
         initial_folder: str = "",
         save_as: bool = False, # show `save as` dialog
@@ -189,33 +297,64 @@
             **kw
             ) -> Union[str, None]:
     """Popup a folder selection dialog. Return the folder selected."""
     if title is None:
         title = message
     return filedialog.askdirectory(title=title, initialdir=default_path, **kw)
 
+def popup_memo(
+        message: str,
+        title: Union[str, None] = None,
+        size: tuple[int,int] = [60, 8],
+        readonly: bool = False,
+        ok_label: Union[str, None] = None,
+        cancel_label: Union[str, None] = None,
+        cancel_value: Union[str,None] = None,
+        font: Union[FontType, None] = None
+        ) -> Union[str, None]:
+    """Display a multiline message in a popup window. Return the text entered. if canceled, return cancel_value."""
+    return popup_scrolled(message, title, size, readonly, ok_label, cancel_label, cancel_value, font)
+
 def popup_scrolled(
             message: str,
-            title: str = "",
+            title: tuple[str, None] = None,
             size: tuple[int,int] = [40, 5],
             readonly: bool = False,
+            ok_label: Union[str, None] = None,
+            cancel_label: Union[str, None] = None,
+            cancel_value: Union[str,None] = None,
             font: Union[FontType, None] = None
             ) -> Union[str, None]:
-    """Display a message in a popup window with a text entry. Return the text entered."""
+    """
+    Display a multiline message in a popup window. Return the text entered. if canceled, return cancel_value.
+    #### Example:
+    ```py
+    import TkEasyGUI as eg
+    text = eg.popup_scrolled("This is a long text.", "Information")
+    eg.print(text)
+    ```
+    """
+    result = cancel_value
+    if cancel_label is None:
+        cancel_label = le.get_text("Cancel")
+    if ok_label is None:
+        ok_label = le.get_text("OK")
+    if title is None:
+        title = le.get_text("Information")
     win = eg.Window(title, layout=[
         [eg.Multiline(message, key="-text-", size=size, readonly=readonly, font=font)],
-        [eg.Button("OK", width=9), eg.Button("Cancel", width=5)]
+        [eg.Button(ok_label, width=9), eg.Button(cancel_label, width=5)]
     ], modal=True)
     result = None
     while win.is_alive():
         event, _ = win.read()
-        if event == "OK":
+        if event == ok_label:
             result = win["-text-"].get()
             break
-        if event == "Cancel":
+        if event == cancel_label:
             break
     win.close()
     return result
 
 def popup_get_date(
         message: str = "",
         title: str = "",
@@ -326,19 +465,20 @@
             current_date = datetime(year=current_date.year, month=current_date.month, day=int(label))
             update_result(current_date)
     window.close()
     return result
 
 #------------------------------------------------------------------------------
 # for notify
+#------------------------------------------------------------------------------
 def popup_notify(message: str, title: str="") -> None:
     """Popup a information"""
-    if eg.is_mac():
+    if is_mac():
         send_notification_mac(message, title)
-    elif eg.is_win():
+    elif is_win():
         send_notification_win(message, title)
     else:
         popup_buttons(message, title, buttons=["OK"], auto_close_duration=1)
 
 def send_notification_mac(message: str, title: str=""):
     """"Send Notification on mac"""
     if title == "":
@@ -364,14 +504,15 @@
 [Windows.UI.Notifications.ToastNotificationManager]::CreateToastNotifier($AppId).Show($TemplateContent)
 '''
     # Execute PowerShell
     subprocess.run(["powershell", "-Command", powershell_script])
 
 #------------------------------------------------------------------------------
 # TkEasyGUI original dialogs
+#------------------------------------------------------------------------------
 
 def popup_color(title: str="", default_color: Union[str, None]=None) -> (Union[str, None]):
     """Popup a color selection dialog. Return the color selected."""
     col = colorchooser.askcolor(title=title, color=default_color)
     if col[1] is None:
         return default_color
     return f"{col[1]}".upper()
@@ -404,39 +545,108 @@
             else:
                 if len(selected) == 1:
                     result = selected[0]
             break
     win.close()
     return result
 
+def popup_image(
+        message: str,
+        title: Union[str,None] = None,
+        image_path: Union[str,None] = None,
+        image_data: Union[bytes,None] = None,
+        size: tuple[int,int] = (400, 300),
+        ok_label: Union[str, None] = None,
+        ok_value: str = "OK",
+        cancel_label: Union[str, None] = None,
+        cancel_value: str = "Cancel",
+        font: Union[FontType, None] = None,
+        ) -> str:
+    """Display an image in a popup window. Return the text entered."""
+    if title is None:
+        title = message
+    if ok_label is None:
+        ok_label = le.get_text("OK")
+    if cancel_label is None:
+        cancel_label = le.get_text("Cancel")
+    win = eg.Window(title, layout=[
+        [eg.Text(message)],
+        [eg.Image(image_path, image_data, size=size)],
+        [eg.Button(ok_label, width=9), eg.Button(cancel_label, width=5)]
+    ], modal=True, font=font)
+    result = cancel_value
+    while win.is_alive():
+        event, _ = win.read()
+        if event == ok_label:
+            result = ok_value
+            break
+        if event == cancel_label:
+            break
+    win.close()
+    return result
+
+
+#------------------------------------------------------------------------------
+# TKinter alias
 #------------------------------------------------------------------------------
-# TKinter
 def ask_yes_no(message: str, title: str="Question") -> bool:
     """Display a message in a popup window with Yes and No buttons. Return True or False. (use Tkinter)"""
     return messagebox.askyesno(title, message)
 
 def ask_ok_cancel(message: str, title: str="Question") -> bool:
     """Display a message in a popup window with OK and Cancel buttons. Return True or False. (use Tkinter)"""
     return messagebox.askokcancel(title, message)
 
 def ask_retry_cancel(message: str, title: str="Question") -> bool:
     """Display a message in a popup window with Retry and Cancel buttons. Return True or False. (use Tkinter)"""
     return messagebox.askretrycancel(title, message)
 
 def show_message(
         message: str,
-        title: str="Information"
+        title: Union[str,None] = None
     ) -> None:
     """show message in a popup window"""
+    title = title if title is not None else le.get_text("Information")
     messagebox.showinfo(title, message)
 
-def show_info(message: str, title: str="Information") -> None:
+def show_info(
+        message: str,
+        title: Union[str,None] = None
+    ) -> None:
     """show message in a popup window"""
+    title = title if title is not None else le.get_text("Information")
     messagebox.showinfo(title, message)
 
 def msgbox(
         message: str, # message
-        title: str="Message" # dialog title
+        title: Union[str,None] = None
     ) -> None:
     """show message in a popup window like VB"""
+    title = title if title is not None else le.get_text("Information")
     messagebox.showinfo(title, message)
 
+#------------------------------------------------------------------------------
+# TkEasyGUI original dialogs
+#------------------------------------------------------------------------------
+def input(
+        message: str,
+        title: Union[str,None] = None,
+        default: str = ""
+    ) -> str:
+    """Display a message in a popup window with a text entry. Return the text entered."""
+    return popup_input(message, title, default)
+
+def print(*args, **kw) -> None:
+    """Print message to popup window."""
+    lines = " ".join([str(a) for a in args])
+    popup(lines)
+
+def confirm(
+        question: str,
+        title: Union[str,None] = None
+    ) -> bool:
+    """Display a message in a popup window with Yes and No buttons. Return True or False."""
+    return popup_yes_no(question, title, yes_value="Yes") == "Yes"
+
+#------------------------------------------------------------------------------
+# To prevent the display of an empty window
+_ = get_root_window()
```

### Comparing `tkeasygui-0.2.49/TkEasyGUI/widgets.py` & `tkeasygui-0.2.55/TkEasyGUI/widgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,27 +13,38 @@
 from tkinter import scrolledtext, ttk
 from typing import Any, Union
 
 # from typing import TypeAlias
 from PIL import Image as PILImage
 from PIL import ImageTk
 
-from . import dialogs, utils
+from . import dialogs, utils, version
 from .utils import (
+    # type alias
     Element,
     EventMode,
     FontType,
     ListboxSelectMode,
     OrientationType,
     PadType,
     PointType,
     ReliefType,
     TextAlign,
     TextVAlign,
-    Window,
+    # Window,
+        _window_count,
+    _window_parent,
+    _window_pop,
+    _window_push,
+    generate_element_id,
+    generate_element_style_key,
+    get_current_theme,
+    get_root_window,
+    get_ttk_style,
+    register_element_key,
 )
 
 #------------------------------------------------------------------------------
 # Const
 #------------------------------------------------------------------------------
 WINDOW_CLOSED: str = "WINDOW_CLOSED"
 WIN_CLOSED: str = "WINDOW_CLOSED"
@@ -48,165 +59,23 @@
 TABLE_SELECT_MODE_BROWSE: str = tk.BROWSE
 TABLE_SELECT_MODE_EXTENDED: str = tk.EXTENDED
 EG_SWAP_EVENT_NAME: str = "--swap_event_name--"
 
 # about color (Thanks)
 # https://kuroro.blog/python/YcZ6Yh4PswqUzaQXwnG2/
 
-#------------------------------------------------------------------------------
-# utility
-def get_platform() -> str:
-    """get platform"""
-    return platform.system()
-
-def is_mac() -> bool:
-    """platform : is mac?"""
-    return get_platform() == "Darwin"
-def is_win() -> bool:
-    """platform : is Windows?"""
-    return get_platform() == "Windows"
-
-#------------------------------------------------------------------------------
-# theme
-_tkeasygui_info: dict[str, Any] = {}
-def theme(name: str) -> None:
-    """Set theme"""
-    set_theme(name)
-
-def set_theme(name: str) -> None:
-    """Change look and feel"""
-    win = get_root_window()
-    win.withdraw()
-    style = get_ttk_style()
-    style.theme_use(name)
-    _tkeasygui_info["theme"] = name
-
-def get_tnemes() -> list[str]:
-    """
-    Get theme list
-    ```py
-    print(get_themes())
-    ```
-    """
-    win = get_root_window()
-    win.withdraw()
-    return ttk.Style().theme_names()
-
-def get_current_theme() -> str:
-    """Get current theme"""
-    return _tkeasygui_info.get("theme", "")
-
-def set_default_theme() -> None:
-    """
-    Set default theme
-    ```py
-    print(get_themes())
-    ```
-    """
-    if is_mac():
-        # ('aqua', 'clam', 'alt', 'default', 'classic')
-        set_theme("aqua")
-    elif is_win():
-        # ('winnative', 'clam', 'alt', 'default', 'classic', 'vista', 'xpnative')
-        # set_theme("winnative")
-        # set_theme("default")
-        set_theme("vista")
-    else:
-        set_theme("clam")
-
-def convert_color_rgb16(color_name: str) -> tuple[int, int, int]:
-    """Convert color to RGB, return (r, g, b) tuple. range=0-65535"""
-    root = get_root_window()
-    return root.winfo_rgb(color_name)
-
-def convert_color_html(color_name: str) -> str:
-    """Convert RGB color(16bit tuple) to HTML color name."""
-    r, g, b = convert_color_rgb16(color_name)
-    return f"#{r//256:02x}{g//256:02x}{b//256:02x}"
 
 #------------------------------------------------------------------------------
 # Widget wrapper
 #------------------------------------------------------------------------------
 class TkEasyError(Exception):
     def __init__(self, message="TkEasyError"):
         self.message = message
         super().__init__(self.message)
 
-# Prioritize compatibility with PySimpleGUI
-_compatibility: bool = True
-def set_PySimpleGUI_compatibility(flag: bool=True) -> None:
-    """Set compatibility with PySimpleGUI (Default=True)"""
-    global _compatibility
-    _compatibility = flag
-
-# only one root element
-_root_window: Union[tk.Tk, None] = None
-_ttk_style: Union[ttk.Style, None] = None
-def get_root_window() -> tk.Tk:
-    """Get root window."""
-    global _root_window
-    if _root_window is None:
-        _root_window = tk._get_default_root() # tk.Tk()
-        _root_window.eval('tk::PlaceWindow . center')
-        _root_window.attributes('-alpha', 0)
-        _root_window.withdraw()
-        # set theme
-        try:
-            if "theme" in _tkeasygui_info:
-                name = _tkeasygui_info["theme"]
-                _ttk_style = get_ttk_style()
-                _ttk_style.theme_use(name)
-            else:
-                set_default_theme()
-        except Exception as e:
-            print(f"TkEasyGUI.theme: failed to set theme {name} {e}", file=sys.stderr)
-            pass
-    return _root_window
-
-def get_font_list() -> list[str]:
-    """Get font list"""
-    root = get_root_window()
-    root.withdraw()
-    return list(tkfont.families())
-
-def get_ttk_style() -> ttk.Style:
-    """Get ttk style"""
-    global _ttk_style
-    if _ttk_style is None:
-        _ttk_style = ttk.Style()
-    return _ttk_style
-
-# active window
-_window_list: list[Window] = []
-def _get_active_window() -> Union[tk.Toplevel, None]:
-    """Get the active window."""
-    if len(_window_list) == 0:
-        return None
-    return _window_list[-1].window
-
-def _window_parent() -> Union[Window, None]:
-    """Get the parent window."""
-    if len(_window_list) == 0:
-        return None
-    return _window_list[-1]
-
-def _window_count() -> int:
-    """Get the number of windows."""
-    return len(_window_list)
-
-def _window_push(win: Window) -> None:
-    """Push a window to the list."""
-    _window_list.append(win)
-
-def _window_pop(win: Window) -> None:
-    """Pop a window from the list."""
-    i = _window_list.index(win)
-    if i >= 0:
-        _window_list.pop()
-
 class Window:
     """
     Main window object in TkEasyGUI
     """
     def __init__(
                 self,
                 title: str,
@@ -219,26 +88,26 @@
                 no_titlebar: bool = False, # hide titlebar
                 grab_anywhere: bool = False, # can move window by dragging anywhere
                 alpha_channel: float = 1.0, # window alpha channel
                 enable_key_events: bool = False, # enable keyboard events
                 return_keyboard_events: bool = False, # enable keyboard events (for compatibility)
                 location: Union[tuple[int, int], None] = None, # window location
                 center_window: bool = True, # move window to center
+                row_padding: int = 2, # row padding
                 **kw) -> None:
         """Create a window with a layout of widgets."""
         self.modal: bool = modal
         # check active window
-        active_win = _get_active_window()
+        active_win = utils._get_active_window()
         if active_win is None:
             active_win = get_root_window()
         self.window: tk.Toplevel = tk.Toplevel(master=active_win)
         self.timeout: Union[int, None] = None
         self.timeout_key: str = WINDOW_TIMEOUT
         self.timeout_id: Union[str, None] = None
-        self.focus_timer_id: Union[str, None] = None
         self.events: Queue = Queue()
         self.key_elements: dict[str, Element] = {}
         self.last_values: dict[str, Any] = {}
         self.flag_alive: bool = True # Pressing the close button will turn this flag to False.
         self.layout: list[list[Element]] = layout
         self._event_hooks: dict[str, list[callable]] = {}
         self.font: Union[FontType, None] = font
@@ -254,14 +123,15 @@
         self._start_y: Union[int, None] = None
         self._mouse_x: Union[int, None] = None
         self._mouse_y: Union[int, None] = None
         self.alpha_channel: float = alpha_channel
         self.enable_key_events: bool = enable_key_events
         self.return_keyboard_events: bool = return_keyboard_events
         self.font_size_average: tuple[int, int] = (12, 10)
+        self.row_padding: int = row_padding
         # Frame
         self.frame: ttk.Frame = ttk.Frame(self.window, padding=10)
         self.frame.configure(style="TFrame")
         # set window properties
         self.window.title(title)
         self.window.protocol("WM_DELETE_WINDOW", lambda : self._close_handler())
         self.size: Union[tuple[int, int], None] = size
@@ -360,31 +230,34 @@
         """
         for event_name, handle_list in hooks.items():
             for handle in handle_list:
                 if event_name not in self._event_hooks:
                     self._event_hooks[event_name] = []
                 self._event_hooks[event_name].append(handle)
     
-    def _create_widget(self, parent: tk.Widget, layout: list[list["Element"]]):
+    def _create_widget(self, parent: tk.Widget, layout: list[list["Element"]], align: TextAlign="left", valign: TextVAlign="top"):
         """create widget from layout"""
         # check layout
         if not (len(layout) > 0 and (isinstance(layout[0], list) or isinstance(layout[0], tuple))):
             raise TkEasyError(f"Invalid layout, should specify a two-dimensional list: {layout}")
         # prepare create
         for widgets in layout:
             for elem in widgets:
                 elem.prepare_create(self)
         # create widgets
         self.need_focus_widget: tk.Widget|None = None
         for row_no, widgets in enumerate(layout):
             # frame_row = ttk.Frame(parent, padding=5, name=f"tkeasygui_frame_row_{row_no}")
-            frame_row = ttk.Frame(parent, name=f"tkeasygui_frame_row_{row_no}")
+            frame_row = ttk.Frame(parent, padding=self.row_padding ,name=f"tkeasygui_frame_row_{row_no}")
             # columns
             prev_element: Element|None = None
-            row_prop: dict[str, Any] = {"expand": False, "fill": "x", "side": "top"}
+            row_prop: dict[str, Any] = {"expand": False, "fill": "x", "side": valign}
+            # reversed?
+            if align == "right":
+                widgets = reversed(widgets)
             for col_no, elemment in enumerate(widgets):
                 # create widget
                 elem: Element = elemment
                 # set window and parent
                 elem.window = self
                 elem.parent = frame_row
                 elem.col_no = col_no
@@ -412,29 +285,30 @@
                 # check specila key
                 if (self.need_focus_widget is None) and (elem.key == "OK" or elem.key == "Yes"):
                     self.need_focus_widget = widget
                 # create sub widgets
                 try:
                     # has children?
                     if elem.has_children:
-                        self._create_widget(widget, elem.layout)
+                        self._create_widget(widget, elem.layout, align=elem.text_align, valign=elem.vertical_alignment)
                 except Exception as e:
+                    print(e.__traceback__, file=sys.stderr)
                     raise TkEasyError(
-                        f"Window._create_widget.Failed_sub_widgets `{elem.element_type}` key=`{elem.key}` {elem.props} reason:{e}"
+                        f"Window._create_widget.Failed(children) `{elem.element_type}` key=`{elem.key}` {elem.props} reason:{e}"
                     ) from e
                 # post create
                 elem.post_create(self, frame_row)
                 # bind event (before create)
                 for event_name, handle_t in elem._bind_dict.items():
                     self.bind(elem, event_name, handle_t[0], handle_t[1], handle_t[2])
                 # menu ?
                 if isinstance(elem, Menu):
                     continue
                 # pack widget
-                fill_props = elem._get_pack_props()
+                fill_props = elem._get_pack_props(align, valign)
                 widget.pack(**fill_props)
                 # expand_y?
                 if elem.expand_y:
                     row_prop["expand"] = True
                     row_prop["fill"] = "both"
                 # pady
                 if elem.pady is not None:
@@ -513,33 +387,36 @@
                     result.append(elem)
         return result
 
     def read(self, timeout: Union[int, None] = None, timeout_key: str="-TIMEOUT-") -> tuple[str, dict[str, Any]]:
         """ Read events from the window."""
         self.timeout = timeout
         self.timeout_key = timeout_key
-        time_id = time_checker_start()
+        timeout_chcker_id = time_checker_start()
+        # get root window
+        root = get_root_window()
+        # update window before mainloop
+        root.update() 
+        # set focus timer (once when window show)
+        self.window.after("idle", _focus_window, self)
+        # mainloop
         while True:
             # set timeout
             if self.timeout_id is not None:
                 self.window.after_cancel(self.timeout_id)
             self.timeout_id = self.window.after("idle", self._window_idle_handler)
-            # set focus timer (once when window show)
-            if self.focus_timer_id is None:
-                self.focus_timer_id = self.window.after("idle", _focus_window, self) # focus timer
             # mainloop - should be called only once
-            root = get_root_window()
             root.mainloop()
             # after mainloop, check events
             if not self.events.empty():
                 break
             # check timeout
             if timeout is None:
                 continue # no timeout
-            interval = time_checker_end(time_id)
+            interval = time_checker_end(timeout_chcker_id)
             if interval > timeout:
                 return (self.timeout_key, {}) # return timeout event
         # return event
         key, values = self.events.get()
         if key in self._event_hooks:
             flag_stop = self._dispatch_event_hooks(key, values)
             if flag_stop:
@@ -685,21 +562,22 @@
             self.window.overrideredirect(flag)
             self._no_titlebar = flag
         except Exception:
             pass
 
     def close(self) -> None:
         """Close the window."""
-        global active_window
         try:
             self.flag_alive = False
-            self.window.quit()
-            self.window.destroy()
             _window_pop(self)
-        except Exception as _:
+            self.window.destroy() # close window
+            if _window_count() == 0:
+                self.window.quit() # quit app
+        except Exception as e:
+            print(f"Window.close.failed: {e}", file=sys.stderr)
             pass
 
     def is_alive(self) -> bool:
         """Check if the window is alive."""
         return self.flag_alive
     
     def cancel_close(self) -> None:
@@ -796,15 +674,15 @@
 
 def _exit_mainloop() -> None:
     """Exit mainloop"""
     root = get_root_window()
     try:
         root.quit() # exit from mainloop
     except Exception:
-        # print("_exit_mainloop: failed to exit mainloop")
+        print("_exit_mainloop: failed to exit mainloop", file=sys.stderr)
         pass
 
 def _focus_window(self: Window) -> None:
     """Focus window"""
     if not self.flag_alive:
         return
     if self.need_focus_widget is not None:
@@ -854,14 +732,15 @@
         self.prev_element: Element|None = None
         self.next_element: Element|None = None
         self.window: Window|None = None
         self.parent: tk.Widget|None = None
         self._bind_dict: dict[str, tuple[str, bool, EventMode]] = {}
         self.user_bind_event: tk.Event|None = None # when bind event fired then set this value
         self.vertical_alignment: TextVAlign = "center"
+        self.text_align: TextAlign = "left"
         self.padx: int|tuple[int,int]|None = 1
         self.pady: int|tuple[int,int]|None = None
         self.font: Union[FontType, None] = None
         self.has_font_prop: bool = True
         self.col_no: int = -1
         self.row_no: int = -1
     
@@ -928,17 +807,22 @@
         if color is not None:
             self.props["fg"] = color
         if text_color is not None:
             self.props["fg"] = text_color
         if background_color is not None:
             self.props["bg"] = background_color
 
-    def _get_pack_props(self) -> dict[str, Any]:
+    def _get_pack_props(self, align: str="left", valign: str="top") -> dict[str, Any]:
         """Get the fill property in `pack` method."""
         props: dict[str, Any] = {"expand": False, "fill": "none", "side": "left"}
+        if align == "right":
+            props["side"] = "right"
+        elif align == "center":
+            props["fill"] = "both"
+            props["expand"] = True
         # check expand
         if self.expand_x and self.expand_y:
             props["expand"] = True
             props["fill"] = "both"
         elif self.expand_x:
             props["expand"] = True
             props["fill"] = "x"
@@ -1139,14 +1023,16 @@
                 relief: ReliefType="groove",
                 # text props
                 font: Union[FontType, None] = None, # font
                 color: Union[str, None] = None,
                 text_color: Union[str, None] = None,
                 background_color: Union[str, None] = None,
                 label_outside: bool=False,
+                vertical_alignment: TextVAlign="top", # vertical alignment
+                text_align: Union[TextAlign, None]="left", # text align
                 # pack props
                 expand_x: bool = False,
                 expand_y: bool = False,
                 pad: Union[PadType, None] = None,
                 # other
                 metadata: Union[dict[str, Any], None] = None,
                 use_ttk: bool=False,
@@ -1154,14 +1040,16 @@
         style_name = "TLabelframe" if use_ttk else ""
         super().__init__("Frame", style_name, key, False, metadata, **kw)
         self.has_children = True
         self.layout = layout
         self.label_outside = label_outside
         self.props["text"] = title
         self.props["relief"] = relief
+        self.text_align = text_align
+        self.vertical_alignment = vertical_alignment
         self._set_text_props(color=color, text_color=text_color, background_color=background_color, font=font)
         self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
         self.use_ttk: bool = use_ttk
 
         if size is not None:
             self.props["size"] = size
 
@@ -1208,27 +1096,30 @@
                 pad: Union[PadType, None] = None,
                 # other
                 metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         super().__init__("Column", "TFrame", key, False, metadata, **kw)
         self.has_children = True
         self.layout = layout
+        self.text_align = text_align
         self.vertical_alignment = vertical_alignment
         self.has_font_prop = False
+        self.use_ttk = False
         self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
         if size is not None:
             self.props["size"] = size
         if background_color is not None:
             self.props["background_color"] = background_color
         if text_align is not None:
             self.props["anchor"] = self._justify_to_anchor(text_align)
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
-        # self.widget = tk.Frame(parent, **self.props)
-        self.widget = ttk.Frame(parent, style=self.style_name, **self.props)
+        # if self.use_ttk:
+        #     self.widget = ttk.Frame(parent, style=self.style_name, **self.props)
+        self.widget = tk.Frame(parent, **self.props)
         return self.widget
 
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
     def update(self, *args, **kw) -> None:
@@ -1896,14 +1787,15 @@
                 enable_focus_events: bool = False,
                 size: tuple[int, int] = (50, 10), # element size (unit=character)
                 # text props
                 font: Union[FontType, None] = None, # font
                 color: Union[str, None] = None, # text color
                 text_color: Union[str, None] = None, # same as color
                 background_color: Union[str, None] = None, # background color
+                text_align: Union[TextAlign, None] = None, # text align
                 # pack props
                 expand_x: bool = False,
                 expand_y: bool = False,
                 pad: Union[PadType, None] = None,
                 # other
                 readonly_background_color: Union[str, None] = None,
                 metadata: Union[dict[str, Any], None] = None,
@@ -1912,14 +1804,15 @@
         super().__init__("Multiline", "", key, True, metadata, **kw)
         if default_text is not None:
             text = default_text
         self.props["text"] = text
         self.props["size"] = size
         self._set_text_props(font=font, color=color, text_color=text_color, background_color=background_color)
         self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
+        self.text_align = text_align
         if readonly_background_color is not None:
             self.readonly_background_color = readonly_background_color
         self.has_value = True
         self.readonly = readonly
         # bind events
         if enable_events:
             self.bind_events({
@@ -1938,17 +1831,22 @@
             }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         """Create a Multiline widget."""
         # text
         text = self.props.pop("text", "")
         # create
-        self.widget = scrolledtext.ScrolledText(parent, **self.props)
-        # set text
-        self.widget.insert("1.0", text)
+        self.widget: scrolledtext.ScrolledText = scrolledtext.ScrolledText(parent, **self.props)
+        # text_align
+        if self.text_align is not None:
+            self.widget.tag_configure(self.text_align, justify=self.text_align)
+            self.widget.insert("1.0", text, self.text_align)
+        else:
+            # set text
+            self.widget.insert("1.0", text)
         # readonly
         if self.readonly:
             self.set_readonly(self.readonly)
         return self.widget
 
     def get(self) -> Any:
         """Get the value of the widget."""
@@ -2017,16 +1915,21 @@
     def set_text(self, text: str) -> None:
         """Set text"""
         if self.widget is None:
             return
         if self.readonly:
             self._widget_update(state=tk.NORMAL)
         self.props["text"] = text
+        # clear text
         self.widget.delete("1.0", "end") # clear text
-        self.widget.insert("1.0", text) # set text
+        # set text
+        if self.text_align is not None:
+           self.widget.insert("1.0", text, self.text_align)
+        else:
+            self.widget.insert("1.0", text)
         if self.readonly:
             self._widget_update(state=tk.DISABLED)
     
     def get_selection_pos(self) -> tuple[str, str]:
         """Get selection position, returns (start_pos, end_pos)."""
         if self.widget is None:
             return ("", "")
@@ -2563,19 +2466,27 @@
             self.bind_events({
                 "<<ListboxSelect>>": "select"
             }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         """[Listbox.create] create Listbox widget"""
         self.window: Window = win
-        self.widget = tk.Listbox(parent, selectmode=self.select_mode, **self.props)
+        # create frame
+        self.widget_frame: tk.Frame = tk.Frame(parent)
+        # create listbox and scrollbar
+        self.widget:tk.Listbox = tk.Listbox(self.widget_frame, selectmode=self.select_mode, **self.props)
+        self.widget_scrollbar = tk.Scrollbar(self.widget_frame,command=self.widget.yview)
+        self.widget.config(yscrollcommand=self.widget_scrollbar.set)
+        # pack
+        self.widget.pack(side="left", fill="both", expand=True)
+        self.widget_scrollbar.pack(side="right", fill="y")
         # insert values
         self.set_values(self.values)
         self.select_values(self.default_values)
-        return self.widget
+        return self.widget_frame
 
     def select_values(self, values: list[str]) -> None:
         """Select values"""
         if self.widget is None:
             return
         for v in values:
             try:
@@ -2798,17 +2709,20 @@
         """Get the value of the widget."""
         if self.widget is None:
             return []
         record_ids = self.widget.focus()
         if self.event_returns_values:
             record_values = self.widget.item(record_ids, "values")
         else:
-            if isinstance(record_ids, str):
-                record_ids = [record_ids]
-            record_values = list(map(lambda id_s: int(id_s), record_ids))
+            if record_ids is None or record_ids == "":
+                record_values = []
+            else:
+                if isinstance(record_ids, str):
+                    record_ids = [record_ids]
+                record_values = list(map(lambda id_s: int(id_s), record_ids))
         return record_values
 
     def _table_events(self, _event: Any) -> None:
         """Handle events."""
         self.window._event_handler(self.key, {})
 
     def update(self, *args, **kw) -> None:
@@ -3016,53 +2930,14 @@
             title=self.title,
             default_color=self.default_color,
         )
         if (target is not None) and (result is not None) and (result != ""):
             target.update(result)
         return result
 
-
-#------------------------------------------------------------------------------
-# Utility functions
-#------------------------------------------------------------------------------
-
-# global variables
-# auto generate element key id
-_element_style_key_ids: dict[str, int] = {}
-_element_key_names: dict[str, bool] = {}
-def generate_element_style_key(element_type: str) -> int:
-    """Get a unique id for an element."""
-    element_type = element_type.lower()
-    if element_type not in _element_style_key_ids:
-        _element_style_key_ids[element_type] = 0
-    key: str = ""
-    while True:
-        _element_style_key_ids[element_type] += 1
-        element_id = _element_style_key_ids[element_type]
-        key = f"-{element_type}{element_id}-"
-        if key not in _element_key_names:
-            _element_key_names[key] = True
-            break
-    return key
-
-def register_element_key(key: str) -> bool:
-    """Register element key."""
-    if key in _element_key_names:
-        return False
-    _element_key_names[key] = True
-    return True
-
-_elements_with_value: int = 0
-def generate_element_id() -> int:
-    """Generate a unique id for a value element."""
-    global _elements_with_value
-    element_id = _elements_with_value
-    _elements_with_value += 1
-    return element_id
-
 def rgb(r: int, g: int, b: int) -> str:
     r = r & 0xFF
     g = g & 0xFF
     b = b & 0xFF
     return f"#{r:02x}{g:02x}{b:02x}"
 
 def image_resize(img: PILImage, size: tuple[int, int]) -> PILImage:
@@ -3127,7 +3002,44 @@
 def time_checker_start() -> datetime:
     return datetime.now()
 
 def time_checker_end(start_time: datetime) -> int:
     elapsed_time = (datetime.now() - start_time).total_seconds()
     msec = int(elapsed_time * 1000)
     return msec
+
+# get system info
+
+def get_tk_version() -> str:
+    """Get tk version"""
+    root = get_root_window()
+    tkversion = root.tk.call("info", "patchlevel")
+    return tkversion
+
+def get_tcl_version() -> str:
+    """Get tcl version"""
+    root = get_root_window()
+    tclversion = root.tk.call("info", "tclversion")
+    return tclversion
+
+def get_font_list() -> list[str]:
+    """Get font list"""
+    root = get_root_window()
+    root.withdraw()
+    return list(tkfont.families())
+
+def get_system_info():
+    # node={platform.node()}
+    py_ver = sys.version.replace('\n', '')
+    return f"""
+tkeasygui={version.__version__}
+python={py_ver}
+tcl_tk={get_tk_version()}
+os={platform.system()}
+os_version={platform.version()}
+os_release={platform.release()}
+architecture={platform.architecture()}
+processor={platform.processor()}
+    """.strip()
+
+
+_compatibility = utils._compatibility
```

### Comparing `tkeasygui-0.2.49/TkEasyGUI.egg-info/PKG-INFO` & `tkeasygui-0.2.55/TkEasyGUI.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.49
+Version: 0.2.55
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -45,26 +45,30 @@
 License-File: LICENSE
 Requires-Dist: Pillow
 Requires-Dist: pyperclip
 
 # TkEasyGUI
 
 `TkEasyGUI` is a Python library that allows for the easy and simple creation of GUI applications.
-In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
 
-Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
+<img src="https://github.com/kujirahand/tkeasygui-python/raw/main/docs/image/logo-button.jpg" width="180" alt="TkEasyGUI Logo">
 
-This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
+- Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
+- In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
+- This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
 
 - [👉日本語](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md) / [👉中文](https://github.com/kujirahand/tkeasygui-python/blob/main/README-zh.md)
 
+
 ## Platform
 
 - Windows / macOS / Linux (Tkinter required)
 
+<img src="https://github.com/kujirahand/tkeasygui-python/raw/main/docs/image/tkeasygui-shot640.jpg" width="300" alt="TkEasyGUI">
+
 ## Install
 
 Install from pypi
 
 
 ```sh
 python -m pip install TkEasyGUI
@@ -77,14 +81,23 @@
 python -m pip install git+https://github.com/kujirahand/tkeasygui-python
 ```
 
 - (memo) Updating from older versions (less than 0.2.24) will fail. ([See the solution](https://github.com/kujirahand/tkeasygui-python/blob/main/docs/installation_trouble.md))
 
 ## How to use
 
+Using TkEasyGUI is simple. If you only want to display a dialog, it requires just two lines of code.
+
+```py
+import TkEasyGUI as eg
+eg.popup("A joyful heart is good medicine.")
+```
+
+###
+
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
 import TkEasyGUI as eg
 # define layout
 layout = [[eg.Text("Hello, World!")],
           [eg.Button("Exit")]]
```

### Comparing `tkeasygui-0.2.49/pyproject.toml` & `tkeasygui-0.2.55/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TkEasyGUI"
-version = "0.2.49"
+version = "0.2.55"
 dependencies = [
   "Pillow",
   "pyperclip",
 ]
 requires-python = ">=3.9"
 authors = [
   { name="kujirahand", email="web@kujirahand.com" },
```

