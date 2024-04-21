# Comparing `tmp/jdDBusDebugger-2.0.tar.gz` & `tmp/jddbusdebugger-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdDBusDebugger-2.0.tar", last modified: Wed Jan 31 18:05:15 2024, max compression
+gzip compressed data, was "jddbusdebugger-3.0.tar", last modified: Sun Apr 21 15:11:43 2024, max compression
```

## Comparing `jdDBusDebugger-2.0.tar` & `jddbusdebugger-3.0.tar`

### file list

```diff
@@ -1,84 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:05:15.062427 jdDBusDebugger-2.0/
--rw-r--r--   0 root         (0) root         (0)     2870 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/BuildBackend.py
--rw-r--r--   0 root         (0) root         (0)    35087 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      243 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4913 2024-01-31 18:05:15.062427 jdDBusDebugger-2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3792 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:05:15.054427 jdDBusDebugger-2.0/jdDBusDebugger/
--rw-r--r--   0 root         (0) root         (0)       60 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/Constants.py
--rw-r--r--   0 root         (0) root         (0)     1828 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/Environment.py
--rw-r--r--   0 root         (0) root         (0)     1622 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/Functions.py
--rw-r--r--   0 root         (0) root         (0)   125260 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/Icon.png
--rw-r--r--   0 root         (0) root         (0)     1446 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:05:15.054427 jdDBusDebugger-2.0/jdDBusDebugger/core/
--rw-r--r--   0 root         (0) root         (0)      299 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/core/Languages.py
--rw-r--r--   0 root         (0) root         (0)     3416 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/core/MacroManager.py
--rw-r--r--   0 root         (0) root         (0)     1501 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/core/Settings.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:05:15.054427 jdDBusDebugger-2.0/jdDBusDebugger/data/
--rw-r--r--   0 root         (0) root         (0)      176 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/data/changelog.html
--rw-r--r--   0 root         (0) root         (0)       39 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/data/translators.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:05:15.054427 jdDBusDebugger-2.0/jdDBusDebugger/gui/
--rw-r--r--   0 root         (0) root         (0)     1777 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/AboutDialog.py
--rw-r--r--   0 root         (0) root         (0)    22723 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/CentralWidget.py
--rw-r--r--   0 root         (0) root         (0)     2262 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/ConnectDialog.py
--rw-r--r--   0 root         (0) root         (0)     1499 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/EmitSignalDialog.py
--rw-r--r--   0 root         (0) root         (0)     1489 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/GenerateScriptDialog.py
--rw-r--r--   0 root         (0) root         (0)    10704 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/MainWindow.py
--rw-r--r--   0 root         (0) root         (0)     6124 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/ManageMacrosDialog.py
--rw-r--r--   0 root         (0) root         (0)     3074 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/SettingsDialog.py
--rw-r--r--   0 root         (0) root         (0)      939 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/WelcomeDialog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:05:15.058427 jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/
--rw-r--r--   0 root         (0) root         (0)     2798 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/ArgumentInput.py
--rw-r--r--   0 root         (0) root         (0)     3443 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/ArrayInput.py
--rw-r--r--   0 root         (0) root         (0)      865 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/BrowseButton.py
--rw-r--r--   0 root         (0) root         (0)     1859 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/BytearrayInput.py
--rw-r--r--   0 root         (0) root         (0)     5770 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/DictInput.py
--rw-r--r--   0 root         (0) root         (0)     4598 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/InputHandler.py
--rw-r--r--   0 root         (0) root         (0)     2512 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/SingleValueInputDialog.py
--rw-r--r--   0 root         (0) root         (0)     5103 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/StructInput.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/VariantEdit.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:05:15.058427 jdDBusDebugger-2.0/jdDBusDebugger/translations/
--rw-r--r--   0 root         (0) root         (0)    42126 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/translations/jdDBusDebugger_de.ts
--rw-r--r--   0 root         (0) root         (0)    42056 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/translations/jdDBusDebugger_nl.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:05:15.058427 jdDBusDebugger-2.0/jdDBusDebugger/types/
--rw-r--r--   0 root         (0) root         (0)     1991 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/Connection.py
--rw-r--r--   0 root         (0) root         (0)     7053 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/DBusType.py
--rw-r--r--   0 root         (0) root         (0)     4060 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/DBusValue.py
--rw-r--r--   0 root         (0) root         (0)      460 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/EnumHelper.py
--rw-r--r--   0 root         (0) root         (0)     1687 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/Interface.py
--rw-r--r--   0 root         (0) root         (0)     2583 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/Macro.py
--rw-r--r--   0 root         (0) root         (0)     1294 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/Method.py
--rw-r--r--   0 root         (0) root         (0)     2111 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/Property.py
--rw-r--r--   0 root         (0) root         (0)     2664 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/Service.py
--rw-r--r--   0 root         (0) root         (0)      553 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/Signal.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:05:15.058427 jdDBusDebugger-2.0/jdDBusDebugger/types/actions/
--rw-r--r--   0 root         (0) root         (0)      567 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/actions/ActionBase.py
--rw-r--r--   0 root         (0) root         (0)     2732 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/actions/CallAction.py
--rw-r--r--   0 root         (0) root         (0)     1709 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/actions/EmitAction.py
--rw-r--r--   0 root         (0) root         (0)     2906 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/actions/PropertyAction.py
--rw-r--r--   0 root         (0) root         (0)     1602 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/actions/SignalAction.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/types/actions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:05:15.058427 jdDBusDebugger-2.0/jdDBusDebugger/ui/
--rw-r--r--   0 root         (0) root         (0)     3982 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/ui/AboutDialog.ui
--rw-r--r--   0 root         (0) root         (0)     3888 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/ui/CentralWidget.ui
--rw-r--r--   0 root         (0) root         (0)     2634 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/ui/ConnectDialog.ui
--rw-r--r--   0 root         (0) root         (0)     2450 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/ui/EmitSignalDialog.ui
--rw-r--r--   0 root         (0) root         (0)     2223 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/ui/GenerateScriptDialog.ui
--rw-r--r--   0 root         (0) root         (0)     5508 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/ui/MainWindow.ui
--rw-r--r--   0 root         (0) root         (0)     1780 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/ui/ManageMacrosDialog.ui
--rw-r--r--   0 root         (0) root         (0)     3062 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/ui/SettingsDialog.ui
--rw-r--r--   0 root         (0) root         (0)     3253 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/ui/WelcomeDialog.ui
--rw-r--r--   0 root         (0) root         (0)        4 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/jdDBusDebugger/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:05:15.058427 jdDBusDebugger-2.0/jdDBusDebugger.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4913 2024-01-31 18:05:15.000000 jdDBusDebugger-2.0/jdDBusDebugger.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2540 2024-01-31 18:05:15.000000 jdDBusDebugger-2.0/jdDBusDebugger.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 18:05:15.000000 jdDBusDebugger-2.0/jdDBusDebugger.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-01-31 18:05:15.000000 jdDBusDebugger-2.0/jdDBusDebugger.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-01-31 18:05:15.000000 jdDBusDebugger-2.0/jdDBusDebugger.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-01-31 18:05:15.000000 jdDBusDebugger-2.0/jdDBusDebugger.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1397 2024-01-31 18:04:39.000000 jdDBusDebugger-2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-31 18:05:15.062427 jdDBusDebugger-2.0/setup.cfg
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.318877 jddbusdebugger-3.0/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2870 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/BuildBackend.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    35087 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/LICENSE
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      243 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/MANIFEST.in
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4936 2024-04-21 15:11:43.318877 jddbusdebugger-3.0/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3792 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/README.md
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.305544 jddbusdebugger-3.0/jdDBusDebugger/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       60 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/Constants.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1828 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/Environment.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1622 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/Functions.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)   125260 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/Icon.png
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1446 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/__init__.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       26 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/__main__.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.305544 jddbusdebugger-3.0/jdDBusDebugger/core/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      299 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/core/Languages.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3416 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/core/MacroManager.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1501 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/core/Settings.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        0 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/core/__init__.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.305544 jddbusdebugger-3.0/jdDBusDebugger/data/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      176 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/data/changelog.html
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       39 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/data/translators.json
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.308877 jddbusdebugger-3.0/jdDBusDebugger/gui/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1777 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/AboutDialog.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    22871 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/CentralWidget.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2262 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/ConnectDialog.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1499 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/EmitSignalDialog.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1489 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/GenerateScriptDialog.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    10948 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/MainWindow.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6124 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/ManageMacrosDialog.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    10541 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/MonitorWindow.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3074 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/SettingsDialog.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      939 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/WelcomeDialog.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.312210 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2798 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/ArgumentInput.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3443 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/ArrayInput.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      865 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/BrowseButton.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1859 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/BytearrayInput.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5770 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/DictInput.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4679 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/InputHandler.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2512 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/SingleValueInputDialog.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5103 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/StructInput.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1509 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/VariantEdit.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        0 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/__init__.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.312210 jddbusdebugger-3.0/jdDBusDebugger/translations/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    46119 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_de.ts
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    46050 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_nl.ts
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.315544 jddbusdebugger-3.0/jdDBusDebugger/types/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1991 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Connection.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     7053 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/DBusType.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4171 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/DBusValue.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      460 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/EnumHelper.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1687 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Interface.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2583 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Macro.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1294 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Method.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2111 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Property.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3129 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Service.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      553 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Signal.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        0 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/__init__.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.315544 jddbusdebugger-3.0/jdDBusDebugger/types/actions/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      567 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/ActionBase.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2732 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/CallAction.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1709 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/EmitAction.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2906 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/PropertyAction.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1602 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/SignalAction.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        0 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/__init__.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.318877 jddbusdebugger-3.0/jdDBusDebugger/ui/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3982 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/AboutDialog.ui
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3888 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/CentralWidget.ui
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2634 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/ConnectDialog.ui
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2450 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/EmitSignalDialog.ui
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2223 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/GenerateScriptDialog.ui
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5662 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/MainWindow.ui
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1780 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/ManageMacrosDialog.ui
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5102 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/MonitorWindow.ui
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3062 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/SettingsDialog.ui
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3253 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/WelcomeDialog.ui
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        4 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/version.txt
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.318877 jddbusdebugger-3.0/jdDBusDebugger.egg-info/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4936 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2611 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/SOURCES.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/dependency_links.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       51 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/entry_points.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       19 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/requires.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       15 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/top_level.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1410 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/pyproject.toml
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2024-04-21 15:11:43.318877 jddbusdebugger-3.0/setup.cfg
```

### Comparing `jdDBusDebugger-2.0/BuildBackend.py` & `jddbusdebugger-3.0/BuildBackend.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/LICENSE` & `jddbusdebugger-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/PKG-INFO` & `jddbusdebugger-3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdDBusDebugger
-Version: 2.0
+Version: 3.0
 Summary: An advanced D-Bus Debugger
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdDBusDebugger
 Project-URL: Issues, https://codeberg.org/JakobDev/jdDBusDebugger/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdDBusDebugger
 Project-URL: Donation, https://ko-fi.com/jakobdev
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyQt6
 Requires-Dist: lxml
+Requires-Dist: jeepney
 
 <h1 align="center">jdDBusDebugger</h1>
 
 <h3 align="center">An advanced D-Bus Debugger</h3>
 
 <p align="center">
     <img alt="jdDBusDebugger" src="screenshots/MainWindow.png"/>
```

### Comparing `jdDBusDebugger-2.0/README.md` & `jddbusdebugger-3.0/README.md`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/Environment.py` & `jddbusdebugger-3.0/jdDBusDebugger/Environment.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/Functions.py` & `jddbusdebugger-3.0/jdDBusDebugger/Functions.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/Icon.png` & `jddbusdebugger-3.0/jdDBusDebugger/Icon.png`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/__init__.py` & `jddbusdebugger-3.0/jdDBusDebugger/__init__.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/core/MacroManager.py` & `jddbusdebugger-3.0/jdDBusDebugger/core/MacroManager.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/core/Settings.py` & `jddbusdebugger-3.0/jdDBusDebugger/core/Settings.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/AboutDialog.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/AboutDialog.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/CentralWidget.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/CentralWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,15 +329,18 @@
         for arg in arguments:
             dbus_arguments.append(arg.get_value())
 
         call.setArguments(dbus_arguments)
         result = self.connection.connection.call(call)
 
         if result.errorName() != "":
-            self.add_log_error(result.errorMessage())
+            if result.errorMessage() == "":
+                self.add_log_error(result.errorName())
+            else:
+                self.add_log_error(f"{result.errorName()}: {result.errorMessage()}")
             return
 
         if method.return_type is not None and method.return_type.type_const == DBusTypeEnum.OBJECT_PATH:
             object_path = result.arguments()[0]
 
             match self._env.settings.get("methodReturnsObjectPath"):
                 case "add":
