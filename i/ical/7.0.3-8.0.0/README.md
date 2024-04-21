# Comparing `tmp/ical-7.0.3.tar.gz` & `tmp/ical-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ical-7.0.3.tar", last modified: Fri Mar 15 15:50:24 2024, max compression
+gzip compressed data, was "ical-8.0.0.tar", last modified: Sun Apr 21 03:10:37 2024, max compression
```

## Comparing `ical-7.0.3.tar` & `ical-8.0.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:50:24.575039 ical-7.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-15 15:50:20.000000 ical-7.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-03-15 15:50:24.575039 ical-7.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-15 15:50:20.000000 ical-7.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:50:24.567039 ical-7.0.3/ical/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-15 15:50:20.000000 ical-7.0.3/ical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-03-15 15:50:20.000000 ical-7.0.3/ical/alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-03-15 15:50:20.000000 ical-7.0.3/ical/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-03-15 15:50:20.000000 ical-7.0.3/ical/calendar_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    13936 2024-03-15 15:50:20.000000 ical-7.0.3/ical/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-15 15:50:20.000000 ical-7.0.3/ical/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17245 2024-03-15 15:50:20.000000 ical-7.0.3/ical/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-15 15:50:20.000000 ical-7.0.3/ical/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-03-15 15:50:20.000000 ical-7.0.3/ical/freebusy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-03-15 15:50:20.000000 ical-7.0.3/ical/iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-03-15 15:50:20.000000 ical-7.0.3/ical/journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-03-15 15:50:20.000000 ical-7.0.3/ical/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:50:24.567039 ical-7.0.3/ical/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-15 15:50:20.000000 ical-7.0.3/ical/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-03-15 15:50:20.000000 ical-7.0.3/ical/parsing/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-15 15:50:20.000000 ical-7.0.3/ical/parsing/const.py
--rw-r--r--   0 runner    (1001) docker     (127)   254594 2024-03-15 15:50:20.000000 ical-7.0.3/ical/parsing/emoji.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-15 15:50:20.000000 ical-7.0.3/ical/parsing/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-15 15:50:20.000000 ical-7.0.3/ical/parsing/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-03-15 15:50:20.000000 ical-7.0.3/ical/parsing/unicode.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:50:20.000000 ical-7.0.3/ical/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-03-15 15:50:20.000000 ical-7.0.3/ical/recur_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-03-15 15:50:20.000000 ical-7.0.3/ical/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-03-15 15:50:20.000000 ical-7.0.3/ical/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-03-15 15:50:20.000000 ical-7.0.3/ical/timespan.py
--rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-03-15 15:50:20.000000 ical-7.0.3/ical/timezone.py
--rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-03-15 15:50:20.000000 ical-7.0.3/ical/todo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:50:24.571040 ical-7.0.3/ical/types/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/cal_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/float.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/geo.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/period.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/priority.py
--rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/recur.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-15 15:50:20.000000 ical-7.0.3/ical/types/utc_offset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:50:24.571040 ical-7.0.3/ical/tzif/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-15 15:50:20.000000 ical-7.0.3/ical/tzif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-15 15:50:20.000000 ical-7.0.3/ical/tzif/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-03-15 15:50:20.000000 ical-7.0.3/ical/tzif/timezoneinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-03-15 15:50:20.000000 ical-7.0.3/ical/tzif/tz_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-03-15 15:50:20.000000 ical-7.0.3/ical/tzif/tzif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-15 15:50:20.000000 ical-7.0.3/ical/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:50:24.575039 ical-7.0.3/ical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-03-15 15:50:24.000000 ical-7.0.3/ical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-15 15:50:24.000000 ical-7.0.3/ical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 15:50:24.000000 ical-7.0.3/ical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-15 15:50:24.000000 ical-7.0.3/ical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 15:50:24.000000 ical-7.0.3/ical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-15 15:50:24.579040 ical-7.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-15 15:50:20.000000 ical-7.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:50:24.575039 ical-7.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_calendar_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_freebusy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    43351 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_timezone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-03-15 15:50:20.000000 ical-7.0.3/tests/test_todo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:10:37.657776 ical-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 03:10:29.000000 ical-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-21 03:10:37.657776 ical-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-21 03:10:29.000000 ical-8.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:10:37.649776 ical-8.0.0/ical/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-21 03:10:29.000000 ical-8.0.0/ical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-21 03:10:29.000000 ical-8.0.0/ical/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-21 03:10:29.000000 ical-8.0.0/ical/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-21 03:10:29.000000 ical-8.0.0/ical/calendar_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13936 2024-04-21 03:10:29.000000 ical-8.0.0/ical/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-21 03:10:29.000000 ical-8.0.0/ical/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17245 2024-04-21 03:10:29.000000 ical-8.0.0/ical/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-21 03:10:29.000000 ical-8.0.0/ical/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-21 03:10:29.000000 ical-8.0.0/ical/freebusy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-04-21 03:10:29.000000 ical-8.0.0/ical/iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-21 03:10:29.000000 ical-8.0.0/ical/journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-21 03:10:29.000000 ical-8.0.0/ical/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:10:37.649776 ical-8.0.0/ical/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 03:10:29.000000 ical-8.0.0/ical/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-21 03:10:29.000000 ical-8.0.0/ical/parsing/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-21 03:10:29.000000 ical-8.0.0/ical/parsing/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)   254594 2024-04-21 03:10:29.000000 ical-8.0.0/ical/parsing/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-21 03:10:29.000000 ical-8.0.0/ical/parsing/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-21 03:10:29.000000 ical-8.0.0/ical/parsing/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-21 03:10:29.000000 ical-8.0.0/ical/parsing/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:10:29.000000 ical-8.0.0/ical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-21 03:10:29.000000 ical-8.0.0/ical/recur_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-04-21 03:10:29.000000 ical-8.0.0/ical/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-21 03:10:29.000000 ical-8.0.0/ical/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-21 03:10:29.000000 ical-8.0.0/ical/timespan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-04-21 03:10:29.000000 ical-8.0.0/ical/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-04-21 03:10:29.000000 ical-8.0.0/ical/todo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:10:37.653776 ical-8.0.0/ical/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/cal_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/period.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/recur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-21 03:10:29.000000 ical-8.0.0/ical/types/utc_offset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:10:37.653776 ical-8.0.0/ical/tzif/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-21 03:10:29.000000 ical-8.0.0/ical/tzif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-21 03:10:29.000000 ical-8.0.0/ical/tzif/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-21 03:10:29.000000 ical-8.0.0/ical/tzif/timezoneinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-21 03:10:29.000000 ical-8.0.0/ical/tzif/tz_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-21 03:10:29.000000 ical-8.0.0/ical/tzif/tzif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-21 03:10:29.000000 ical-8.0.0/ical/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:10:37.657776 ical-8.0.0/ical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-21 03:10:37.000000 ical-8.0.0/ical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-21 03:10:37.000000 ical-8.0.0/ical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 03:10:37.000000 ical-8.0.0/ical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-21 03:10:37.000000 ical-8.0.0/ical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-21 03:10:37.000000 ical-8.0.0/ical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-21 03:10:37.657776 ical-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-21 03:10:29.000000 ical-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:10:37.657776 ical-8.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_calendar_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_freebusy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43351 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-04-21 03:10:29.000000 ical-8.0.0/tests/test_todo.py
```

### Comparing `ical-7.0.3/LICENSE` & `ical-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/PKG-INFO` & `ical-8.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ical
-Version: 7.0.3
+Version: 8.0.0
 Summary: Python iCalendar implementation (rfc 2445)
 Home-page: https://github.com/allenporter/ical
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `ical-7.0.3/README.md` & `ical-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/alarm.py` & `ical-8.0.0/ical/alarm.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/calendar.py` & `ical-8.0.0/ical/calendar.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/calendar_stream.py` & `ical-8.0.0/ical/calendar_stream.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/component.py` & `ical-8.0.0/ical/component.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/diagnostics.py` & `ical-8.0.0/ical/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/event.py` & `ical-8.0.0/ical/event.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/exceptions.py` & `ical-8.0.0/ical/exceptions.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/freebusy.py` & `ical-8.0.0/ical/freebusy.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/iter.py` & `ical-8.0.0/ical/iter.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/journal.py` & `ical-8.0.0/ical/journal.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/list.py` & `ical-8.0.0/ical/list.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/parsing/component.py` & `ical-8.0.0/ical/parsing/component.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/parsing/emoji.py` & `ical-8.0.0/ical/parsing/emoji.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/parsing/parser.py` & `ical-8.0.0/ical/parsing/parser.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/parsing/property.py` & `ical-8.0.0/ical/parsing/property.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/parsing/unicode.py` & `ical-8.0.0/ical/parsing/unicode.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/recur_adapter.py` & `ical-8.0.0/ical/recur_adapter.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/store.py` & `ical-8.0.0/ical/store.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/timeline.py` & `ical-8.0.0/ical/timeline.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/timespan.py` & `ical-8.0.0/ical/timespan.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/timezone.py` & `ical-8.0.0/ical/timezone.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     from pydantic import Field, root_validator, validator  # type: ignore[no-redef, assignment]
 
 from .component import ComponentModel
 from .iter import MergedIterable, RecurIterable
 from .parsing.property import ParsedProperty
 from .types import Recur, Uri, UtcOffset
 from .tzif import timezoneinfo, tz_rule
-from .util import dtstamp_factory
 
 __all__ = [
     "Timezone",
     "Observance",
 ]
 
 _LOGGER = logging.getLogger(__name__)
@@ -131,19 +130,14 @@
 class Timezone(ComponentModel):
     """A single free/busy entry on a calendar.
 
     A Timezone must have at least one definition of a standard or daylight
     sub-component.
     """
 
-    dtstamp: Union[datetime.datetime, datetime.date] = Field(
-        default_factory=lambda: dtstamp_factory()
-    )
-    """Last revision date."""
-
     tz_id: str = Field(alias="tzid")
     """An identifier for this Timezone, unique within a calendar."""
 
     standard: list[Observance] = Field(default_factory=list)
     """Describes the base offset from UTC for the time zone."""
 
     daylight: list[Observance] = Field(default_factory=list)
```

