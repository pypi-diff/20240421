# Comparing `tmp/tsformatter-0.2.0.tar.gz` & `tmp/tsformatter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsformatter-0.2.0.tar", last modified: Mon Nov  7 18:18:29 2022, max compression
+gzip compressed data, was "tsformatter-0.2.1.tar", last modified: Sun Apr 21 18:36:06 2024, max compression
```

## Comparing `tsformatter-0.2.0.tar` & `tsformatter-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-11-07 18:18:29.125755 tsformatter-0.2.0/
--rw-rw-rw-   0        0        0     1083 2022-02-11 17:23:52.000000 tsformatter-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4728 2022-11-07 18:18:29.124739 tsformatter-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4280 2022-10-18 20:59:22.000000 tsformatter-0.2.0/README.md
--rw-rw-rw-   0        0        0      958 2022-11-07 18:18:06.000000 tsformatter-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-07 18:18:29.125755 tsformatter-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-11-07 18:18:29.123751 tsformatter-0.2.0/tsformatter.egg-info/
--rw-rw-rw-   0        0        0     4728 2022-11-07 18:18:29.000000 tsformatter-0.2.0/tsformatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2022-11-07 18:18:29.000000 tsformatter-0.2.0/tsformatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-07 18:18:29.000000 tsformatter-0.2.0/tsformatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2022-11-07 18:18:29.000000 tsformatter-0.2.0/tsformatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-11-07 18:18:29.000000 tsformatter-0.2.0/tsformatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3029 2022-10-18 20:18:19.000000 tsformatter-0.2.0/tsformatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:36:06.521929 tsformatter-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-21 18:36:00.000000 tsformatter-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-21 18:36:06.521929 tsformatter-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-21 18:36:00.000000 tsformatter-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-21 18:36:00.000000 tsformatter-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 18:36:06.521929 tsformatter-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:36:06.517929 tsformatter-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-21 18:36:00.000000 tsformatter-0.2.1/tests/test_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:36:06.521929 tsformatter-0.2.1/tsformatter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-21 18:36:00.000000 tsformatter-0.2.1/tsformatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 18:36:00.000000 tsformatter-0.2.1/tsformatter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 18:36:06.521929 tsformatter-0.2.1/tsformatter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-21 18:36:06.000000 tsformatter-0.2.1/tsformatter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-21 18:36:06.000000 tsformatter-0.2.1/tsformatter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 18:36:06.000000 tsformatter-0.2.1/tsformatter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-21 18:36:06.000000 tsformatter-0.2.1/tsformatter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 18:36:06.000000 tsformatter-0.2.1/tsformatter.egg-info/top_level.txt
```

### Comparing `tsformatter-0.2.0/PKG-INFO` & `tsformatter-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,161 +1,164 @@
-Metadata-Version: 2.1
-Name: tsformatter
-Version: 0.2.0
-Summary: Helper package to format TeamSpeak BBCode
-Author: 0x4aK
-Project-URL: Homepage, https://github.com/0x4aK/tsformatter
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
-# TSFormatter
-
-Helper package to format TeamSpeak BBCode
-
-## 📦 Installation
-
-```shell
-pip install tsformatter
-```
-
-## ✏️ Usage
-
-importing the formatter
-
-```python
-from tsformatter import formatter
-```
-
-### Colors
-
-```python
-# Using HTML color name
->>> formatter.color("red", "This text is red")
-'[COLOR=red]This text is red[/COLOR]'
-
->>> formatter.color("PaleTurquoise", "This text is turquoise")
-'[COLOR=PaleTurquoise]This text is turquoise[/COLOR]'
-
-
-# Using Hex Triplet
->>> formatter.color("#f00", "This text is red")
-'[COLOR=f00]This text is red[/COLOR]'
-
->>> formatter.color("#AFEEEE", "This text is turquoise")
-'[COLOR=#AFEEEE]This text is turquoise[/COLOR]'
-```
-
-### Horizontal line
-
-```python
->>> formatter.hr
-'[HR]'
-```
-
-### Images
-
-```python
->>> formatter.img("https://i.imgur.com/ml09ccU.png")
-'[IMG]https://i.imgur.com/ml09ccU.png[/IMG]'
-```
-
-### Links
-
-```python
-# Without specifying link text
->>> formatter.link("https://www.teamspeak.com/")
-'[URL]https://www.teamspeak.com/[/URL]'
-
-# With a link text
-formatter.link("https://www.teamspeak.com/", "TeamSpeak Website")
-'[URL=https://www.teamspeak.com/]TeamSpeak Website[/URL]'
-```
-
-### Lists
-
-```python
-# Default style of the list is bullet list
->>> formatter.list_(f"List item #{x}" for x in range(1, 6))
-'[LIST]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
-
-
-# You can specify the style of the list
->>> formatter.list_((f"List item #{x}" for x in range(1, 6)), style="1")
-'[LIST=1]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
-```
-
-#### List styles that work:
-
-| Style   |                    "1"                    |                       "a"                        |                      "i"                      |                      "A"                      |                      "I"                      |
-| ------- | :---------------------------------------: | :----------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: |
-| Renders | ![numberic](.github/img/list_numeric.png) | ![alpha lower](.github/img/list_alpha_lower.png) | ![numberic](.github/img/list_roman_lower.png) | ![numberic](.github/img/list_alpha_upper.png) | ![numberic](.github/img/list_roman_upper.png) |
-
-### Placement
-
-```python
->>> formatter.left("Formatted to the left")
-'[LEFT]Formatted to the left[/LEFT]'
-
->>> formatter.right("Formatted to the right")
-'[RIGHT]Formatted to the right[/RIGHT]'
-
->>> formatter.center("Center of the space")
-'[CENTER]Center of the space[/CENTER]'
-```
-
-### Size
-
-```python
-# Using absolute sizes
->>> formatter.size(24, "I am huge!")
-'[SIZE=24]I am huge![/SIZE]'
-
-# Relative sizes can be either positive or negative
->>> formatter.size('-4', "I am 4 units smaller than the rest")
-'[SIZE=-2]I am 2 units smaller than the rest[/SIZE]'
-
->>> formatter.size('+2', "I am 2 units bigger than the rest")
-'[SIZE=+2]I am 2 units bigger than the rest[/SIZE]'
-```
-
-### Styles
-
-```python
->>> formatter.bold("Example text")
-'[B]Example text[/B]'
-
->>> formatter.italic("Example text")
-'[I]Example text[/I]'
-
->>> formatter.underline("Example text")
-'[U]Example text[/U]'
-
->>> formatter.strike("Example text")
-'[S]Example text[/S]'
-```
-
-### Tables
-
-```python
-
->>> header = ("Place", "City", "Date")
->>> data1 = ("Statue of Liberty", "New York City", "October 28, 1886")
->>> data2 = ("Eiffel Tower", "Paris", "31 March, 1889")
->>> data3 = ("Big Ben", "London", "31 May, 1859")
-
->>> formatter.table(
-        formatter.table_header_row(header),
-        formatter.table_row(data1),
-        formatter.table_row(data2),
-        formatter.table_row(data3)
-    )
-'[TABLE]\n[TR][TH]Place[/TH][TH]City[/TH][TH]Date[/TH][/TR]\n[TR][TD]Statue of Liberty[/TD][TD]New York City[/TD][TD]October 28, 1886[/TD][/TR]\n[TR][TD]Eiffel Tower[/TD][TD]Paris[/TD][TD]31 March, 1889[/TD][/TR]\n[TR][TD]Big Ben[/TD][TD]London[/TD][TD]31 May, 1859[/TD][/TR]\n[/TABLE]'
-```
-
-#### Results when rendered by TeamSpeak client:
-
-![table example](.github/img/table.png)
+Metadata-Version: 2.1
+Name: tsformatter
+Version: 0.2.1
+Summary: Helper package to format TeamSpeak BBCode
+Author: 0x4aK
+Project-URL: Homepage, https://github.com/0x4aK/tsformatter
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: tests
+Requires-Dist: mypy>=1.9.0; extra == "tests"
+Requires-Dist: pytest==8.1.1; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
+
+# TSFormatter
+
+Helper package to format TeamSpeak BBCode
+
+## 📦 Installation
+
+```shell
+pip install tsformatter
+```
+
+## ✏️ Usage
+
+importing the formatter
+
+```python
+import tsformatter
+```
+
+### Colors
+
+```python
+# Using HTML color name
+>>> tsformatter.color("red", "This text is red")
+'[COLOR=red]This text is red[/COLOR]'
+
+>>> tsformatter.color("PaleTurquoise", "This text is turquoise")
+'[COLOR=PaleTurquoise]This text is turquoise[/COLOR]'
+
+
+# Using Hex Triplet
+>>> tsformatter.color("#f00", "This text is red")
+'[COLOR=f00]This text is red[/COLOR]'
+
+>>> tsformatter.color("#AFEEEE", "This text is turquoise")
+'[COLOR=#AFEEEE]This text is turquoise[/COLOR]'
+```
+
+### Horizontal line
+
+```python
+>>> tsformatter.hr
+'[HR]'
+```
+
+### Images
+
+```python
+>>> tsformatter.img("https://i.imgur.com/ml09ccU.png")
+'[IMG]https://i.imgur.com/ml09ccU.png[/IMG]'
+```
+
+### Links
+
+```python
+# Without specifying link text
+>>> tsformatter.link("https://www.teamspeak.com/")
+'[URL]https://www.teamspeak.com/[/URL]'
+
+# With a link text
+>>> tsformatter.link("https://www.teamspeak.com/", "TeamSpeak Website")
+'[URL=https://www.teamspeak.com/]TeamSpeak Website[/URL]'
+```
+
+### Lists
+
+```python
+# Default style of the list is bullet list
+>>> tsformatter.list_(f"List item #{x}" for x in range(1, 6))
+'[LIST]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
+
+
+# You can specify the style of the list
+>>> tsformatter.list_((f"List item #{x}" for x in range(1, 6)), style="1")
+'[LIST=1]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
+```
+
+#### List styles that work:
+
+| Style   |                    "1"                    |                       "a"                        |                      "i"                      |                      "A"                      |                      "I"                      |
+| ------- | :---------------------------------------: | :----------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: |
+| Renders | ![numberic](.github/img/list_numeric.png) | ![alpha lower](.github/img/list_alpha_lower.png) | ![numberic](.github/img/list_roman_lower.png) | ![numberic](.github/img/list_alpha_upper.png) | ![numberic](.github/img/list_roman_upper.png) |
+
+### Placement
+
+```python
+>>> tsformatter.left("Formatted to the left")
+'[LEFT]Formatted to the left[/LEFT]'
+
+>>> tsformatter.right("Formatted to the right")
+'[RIGHT]Formatted to the right[/RIGHT]'
+
+>>> tsformatter.center("Center of the space")
+'[CENTER]Center of the space[/CENTER]'
+```
+
+### Size
+
+```python
+# Using absolute sizes
+>>> tsformatter.size(24, "I am huge!")
+'[SIZE=24]I am huge![/SIZE]'
+
+# Relative sizes can be either positive or negative
+>>> tsformatter.size('-4', "I am 4 units smaller than the rest")
+'[SIZE=-2]I am 2 units smaller than the rest[/SIZE]'
+
+>>> tsformatter.size('+2', "I am 2 units bigger than the rest")
+'[SIZE=+2]I am 2 units bigger than the rest[/SIZE]'
+```
+
+### Styles
+
+```python
+>>> tsformatter.bold("Example text")
+'[B]Example text[/B]'
+
+>>> tsformatter.italic("Example text")
+'[I]Example text[/I]'
+
+>>> tsformatter.underline("Example text")
+'[U]Example text[/U]'
+
+>>> tsformatter.strike("Example text")
+'[S]Example text[/S]'
+```
+
+### Tables
+
+```python
+
+>>> header = ("Place", "City", "Date")
+>>> data1 = ("Statue of Liberty", "New York City", "October 28, 1886")
+>>> data2 = ("Eiffel Tower", "Paris", "31 March, 1889")
+>>> data3 = ("Big Ben", "London", "31 May, 1859")
+
+>>> tsformatter.table(
+        tsformatter.table_header_row(header),
+        tsformatter.table_row(data1),
+        tsformatter.table_row(data2),
+        tsformatter.table_row(data3)
+    )
+'[TABLE]\n[TR][TH]Place[/TH][TH]City[/TH][TH]Date[/TH][/TR]\n[TR][TD]Statue of Liberty[/TD][TD]New York City[/TD][TD]October 28, 1886[/TD][/TR]\n[TR][TD]Eiffel Tower[/TD][TD]Paris[/TD][TD]31 March, 1889[/TD][/TR]\n[TR][TD]Big Ben[/TD][TD]London[/TD][TD]31 May, 1859[/TD][/TR]\n[/TABLE]'
+```
+
+#### Results when rendered by TeamSpeak client:
+
+![table example](.github/img/table.png)
```

### Comparing `tsformatter-0.2.0/README.md` & `tsformatter-0.2.1/tsformatter.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,147 +1,164 @@
-# TSFormatter
-
-Helper package to format TeamSpeak BBCode
-
-## 📦 Installation
-
-```shell
-pip install tsformatter
-```
-
-## ✏️ Usage
-
-importing the formatter
-
-```python
-from tsformatter import formatter
-```
-
-### Colors
-
-```python
-# Using HTML color name
->>> formatter.color("red", "This text is red")
-'[COLOR=red]This text is red[/COLOR]'
-
->>> formatter.color("PaleTurquoise", "This text is turquoise")
-'[COLOR=PaleTurquoise]This text is turquoise[/COLOR]'
-
-
-# Using Hex Triplet
->>> formatter.color("#f00", "This text is red")
-'[COLOR=f00]This text is red[/COLOR]'
-
->>> formatter.color("#AFEEEE", "This text is turquoise")
-'[COLOR=#AFEEEE]This text is turquoise[/COLOR]'
-```
-
-### Horizontal line
-
-```python
->>> formatter.hr
-'[HR]'
-```
-
-### Images
-
-```python
->>> formatter.img("https://i.imgur.com/ml09ccU.png")
-'[IMG]https://i.imgur.com/ml09ccU.png[/IMG]'
-```
-
-### Links
-
-```python
-# Without specifying link text
->>> formatter.link("https://www.teamspeak.com/")
-'[URL]https://www.teamspeak.com/[/URL]'
-
-# With a link text
-formatter.link("https://www.teamspeak.com/", "TeamSpeak Website")
-'[URL=https://www.teamspeak.com/]TeamSpeak Website[/URL]'
-```
-
-### Lists
-
-```python
-# Default style of the list is bullet list
->>> formatter.list_(f"List item #{x}" for x in range(1, 6))
-'[LIST]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
-
-
-# You can specify the style of the list
->>> formatter.list_((f"List item #{x}" for x in range(1, 6)), style="1")
-'[LIST=1]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
-```
-
-#### List styles that work:
-
-| Style   |                    "1"                    |                       "a"                        |                      "i"                      |                      "A"                      |                      "I"                      |
-| ------- | :---------------------------------------: | :----------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: |
-| Renders | ![numberic](.github/img/list_numeric.png) | ![alpha lower](.github/img/list_alpha_lower.png) | ![numberic](.github/img/list_roman_lower.png) | ![numberic](.github/img/list_alpha_upper.png) | ![numberic](.github/img/list_roman_upper.png) |
-
-### Placement
-
-```python
->>> formatter.left("Formatted to the left")
-'[LEFT]Formatted to the left[/LEFT]'
-
->>> formatter.right("Formatted to the right")
-'[RIGHT]Formatted to the right[/RIGHT]'
-
->>> formatter.center("Center of the space")
-'[CENTER]Center of the space[/CENTER]'
-```
-
-### Size
-
-```python
-# Using absolute sizes
->>> formatter.size(24, "I am huge!")
-'[SIZE=24]I am huge![/SIZE]'
-
-# Relative sizes can be either positive or negative
->>> formatter.size('-4', "I am 4 units smaller than the rest")
-'[SIZE=-2]I am 2 units smaller than the rest[/SIZE]'
-
->>> formatter.size('+2', "I am 2 units bigger than the rest")
-'[SIZE=+2]I am 2 units bigger than the rest[/SIZE]'
-```
-
-### Styles
-
-```python
->>> formatter.bold("Example text")
-'[B]Example text[/B]'
-
->>> formatter.italic("Example text")
-'[I]Example text[/I]'
-
->>> formatter.underline("Example text")
-'[U]Example text[/U]'
-
->>> formatter.strike("Example text")
-'[S]Example text[/S]'
-```
-
-### Tables
-
-```python
-
->>> header = ("Place", "City", "Date")
->>> data1 = ("Statue of Liberty", "New York City", "October 28, 1886")
->>> data2 = ("Eiffel Tower", "Paris", "31 March, 1889")
->>> data3 = ("Big Ben", "London", "31 May, 1859")
-
->>> formatter.table(
-        formatter.table_header_row(header),
-        formatter.table_row(data1),
-        formatter.table_row(data2),
-        formatter.table_row(data3)
-    )
-'[TABLE]\n[TR][TH]Place[/TH][TH]City[/TH][TH]Date[/TH][/TR]\n[TR][TD]Statue of Liberty[/TD][TD]New York City[/TD][TD]October 28, 1886[/TD][/TR]\n[TR][TD]Eiffel Tower[/TD][TD]Paris[/TD][TD]31 March, 1889[/TD][/TR]\n[TR][TD]Big Ben[/TD][TD]London[/TD][TD]31 May, 1859[/TD][/TR]\n[/TABLE]'
-```
-
-#### Results when rendered by TeamSpeak client:
-
-![table example](.github/img/table.png)
+Metadata-Version: 2.1
+Name: tsformatter
+Version: 0.2.1
+Summary: Helper package to format TeamSpeak BBCode
+Author: 0x4aK
+Project-URL: Homepage, https://github.com/0x4aK/tsformatter
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: tests
+Requires-Dist: mypy>=1.9.0; extra == "tests"
+Requires-Dist: pytest==8.1.1; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
+
+# TSFormatter
+
+Helper package to format TeamSpeak BBCode
+
+## 📦 Installation
+
+```shell
+pip install tsformatter
+```
+
+## ✏️ Usage
+
+importing the formatter
+
+```python
+import tsformatter
+```
+
+### Colors
+
+```python
+# Using HTML color name
+>>> tsformatter.color("red", "This text is red")
+'[COLOR=red]This text is red[/COLOR]'
+
+>>> tsformatter.color("PaleTurquoise", "This text is turquoise")
+'[COLOR=PaleTurquoise]This text is turquoise[/COLOR]'
+
+
+# Using Hex Triplet
+>>> tsformatter.color("#f00", "This text is red")
+'[COLOR=f00]This text is red[/COLOR]'
+
+>>> tsformatter.color("#AFEEEE", "This text is turquoise")
+'[COLOR=#AFEEEE]This text is turquoise[/COLOR]'
+```
+
+### Horizontal line
+
+```python
+>>> tsformatter.hr
+'[HR]'
+```
+
+### Images
+
+```python
+>>> tsformatter.img("https://i.imgur.com/ml09ccU.png")
+'[IMG]https://i.imgur.com/ml09ccU.png[/IMG]'
+```
+
+### Links
+
+```python
+# Without specifying link text
+>>> tsformatter.link("https://www.teamspeak.com/")
+'[URL]https://www.teamspeak.com/[/URL]'
+
+# With a link text
+>>> tsformatter.link("https://www.teamspeak.com/", "TeamSpeak Website")
+'[URL=https://www.teamspeak.com/]TeamSpeak Website[/URL]'
+```
+
+### Lists
+
+```python
+# Default style of the list is bullet list
+>>> tsformatter.list_(f"List item #{x}" for x in range(1, 6))
+'[LIST]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
+
+
+# You can specify the style of the list
+>>> tsformatter.list_((f"List item #{x}" for x in range(1, 6)), style="1")
+'[LIST=1]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
+```
+
+#### List styles that work:
+
+| Style   |                    "1"                    |                       "a"                        |                      "i"                      |                      "A"                      |                      "I"                      |
+| ------- | :---------------------------------------: | :----------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: |
+| Renders | ![numberic](.github/img/list_numeric.png) | ![alpha lower](.github/img/list_alpha_lower.png) | ![numberic](.github/img/list_roman_lower.png) | ![numberic](.github/img/list_alpha_upper.png) | ![numberic](.github/img/list_roman_upper.png) |
+
+### Placement
+
+```python
+>>> tsformatter.left("Formatted to the left")
+'[LEFT]Formatted to the left[/LEFT]'
+
+>>> tsformatter.right("Formatted to the right")
+'[RIGHT]Formatted to the right[/RIGHT]'
+
+>>> tsformatter.center("Center of the space")
+'[CENTER]Center of the space[/CENTER]'
+```
+
+### Size
+
+```python
+# Using absolute sizes
+>>> tsformatter.size(24, "I am huge!")
+'[SIZE=24]I am huge![/SIZE]'
+
+# Relative sizes can be either positive or negative
+>>> tsformatter.size('-4', "I am 4 units smaller than the rest")
+'[SIZE=-2]I am 2 units smaller than the rest[/SIZE]'
+
+>>> tsformatter.size('+2', "I am 2 units bigger than the rest")
+'[SIZE=+2]I am 2 units bigger than the rest[/SIZE]'
+```
+
+### Styles
+
+```python
+>>> tsformatter.bold("Example text")
+'[B]Example text[/B]'
+
+>>> tsformatter.italic("Example text")
+'[I]Example text[/I]'
+
+>>> tsformatter.underline("Example text")
+'[U]Example text[/U]'
+
+>>> tsformatter.strike("Example text")
+'[S]Example text[/S]'
+```
+
+### Tables
+
+```python
+
+>>> header = ("Place", "City", "Date")
+>>> data1 = ("Statue of Liberty", "New York City", "October 28, 1886")
+>>> data2 = ("Eiffel Tower", "Paris", "31 March, 1889")
+>>> data3 = ("Big Ben", "London", "31 May, 1859")
+
+>>> tsformatter.table(
+        tsformatter.table_header_row(header),
+        tsformatter.table_row(data1),
+        tsformatter.table_row(data2),
+        tsformatter.table_row(data3)
+    )
+'[TABLE]\n[TR][TH]Place[/TH][TH]City[/TH][TH]Date[/TH][/TR]\n[TR][TD]Statue of Liberty[/TD][TD]New York City[/TD][TD]October 28, 1886[/TD][/TR]\n[TR][TD]Eiffel Tower[/TD][TD]Paris[/TD][TD]31 March, 1889[/TD][/TR]\n[TR][TD]Big Ben[/TD][TD]London[/TD][TD]31 May, 1859[/TD][/TR]\n[/TABLE]'
+```
+
+#### Results when rendered by TeamSpeak client:
+
+![table example](.github/img/table.png)
```

### Comparing `tsformatter-0.2.0/tsformatter.egg-info/PKG-INFO` & `tsformatter-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,147 @@
-Metadata-Version: 2.1
-Name: tsformatter
-Version: 0.2.0
-Summary: Helper package to format TeamSpeak BBCode
-Author: 0x4aK
-Project-URL: Homepage, https://github.com/0x4aK/tsformatter
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
-# TSFormatter
-
-Helper package to format TeamSpeak BBCode
-
-## 📦 Installation
-
-```shell
-pip install tsformatter
-```
-
-## ✏️ Usage
-
-importing the formatter
-
-```python
-from tsformatter import formatter
-```
-
-### Colors
-
-```python
-# Using HTML color name
->>> formatter.color("red", "This text is red")
-'[COLOR=red]This text is red[/COLOR]'
-
->>> formatter.color("PaleTurquoise", "This text is turquoise")
-'[COLOR=PaleTurquoise]This text is turquoise[/COLOR]'
-
-
-# Using Hex Triplet
->>> formatter.color("#f00", "This text is red")
-'[COLOR=f00]This text is red[/COLOR]'
-
->>> formatter.color("#AFEEEE", "This text is turquoise")
-'[COLOR=#AFEEEE]This text is turquoise[/COLOR]'
-```
-
-### Horizontal line
-
-```python
->>> formatter.hr
-'[HR]'
-```
-
-### Images
-
-```python
->>> formatter.img("https://i.imgur.com/ml09ccU.png")
-'[IMG]https://i.imgur.com/ml09ccU.png[/IMG]'
-```
-
-### Links
-
-```python
-# Without specifying link text
->>> formatter.link("https://www.teamspeak.com/")
-'[URL]https://www.teamspeak.com/[/URL]'
-
-# With a link text
-formatter.link("https://www.teamspeak.com/", "TeamSpeak Website")
-'[URL=https://www.teamspeak.com/]TeamSpeak Website[/URL]'
-```
-
-### Lists
-
-```python
-# Default style of the list is bullet list
->>> formatter.list_(f"List item #{x}" for x in range(1, 6))
-'[LIST]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
-
-
-# You can specify the style of the list
->>> formatter.list_((f"List item #{x}" for x in range(1, 6)), style="1")
-'[LIST=1]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
-```
-
-#### List styles that work:
-
-| Style   |                    "1"                    |                       "a"                        |                      "i"                      |                      "A"                      |                      "I"                      |
-| ------- | :---------------------------------------: | :----------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: |
-| Renders | ![numberic](.github/img/list_numeric.png) | ![alpha lower](.github/img/list_alpha_lower.png) | ![numberic](.github/img/list_roman_lower.png) | ![numberic](.github/img/list_alpha_upper.png) | ![numberic](.github/img/list_roman_upper.png) |
-
-### Placement
-
-```python
->>> formatter.left("Formatted to the left")
-'[LEFT]Formatted to the left[/LEFT]'
-
->>> formatter.right("Formatted to the right")
-'[RIGHT]Formatted to the right[/RIGHT]'
-
->>> formatter.center("Center of the space")
-'[CENTER]Center of the space[/CENTER]'
-```
-
-### Size
-
-```python
-# Using absolute sizes
->>> formatter.size(24, "I am huge!")
-'[SIZE=24]I am huge![/SIZE]'
-
-# Relative sizes can be either positive or negative
->>> formatter.size('-4', "I am 4 units smaller than the rest")
-'[SIZE=-2]I am 2 units smaller than the rest[/SIZE]'
-
->>> formatter.size('+2', "I am 2 units bigger than the rest")
-'[SIZE=+2]I am 2 units bigger than the rest[/SIZE]'
-```
-
-### Styles
-
-```python
->>> formatter.bold("Example text")
-'[B]Example text[/B]'
-
->>> formatter.italic("Example text")
-'[I]Example text[/I]'
-
->>> formatter.underline("Example text")
-'[U]Example text[/U]'
-
->>> formatter.strike("Example text")
-'[S]Example text[/S]'
-```
-
-### Tables
-
-```python
-
->>> header = ("Place", "City", "Date")
->>> data1 = ("Statue of Liberty", "New York City", "October 28, 1886")
->>> data2 = ("Eiffel Tower", "Paris", "31 March, 1889")
->>> data3 = ("Big Ben", "London", "31 May, 1859")
-
->>> formatter.table(
-        formatter.table_header_row(header),
-        formatter.table_row(data1),
-        formatter.table_row(data2),
-        formatter.table_row(data3)
-    )
-'[TABLE]\n[TR][TH]Place[/TH][TH]City[/TH][TH]Date[/TH][/TR]\n[TR][TD]Statue of Liberty[/TD][TD]New York City[/TD][TD]October 28, 1886[/TD][/TR]\n[TR][TD]Eiffel Tower[/TD][TD]Paris[/TD][TD]31 March, 1889[/TD][/TR]\n[TR][TD]Big Ben[/TD][TD]London[/TD][TD]31 May, 1859[/TD][/TR]\n[/TABLE]'
-```
-
-#### Results when rendered by TeamSpeak client:
-
-![table example](.github/img/table.png)
+# TSFormatter
+
+Helper package to format TeamSpeak BBCode
+
+## 📦 Installation
+
+```shell
+pip install tsformatter
+```
+
+## ✏️ Usage
+
+importing the formatter
+
+```python
+import tsformatter
+```
+
+### Colors
+
+```python
+# Using HTML color name
+>>> tsformatter.color("red", "This text is red")
+'[COLOR=red]This text is red[/COLOR]'
+
+>>> tsformatter.color("PaleTurquoise", "This text is turquoise")
+'[COLOR=PaleTurquoise]This text is turquoise[/COLOR]'
+
+
+# Using Hex Triplet
+>>> tsformatter.color("#f00", "This text is red")
+'[COLOR=f00]This text is red[/COLOR]'
+
+>>> tsformatter.color("#AFEEEE", "This text is turquoise")
+'[COLOR=#AFEEEE]This text is turquoise[/COLOR]'
+```
+
+### Horizontal line
+
+```python
+>>> tsformatter.hr
+'[HR]'
+```
+
+### Images
+
+```python
+>>> tsformatter.img("https://i.imgur.com/ml09ccU.png")
+'[IMG]https://i.imgur.com/ml09ccU.png[/IMG]'
+```
+
+### Links
+
+```python
+# Without specifying link text
+>>> tsformatter.link("https://www.teamspeak.com/")
+'[URL]https://www.teamspeak.com/[/URL]'
+
+# With a link text
+>>> tsformatter.link("https://www.teamspeak.com/", "TeamSpeak Website")
+'[URL=https://www.teamspeak.com/]TeamSpeak Website[/URL]'
+```
+
+### Lists
+
+```python
+# Default style of the list is bullet list
+>>> tsformatter.list_(f"List item #{x}" for x in range(1, 6))
+'[LIST]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
+
+
+# You can specify the style of the list
+>>> tsformatter.list_((f"List item #{x}" for x in range(1, 6)), style="1")
+'[LIST=1]\n[*]List item #1\n[*]List item #2\n[*]List item #3\n[*]List item #4\n[*]List item #5\n[/LIST]'
+```
+
+#### List styles that work:
+
+| Style   |                    "1"                    |                       "a"                        |                      "i"                      |                      "A"                      |                      "I"                      |
+| ------- | :---------------------------------------: | :----------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: | :-------------------------------------------: |
+| Renders | ![numberic](.github/img/list_numeric.png) | ![alpha lower](.github/img/list_alpha_lower.png) | ![numberic](.github/img/list_roman_lower.png) | ![numberic](.github/img/list_alpha_upper.png) | ![numberic](.github/img/list_roman_upper.png) |
+
+### Placement
+
+```python
+>>> tsformatter.left("Formatted to the left")
+'[LEFT]Formatted to the left[/LEFT]'
+
+>>> tsformatter.right("Formatted to the right")
+'[RIGHT]Formatted to the right[/RIGHT]'
+
+>>> tsformatter.center("Center of the space")
+'[CENTER]Center of the space[/CENTER]'
+```
+
+### Size
+
+```python
+# Using absolute sizes
+>>> tsformatter.size(24, "I am huge!")
+'[SIZE=24]I am huge![/SIZE]'
+
+# Relative sizes can be either positive or negative
+>>> tsformatter.size('-4', "I am 4 units smaller than the rest")
+'[SIZE=-2]I am 2 units smaller than the rest[/SIZE]'
+
+>>> tsformatter.size('+2', "I am 2 units bigger than the rest")
+'[SIZE=+2]I am 2 units bigger than the rest[/SIZE]'
+```
+
+### Styles
+
+```python
+>>> tsformatter.bold("Example text")
+'[B]Example text[/B]'
+
+>>> tsformatter.italic("Example text")
+'[I]Example text[/I]'
+
+>>> tsformatter.underline("Example text")
+'[U]Example text[/U]'
+
+>>> tsformatter.strike("Example text")
+'[S]Example text[/S]'
+```
+
+### Tables
+
+```python
+
+>>> header = ("Place", "City", "Date")
+>>> data1 = ("Statue of Liberty", "New York City", "October 28, 1886")
+>>> data2 = ("Eiffel Tower", "Paris", "31 March, 1889")
+>>> data3 = ("Big Ben", "London", "31 May, 1859")
+
+>>> tsformatter.table(
+        tsformatter.table_header_row(header),
+        tsformatter.table_row(data1),
+        tsformatter.table_row(data2),
+        tsformatter.table_row(data3)
+    )
+'[TABLE]\n[TR][TH]Place[/TH][TH]City[/TH][TH]Date[/TH][/TR]\n[TR][TD]Statue of Liberty[/TD][TD]New York City[/TD][TD]October 28, 1886[/TD][/TR]\n[TR][TD]Eiffel Tower[/TD][TD]Paris[/TD][TD]31 March, 1889[/TD][/TR]\n[TR][TD]Big Ben[/TD][TD]London[/TD][TD]31 May, 1859[/TD][/TR]\n[/TABLE]'
+```
+
+#### Results when rendered by TeamSpeak client:
+
+![table example](.github/img/table.png)
```