```

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/ConnectDialog.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/ConnectDialog.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/EmitSignalDialog.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/EmitSignalDialog.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/GenerateScriptDialog.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/GenerateScriptDialog.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/MainWindow.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/MainWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Literal, TYPE_CHECKING
 from ..types.Connection import Connection
 from PyQt6.QtCore import QCoreApplication
 from .WelcomeDialog import WelcomeDialog
 from PyQt6.QtDBus import QDBusConnection
 from .CentralWidget import CentralWidget
 from .ConnectDialog import ConnectDialog
+from .MonitorWindow import MonitorWindow
 from ..Functions import read_json_file
 from .AboutDialog import AboutDialog
 from PyQt6.QtGui import QAction
 import webbrowser
 import json
 import sys
 import os
@@ -46,14 +47,15 @@
         self.stop_recording_macro_action.triggered.connect(self._stop_recording_macro_action_clicked)
         self.run_macro_action.triggered.connect(self._run_macro_action_clicked)
         self.save_macro_action.triggered.connect(self._save_macro_action_clicked)
         self.generate_script_macro_action.triggered.connect(self._generate_script_macro_action_clicked)
         self.manage_macros_action.triggered.connect(self._manage_macros_action_clicked)
 
         self.emit_signal_action.triggered.connect(lambda: EmitSignalDialog(self).open_dialog())
+        self.monitor_action.triggered.connect(lambda: MonitorWindow(self).open_window())
 
         self.show_welcome_dialog_action.triggered.connect(lambda: WelcomeDialog(self._env).open_dialog())
         self.view_source_action.triggered.connect(lambda: webbrowser.open("https://codeberg.org/JakobDev/jdDBusDebugger"))
         self.report_bug_action.triggered.connect(lambda: webbrowser.open("https://codeberg.org/JakobDev/jdDBusDebugger/issues"))
         self.translate_action.triggered.connect(lambda: webbrowser.open("https://translate.codeberg.org/projects/jdDBusDebugger"))
         self.donate_action.triggered.connect(lambda: webbrowser.open("https://ko-fi.com/jakobdev"))
         self.about_action.triggered.connect(lambda: AboutDialog(self._env).exec())
@@ -201,22 +203,25 @@
             return
 
         if self.macro_manager.get_macro_by_name(name) is not None:
             QMessageBox.critical(self, QCoreApplication.translate("MainWindow", "Name exists"), QCoreApplication.translate("MainWindow", "There is already a macro with this name"))
             return
 
         self.macro_manager.save_current_macro(name, self.get_current_central_widget().connection)
+        self._update_macro_menu()
 
     def _manage_macros_action_clicked(self) -> None:
         ManageMacrosDialog(self, self.macro_manager).open_dialog()
+        self._update_macro_actions_enabled()
+        self._update_macro_menu()
 
     def _generate_script_macro_action_clicked(self) -> None:
         GenerateScriptDialog().open_dialog(self.macro_manager.get_current_actions())
 
     def has_connection_name(self, name: str) -> bool:
         for pos in range(self.tab_widget.count()):
             if self.tab_widget.tabText(pos) == name.lower():
                 return True
         return False
 
     def get_current_central_widget(self) -> CentralWidget:
-        return self.tab_widget.currentWidget()
+        return self.tab_widget.currentWidget()
```

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/ManageMacrosDialog.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/ManageMacrosDialog.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/SettingsDialog.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/WelcomeDialog.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/WelcomeDialog.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/ArgumentInput.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/ArgumentInput.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/ArrayInput.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/ArrayInput.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/BrowseButton.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/BrowseButton.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/BytearrayInput.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/BytearrayInput.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/DictInput.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/DictInput.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/InputHandler.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/InputHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                 spin_box.setMaximum(SPIN_BOX_MAXIMUM)
                 return spin_box
             case DBusTypeEnum.BOOLEAN:
                 boolean_box = QComboBox()
                 boolean_box.addItem(QCoreApplication.translate("InputHandler", "True"), True)
                 boolean_box.addItem(QCoreApplication.translate("InputHandler", "False"), False)
                 return boolean_box
-            case DBusTypeEnum.STRING:
+            case DBusTypeEnum.STRING | DBusTypeEnum.OBJECT_PATH:
                 return QLineEdit()
             case DBusTypeEnum.VARIANT:
                 return self._variant_edit()
             case DBusTypeEnum.ARRAY:
                 return self._array_button(parent, dbus_type)
             case DBusTypeEnum.DICT:
                 return self._dict_button(None)
@@ -64,26 +64,26 @@
             case DBusTypeEnum.INTEGER:
                 widget.setValue(value.value)
             case DBusTypeEnum.BOOLEAN:
                 if value.value is True:
                     widget.setCurrentIndex(0)
                 elif value.value is False:
                     widget.setCurrentIndex(1)
-            case DBusTypeEnum.STRING:
+            case DBusTypeEnum.STRING | DBusTypeEnum.OBJECT_PATH:
                 widget.setText(value.value)
 
     def get_value_from_widget(self, widget: QWidget, dbus_type: DBusType) -> DBusValue:
         match dbus_type.type_const:
             case DBusTypeEnum.INTEGER:
                 return DBusValue.create(dbus_type, widget.value())
             case DBusTypeEnum.DOUBLE:
                 return DBusValue.create(dbus_type, widget.value())
             case DBusTypeEnum.BOOLEAN:
                 return DBusValue.create(dbus_type, widget.currentData())
-            case DBusTypeEnum.STRING:
+            case DBusTypeEnum.STRING | DBusTypeEnum.OBJECT_PATH:
                 return DBusValue.create(dbus_type, widget.text())
             case DBusTypeEnum.VARIANT:
                 return widget.get_value()
             case DBusTypeEnum.ARRAY:
                 return widget.get_array()
             case DBusTypeEnum.DICT:
                 return DBusValue.create(dbus_type, widget.get_dict())
```

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/SingleValueInputDialog.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/SingleValueInputDialog.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/StructInput.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/StructInput.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/gui/types_input/VariantEdit.py` & `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/VariantEdit.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/translations/jdDBusDebugger_de.ts` & `jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_nl.ts`

 * *Files 14% similar despite different names*

#### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/translations/jdDBusDebugger_de.ts` & `jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_nl.ts`