### Comparing `ical-7.0.3/ical/todo.py` & `ical-8.0.0/ical/todo.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/__init__.py` & `ical-8.0.0/ical/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/boolean.py` & `ical-8.0.0/ical/types/boolean.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/cal_address.py` & `ical-8.0.0/ical/types/cal_address.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/data_types.py` & `ical-8.0.0/ical/types/data_types.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/date.py` & `ical-8.0.0/ical/types/date.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/date_time.py` & `ical-8.0.0/ical/types/date_time.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/duration.py` & `ical-8.0.0/ical/types/duration.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/geo.py` & `ical-8.0.0/ical/types/geo.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/integer.py` & `ical-8.0.0/ical/types/integer.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/parsing.py` & `ical-8.0.0/ical/types/parsing.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/period.py` & `ical-8.0.0/ical/types/period.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/priority.py` & `ical-8.0.0/ical/types/priority.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/recur.py` & `ical-8.0.0/ical/types/recur.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/relation.py` & `ical-8.0.0/ical/types/relation.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/request_status.py` & `ical-8.0.0/ical/types/request_status.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/text.py` & `ical-8.0.0/ical/types/text.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/uri.py` & `ical-8.0.0/ical/types/uri.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/types/utc_offset.py` & `ical-8.0.0/ical/types/utc_offset.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/tzif/model.py` & `ical-8.0.0/ical/tzif/model.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/tzif/timezoneinfo.py` & `ical-8.0.0/ical/tzif/timezoneinfo.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/tzif/tz_rule.py` & `ical-8.0.0/ical/tzif/tz_rule.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/tzif/tzif.py` & `ical-8.0.0/ical/tzif/tzif.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical/util.py` & `ical-8.0.0/ical/util.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/ical.egg-info/PKG-INFO` & `ical-8.0.0/ical.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ical
-Version: 7.0.3
+Version: 8.0.0
 Summary: Python iCalendar implementation (rfc 2445)
 Home-page: https://github.com/allenporter/ical
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `ical-7.0.3/ical.egg-info/SOURCES.txt` & `ical-8.0.0/ical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/setup.cfg` & `ical-8.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ical
-version = 7.0.3
+version = 8.0.0
 description = Python iCalendar implementation (rfc 2445)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/ical
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `ical-7.0.3/tests/test_alarm.py` & `ical-8.0.0/tests/test_alarm.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_calendar.py` & `ical-8.0.0/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_calendar_stream.py` & `ical-8.0.0/tests/test_calendar_stream.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_component.py` & `ical-8.0.0/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_diagnostics.py` & `ical-8.0.0/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_event.py` & `ical-8.0.0/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_freebusy.py` & `ical-8.0.0/tests/test_freebusy.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_iter.py` & `ical-8.0.0/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_journal.py` & `ical-8.0.0/tests/test_journal.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_list.py` & `ical-8.0.0/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_store.py` & `ical-8.0.0/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_timeline.py` & `ical-8.0.0/tests/test_timeline.py`

 * *Files identical despite different names*

### Comparing `ical-7.0.3/tests/test_timezone.py` & `ical-8.0.0/tests/test_timezone.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,15 +90,14 @@
     stream = IcsCalendarStream(calendars=[calendar])
     assert stream.ics() == inspect.cleandoc(
         """
        BEGIN:VCALENDAR
        PRODID:-//example//1.2.3
        VERSION:2.0
        BEGIN:VTIMEZONE
-       DTSTAMP:20220822T123000
        TZID:America/New_York
        BEGIN:STANDARD
        DTSTART:20101107T020000
        TZOFFSETTO:-0500
        TZOFFSETFROM:-0400
        RRULE:FREQ=YEARLY;BYDAY=1SU;BYMONTH=11
        TZNAME:EST
@@ -152,15 +151,14 @@
     stream = IcsCalendarStream(calendars=[calendar])
     assert stream.ics() == inspect.cleandoc(
         """
        BEGIN:VCALENDAR
        PRODID:-//example//1.2.3
        VERSION:2.0
        BEGIN:VTIMEZONE
-       DTSTAMP:20220822T123000
        TZID:Asia/Tokyo
        BEGIN:STANDARD
        DTSTART:20100101T000000
        TZOFFSETTO:0900
        TZOFFSETFROM:0900
        TZNAME:JST
        END:STANDARD
@@ -171,7 +169,48 @@
 
 
 def test_invalid_tzif_key() -> None:
     """Test creating a timezone object from tzif data that does not exist."""
 
     with pytest.raises(TimezoneInfoError, match=r"Unable to find timezone"):
         Timezone.from_tzif("invalid")
+
+
+
+@freeze_time("2022-08-22 12:30:00")
+def test_clear_old_dtstamp(
+    mock_prodid: Generator[None, None, None]
+) -> None:
+    """Verify a timezone created from a tzif timezone info with a fixed offset"""
+
+    stream = IcsCalendarStream.from_ics(inspect.cleandoc("""
+       BEGIN:VCALENDAR
+       PRODID:-//example//1.2.3
+       VERSION:2.0
+       BEGIN:VTIMEZONE
+       DTSTAMP:20220822T123000
+       TZID:Asia/Tokyo
+       BEGIN:STANDARD
+       DTSTART:20100101T000000
+       TZOFFSETTO:0900
+       TZOFFSETFROM:0900
+       TZNAME:JST
+       END:STANDARD
+       END:VTIMEZONE
+       END:VCALENDAR
+    """))
+    # DTSTAMP is omitted from the output
+    assert stream.ics() == inspect.cleandoc("""
+       BEGIN:VCALENDAR
+       PRODID:-//example//1.2.3
+       VERSION:2.0
+       BEGIN:VTIMEZONE
+       TZID:Asia/Tokyo
+       BEGIN:STANDARD
+       DTSTART:20100101T000000
+       TZOFFSETTO:0900
+       TZOFFSETFROM:0900
+       TZNAME:JST
+       END:STANDARD
+       END:VTIMEZONE
+       END:VCALENDAR
+    """)
```

### Comparing `ical-7.0.3/tests/test_todo.py` & `ical-8.0.0/tests/test_todo.py`

 * *Files identical despite different names*