```diff
@@ -1,1034 +1,1170 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="de">
+<TS version="2.1" language="nl">
   <context>
     <name>AboutDialog</name>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="125"/>
-      <location filename="../ui/AboutDialog_ui.py" line="122"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>About</source>
-      <translation>Über</translation>
+      <translation>Over</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="123"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>An advanced D-Bus Debugger</source>
-      <translation>Ein fortgeschrittener D-Bus-Debugger</translation>
+      <translation>Een uitgebreid D-Bus-foutopsporingsprogramma</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="124"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>This Program is licensed under GPL 3</source>
-      <translation>Dieses Programm ist unter der GPL 3 lizenziert</translation>
+      <translation>Dit programma is uitgebracht onder de GPL 3-licentie</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="127"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Translators</source>
-      <translation>Übersetzer</translation>
+      <translation>Vertalers</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="126"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>The following people translated jdDBusDebugger:</source>
-      <translation>Die folgenden Personen haben jdDBusDebugger übersetzt:</translation>
+      <translation>De volgende personen hebben jdDBusDebugger vertaald:</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="128"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Changelog</source>
-      <translation>Änderungsprotokoll</translation>
+      <translation>Wijzigingslog</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="129"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Close</source>
-      <translation>Schließen</translation>
+      <translation>Sluiten</translation>
     </message>
   </context>
   <context>
     <name>ArgumentInput</name>
     <message>
-      <location filename="../gui/types_input/ArgumentInput.py" line="26"/>
+      <location filename="../gui/types_input/ArgumentInput.py" line="27"/>
       <source>OK</source>
-      <translation>OK</translation>
+      <translation>Oké</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/ArgumentInput.py" line="27"/>
+      <location filename="../gui/types_input/ArgumentInput.py" line="28"/>
       <source>Cancel</source>
-      <translation>Abbrechen</translation>
+      <translation>Annuleren</translation>
     </message>
   </context>
   <context>
     <name>ArrayInput</name>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="21"/>
       <source>Add</source>
-      <translation>Hinzufügen</translation>
+      <translation>Toevoegen</translation>
     </message>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="22"/>
       <source>Remove</source>
-      <translation>Entfernen</translation>
+      <translation>Verwijderen</translation>
     </message>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="23"/>
       <source>OK</source>
-      <translation>OK</translation>
+      <translation>Oké</translation>
     </message>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="64"/>
       <location filename="../gui/types_input/ArrayInput.py" line="42"/>
       <source>Edit Array</source>
-      <translation>Array berabeiten</translation>
+      <translation>Reeks bewerken</translation>
     </message>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="83"/>
       <source>Select type</source>
-      <translation>Typ auswählen</translation>
+      <translation>Kies een type</translation>
     </message>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="83"/>
       <source>Select a type for this array</source>
-      <translation>Wähle einen typ für dieses Array aus</translation>
+      <translation>Kies een type voor deze reeks</translation>
     </message>
   </context>
   <context>
     <name>BrowseButton</name>
     <message>
       <location filename="../gui/types_input/BrowseButton.py" line="8"/>
       <source>Browse</source>
-      <translation>Durchsuchen</translation>
+      <translation>Kiezen</translation>
     </message>
     <message>
       <location filename="../gui/types_input/BrowseButton.py" line="28"/>
       <source>No file selected</source>
-      <translation>Keine Datei ausgewählt</translation>
+      <translation>Geen bestand gekozen</translation>
     </message>
   </context>
   <context>
     <name>BytearrayInput</name>
     <message>
       <location filename="../gui/types_input/BytearrayInput.py" line="12"/>
       <source>String</source>
-      <translation>String</translation>
+      <translation>Tekenreeks</translation>
     </message>
     <message>
       <location filename="../gui/types_input/BytearrayInput.py" line="13"/>
       <source>File</source>
-      <translation>Datei</translation>
+      <translation>Bestand</translation>
     </message>
   </context>
   <context>
     <name>CentralWidget</name>
     <message>
       <location filename="../gui/CentralWidget.py" line="42"/>
       <source>Call</source>
-      <translation>Aufrufen</translation>
+      <translation>Aanroepen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="73"/>
       <source>Get value</source>
-      <translation>Wert auslesen</translation>
+      <translation>Waarde opvragen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="78"/>
       <source>Set value</source>
-      <translation>Wert setzen</translation>
+      <translation>Waarde instellen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="113"/>
       <source>Disconnect</source>
-      <translation>Trennen</translation>
+      <translation>Verbinding verbreken</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="115"/>
       <source>Connect</source>
       <translation>Verbinden</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="197"/>
       <location filename="../gui/CentralWidget.py" line="164"/>
       <source>An error occurred while retrieving the data for this connection: {{error}}</source>
-      <translation>Beim Abruf der Daten für diese Verbindung ist ein Fehler aufgetreten: {{error}}</translation>
+      <translation>Er is een fout opgetreden tĳdens het ophalen van de gegevens: {{error}}</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="177"/>
       <source>Yes</source>
       <translation>Ja</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="179"/>
       <source>No</source>
-      <translation>Nein</translation>
+      <translation>Nee</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="219"/>
       <source>Methods</source>
       <translation>Methoden</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="226"/>
       <source>Properties</source>
-      <translation>Eigenschaften</translation>
+      <translation>Eigenschappen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="233"/>
       <source>Signals</source>
-      <translation>Signale</translation>
+      <translation>Signalen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="285"/>
       <source>Copy</source>
-      <translation>Kopieren</translation>
+      <translation>Kopiëren</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <location filename="../gui/CentralWidget.py" line="296"/>
       <source>Refresh</source>
-      <translation>Neu laden</translation>
+      <translation>Herladen</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
-      <location filename="../gui/CentralWidget.py" line="346"/>
+      <location filename="../gui/CentralWidget.py" line="349"/>
       <location filename="../gui/CentralWidget.py" line="305"/>
       <source>Add object path</source>
-      <translation>Objektpfad hinzufügen</translation>
+      <translation>Objectlocatie toevoegen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="305"/>
       <source>If this service has a object path that is not found trough introspection, you cann add it here</source>
-      <translation>Wenn der Service einen Objektpfad besitzt, der nciht gefunden wurde, kannst du ihn hier hinzufügen</translation>
+      <translation>Als deze dienst beschikt over een objectlocatie die niet door middel van introspectie is aangetroffen, voeg deze dan hier toe</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="316"/>
       <source>Path not loaded</source>
-      <translation>Pfad nicht geladen</translation>
+      <translation>De locatie is niet geladen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="316"/>
       <source>The given object path could not be loaded</source>
-      <translation>Der angegebene Pfad konnte nicht geladen werden</translation>
+      <translation>Deze opgegeven objectlocatie kan niet worden geladen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="324"/>
       <source>Calling {{method}}</source>
-      <translation>Rufe {{method}} auf</translation>
+      <translation>{{method}} wordt aangeroepen</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="346"/>
+      <location filename="../gui/CentralWidget.py" line="349"/>
       <source>This method returned the object path {{path}}. Do you want to add it to the list?</source>
-      <translation>Diese Methode hat den Objektpfad {{path}} zurückgegeben. Möchtest du ihn zur Liste hinzufügen?</translation>
+      <translation>Deze methode koppelde de objectlocatie ‘{{path}}’ terug. Wil je deze toevoegen aan de lĳst?</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="364"/>
+      <location filename="../gui/CentralWidget.py" line="367"/>
       <source>No return value</source>
-      <translation>Kein Rückgabewert</translation>
+      <translation>Geen terugkoppelwaarde</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="374"/>
+      <location filename="../gui/CentralWidget.py" line="377"/>
       <source>Get value of Property {{property}}</source>
-      <translation>Lese Wert der Eigenschaft {{property}} aus</translation>
+      <translation>Waarde opvragen van eigenschap ‘{{property}}’</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="391"/>
+      <location filename="../gui/CentralWidget.py" line="394"/>
       <source>Set value of Property {{property}} to {{value}}</source>
-      <translation>Setzte Wert der Eigenschaft {{property}} auf {{value}}</translation>
+      <translation>Waarde van eigenschap ‘{{property}}’ instellen op ‘{{value}}’</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="393"/>
+      <location filename="../gui/CentralWidget.py" line="396"/>
       <source>Failed to set Property {{property}} to {{value}}: {{error}}</source>
-      <translation>Setzen des Wertes der Eigenschaft {{property}} auf {{value}} fehlgeschlagen: {{error}}</translation>
+      <translation>De eigenschap ‘{{property}}’ kan niet worden ingesteld op ‘{{value}}’: {{error}}</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="401"/>
+      <location filename="../gui/CentralWidget.py" line="404"/>
       <source>Connected to Signal {{signal}}</source>
-      <translation>Mit Signal {{signal}} verbunden</translation>
+      <translation>Verbonden met signaal ‘{{signal}}’</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="409"/>
+      <location filename="../gui/CentralWidget.py" line="412"/>
       <source>Disconnected from Signal {{signal}}</source>
-      <translation>Von Signal {{signal}} getrennt</translation>
+      <translation>Verbinding verbroken met signaal ‘{{signal}}’</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="414"/>
+      <location filename="../gui/CentralWidget.py" line="417"/>
       <source>Signal {{signal}} emited: {{reply}}</source>
-      <translation>SIgnal {{signal}} wurde ausgelöst: {{reply}}</translation>
+      <translation>Signaal ‘{{signal}}’ verstuurd: {{reply}}</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="437"/>
+      <location filename="../gui/CentralWidget.py" line="440"/>
       <source>Method {{method}} was not found</source>
-      <translation>Methode {{method}} wurde nicht gefunden</translation>
+      <translation>‘{{methode}}’ bestaat niet</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="445"/>
+      <location filename="../gui/CentralWidget.py" line="448"/>
       <source>Property {{property}} was not found</source>
-      <translation>Eigenschaft {{property}} wurde nicht gefunden</translation>
+      <translation>‘{{property}}’ bestaat niet</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="457"/>
+      <location filename="../gui/CentralWidget.py" line="460"/>
       <source>Signal {{signal}} was not found</source>
-      <translation>SIgnal {{signal}} wurde nicht gefunden</translation>
+      <translation>‘{{signal}}’ bestaat niet</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="477"/>
+      <location filename="../gui/CentralWidget.py" line="480"/>
       <source>Signal was emited on path {{path}} and interface {{interface}} with these arguments: {{arguments}}</source>
-      <translation>Signal wurde auf Pfad {{Pfad}} und Schnittstelle {{Schnittstelle}} mit diesen Argumenten gesendet: {{Argumente}}</translation>
+      <translation>Er is een signaal uitgegaan op {{path}} en interface ‘{{interface}}’ met de volgende opties: {{arguments}}</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="479"/>
+      <location filename="../gui/CentralWidget.py" line="482"/>
       <source>Could not emit Signal on path {{path}} and interface {{interface}} with these arguments: {{arguments}}</source>
-      <translation>Konnte kein Signal auf Pfad {{Pfad}} und Schnittstelle {{Schnittstelle}} mit diesen Argumenten aussenden: {{Argumente}}</translation>
+      <translation>Er kan geen signaal worden uitgestuurd op {{path}} en interface ‘{{interface}}’ met de volgende opties: {{arguments}}</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="488"/>
+      <location filename="../gui/CentralWidget.py" line="491"/>
       <source>Service {{service}} was not found</source>
-      <translation>Service {{service}} wurde nicht gefunden</translation>
+      <translation>‘{{service}}’ bestaat niet</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="496"/>
+      <location filename="../gui/CentralWidget.py" line="499"/>
       <source>Interface {{interface}} was not found on {{path}}</source>
-      <translation>Interface {{interface}} wurde auf {{path}} nicht gefunden</translation>
+      <translation>‘{{interface}}’ is niet aangetroffen in {{path}}</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Services</source>
-      <translation>Services</translation>
+      <translation>Diensten</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Search</source>
-      <translation>Suche</translation>
+      <translation>Zoeken</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Name</source>
-      <translation>Name</translation>
+      <translation>Naam</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Activatable</source>
-      <translation>Aktivierbar</translation>
+      <translation>Activeerbaar</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>PID</source>
       <translation>PID</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Objects</source>
-      <translation>Objekte</translation>
+      <translation>Objecten</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Clear</source>
-      <translation>Löschen</translation>
+      <translation>Wissen</translation>
     </message>
   </context>
   <context>
     <name>ConnectDialog</name>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="30"/>
+      <location filename="../gui/ConnectDialog.py" line="34"/>
       <source>Name not set</source>
-      <translation>Name nicht angegeben</translation>
+      <translation>Geen naam ingesteld</translation>
     </message>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="30"/>
+      <location filename="../gui/ConnectDialog.py" line="34"/>
       <source>You need to enter a name</source>
-      <translation>Du musst einen Namen angeben</translation>
+      <translation>Voer een naam in</translation>
     </message>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="34"/>
+      <location filename="../gui/ConnectDialog.py" line="38"/>
       <source>Adress not set</source>
-      <translation>Adresse nicht angegeben</translation>
+      <translation>Geen adres ingesteld</translation>
     </message>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="34"/>
+      <location filename="../gui/ConnectDialog.py" line="38"/>
       <source>You need to enter a address</source>
-      <translation>Du musst eine Adresse angeben</translation>
+      <translation>Voer een adres in</translation>
     </message>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="39"/>
+      <location filename="../gui/ConnectDialog.py" line="43"/>
       <source>Invalid Address</source>
-      <translation>Ungültige Adresse</translation>
+      <translation>Ongeldig adres</translation>
     </message>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="39"/>
+      <location filename="../gui/ConnectDialog.py" line="43"/>
       <source>Could not connect to {{address}}</source>
-      <translation>Konnte keine Verbindung mit {{address}} herstellen</translation>
+      <translation>Er kan geen verbinding worden gemaakt met {{address}}</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>Connect</source>
-      <translation>Verbinde</translation>
+      <translation>Verbinden</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>You can connect here with your custom D-Bus address</source>
-      <translation>Du kannst dich hier mit einer eigenen D-Bus Adresse verbinden</translation>
+      <translation>Je kunt hier verbinding maken met je eigen D-Bus-adres</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>Name:</source>
-      <translation>Name:</translation>
+      <translation>Naam:</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>Address:</source>
-      <translation>Adresse:</translation>
+      <translation>Adres:</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>Auto connect on startup</source>
-      <translation>Beim Starten automatisch verbinden</translation>
+      <translation>Automatisch verbinden na opstarten</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>OK</translation>
+      <translation>Oké</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Abbrechen</translation>
+      <translation>Annuleren</translation>
     </message>
   </context>
   <context>
     <name>DictInput</name>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="28"/>
+      <location filename="../gui/types_input/DictInput.py" line="29"/>
       <source>Add</source>
-      <translation>Hinzufügen</translation>
+      <translation>Toevoegen</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="29"/>
+      <location filename="../gui/types_input/DictInput.py" line="30"/>
       <source>OK</source>
-      <translation>OK</translation>
+      <translation>Oké</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="31"/>
+      <location filename="../gui/types_input/DictInput.py" line="32"/>
       <source>Key</source>
-      <translation>Schlüssel</translation>
+      <translation>Sleutel</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="31"/>
+      <location filename="../gui/types_input/DictInput.py" line="32"/>
       <source>Type</source>
-      <translation>Typ</translation>
+      <translation>Type</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="31"/>
+      <location filename="../gui/types_input/DictInput.py" line="32"/>
       <source>Value</source>
-      <translation>Wert</translation>
+      <translation>Waarde</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="77"/>
-      <location filename="../gui/types_input/DictInput.py" line="31"/>
+      <location filename="../gui/types_input/DictInput.py" line="80"/>
+      <location filename="../gui/types_input/DictInput.py" line="32"/>
       <source>Remove</source>
-      <translation>Löschen</translation>
+      <translation>Verwijderen</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="46"/>
+      <location filename="../gui/types_input/DictInput.py" line="49"/>
       <source>Edit Dictionary</source>
-      <translation>Wörterbuch bearbeiten</translation>
+      <translation>Woordenboek bewerken</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="88"/>
+      <location filename="../gui/types_input/DictInput.py" line="91"/>
       <source>The key must not be empty</source>
-      <translation>Der Schlüssel darf nicht leer sein</translation>
+      <translation>Voer een sleutel in</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="91"/>
+      <location filename="../gui/types_input/DictInput.py" line="94"/>
       <source>The key {{key}} appears more than once</source>
-      <translation>Der Schlüssel {{key}} existiert mehr als einmal</translation>
+      <translation>‘{{key}}’ is meer dan eens ingevoerd</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="115"/>
+      <location filename="../gui/types_input/DictInput.py" line="118"/>
       <source>Data invalid</source>
-      <translation>Daten ungültig</translation>
+      <translation>Ongeldige gegevens</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="115"/>
+      <location filename="../gui/types_input/DictInput.py" line="118"/>
       <source>Your data is not valid</source>
-      <translation>Die Daten sind ungültig</translation>
+      <translation>Je gegevens zĳn ongeldig</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="121"/>
+      <location filename="../gui/types_input/DictInput.py" line="124"/>
       <source>Edit Dict</source>
-      <translation>Ver</translation>
+      <translation>Woordenboek bewerken</translation>
     </message>
   </context>
   <context>
     <name>EmitSignalDialog</name>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Emit Signal</source>
-      <translation>Signal senden</translation>
+      <translation>Signaal uitsturen</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Path:</source>
-      <translation>Pfad:</translation>
+      <translation>Locatie:</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Interface:</source>
-      <translation>Schnitstelle:</translation>
+      <translation>Interface:</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Name:</source>
-      <translation>Name:</translation>
+      <translation>Naam:</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Arguments:</source>
-      <translation>Argumente:</translation>
+      <translation>Opties:</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>OK</translation>
+      <translation>Oké</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Abbrechen</translation>
+      <translation>Annuleren</translation>
     </message>
   </context>
   <context>
     <name>GenerateScriptDialog</name>
     <message>
       <location filename="../ui/GenerateScriptDialog.ui" line="0"/>
       <source>Script</source>
-      <translation>Skript</translation>
+      <translation>Script</translation>
     </message>
     <message>
       <location filename="../ui/GenerateScriptDialog.ui" line="0"/>
       <source>Here are the shell commands for this macro</source>
-      <translation>Hier sind alle Shell Befehle dür dieses Makro</translation>
+      <translation>Dit zĳn de bĳ de macro behorende shellopdrachten</translation>
     </message>
     <message>
       <location filename="../ui/GenerateScriptDialog.ui" line="0"/>
       <source>These commands are without warranty. It may not work with complexer types.</source>
-      <translation>Diese befhle kommen ohne Gewähr. Sie funktionieren möglicherweise nicht mit komplexeren Typen.</translation>
+      <translation>Let op: deze opdrachten worden getoond zonder enige vorm van garantie en werken mogelĳk niet met complexere types.</translation>
     </message>
     <message>
       <location filename="../ui/GenerateScriptDialog.ui" line="0"/>
       <source>Generator:</source>
       <translation>Generator:</translation>
     </message>
     <message>
       <location filename="../ui/GenerateScriptDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>OK</translation>
+      <translation>Oké</translation>
     </message>
   </context>
   <context>
     <name>InputHandler</name>
     <message>
       <location filename="../gui/types_input/InputHandler.py" line="42"/>
       <source>True</source>
-      <translation>Wahr</translation>
+      <translation>Waar</translation>
     </message>
     <message>
       <location filename="../gui/types_input/InputHandler.py" line="43"/>
       <source>False</source>
-      <translation>Falsch</translation>
+      <translation>Onwaar</translation>
     </message>
     <message>
       <location filename="../gui/types_input/InputHandler.py" line="60"/>
       <source>Unsupported type</source>
-      <translation>Nicht unterstützter Typ</translation>
+      <translation>Niet-ondersteund type</translation>
     </message>
   </context>
   <context>
     <name>Language</name>
     <message>
       <location filename="../core/Languages.py" line="6"/>
       <source>English</source>
-      <translation>Englisch</translation>
+      <translation>Engels</translation>
     </message>
     <message>
       <location filename="../core/Languages.py" line="7"/>
       <source>German</source>
-      <translation>Deutsch</translation>
+      <translation>Duits</translation>
     </message>
     <message>
       <location filename="../core/Languages.py" line="8"/>
       <source>Dutch</source>
-      <translation>Niederländisch</translation>
+      <translation>Nederlands</translation>
     </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
-      <location filename="../gui/MainWindow.py" line="93"/>
+      <location filename="../gui/MainWindow.py" line="95"/>
       <source>Session</source>
-      <translation>Sitzung</translation>
+      <translation>Sessie</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="96"/>
+      <location filename="../gui/MainWindow.py" line="98"/>
       <source>Could not connect to session bus</source>
-      <translation>Konnte nicht zum Sitzungsbus verbinden</translation>
+      <translation>Kan niet verbinden met sessiebus</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="96"/>
+      <location filename="../gui/MainWindow.py" line="98"/>
       <source>jdDBusDebugger was unable to connect to the session bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
-      <translation>jdDBusDebugger konnte sich nicht mit dem Sitzungsbus verbinden. Wenn du jdDBusDebugger in einer Sandboxumgebung ausführst stelle sicher, dass es die notwendigen Berechtigungen hat.</translation>
+      <translation>jdDBusDebugger kan geen verbinding maken met de sessiebus. Als je het programma uitvoert in een gesandboxte omgeving, zorg er dan voor dat het juiste recht is toegekend.</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="101"/>
+      <location filename="../gui/MainWindow.py" line="103"/>
       <source>System</source>
-      <translation>System</translation>
+      <translation>Systeem</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="104"/>
+      <location filename="../gui/MainWindow.py" line="106"/>
       <source>Could not connect to system bus</source>
-      <translation>Konnte nicht zum Systembus verbinden</translation>
+      <translation>Kan niet verbinden met systeembus</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="104"/>
+      <location filename="../gui/MainWindow.py" line="106"/>
       <source>jdDBusDebugger was unable to connect to the system bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
-      <translation>jdDBusDebugger konnte sich nicht mit dem Systembus verbinden. Wenn du jdDBusDebugger in einer Sandboxumgebung ausführst stelle sicher, dass es die notwendigen Berechtigungen hat.</translation>
+      <translation>jdDBusDebugger kan geen verbinding maken met de systeembus. Als je het programma uitvoert in een gesandboxte omgeving, zorg er dan voor dat het juiste recht is toegekend.</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="204"/>
-      <location filename="../gui/MainWindow.py" line="110"/>
+      <location filename="../gui/MainWindow.py" line="206"/>
+      <location filename="../gui/MainWindow.py" line="112"/>
       <source>Name exists</source>
-      <translation>Name existiert</translation>
+      <translation>Deze naam is al in gebruik</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="110"/>
+      <location filename="../gui/MainWindow.py" line="112"/>
       <source>Could not connect to {{connection}}</source>
-      <translation>Konnte nicht zu {{connection}} verbinden</translation>
+      <translation>Er kan geen verbinding worden gemaakt met {{connection}}</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="167"/>
+      <location filename="../gui/MainWindow.py" line="169"/>
       <source>You have no macros saved</source>
-      <translation>DU hast keine Makros gespeichert</translation>
+      <translation>Er zĳn nog geen macro's</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="198"/>
+      <location filename="../gui/MainWindow.py" line="200"/>
       <source>Enter Name</source>
-      <translation>Namen eingeben</translation>
+      <translation>Voer een naam in</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="198"/>
+      <location filename="../gui/MainWindow.py" line="200"/>
       <source>Please enter a name for your macro</source>
-      <translation>Bitte gib einen Namen für dein Makro ein</translation>
+      <translation>Geef de macro een naam</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="204"/>
+      <location filename="../gui/MainWindow.py" line="206"/>
       <source>There is already a macro with this name</source>
-      <translation>Es existiert bereits ein Makro mit diesem Namen</translation>
+      <translation>Er is al een macro met deze naam</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="162"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>File</source>
-      <translation>Datei</translation>
+      <translation>Bestand</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="163"/>
-      <location filename="../ui/MainWindow_ui.py" line="154"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Settings</source>
-      <translation>Einstellungen</translation>
+      <translation>Instellingen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="164"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Macros</source>
-      <translation>Makros</translation>
+      <translation>Macro's</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="165"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Run saved</source>
-      <translation>Gespeicherte ausführen</translation>
+      <translation>De routine is opgeslagen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="166"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Tools</source>
-      <translation>Werkzeuge</translation>
+      <translation>Hulpmiddelen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="146"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Start Recording</source>
-      <translation>Aufzeichnung starten</translation>
+      <translation>Opname starten</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="147"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Stop Recording</source>
-      <translation>Aufzeichnung stoppen</translation>
+      <translation>Opname stoppen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="148"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Run</source>
-      <translation>Ausführen</translation>
+      <translation>Uitvoeren</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="149"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Save</source>
-      <translation>Speichern</translation>
+      <translation>Opslaan</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="150"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Manage</source>
-      <translation>Verwalten</translation>
+      <translation>Beheren</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="151"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Exit</source>
-      <translation>Beenden</translation>
+      <translation>Afsluiten</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="152"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Generate Script</source>
-      <translation>Skript erstellen</translation>
+      <translation>Script genereren</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="153"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Connect</source>
       <translation>Verbinden</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="155"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Report Bug</source>
-      <translation>Fehler melden</translation>
+      <translation>Bug melden</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="156"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Translate</source>
-      <translation>Übersetzen</translation>
+      <translation>Vertalen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="157"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Donate</source>
-      <translation>Spenden</translation>
+      <translation>Doneren</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="158"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About</source>
-      <translation>Über</translation>
+      <translation>Over</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="159"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About Qt</source>
-      <translation>Über Qt</translation>
+      <translation>Over Qt</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="160"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Show welcome dialog</source>
-      <translation>Willkommensdialog anzeigen</translation>
+      <translation>Welkomstvenster tonen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="161"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Emit Signal</source>
-      <translation>Signal senden</translation>
+      <translation>Signaal uitsturen</translation>
+    </message>
+    <message>
+      <location filename="../ui/MainWindow.ui" line="0"/>
+      <source>Monitor</source>
+      <translation>Monitoren</translation>
     </message>
   </context>
   <context>
     <name>ManageMacrosDialog</name>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="126"/>
       <location filename="../gui/ManageMacrosDialog.py" line="58"/>
       <source>Enter name</source>
-      <translation>Name eingeben</translation>
+      <translation>Voer een naam in</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="58"/>
       <source>Please enter a new name for the macro</source>
-      <translation>Bitte gib einen Namen für das Makro ein</translation>
+      <translation>Geef de macro een nieuwe naam</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="132"/>
       <location filename="../gui/ManageMacrosDialog.py" line="64"/>
       <source>Name exists</source>
-      <translation>Name existiert</translation>
+      <translation>Deze naam is al in gebruik</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="132"/>
       <location filename="../gui/ManageMacrosDialog.py" line="64"/>
       <source>There is already a macro with this name</source>
-      <translation>Es existiert bereits ein Makro mit diesem Namen</translation>
+      <translation>Er is al een macro met deze naam</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="75"/>
       <source>Delete macro</source>
-      <translation>Makro löschen</translation>
+      <translation>Macro verwijderen</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="75"/>
       <source>This will delete {{name}} forever. Are you sure??</source>
-      <translation>Dies löscht {{name}} für immer. Bist du sicher?</translation>
+      <translation>Let op: ‘{{name}}’ wordt permanent verwĳderd. Weet je het zeker?</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="108"/>
       <location filename="../gui/ManageMacrosDialog.py" line="90"/>
       <source>JSON files</source>
-      <translation>JSON Dateien</translation>
+      <translation>Json-bestanden</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="108"/>
       <location filename="../gui/ManageMacrosDialog.py" line="90"/>
       <source>All Files</source>
-      <translation>Alle Dateien</translation>
+      <translation>Alle bestanden</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="105"/>
       <source>Could not export macro</source>
-      <translation>Konnte Makro nicht exportieren</translation>
+      <translation>Kan macro niet exporteren</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="105"/>
       <source>The macro could not be exported to {{path}} due to an error</source>
-      <translation>Das Makro konnte aufgrund eines Fehlers nicht nach {{path}} exportiert werden</translation>
+      <translation>Wegens een foutmelding kan de macro kan niet worden geëxporteerd naar {{path}}</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="122"/>
       <source>Could not import macro</source>
-      <translation>Konnte Makro nicht importieren</translation>
+      <translation>Kan macro niet importeren</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="122"/>
       <source>The macro could not be imported. Please make sure you use the correct file.</source>
-      <translation>Das Makro konnte nicht importiert werden. Stelle sicher, dass du die korrekte Datei benutzt.</translation>
+      <translation>De macro kan niet worden geïmporteerd. Controleer of je het juiste bestand hebt gekozen.</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="126"/>
       <source>Please enter a name for the macro</source>
-      <translation>Bitte gib einen Namen für das Makro ein</translation>
+      <translation>Geef de macro een naam</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>Manage Macros</source>
-      <translation>Makros verwalten</translation>
+      <translation>Macro's beheren</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>Rename</source>
-      <translation>Umbennen</translation>
+      <translation>Naam wĳzigen</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>Delete</source>
-      <translation>Löschen</translation>
+      <translation>Verwijderen</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>View Script</source>
-      <translation>Skript ansehen</translation>
+      <translation>Script bekĳken</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>Export</source>
-      <translation>Exportieren</translation>
+      <translation>Exporteren</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>Import</source>
-      <translation>Importieren</translation>
+      <translation>Importeren</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>OK</translation>
+      <translation>Oké</translation>
+    </message>
+  </context>
+  <context>
+    <name>MonitorWindow</name>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <location filename="../gui/MonitorWindow.py" line="63"/>
+      <source>Method call</source>
+      <comment>Message type</comment>
+      <translation>Aanroepmethode</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <location filename="../gui/MonitorWindow.py" line="65"/>
+      <source>Method return</source>
+      <comment>Message type</comment>
+      <translation>Terugroepmethode</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <location filename="../gui/MonitorWindow.py" line="67"/>
+      <source>Error</source>
+      <comment>Message type</comment>
+      <translation>Foutmelding</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <location filename="../gui/MonitorWindow.py" line="69"/>
+      <source>Signal</source>
+      <comment>Message type</comment>
+      <translation>Signaal</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="71"/>
+      <source>Unknown</source>
+      <comment>Message type</comment>
+      <translation>Onbekend</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="137"/>
+      <source>Type</source>
+      <comment>Table Header</comment>
+      <translation>Type</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="138"/>
+      <source>Sender</source>
+      <comment>Table Header</comment>
+      <translation>Afzender</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="139"/>
+      <source>Destination</source>
+      <comment>Table Header</comment>
+      <translation>Bestemming</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="140"/>
+      <source>Path</source>
+      <comment>Table Header</comment>
+      <translation>Locatie</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="141"/>
+      <source>Interface</source>
+      <comment>Table Header</comment>
+      <translation>Interface</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="142"/>
+      <source>Member</source>
+      <comment>Table Header</comment>
+      <translation>Lid</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="143"/>
+      <source>Signature</source>
+      <comment>Table Header</comment>
+      <translation>Ondertekening</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="144"/>
+      <source>Body</source>
+      <comment>Table Header</comment>
+      <translation>Inhoud</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="221"/>
+      <source>Error</source>
+      <translation>Foutmelding</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="222"/>
+      <source>Could not start monitor session</source>
+      <translation>De sessie kan niet worden gestart</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="235"/>
+      <source>Monitor Session</source>
+      <translation>Sessie monitoren</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="237"/>
+      <source>Monitor System</source>
+      <translation>Systeem monitoren</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="239"/>
+      <source>Monitor {{name}}</source>
+      <translation>{{name}} monitoren</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Filter</source>
+      <translation>Filteren</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Destination:</source>
+      <translation>Bestemming:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Path:</source>
+      <translation>Locatie:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Sender:</source>
+      <translation>Afzender:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Member:</source>
+      <translation>Lid:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Interface:</source>
+      <translation>Interface:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Signature:</source>
+      <translation>Ondertekening:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Type:</source>
+      <translation>Type:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Clear</source>
+      <translation>Wissen</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>OK</source>
+      <translation>Oké</translation>
     </message>
   </context>
   <context>
     <name>SettingsDialog</name>
     <message>
-      <location filename="../gui/SettingsDialog.py" line="29"/>
+      <location filename="../gui/SettingsDialog.py" line="30"/>
       <source>Use system language</source>
-      <translation>Benutze Systemsprache</translation>
+      <translation>Systeemtaal</translation>
     </message>
     <message>
-      <location filename="../gui/SettingsDialog.py" line="31"/>
+      <location filename="../gui/SettingsDialog.py" line="32"/>
       <source>Add object path to list</source>
-      <translation>Füge Objektpfad zur Liste hinzu</translation>
+      <translation>Objectlocatie toevoegen aan lĳst</translation>
     </message>
     <message>
-      <location filename="../gui/SettingsDialog.py" line="32"/>
+      <location filename="../gui/SettingsDialog.py" line="33"/>
       <source>Ask the User</source>
-      <translation>Frage den Benutzer</translation>
+      <translation>Om actie vragen</translation>
     </message>
     <message>
-      <location filename="../gui/SettingsDialog.py" line="33"/>
+      <location filename="../gui/SettingsDialog.py" line="34"/>
       <source>Do nothing</source>
-      <translation>Nichtstun</translation>
+      <translation>Niets doen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Settings</source>
-      <translation>Einstellungen</translation>
+      <translation>Instellingen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Language:</source>
-      <translation>Sprache:</translation>
+      <translation>Taal:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>(needs restart)</source>
-      <translation>(benötigt Neustart)</translation>
+      <translation>(herstart vereist)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>When a method returns a object path:</source>
-      <translation>Wenn eine Methode einen Objektpfad zurückgibt:</translation>
+      <translation>Als een methode een objectlocatie terugkoppelt:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Warn if the connection to the session bus or the system bus fails</source>
-      <translation>Warnen, falls die Verbindung zum Sitzungsbus oder zum Systembus fehlschlägt</translation>
+      <translation>Waarschuwen als de verbinding met de sessie- of systeembus mislukt</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Reset</source>
-      <translation>Zurücksetzen</translation>
+      <translation>Standaardwaarden</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>OK</translation>
+      <translation>Oké</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Abbrechen</translation>
+      <translation>Annuleren</translation>
     </message>
   </context>
   <context>
     <name>SingleValueInputDialog</name>
     <message>
-      <location filename="../gui/types_input/SingleValueInputDialog.py" line="21"/>
+      <location filename="../gui/types_input/SingleValueInputDialog.py" line="22"/>
       <source>OK</source>
-      <translation>OK</translation>
+      <translation>Oké</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/SingleValueInputDialog.py" line="22"/>
+      <location filename="../gui/types_input/SingleValueInputDialog.py" line="23"/>
       <source>Cancel</source>
-      <translation>Abbrechen</translation>
+      <translation>Annuleren</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/SingleValueInputDialog.py" line="37"/>
+      <location filename="../gui/types_input/SingleValueInputDialog.py" line="41"/>
       <source>Enter value</source>
-      <translation>Wert eingeben</translation>
+      <translation>Voer een waarde in</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/SingleValueInputDialog.py" line="42"/>
+      <location filename="../gui/types_input/SingleValueInputDialog.py" line="46"/>
       <source>Invalid data</source>
-      <translation>Ungültige Daten</translation>
+      <translation>Ongeldige gegevens</translation>
     </message>
   </context>
   <context>
     <name>StructInput</name>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="27"/>
+      <location filename="../gui/types_input/StructInput.py" line="28"/>
       <source>Add</source>
-      <translation>Hinzufügen</translation>
+      <translation>Toevoegen</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="28"/>
+      <location filename="../gui/types_input/StructInput.py" line="29"/>
       <source>OK</source>
-      <translation>OK</translation>
+      <translation>Oké</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="30"/>
+      <location filename="../gui/types_input/StructInput.py" line="31"/>
       <source>Type</source>
-      <translation>Typ</translation>
+      <translation>Type</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="30"/>
+      <location filename="../gui/types_input/StructInput.py" line="31"/>
       <source>Value</source>
-      <translation>Wert</translation>
+      <translation>Waarde</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="74"/>
-      <location filename="../gui/types_input/StructInput.py" line="30"/>
+      <location filename="../gui/types_input/StructInput.py" line="77"/>
+      <location filename="../gui/types_input/StructInput.py" line="31"/>
       <source>Remove</source>
-      <translation>Löschen</translation>
+      <translation>Verwijderen</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="108"/>
-      <location filename="../gui/types_input/StructInput.py" line="45"/>
+      <location filename="../gui/types_input/StructInput.py" line="111"/>
+      <location filename="../gui/types_input/StructInput.py" line="48"/>
       <source>Edit Struct</source>
-      <translation>Struktur bearbeiten</translation>
+      <translation>Struct bewerken</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="102"/>
+      <location filename="../gui/types_input/StructInput.py" line="105"/>
       <source>Data invalid</source>
-      <translation>Daten ungültig</translation>
+      <translation>Ongeldige gegevens</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="102"/>
+      <location filename="../gui/types_input/StructInput.py" line="105"/>
       <source>Your data is not valid</source>
-      <translation>Die Daten sind ungültig</translation>
+      <translation>Je gegevens zĳn ongeldig</translation>
     </message>
   </context>
   <context>
     <name>WelcomeDialog</name>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome</source>
-      <translation>Willkommen</translation>
+      <translation>Welkom</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome to jdDBusDebugger!</source>
-      <translation>Willkommen bei jdDBusDebugger!</translation>
+      <translation>Welkom in jdDBusDebugger!</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program allows you to easily debug your D-Bus interfaces. You can do everything in a nice GUI, so you don't need to fund out how to correctly format the input.</source>
-      <translation>Dieses Programm erlaubt dir einfach deine D-Bus Schnittstellen zu debuggen. Du kannst alles in einer leicht zu benutzenden GUI erledigen, sodass du nicht lernen musst, wie man alle Daten korrekt formatiert.</translation>
+      <translation>Met dit programma kun je gemakkelĳk fouten opsporen in D-Bus-interfaces. Alles zit verpakt in een mooi grafisch jasje, zodat je niet hoeft uit te vogelen hoe je de invoer moet opmaken.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>You can also record macros, so you can repeat your tests easily. It is even possible to generate a shell script out of a macro.</source>
-      <translation>Du kannst auch Makros aufnehme, sodass du deine tests einfach wiederholen kannst. Es ist sogar möglich aus deinen Makros ein Shellskript zu generieren.</translation>
+      <translation>Daarnaast kun je macro's opnemen, zodat je testen gemakkelĳk kunt herhalen. Ook kun je van een macro een shellscript maken.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Not every complex type is supported at the Moment, but I will keep working on adding it.</source>
-      <translation>Aktuell wird nicht jeder komlexer Typ unterstützt. An der Unterstützung wird jedoch bereits gearbeitet.</translation>
+      <translation>Momenteel is er nog geen ondersteuning voor elk complex type, maar ik zal in de toekomst meer toevoegen.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>If you want to report a Bug or left Feedback, use ?&gt;Report bug</source>
-      <translation>Wenn du einen Fehler melden oder Feedback geben möchtest, benutze ?&gt;Fehler melden</translation>
+      <translation>Als je een bug wilt melden of feedback wilt delen, dan kan dat via ? → Bug melden</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Show this on startup</source>
-      <translation>Beim starten anzeigen</translation>
+      <translation>Altĳd tonen na opstarten</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>OK</translation>
+      <translation>Oké</translation>
     </message>
   </context>
 </TS>
```

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/translations/jdDBusDebugger_nl.ts` & `jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_de.ts`

 * *Files 10% similar despite different names*

#### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/translations/jdDBusDebugger_nl.ts` & `jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_de.ts`

```diff
@@ -1,1034 +1,1170 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="nl">
+<TS version="2.1" language="de_DE">
   <context>
     <name>AboutDialog</name>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="125"/>
-      <location filename="../ui/AboutDialog_ui.py" line="122"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>About</source>
-      <translation>Over</translation>
+      <translation>Über</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="123"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>An advanced D-Bus Debugger</source>
-      <translation>Een uitgebreid D-Bus-foutopsporingsprogramma</translation>
+      <translation>Ein fortgeschrittener D-Bus-Debugger</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="124"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>This Program is licensed under GPL 3</source>
-      <translation>Dit programma is uitgebracht onder de GPL 3-licentie</translation>
+      <translation>Dieses Programm ist unter der GPL 3 lizenziert</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="127"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Translators</source>
-      <translation>Vertalers</translation>
+      <translation>Übersetzer</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="126"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>The following people translated jdDBusDebugger:</source>
-      <translation>De volgende personen hebben jdDBusDebugger vertaald:</translation>
+      <translation>Die folgenden Personen haben jdDBusDebugger übersetzt:</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="128"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Changelog</source>
-      <translation>Wijzigingslog</translation>
+      <translation>Änderungsprotokoll</translation>
     </message>
     <message>
-      <location filename="../ui/AboutDialog_ui.py" line="129"/>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Close</source>
-      <translation>Sluiten</translation>
+      <translation>Schließen</translation>
     </message>
   </context>
   <context>
     <name>ArgumentInput</name>
     <message>
-      <location filename="../gui/types_input/ArgumentInput.py" line="26"/>
+      <location filename="../gui/types_input/ArgumentInput.py" line="27"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/ArgumentInput.py" line="27"/>
+      <location filename="../gui/types_input/ArgumentInput.py" line="28"/>
       <source>Cancel</source>
-      <translation>Annuleren</translation>
+      <translation>Abbrechen</translation>
     </message>
   </context>
   <context>
     <name>ArrayInput</name>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="21"/>
       <source>Add</source>
-      <translation>Toevoegen</translation>
+      <translation>Hinzufügen</translation>
     </message>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="22"/>
       <source>Remove</source>
-      <translation>Verwijderen</translation>
+      <translation>Entfernen</translation>
     </message>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="23"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
     </message>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="64"/>
       <location filename="../gui/types_input/ArrayInput.py" line="42"/>
       <source>Edit Array</source>
-      <translation>Reeks bewerken</translation>
+      <translation>Array berabeiten</translation>
     </message>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="83"/>
       <source>Select type</source>
-      <translation>Kies een type</translation>
+      <translation>Typ auswählen</translation>
     </message>
     <message>
       <location filename="../gui/types_input/ArrayInput.py" line="83"/>
       <source>Select a type for this array</source>
-      <translation>Kies een type voor deze reeks</translation>
+      <translation>Wähle einen typ für dieses Array aus</translation>
     </message>
   </context>
   <context>
     <name>BrowseButton</name>
     <message>
       <location filename="../gui/types_input/BrowseButton.py" line="8"/>
       <source>Browse</source>
-      <translation>Kiezen</translation>
+      <translation>Durchsuchen</translation>
     </message>
     <message>
       <location filename="../gui/types_input/BrowseButton.py" line="28"/>
       <source>No file selected</source>
-      <translation>Geen bestand gekozen</translation>
+      <translation>Keine Datei ausgewählt</translation>
     </message>
   </context>
   <context>
     <name>BytearrayInput</name>
     <message>
       <location filename="../gui/types_input/BytearrayInput.py" line="12"/>
       <source>String</source>
-      <translation>Tekenreeks</translation>
+      <translation>String</translation>
     </message>
     <message>
       <location filename="../gui/types_input/BytearrayInput.py" line="13"/>
       <source>File</source>
-      <translation>Bestand</translation>
+      <translation>Datei</translation>
     </message>
   </context>
   <context>
     <name>CentralWidget</name>
     <message>
       <location filename="../gui/CentralWidget.py" line="42"/>
       <source>Call</source>
-      <translation>Aanroepen</translation>
+      <translation>Aufrufen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="73"/>
       <source>Get value</source>
-      <translation>Waarde opvragen</translation>
+      <translation>Wert auslesen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="78"/>
       <source>Set value</source>
-      <translation>Waarde instellen</translation>
+      <translation>Wert setzen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="113"/>
       <source>Disconnect</source>
-      <translation>Verbinding verbreken</translation>
+      <translation>Trennen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="115"/>
       <source>Connect</source>
       <translation>Verbinden</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="197"/>
       <location filename="../gui/CentralWidget.py" line="164"/>
       <source>An error occurred while retrieving the data for this connection: {{error}}</source>
-      <translation>Er is een fout opgetreden tĳdens het ophalen van de gegevens: {{error}}</translation>
+      <translation>Beim Abruf der Daten für diese Verbindung ist ein Fehler aufgetreten: {{error}}</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="177"/>
       <source>Yes</source>
       <translation>Ja</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="179"/>
       <source>No</source>
-      <translation>Nee</translation>
+      <translation>Nein</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="219"/>
       <source>Methods</source>
       <translation>Methoden</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="226"/>
       <source>Properties</source>
-      <translation>Eigenschappen</translation>
+      <translation>Eigenschaften</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="233"/>
       <source>Signals</source>
-      <translation>Signalen</translation>
+      <translation>Signale</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="285"/>
       <source>Copy</source>
-      <translation>Kopiëren</translation>
+      <translation>Kopieren</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <location filename="../gui/CentralWidget.py" line="296"/>
       <source>Refresh</source>
-      <translation>Herladen</translation>
+      <translation>Neu laden</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
-      <location filename="../gui/CentralWidget.py" line="346"/>
+      <location filename="../gui/CentralWidget.py" line="349"/>
       <location filename="../gui/CentralWidget.py" line="305"/>
       <source>Add object path</source>
-      <translation>Objectlocatie toevoegen</translation>
+      <translation>Objektpfad hinzufügen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="305"/>
       <source>If this service has a object path that is not found trough introspection, you cann add it here</source>
-      <translation>Als deze dienst beschikt over een objectlocatie die niet door middel van introspectie is aangetroffen, voeg deze dan hier toe</translation>
+      <translation>Wenn der Service einen Objektpfad besitzt, der nciht gefunden wurde, kannst du ihn hier hinzufügen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="316"/>
       <source>Path not loaded</source>
-      <translation>De locatie is niet geladen</translation>
+      <translation>Pfad nicht geladen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="316"/>
       <source>The given object path could not be loaded</source>
-      <translation>Deze opgegeven objectlocatie kan niet worden geladen</translation>
+      <translation>Der angegebene Pfad konnte nicht geladen werden</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="324"/>
       <source>Calling {{method}}</source>
-      <translation>{{method}} wordt aangeroepen</translation>
+      <translation>Rufe {{method}} auf</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="346"/>
+      <location filename="../gui/CentralWidget.py" line="349"/>
       <source>This method returned the object path {{path}}. Do you want to add it to the list?</source>
-      <translation>Deze methode koppelde de objectlocatie ‘{{path}}’ terug. Wil je deze toevoegen aan de lĳst?</translation>
+      <translation>Diese Methode hat den Objektpfad {{path}} zurückgegeben. Möchtest du ihn zur Liste hinzufügen?</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="364"/>
+      <location filename="../gui/CentralWidget.py" line="367"/>
       <source>No return value</source>
-      <translation>Geen terugkoppelwaarde</translation>
+      <translation>Kein Rückgabewert</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="374"/>
+      <location filename="../gui/CentralWidget.py" line="377"/>
       <source>Get value of Property {{property}}</source>
-      <translation>Waarde opvragen van eigenschap ‘{{property}}’</translation>
+      <translation>Lese Wert der Eigenschaft {{property}} aus</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="391"/>
+      <location filename="../gui/CentralWidget.py" line="394"/>
       <source>Set value of Property {{property}} to {{value}}</source>
-      <translation>Waarde van eigenschap ‘{{property}}’ instellen op ‘{{value}}’</translation>
+      <translation>Setzte Wert der Eigenschaft {{property}} auf {{value}}</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="393"/>
+      <location filename="../gui/CentralWidget.py" line="396"/>
       <source>Failed to set Property {{property}} to {{value}}: {{error}}</source>
-      <translation>De eigenschap ‘{{property}}’ kan niet worden ingesteld op ‘{{value}}’: {{error}}</translation>
+      <translation>Setzen des Wertes der Eigenschaft {{property}} auf {{value}} fehlgeschlagen: {{error}}</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="401"/>
+      <location filename="../gui/CentralWidget.py" line="404"/>
       <source>Connected to Signal {{signal}}</source>
-      <translation>Verbonden met signaal ‘{{signal}}’</translation>
+      <translation>Mit Signal {{signal}} verbunden</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="409"/>
+      <location filename="../gui/CentralWidget.py" line="412"/>
       <source>Disconnected from Signal {{signal}}</source>
-      <translation>Verbinding verbroken met signaal ‘{{signal}}’</translation>
+      <translation>Von Signal {{signal}} getrennt</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="414"/>
+      <location filename="../gui/CentralWidget.py" line="417"/>
       <source>Signal {{signal}} emited: {{reply}}</source>
-      <translation>Signaal ‘{{signal}}’ verstuurd: {{reply}}</translation>
+      <translation>SIgnal {{signal}} wurde ausgelöst: {{reply}}</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="437"/>
+      <location filename="../gui/CentralWidget.py" line="440"/>
       <source>Method {{method}} was not found</source>
-      <translation>‘{{methode}}’ bestaat niet</translation>
+      <translation>Methode {{method}} wurde nicht gefunden</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="445"/>
+      <location filename="../gui/CentralWidget.py" line="448"/>
       <source>Property {{property}} was not found</source>
-      <translation>‘{{property}}’ bestaat niet</translation>
+      <translation>Eigenschaft {{property}} wurde nicht gefunden</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="457"/>
+      <location filename="../gui/CentralWidget.py" line="460"/>
       <source>Signal {{signal}} was not found</source>
-      <translation>‘{{signal}}’ bestaat niet</translation>
+      <translation>SIgnal {{signal}} wurde nicht gefunden</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="477"/>
+      <location filename="../gui/CentralWidget.py" line="480"/>
       <source>Signal was emited on path {{path}} and interface {{interface}} with these arguments: {{arguments}}</source>
-      <translation>Er is een signaal uitgegaan op {{path}} en interface ‘{{interface}}’ met de volgende opties: {{arguments}}</translation>
+      <translation>Signal wurde auf Pfad {{Pfad}} und Schnittstelle {{Schnittstelle}} mit diesen Argumenten gesendet: {{Argumente}}</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="479"/>
+      <location filename="../gui/CentralWidget.py" line="482"/>
       <source>Could not emit Signal on path {{path}} and interface {{interface}} with these arguments: {{arguments}}</source>
-      <translation>Er kan geen signaal worden uitgestuurd op {{path}} en interface ‘{{interface}}’ met de volgende opties: {{arguments}}</translation>
+      <translation>Konnte kein Signal auf Pfad {{Pfad}} und Schnittstelle {{Schnittstelle}} mit diesen Argumenten aussenden: {{Argumente}}</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="488"/>
+      <location filename="../gui/CentralWidget.py" line="491"/>
       <source>Service {{service}} was not found</source>
-      <translation>‘{{service}}’ bestaat niet</translation>
+      <translation>Service {{service}} wurde nicht gefunden</translation>
     </message>
     <message>
-      <location filename="../gui/CentralWidget.py" line="496"/>
+      <location filename="../gui/CentralWidget.py" line="499"/>
       <source>Interface {{interface}} was not found on {{path}}</source>
-      <translation>‘{{interface}}’ is niet aangetroffen in {{path}}</translation>
+      <translation>Interface {{interface}} wurde auf {{path}} nicht gefunden</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Services</source>
-      <translation>Diensten</translation>
+      <translation>Services</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Search</source>
-      <translation>Zoeken</translation>
+      <translation>Suche</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Name</source>
-      <translation>Naam</translation>
+      <translation>Name</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Activatable</source>
-      <translation>Activeerbaar</translation>
+      <translation>Aktivierbar</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>PID</source>
       <translation>PID</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Objects</source>
-      <translation>Objecten</translation>
+      <translation>Objekte</translation>
     </message>
     <message>
       <location filename="../ui/CentralWidget.ui" line="0"/>
       <source>Clear</source>
-      <translation>Wissen</translation>
+      <translation>Löschen</translation>
     </message>
   </context>
   <context>
     <name>ConnectDialog</name>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="30"/>
+      <location filename="../gui/ConnectDialog.py" line="34"/>
       <source>Name not set</source>
-      <translation>Geen naam ingesteld</translation>
+      <translation>Name nicht angegeben</translation>
     </message>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="30"/>
+      <location filename="../gui/ConnectDialog.py" line="34"/>
       <source>You need to enter a name</source>
-      <translation>Voer een naam in</translation>
+      <translation>Du musst einen Namen angeben</translation>
     </message>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="34"/>
+      <location filename="../gui/ConnectDialog.py" line="38"/>
       <source>Adress not set</source>
-      <translation>Geen adres ingesteld</translation>
+      <translation>Adresse nicht angegeben</translation>
     </message>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="34"/>
+      <location filename="../gui/ConnectDialog.py" line="38"/>
       <source>You need to enter a address</source>
-      <translation>Voer een adres in</translation>
+      <translation>Du musst eine Adresse angeben</translation>
     </message>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="39"/>
+      <location filename="../gui/ConnectDialog.py" line="43"/>
       <source>Invalid Address</source>
-      <translation>Ongeldig adres</translation>
+      <translation>Ungültige Adresse</translation>
     </message>
     <message>
-      <location filename="../gui/ConnectDialog.py" line="39"/>
+      <location filename="../gui/ConnectDialog.py" line="43"/>
       <source>Could not connect to {{address}}</source>
-      <translation>Er kan geen verbinding worden gemaakt met {{address}}</translation>
+      <translation>Konnte keine Verbindung mit {{address}} herstellen</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>Connect</source>
-      <translation>Verbinden</translation>
+      <translation>Verbinde</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>You can connect here with your custom D-Bus address</source>
-      <translation>Je kunt hier verbinding maken met je eigen D-Bus-adres</translation>
+      <translation>Du kannst dich hier mit einer eigenen D-Bus Adresse verbinden</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>Name:</source>
-      <translation>Naam:</translation>
+      <translation>Name:</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>Address:</source>
-      <translation>Adres:</translation>
+      <translation>Adresse:</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>Auto connect on startup</source>
-      <translation>Automatisch verbinden na opstarten</translation>
+      <translation>Beim Starten automatisch verbinden</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
     </message>
     <message>
       <location filename="../ui/ConnectDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Annuleren</translation>
+      <translation>Abbrechen</translation>
     </message>
   </context>
   <context>
     <name>DictInput</name>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="28"/>
+      <location filename="../gui/types_input/DictInput.py" line="29"/>
       <source>Add</source>
-      <translation>Toevoegen</translation>
+      <translation>Hinzufügen</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="29"/>
+      <location filename="../gui/types_input/DictInput.py" line="30"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="31"/>
+      <location filename="../gui/types_input/DictInput.py" line="32"/>
       <source>Key</source>
-      <translation>Sleutel</translation>
+      <translation>Schlüssel</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="31"/>
+      <location filename="../gui/types_input/DictInput.py" line="32"/>
       <source>Type</source>
-      <translation>Type</translation>
+      <translation>Typ</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="31"/>
+      <location filename="../gui/types_input/DictInput.py" line="32"/>
       <source>Value</source>
-      <translation>Waarde</translation>
+      <translation>Wert</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="77"/>
-      <location filename="../gui/types_input/DictInput.py" line="31"/>
+      <location filename="../gui/types_input/DictInput.py" line="80"/>
+      <location filename="../gui/types_input/DictInput.py" line="32"/>
       <source>Remove</source>
-      <translation>Verwijderen</translation>
+      <translation>Löschen</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="46"/>
+      <location filename="../gui/types_input/DictInput.py" line="49"/>
       <source>Edit Dictionary</source>
-      <translation>Woordenboek bewerken</translation>
+      <translation>Wörterbuch bearbeiten</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="88"/>
+      <location filename="../gui/types_input/DictInput.py" line="91"/>
       <source>The key must not be empty</source>
-      <translation>Voer een sleutel in</translation>
+      <translation>Der Schlüssel darf nicht leer sein</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="91"/>
+      <location filename="../gui/types_input/DictInput.py" line="94"/>
       <source>The key {{key}} appears more than once</source>
-      <translation>‘{{key}}’ is meer dan eens ingevoerd</translation>
+      <translation>Der Schlüssel {{key}} existiert mehr als einmal</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="115"/>
+      <location filename="../gui/types_input/DictInput.py" line="118"/>
       <source>Data invalid</source>
-      <translation>Ongeldige gegevens</translation>
+      <translation>Daten ungültig</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="115"/>
+      <location filename="../gui/types_input/DictInput.py" line="118"/>
       <source>Your data is not valid</source>
-      <translation>Je gegevens zĳn ongeldig</translation>
+      <translation>Die Daten sind ungültig</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/DictInput.py" line="121"/>
+      <location filename="../gui/types_input/DictInput.py" line="124"/>
       <source>Edit Dict</source>
-      <translation>Woordenboek bewerken</translation>
+      <translation>Ver</translation>
     </message>
   </context>
   <context>
     <name>EmitSignalDialog</name>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Emit Signal</source>
-      <translation>Signaal uitsturen</translation>
+      <translation>Signal senden</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Path:</source>
-      <translation>Locatie:</translation>
+      <translation>Pfad:</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Interface:</source>
-      <translation>Interface:</translation>
+      <translation>Schnitstelle:</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Name:</source>
-      <translation>Naam:</translation>
+      <translation>Name:</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Arguments:</source>
-      <translation>Opties:</translation>
+      <translation>Argumente:</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
     </message>
     <message>
       <location filename="../ui/EmitSignalDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Annuleren</translation>
+      <translation>Abbrechen</translation>
     </message>
   </context>
   <context>
     <name>GenerateScriptDialog</name>
     <message>
       <location filename="../ui/GenerateScriptDialog.ui" line="0"/>
       <source>Script</source>
-      <translation>Script</translation>
+      <translation>Skript</translation>
     </message>
     <message>
       <location filename="../ui/GenerateScriptDialog.ui" line="0"/>
       <source>Here are the shell commands for this macro</source>
-      <translation>Dit zĳn de bĳ de macro behorende shellopdrachten</translation>
+      <translation>Hier sind alle Shell Befehle dür dieses Makro</translation>
     </message>
     <message>
       <location filename="../ui/GenerateScriptDialog.ui" line="0"/>
       <source>These commands are without warranty. It may not work with complexer types.</source>
-      <translation>Let op: deze opdrachten worden getoond zonder enige vorm van garantie en werken mogelĳk niet met complexere types.</translation>
+      <translation>Diese befhle kommen ohne Gewähr. Sie funktionieren möglicherweise nicht mit komplexeren Typen.</translation>
     </message>
     <message>
       <location filename="../ui/GenerateScriptDialog.ui" line="0"/>
       <source>Generator:</source>
       <translation>Generator:</translation>
     </message>
     <message>
       <location filename="../ui/GenerateScriptDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
     </message>
   </context>
   <context>
     <name>InputHandler</name>
     <message>
       <location filename="../gui/types_input/InputHandler.py" line="42"/>
       <source>True</source>
-      <translation>Waar</translation>
+      <translation>Wahr</translation>
     </message>
     <message>
       <location filename="../gui/types_input/InputHandler.py" line="43"/>
       <source>False</source>
-      <translation>Onwaar</translation>
+      <translation>Falsch</translation>
     </message>
     <message>
       <location filename="../gui/types_input/InputHandler.py" line="60"/>
       <source>Unsupported type</source>
-      <translation>Niet-ondersteund type</translation>
+      <translation>Nicht unterstützter Typ</translation>
     </message>
   </context>
   <context>
     <name>Language</name>
     <message>
       <location filename="../core/Languages.py" line="6"/>
       <source>English</source>
-      <translation>Engels</translation>
+      <translation>Englisch</translation>
     </message>
     <message>
       <location filename="../core/Languages.py" line="7"/>
       <source>German</source>
-      <translation>Duits</translation>
+      <translation>Deutsch</translation>
     </message>
     <message>
       <location filename="../core/Languages.py" line="8"/>
       <source>Dutch</source>
-      <translation>Nederlands</translation>
+      <translation>Niederländisch</translation>
     </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
-      <location filename="../gui/MainWindow.py" line="93"/>
+      <location filename="../gui/MainWindow.py" line="95"/>
       <source>Session</source>
-      <translation>Sessie</translation>
+      <translation>Sitzung</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="96"/>
+      <location filename="../gui/MainWindow.py" line="98"/>
       <source>Could not connect to session bus</source>
-      <translation>Kan niet verbinden met sessiebus</translation>
+      <translation>Konnte nicht zum Sitzungsbus verbinden</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="96"/>
+      <location filename="../gui/MainWindow.py" line="98"/>
       <source>jdDBusDebugger was unable to connect to the session bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
-      <translation>jdDBusDebugger kan geen verbinding maken met de sessiebus. Als je het programma uitvoert in een gesandboxte omgeving, zorg er dan voor dat het juiste recht is toegekend.</translation>
+      <translation>jdDBusDebugger konnte sich nicht mit dem Sitzungsbus verbinden. Wenn du jdDBusDebugger in einer Sandboxumgebung ausführst stelle sicher, dass es die notwendigen Berechtigungen hat.</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="101"/>
+      <location filename="../gui/MainWindow.py" line="103"/>
       <source>System</source>
-      <translation>Systeem</translation>
+      <translation>System</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="104"/>
+      <location filename="../gui/MainWindow.py" line="106"/>
       <source>Could not connect to system bus</source>
-      <translation>Kan niet verbinden met systeembus</translation>
+      <translation>Konnte nicht zum Systembus verbinden</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="104"/>
+      <location filename="../gui/MainWindow.py" line="106"/>
       <source>jdDBusDebugger was unable to connect to the system bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
-      <translation>jdDBusDebugger kan geen verbinding maken met de systeembus. Als je het programma uitvoert in een gesandboxte omgeving, zorg er dan voor dat het juiste recht is toegekend.</translation>
+      <translation>jdDBusDebugger konnte sich nicht mit dem Systembus verbinden. Wenn du jdDBusDebugger in einer Sandboxumgebung ausführst stelle sicher, dass es die notwendigen Berechtigungen hat.</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="204"/>
-      <location filename="../gui/MainWindow.py" line="110"/>
+      <location filename="../gui/MainWindow.py" line="206"/>
+      <location filename="../gui/MainWindow.py" line="112"/>
       <source>Name exists</source>
-      <translation>Deze naam is al in gebruik</translation>
+      <translation>Name existiert</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="110"/>
+      <location filename="../gui/MainWindow.py" line="112"/>
       <source>Could not connect to {{connection}}</source>
-      <translation>Er kan geen verbinding worden gemaakt met {{connection}}</translation>
+      <translation>Konnte nicht zu {{connection}} verbinden</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="167"/>
+      <location filename="../gui/MainWindow.py" line="169"/>
       <source>You have no macros saved</source>
-      <translation>Er zĳn nog geen macro's</translation>
+      <translation>DU hast keine Makros gespeichert</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="198"/>
+      <location filename="../gui/MainWindow.py" line="200"/>
       <source>Enter Name</source>
-      <translation>Voer een naam in</translation>
+      <translation>Namen eingeben</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="198"/>
+      <location filename="../gui/MainWindow.py" line="200"/>
       <source>Please enter a name for your macro</source>
-      <translation>Geef de macro een naam</translation>
+      <translation>Bitte gib einen Namen für dein Makro ein</translation>
     </message>
     <message>
-      <location filename="../gui/MainWindow.py" line="204"/>
+      <location filename="../gui/MainWindow.py" line="206"/>
       <source>There is already a macro with this name</source>
-      <translation>Er is al een macro met deze naam</translation>
+      <translation>Es existiert bereits ein Makro mit diesem Namen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="162"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>File</source>
-      <translation>Bestand</translation>
+      <translation>Datei</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="163"/>
-      <location filename="../ui/MainWindow_ui.py" line="154"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Settings</source>
-      <translation>Instellingen</translation>
+      <translation>Einstellungen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="164"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Macros</source>
-      <translation>Macro's</translation>
+      <translation>Makros</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="165"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Run saved</source>
-      <translation>De routine is opgeslagen</translation>
+      <translation>Gespeicherte ausführen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="166"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Tools</source>
-      <translation>Hulpmiddelen</translation>
+      <translation>Werkzeuge</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="146"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Start Recording</source>
-      <translation>Opname starten</translation>
+      <translation>Aufzeichnung starten</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="147"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Stop Recording</source>
-      <translation>Opname stoppen</translation>
+      <translation>Aufzeichnung stoppen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="148"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Run</source>
-      <translation>Uitvoeren</translation>
+      <translation>Ausführen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="149"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Save</source>
-      <translation>Opslaan</translation>
+      <translation>Speichern</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="150"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Manage</source>
-      <translation>Beheren</translation>
+      <translation>Verwalten</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="151"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Exit</source>
-      <translation>Afsluiten</translation>
+      <translation>Beenden</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="152"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Generate Script</source>
-      <translation>Script genereren</translation>
+      <translation>Skript erstellen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="153"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Connect</source>
       <translation>Verbinden</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="155"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Report Bug</source>
-      <translation>Bug melden</translation>
+      <translation>Fehler melden</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="156"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Translate</source>
-      <translation>Vertalen</translation>
+      <translation>Übersetzen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="157"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Donate</source>
-      <translation>Doneren</translation>
+      <translation>Spenden</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="158"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About</source>
-      <translation>Over</translation>
+      <translation>Über</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="159"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About Qt</source>
-      <translation>Over Qt</translation>
+      <translation>Über Qt</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="160"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Show welcome dialog</source>
-      <translation>Welkomstvenster tonen</translation>
+      <translation>Willkommensdialog anzeigen</translation>
     </message>
     <message>
-      <location filename="../ui/MainWindow_ui.py" line="161"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Emit Signal</source>
-      <translation>Signaal uitsturen</translation>
+      <translation>Signal senden</translation>
+    </message>
+    <message>
+      <location filename="../ui/MainWindow.ui" line="0"/>
+      <source>Monitor</source>
+      <translation>Beobachten</translation>
     </message>
   </context>
   <context>
     <name>ManageMacrosDialog</name>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="126"/>
       <location filename="../gui/ManageMacrosDialog.py" line="58"/>
       <source>Enter name</source>
-      <translation>Voer een naam in</translation>
+      <translation>Name eingeben</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="58"/>
       <source>Please enter a new name for the macro</source>
-      <translation>Geef de macro een nieuwe naam</translation>
+      <translation>Bitte gib einen Namen für das Makro ein</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="132"/>
       <location filename="../gui/ManageMacrosDialog.py" line="64"/>
       <source>Name exists</source>
-      <translation>Deze naam is al in gebruik</translation>
+      <translation>Name existiert</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="132"/>
       <location filename="../gui/ManageMacrosDialog.py" line="64"/>
       <source>There is already a macro with this name</source>
-      <translation>Er is al een macro met deze naam</translation>
+      <translation>Es existiert bereits ein Makro mit diesem Namen</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="75"/>
       <source>Delete macro</source>
-      <translation>Macro verwijderen</translation>
+      <translation>Makro löschen</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="75"/>
       <source>This will delete {{name}} forever. Are you sure??</source>
-      <translation>Let op: ‘{{name}}’ wordt permanent verwĳderd. Weet je het zeker?</translation>
+      <translation>Dies löscht {{name}} für immer. Bist du sicher?</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="108"/>
       <location filename="../gui/ManageMacrosDialog.py" line="90"/>
       <source>JSON files</source>
-      <translation>Json-bestanden</translation>
+      <translation>JSON Dateien</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="108"/>
       <location filename="../gui/ManageMacrosDialog.py" line="90"/>
       <source>All Files</source>
-      <translation>Alle bestanden</translation>
+      <translation>Alle Dateien</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="105"/>
       <source>Could not export macro</source>
-      <translation>Kan macro niet exporteren</translation>
+      <translation>Konnte Makro nicht exportieren</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="105"/>
       <source>The macro could not be exported to {{path}} due to an error</source>
-      <translation>Wegens een foutmelding kan de macro kan niet worden geëxporteerd naar {{path}}</translation>
+      <translation>Das Makro konnte aufgrund eines Fehlers nicht nach {{path}} exportiert werden</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="122"/>
       <source>Could not import macro</source>
-      <translation>Kan macro niet importeren</translation>
+      <translation>Konnte Makro nicht importieren</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="122"/>
       <source>The macro could not be imported. Please make sure you use the correct file.</source>
-      <translation>De macro kan niet worden geïmporteerd. Controleer of je het juiste bestand hebt gekozen.</translation>
+      <translation>Das Makro konnte nicht importiert werden. Stelle sicher, dass du die korrekte Datei benutzt.</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="126"/>
       <source>Please enter a name for the macro</source>
-      <translation>Geef de macro een naam</translation>
+      <translation>Bitte gib einen Namen für das Makro ein</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>Manage Macros</source>
-      <translation>Macro's beheren</translation>
+      <translation>Makros verwalten</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>Rename</source>
-      <translation>Naam wĳzigen</translation>
+      <translation>Umbennen</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>Delete</source>
-      <translation>Verwijderen</translation>
+      <translation>Löschen</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>View Script</source>
-      <translation>Script bekĳken</translation>
+      <translation>Skript ansehen</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>Export</source>
-      <translation>Exporteren</translation>
+      <translation>Exportieren</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>Import</source>
-      <translation>Importeren</translation>
+      <translation>Importieren</translation>
     </message>
     <message>
       <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
+    </message>
+  </context>
+  <context>
+    <name>MonitorWindow</name>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <location filename="../gui/MonitorWindow.py" line="63"/>
+      <source>Method call</source>
+      <comment>Message type</comment>
+      <translation>Methodenaufruf</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <location filename="../gui/MonitorWindow.py" line="65"/>
+      <source>Method return</source>
+      <comment>Message type</comment>
+      <translation>Methodenrückgabe</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <location filename="../gui/MonitorWindow.py" line="67"/>
+      <source>Error</source>
+      <comment>Message type</comment>
+      <translation>Fehler</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <location filename="../gui/MonitorWindow.py" line="69"/>
+      <source>Signal</source>
+      <comment>Message type</comment>
+      <translation>Signal</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="71"/>
+      <source>Unknown</source>
+      <comment>Message type</comment>
+      <translation>Unbekannt</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="137"/>
+      <source>Type</source>
+      <comment>Table Header</comment>
+      <translation>Typ</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="138"/>
+      <source>Sender</source>
+      <comment>Table Header</comment>
+      <translation>Sender</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="139"/>
+      <source>Destination</source>
+      <comment>Table Header</comment>
+      <translation>Empfänger</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="140"/>
+      <source>Path</source>
+      <comment>Table Header</comment>
+      <translation>Pfad</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="141"/>
+      <source>Interface</source>
+      <comment>Table Header</comment>
+      <translation>Schnittstelle</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="142"/>
+      <source>Member</source>
+      <comment>Table Header</comment>
+      <translation>Mitglied</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="143"/>
+      <source>Signature</source>
+      <comment>Table Header</comment>
+      <translation>Signatur</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="144"/>
+      <source>Body</source>
+      <comment>Table Header</comment>
+      <translation>Inhalt</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="221"/>
+      <source>Error</source>
+      <translation>Fehler</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="222"/>
+      <source>Could not start monitor session</source>
+      <translation>Monitorsitzung konnte nicht gestartet werden</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="235"/>
+      <source>Monitor Session</source>
+      <translation>Beobachte Sitzung</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="237"/>
+      <source>Monitor System</source>
+      <translation>Beobachte System</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="239"/>
+      <source>Monitor {{name}}</source>
+      <translation>Beobachte {{name}}</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Filter</source>
+      <translation>Filter</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Destination:</source>
+      <translation>Empfänger:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Path:</source>
+      <translation>Pfad:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Sender:</source>
+      <translation>Sender:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Member:</source>
+      <translation>Mitglied:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Interface:</source>
+      <translation>Schnitstelle:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Signature:</source>
+      <translation>Signatur:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Type:</source>
+      <translation>Typ:</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Clear</source>
+      <translation>Löschen</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>OK</source>
+      <translation>OK</translation>
     </message>
   </context>
   <context>
     <name>SettingsDialog</name>
     <message>
-      <location filename="../gui/SettingsDialog.py" line="29"/>
+      <location filename="../gui/SettingsDialog.py" line="30"/>
       <source>Use system language</source>
-      <translation>Systeemtaal</translation>
+      <translation>Benutze Systemsprache</translation>
     </message>
     <message>
-      <location filename="../gui/SettingsDialog.py" line="31"/>
+      <location filename="../gui/SettingsDialog.py" line="32"/>
       <source>Add object path to list</source>
-      <translation>Objectlocatie toevoegen aan lĳst</translation>
+      <translation>Füge Objektpfad zur Liste hinzu</translation>
     </message>
     <message>
-      <location filename="../gui/SettingsDialog.py" line="32"/>
+      <location filename="../gui/SettingsDialog.py" line="33"/>
       <source>Ask the User</source>
-      <translation>Om actie vragen</translation>
+      <translation>Frage den Benutzer</translation>
     </message>
     <message>
-      <location filename="../gui/SettingsDialog.py" line="33"/>
+      <location filename="../gui/SettingsDialog.py" line="34"/>
       <source>Do nothing</source>
-      <translation>Niets doen</translation>
+      <translation>Nichtstun</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Settings</source>
-      <translation>Instellingen</translation>
+      <translation>Einstellungen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Language:</source>
-      <translation>Taal:</translation>
+      <translation>Sprache:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>(needs restart)</source>
-      <translation>(herstart vereist)</translation>
+      <translation>(benötigt Neustart)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>When a method returns a object path:</source>
-      <translation>Als een methode een objectlocatie terugkoppelt:</translation>
+      <translation>Wenn eine Methode einen Objektpfad zurückgibt:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Warn if the connection to the session bus or the system bus fails</source>
-      <translation>Waarschuwen als de verbinding met de sessie- of systeembus mislukt</translation>
+      <translation>Warnen, falls die Verbindung zum Sitzungsbus oder zum Systembus fehlschlägt</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Reset</source>
-      <translation>Standaardwaarden</translation>
+      <translation>Zurücksetzen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Annuleren</translation>
+      <translation>Abbrechen</translation>
     </message>
   </context>
   <context>
     <name>SingleValueInputDialog</name>
     <message>
-      <location filename="../gui/types_input/SingleValueInputDialog.py" line="21"/>
+      <location filename="../gui/types_input/SingleValueInputDialog.py" line="22"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/SingleValueInputDialog.py" line="22"/>
+      <location filename="../gui/types_input/SingleValueInputDialog.py" line="23"/>
       <source>Cancel</source>
-      <translation>Annuleren</translation>
+      <translation>Abbrechen</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/SingleValueInputDialog.py" line="37"/>
+      <location filename="../gui/types_input/SingleValueInputDialog.py" line="41"/>
       <source>Enter value</source>
-      <translation>Voer een waarde in</translation>
+      <translation>Wert eingeben</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/SingleValueInputDialog.py" line="42"/>
+      <location filename="../gui/types_input/SingleValueInputDialog.py" line="46"/>
       <source>Invalid data</source>
-      <translation>Ongeldige gegevens</translation>
+      <translation>Ungültige Daten</translation>
     </message>
   </context>
   <context>
     <name>StructInput</name>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="27"/>
+      <location filename="../gui/types_input/StructInput.py" line="28"/>
       <source>Add</source>
-      <translation>Toevoegen</translation>
+      <translation>Hinzufügen</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="28"/>
+      <location filename="../gui/types_input/StructInput.py" line="29"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="30"/>
+      <location filename="../gui/types_input/StructInput.py" line="31"/>
       <source>Type</source>
-      <translation>Type</translation>
+      <translation>Typ</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="30"/>
+      <location filename="../gui/types_input/StructInput.py" line="31"/>
       <source>Value</source>
-      <translation>Waarde</translation>
+      <translation>Wert</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="74"/>
-      <location filename="../gui/types_input/StructInput.py" line="30"/>
+      <location filename="../gui/types_input/StructInput.py" line="77"/>
+      <location filename="../gui/types_input/StructInput.py" line="31"/>
       <source>Remove</source>
-      <translation>Verwijderen</translation>
+      <translation>Löschen</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="108"/>
-      <location filename="../gui/types_input/StructInput.py" line="45"/>
+      <location filename="../gui/types_input/StructInput.py" line="111"/>
+      <location filename="../gui/types_input/StructInput.py" line="48"/>
       <source>Edit Struct</source>
-      <translation>Struct bewerken</translation>
+      <translation>Struktur bearbeiten</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="102"/>
+      <location filename="../gui/types_input/StructInput.py" line="105"/>
       <source>Data invalid</source>
-      <translation>Ongeldige gegevens</translation>
+      <translation>Daten ungültig</translation>
     </message>
     <message>
-      <location filename="../gui/types_input/StructInput.py" line="102"/>
+      <location filename="../gui/types_input/StructInput.py" line="105"/>
       <source>Your data is not valid</source>
-      <translation>Je gegevens zĳn ongeldig</translation>
+      <translation>Die Daten sind ungültig</translation>
     </message>
   </context>
   <context>
     <name>WelcomeDialog</name>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome</source>
-      <translation>Welkom</translation>
+      <translation>Willkommen</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome to jdDBusDebugger!</source>
-      <translation>Welkom in jdDBusDebugger!</translation>
+      <translation>Willkommen bei jdDBusDebugger!</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program allows you to easily debug your D-Bus interfaces. You can do everything in a nice GUI, so you don't need to fund out how to correctly format the input.</source>
-      <translation>Met dit programma kun je gemakkelĳk fouten opsporen in D-Bus-interfaces. Alles zit verpakt in een mooi grafisch jasje, zodat je niet hoeft uit te vogelen hoe je de invoer moet opmaken.</translation>
+      <translation>Dieses Programm erlaubt dir einfach deine D-Bus Schnittstellen zu debuggen. Du kannst alles in einer leicht zu benutzenden GUI erledigen, sodass du nicht lernen musst, wie man alle Daten korrekt formatiert.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>You can also record macros, so you can repeat your tests easily. It is even possible to generate a shell script out of a macro.</source>
-      <translation>Daarnaast kun je macro's opnemen, zodat je testen gemakkelĳk kunt herhalen. Ook kun je van een macro een shellscript maken.</translation>
+      <translation>Du kannst auch Makros aufnehme, sodass du deine tests einfach wiederholen kannst. Es ist sogar möglich aus deinen Makros ein Shellskript zu generieren.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Not every complex type is supported at the Moment, but I will keep working on adding it.</source>
-      <translation>Momenteel is er nog geen ondersteuning voor elk complex type, maar ik zal in de toekomst meer toevoegen.</translation>
+      <translation>Aktuell wird nicht jeder komlexer Typ unterstützt. An der Unterstützung wird jedoch bereits gearbeitet.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>If you want to report a Bug or left Feedback, use ?&gt;Report bug</source>
-      <translation>Als je een bug wilt melden of feedback wilt delen, dan kan dat via ? → Bug melden</translation>
+      <translation>Wenn du einen Fehler melden oder Feedback geben möchtest, benutze ?&gt;Fehler melden</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Show this on startup</source>
-      <translation>Altĳd tonen na opstarten</translation>
+      <translation>Beim starten anzeigen</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
     </message>
   </context>
 </TS>
```

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/Connection.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/Connection.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/DBusType.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/DBusType.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/DBusValue.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/DBusValue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt6.QtDBus import QDBusVariant, QDBusArgument, QDBusUnixFileDescriptor
+from PyQt6.QtDBus import QDBusVariant, QDBusArgument, QDBusUnixFileDescriptor, QDBusObjectPath
 from .DBusType import DBusTypeEnum, DBusType
 from PyQt6.QtCore import QByteArray
 from .EnumHelper import EnumHelper
 from typing import Any
 
 
 class BytearraySource(EnumHelper):
@@ -96,14 +96,16 @@
                         try:
                             with open(self.value["path"], "rb") as f:
                                 return QByteArray(f.read())
                         except Exception:
                             return QByteArray()
                     case _:
                         return QByteArray()
+            case DBusTypeEnum.OBJECT_PATH:
+                return QDBusObjectPath(self.value)
 
     def get_printable_text(self) -> str:
         match self.dbus_type.type_const:
             case DBusTypeEnum.DICT:
                 print_dict: dict[str, str] = {}
                 for key, value in self.value.items():
                     print_dict[key] = value.get_printable_text()
```

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/Interface.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/Interface.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/Macro.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/Macro.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/Method.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/Method.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/Property.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/Property.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/Service.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/Service.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,28 +34,39 @@
     def _introspect_node(self, parent_path: str, name: str, error_list: list[str]) -> None:
         current_path = parent_path.removesuffix("/") + "/" + name
 
         message = QDBusMessage.createMethodCall(self.name, current_path, "org.freedesktop.DBus.Introspectable", "Introspect")
         result = self.connection.connection.call(message)
 
         if result.errorName() != "":
-            error_list.append(result.errorMessage())
+            if result.errorMessage() == "":
+                error_list.append(result.errorName())
+            else:
+                error_list.append(f"{result.errorName()}: {result.errorMessage()}")
+            return
+
+        if len(result.arguments()) != 1 or not isinstance(result.arguments()[0], str):
+            error_list.append("Introspect has wrong return type")
             return
 
         xml_string: str = result.arguments()[0]
 
-        root = etree.parse(io.BytesIO(xml_string.encode("utf-8")))
+        try:
+            root = etree.parse(io.BytesIO(xml_string.encode("utf-8")))
+
+            self.objects[current_path] = []
+            for interface_element in root.findall("interface"):
+                inter = Interface.from_xml(self, current_path, interface_element)
+                self.objects[current_path].append(inter)
 
-        self.objects[current_path] = []
-        for interface_element in root.findall("interface"):
-            inter = Interface.from_xml(self, current_path, interface_element)
-            self.objects[current_path].append(inter)
+            for child_node in root.findall("node"):
+                self._introspect_node(current_path, child_node.get("name"), error_list)
 
-        for child_node in root.findall("node"):
-            self._introspect_node(current_path, child_node.get("name"), error_list)
+        except Exception as ex:
+            error_list.append(f"Failed to parse Introspect XML: {ex}")
 
     def add_object_path(self, object_path: str) -> tuple[list[Interface] | None, list[str]]:
         error_list: list[str] = []
         self._introspect_node(os.path.dirname(object_path), os.path.basename(object_path), error_list)
         return self.objects.get(object_path), error_list
 
     def load(self) -> list[str]:
```

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/Signal.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/Signal.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/actions/ActionBase.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/actions/ActionBase.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/actions/CallAction.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/actions/CallAction.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/actions/EmitAction.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/actions/EmitAction.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/actions/PropertyAction.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/actions/PropertyAction.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/types/actions/SignalAction.py` & `jddbusdebugger-3.0/jdDBusDebugger/types/actions/SignalAction.py`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/ui/AboutDialog.ui` & `jddbusdebugger-3.0/jdDBusDebugger/ui/AboutDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/ui/CentralWidget.ui` & `jddbusdebugger-3.0/jdDBusDebugger/ui/CentralWidget.ui`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/ui/ConnectDialog.ui` & `jddbusdebugger-3.0/jdDBusDebugger/ui/ConnectDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/ui/EmitSignalDialog.ui` & `jddbusdebugger-3.0/jdDBusDebugger/ui/EmitSignalDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/ui/GenerateScriptDialog.ui` & `jddbusdebugger-3.0/jdDBusDebugger/ui/GenerateScriptDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/ui/MainWindow.ui` & `jddbusdebugger-3.0/jdDBusDebugger/ui/MainWindow.ui`

 * *Files 2% similar despite different names*

#### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/ui/MainWindow.ui` & `jddbusdebugger-3.0/jdDBusDebugger/ui/MainWindow.ui`

```diff
@@ -95,14 +95,15 @@
         <addaction name="about_qt_action"/>
       </widget>
       <widget class="QMenu" name="menuTools">
         <property name="title">
           <string>Tools</string>
         </property>
         <addaction name="emit_signal_action"/>
+        <addaction name="monitor_action"/>
       </widget>
       <addaction name="menuFile"/>
       <addaction name="menuSettings"/>
       <addaction name="menuMacros"/>
       <addaction name="menuTools"/>
       <addaction name="menu"/>
     </widget>
@@ -193,11 +194,16 @@
       </property>
     </action>
     <action name="emit_signal_action">
       <property name="text">
         <string>Emit Signal</string>
       </property>
     </action>
+    <action name="monitor_action">
+      <property name="text">
+        <string>Monitor</string>
+      </property>
+    </action>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/ui/ManageMacrosDialog.ui` & `jddbusdebugger-3.0/jdDBusDebugger/ui/ManageMacrosDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/ui/SettingsDialog.ui` & `jddbusdebugger-3.0/jdDBusDebugger/ui/SettingsDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger/ui/WelcomeDialog.ui` & `jddbusdebugger-3.0/jdDBusDebugger/ui/WelcomeDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger.egg-info/PKG-INFO` & `jddbusdebugger-3.0/jdDBusDebugger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdDBusDebugger
-Version: 2.0
+Version: 3.0
 Summary: An advanced D-Bus Debugger
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdDBusDebugger
 Project-URL: Issues, https://codeberg.org/JakobDev/jdDBusDebugger/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdDBusDebugger
 Project-URL: Donation, https://ko-fi.com/jakobdev
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyQt6
 Requires-Dist: lxml
+Requires-Dist: jeepney
 
 <h1 align="center">jdDBusDebugger</h1>
 
 <h3 align="center">An advanced D-Bus Debugger</h3>
 
 <p align="center">
     <img alt="jdDBusDebugger" src="screenshots/MainWindow.png"/>
```

### Comparing `jdDBusDebugger-2.0/jdDBusDebugger.egg-info/SOURCES.txt` & `jddbusdebugger-3.0/jdDBusDebugger.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 jdDBusDebugger/gui/AboutDialog.py
 jdDBusDebugger/gui/CentralWidget.py
 jdDBusDebugger/gui/ConnectDialog.py
 jdDBusDebugger/gui/EmitSignalDialog.py
 jdDBusDebugger/gui/GenerateScriptDialog.py
 jdDBusDebugger/gui/MainWindow.py
 jdDBusDebugger/gui/ManageMacrosDialog.py
+jdDBusDebugger/gui/MonitorWindow.py
 jdDBusDebugger/gui/SettingsDialog.py
 jdDBusDebugger/gui/WelcomeDialog.py
 jdDBusDebugger/gui/types_input/ArgumentInput.py
 jdDBusDebugger/gui/types_input/ArrayInput.py
 jdDBusDebugger/gui/types_input/BrowseButton.py
 jdDBusDebugger/gui/types_input/BytearrayInput.py
 jdDBusDebugger/gui/types_input/DictInput.py
@@ -63,9 +64,10 @@
 jdDBusDebugger/ui/AboutDialog.ui
 jdDBusDebugger/ui/CentralWidget.ui
 jdDBusDebugger/ui/ConnectDialog.ui
 jdDBusDebugger/ui/EmitSignalDialog.ui
 jdDBusDebugger/ui/GenerateScriptDialog.ui
 jdDBusDebugger/ui/MainWindow.ui
 jdDBusDebugger/ui/ManageMacrosDialog.ui
+jdDBusDebugger/ui/MonitorWindow.ui
 jdDBusDebugger/ui/SettingsDialog.ui
 jdDBusDebugger/ui/WelcomeDialog.ui
```

### Comparing `jdDBusDebugger-2.0/pyproject.toml` & `jddbusdebugger-3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython"
 ]
 dependencies = [
   "PyQt6",
-  "lxml"
+  "lxml",
+  "jeepney"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://codeberg.org/JakobDev/jdDBusDebugger"
 Issues = "https://codeberg.org/JakobDev/jdDBusDebugger/issues"
 Translate = "https://translate.codeberg.org/projects/jdDBusDebugger"
```

