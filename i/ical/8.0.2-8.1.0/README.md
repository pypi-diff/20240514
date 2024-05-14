# Comparing `tmp/ical-8.0.2.tar.gz` & `tmp/ical-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ical-8.0.2.tar", last modified: Mon May 13 00:06:06 2024, max compression
+gzip compressed data, was "ical-8.1.0.tar", last modified: Tue May 14 15:06:21 2024, max compression
```

## Comparing `ical-8.0.2.tar` & `ical-8.1.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.877480 ical-8.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 00:06:02.000000 ical-8.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-13 00:06:06.877480 ical-8.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-13 00:06:02.000000 ical-8.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.869480 ical-8.0.2/ical/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-13 00:06:02.000000 ical-8.0.2/ical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-13 00:06:02.000000 ical-8.0.2/ical/alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-13 00:06:02.000000 ical-8.0.2/ical/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-13 00:06:02.000000 ical-8.0.2/ical/calendar_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    13936 2024-05-13 00:06:02.000000 ical-8.0.2/ical/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-13 00:06:02.000000 ical-8.0.2/ical/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17245 2024-05-13 00:06:02.000000 ical-8.0.2/ical/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-13 00:06:02.000000 ical-8.0.2/ical/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-13 00:06:02.000000 ical-8.0.2/ical/freebusy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-05-13 00:06:02.000000 ical-8.0.2/ical/iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-13 00:06:02.000000 ical-8.0.2/ical/journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-13 00:06:02.000000 ical-8.0.2/ical/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.869480 ical-8.0.2/ical/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/const.py
--rw-r--r--   0 runner    (1001) docker     (127)   254594 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/emoji.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-13 00:06:02.000000 ical-8.0.2/ical/parsing/unicode.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:02.000000 ical-8.0.2/ical/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-13 00:06:02.000000 ical-8.0.2/ical/recur_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18113 2024-05-13 00:06:02.000000 ical-8.0.2/ical/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-13 00:06:02.000000 ical-8.0.2/ical/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-13 00:06:02.000000 ical-8.0.2/ical/timespan.py
--rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-05-13 00:06:02.000000 ical-8.0.2/ical/timezone.py
--rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-05-13 00:06:02.000000 ical-8.0.2/ical/todo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.873479 ical-8.0.2/ical/types/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/cal_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/float.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/geo.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/period.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/priority.py
--rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/recur.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-13 00:06:02.000000 ical-8.0.2/ical/types/utc_offset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.873479 ical-8.0.2/ical/tzif/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 00:06:02.000000 ical-8.0.2/ical/tzif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-13 00:06:02.000000 ical-8.0.2/ical/tzif/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-13 00:06:02.000000 ical-8.0.2/ical/tzif/timezoneinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-13 00:06:02.000000 ical-8.0.2/ical/tzif/tz_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-05-13 00:06:02.000000 ical-8.0.2/ical/tzif/tzif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-13 00:06:02.000000 ical-8.0.2/ical/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.877480 ical-8.0.2/ical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-13 00:06:06.000000 ical-8.0.2/ical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-13 00:06:06.000000 ical-8.0.2/ical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 00:06:06.000000 ical-8.0.2/ical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 00:06:06.000000 ical-8.0.2/ical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 00:06:06.000000 ical-8.0.2/ical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-13 00:06:02.000000 ical-8.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-13 00:06:06.881480 ical-8.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 00:06:02.000000 ical-8.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:06:06.877480 ical-8.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_calendar_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_freebusy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    43647 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_timezone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-05-13 00:06:02.000000 ical-8.0.2/tests/test_todo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:06:21.995002 ical-8.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 15:06:17.000000 ical-8.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-14 15:06:21.995002 ical-8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-14 15:06:17.000000 ical-8.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:06:21.983002 ical-8.1.0/ical/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-14 15:06:17.000000 ical-8.1.0/ical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-14 15:06:17.000000 ical-8.1.0/ical/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-14 15:06:17.000000 ical-8.1.0/ical/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-14 15:06:17.000000 ical-8.1.0/ical/calendar_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13936 2024-05-14 15:06:17.000000 ical-8.1.0/ical/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-14 15:06:17.000000 ical-8.1.0/ical/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17245 2024-05-14 15:06:17.000000 ical-8.1.0/ical/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-14 15:06:17.000000 ical-8.1.0/ical/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-14 15:06:17.000000 ical-8.1.0/ical/freebusy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-05-14 15:06:17.000000 ical-8.1.0/ical/iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-14 15:06:17.000000 ical-8.1.0/ical/journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-14 15:06:17.000000 ical-8.1.0/ical/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:06:21.987002 ical-8.1.0/ical/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 15:06:17.000000 ical-8.1.0/ical/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-14 15:06:17.000000 ical-8.1.0/ical/parsing/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 15:06:17.000000 ical-8.1.0/ical/parsing/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)   282927 2024-05-14 15:06:17.000000 ical-8.1.0/ical/parsing/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-14 15:06:17.000000 ical-8.1.0/ical/parsing/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-14 15:06:17.000000 ical-8.1.0/ical/parsing/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-14 15:06:17.000000 ical-8.1.0/ical/parsing/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:06:17.000000 ical-8.1.0/ical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-14 15:06:17.000000 ical-8.1.0/ical/recur_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18113 2024-05-14 15:06:17.000000 ical-8.1.0/ical/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-14 15:06:17.000000 ical-8.1.0/ical/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-14 15:06:17.000000 ical-8.1.0/ical/timespan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-05-14 15:06:17.000000 ical-8.1.0/ical/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-05-14 15:06:17.000000 ical-8.1.0/ical/todo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:06:21.991002 ical-8.1.0/ical/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/cal_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/period.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/recur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-14 15:06:17.000000 ical-8.1.0/ical/types/utc_offset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:06:21.991002 ical-8.1.0/ical/tzif/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 15:06:17.000000 ical-8.1.0/ical/tzif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-14 15:06:17.000000 ical-8.1.0/ical/tzif/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-14 15:06:17.000000 ical-8.1.0/ical/tzif/timezoneinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-14 15:06:17.000000 ical-8.1.0/ical/tzif/tz_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-05-14 15:06:17.000000 ical-8.1.0/ical/tzif/tzif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-14 15:06:17.000000 ical-8.1.0/ical/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:06:21.995002 ical-8.1.0/ical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-14 15:06:21.000000 ical-8.1.0/ical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-14 15:06:21.000000 ical-8.1.0/ical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:06:21.000000 ical-8.1.0/ical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:06:21.000000 ical-8.1.0/ical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 15:06:21.000000 ical-8.1.0/ical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-14 15:06:17.000000 ical-8.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 15:06:21.995002 ical-8.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 15:06:17.000000 ical-8.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:06:21.995002 ical-8.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_calendar_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_freebusy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43647 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-05-14 15:06:17.000000 ical-8.1.0/tests/test_todo.py
```

### Comparing `ical-8.0.2/LICENSE` & `ical-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/PKG-INFO` & `ical-8.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ical
-Version: 8.0.2
+Version: 8.1.0
 Summary: Python iCalendar implementation (rfc 2445)
 Home-page: https://github.com/allenporter/ical
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `ical-8.0.2/README.md` & `ical-8.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/alarm.py` & `ical-8.1.0/ical/alarm.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/calendar.py` & `ical-8.1.0/ical/calendar.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/calendar_stream.py` & `ical-8.1.0/ical/calendar_stream.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/component.py` & `ical-8.1.0/ical/component.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/diagnostics.py` & `ical-8.1.0/ical/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/event.py` & `ical-8.1.0/ical/event.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/exceptions.py` & `ical-8.1.0/ical/exceptions.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/freebusy.py` & `ical-8.1.0/ical/freebusy.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/iter.py` & `ical-8.1.0/ical/iter.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/journal.py` & `ical-8.1.0/ical/journal.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/list.py` & `ical-8.1.0/ical/list.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/parsing/component.py` & `ical-8.1.0/ical/parsing/component.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/parsing/emoji.py` & `ical-8.1.0/ical/parsing/emoji.py`

 * *Files 8% similar despite different names*

```diff
@@ -318,18 +318,18 @@
   u'\U0001f1f9\U0001f1ec',  # 🇹🇬
   u'\U0001f1f9\U0001f1f0',  # 🇹🇰
   u'\U0001f5fc',  # 🗼
   u'\U0001f1f9\U0001f1f4',  # 🇹🇴
   u'\U0001f1f9\U0001f1f9',  # 🇹🇹
   u'\U0001f1f9\U0001f1e6',  # 🇹🇦
   u'\U0001f1f9\U0001f1f3',  # 🇹🇳
-  u'\U0001f1f9\U0001f1f7',  # 🇹🇷
   u'\U0001f1f9\U0001f1f2',  # 🇹🇲
   u'\U0001f1f9\U0001f1e8',  # 🇹🇨
   u'\U0001f1f9\U0001f1fb',  # 🇹🇻
+  u'\U0001f1f9\U0001f1f7',  # 🇹🇷
   u'\U0001f1fa\U0001f1f2',  # 🇺🇲
   u'\U0001f1fb\U0001f1ee',  # 🇻🇮
   u'\U0001f199',  # 🆙
   u'\U0001f1fa\U0001f1ec',  # 🇺🇬
   u'\U0001f1fa\U0001f1e6',  # 🇺🇦
   u'\U0001f1e6\U0001f1ea',  # 🇦🇪
   u'\U0001f1ec\U0001f1e7',  # 🇬🇧
@@ -539,18 +539,21 @@
   u'\U0001f931\U0001f3fd',  # 🤱🏽
   u'\U0001f9f1',  # 🧱
   u'\U0001f309',  # 🌉
   u'\U0001f4bc',  # 💼
   u'\U0001fa72',  # 🩲
   u'\U0001f506',  # 🔆
   u'\U0001f966',  # 🥦
+  u'\U000026d3\U0000fe0f\U0000200d\U0001f4a5',  # ⛓️‍💥
+  u'\U000026d3\U0000200d\U0001f4a5',  # ⛓‍💥
   u'\U0001f494',  # 💔
   u'\U0001f9f9',  # 🧹
   u'\U0001f7e4',  # 🟤
   u'\U0001f90e',  # 🤎
+  u'\U0001f344\U0000200d\U0001f7eb',  # 🍄‍🟫
   u'\U0001f7eb',  # 🟫
   u'\U0001f9cb',  # 🧋
   u'\U0001fae7',  # 🫧
   u'\U0001faa3',  # 🪣
   u'\U0001f41b',  # 🐛
   u'\U0001f3d7\U0000fe0f',  # 🏗️
   u'\U0001f3d7',  # 🏗
@@ -1143,14 +1146,18 @@
   u'\U0001f9da\U0001f3fb',  # 🧚🏻
   u'\U0001f9da\U0001f3fe',  # 🧚🏾
   u'\U0001f9da\U0001f3fc',  # 🧚🏼
   u'\U0001f9da\U0001f3fd',  # 🧚🏽
   u'\U0001f9c6',  # 🧆
   u'\U0001f342',  # 🍂
   u'\U0001f46a',  # 👪
+  u'\U0001f9d1\U0000200d\U0001f9d1\U0000200d\U0001f9d2',  # 🧑‍🧑‍🧒
+  u'\U0001f9d1\U0000200d\U0001f9d1\U0000200d\U0001f9d2\U0000200d\U0001f9d2',  # 🧑‍🧑‍🧒‍🧒
+  u'\U0001f9d1\U0000200d\U0001f9d2',  # 🧑‍🧒
+  u'\U0001f9d1\U0000200d\U0001f9d2\U0000200d\U0001f9d2',  # 🧑‍🧒‍🧒
   u'\U0001f468\U0000200d\U0001f466',  # 👨‍👦
   u'\U0001f468\U0000200d\U0001f466\U0000200d\U0001f466',  # 👨‍👦‍👦
   u'\U0001f468\U0000200d\U0001f467',  # 👨‍👧
   u'\U0001f468\U0000200d\U0001f467\U0000200d\U0001f466',  # 👨‍👧‍👦
   u'\U0001f468\U0000200d\U0001f467\U0000200d\U0001f467',  # 👨‍👧‍👧
   u'\U0001f468\U0000200d\U0001f468\U0000200d\U0001f466',  # 👨‍👨‍👦
   u'\U0001f468\U0000200d\U0001f468\U0000200d\U0001f466\U0000200d\U0001f466',  # 👨‍👨‍👦‍👦
@@ -1380,14 +1387,18 @@
   u'\U0001faf1\U0001f3fc\U0000200d\U0001faf2\U0001f3fd',  # 🫱🏼‍🫲🏽
   u'\U0001f91d\U0001f3fd',  # 🤝🏽
   u'\U0001faf1\U0001f3fd\U0000200d\U0001faf2\U0001f3ff',  # 🫱🏽‍🫲🏿
   u'\U0001faf1\U0001f3fd\U0000200d\U0001faf2\U0001f3fb',  # 🫱🏽‍🫲🏻
   u'\U0001faf1\U0001f3fd\U0000200d\U0001faf2\U0001f3fe',  # 🫱🏽‍🫲🏾
   u'\U0001faf1\U0001f3fd\U0000200d\U0001faf2\U0001f3fc',  # 🫱🏽‍🫲🏼
   u'\U0001f423',  # 🐣
+  u'\U0001f642\U0000200d\U00002194\U0000fe0f',  # 🙂‍↔️
+  u'\U0001f642\U0000200d\U00002194',  # 🙂‍↔
+  u'\U0001f642\U0000200d\U00002195\U0000fe0f',  # 🙂‍↕️
+  u'\U0001f642\U0000200d\U00002195',  # 🙂‍↕
   u'\U0001f3a7',  # 🎧
   u'\U0001faa6',  # 🪦
   u'\U0001f9d1\U0000200d\U00002695\U0000fe0f',  # 🧑‍⚕️
   u'\U0001f9d1\U0000200d\U00002695',  # 🧑‍⚕
   u'\U0001f9d1\U0001f3ff\U0000200d\U00002695\U0000fe0f',  # 🧑🏿‍⚕️
   u'\U0001f9d1\U0001f3ff\U0000200d\U00002695',  # 🧑🏿‍⚕
   u'\U0001f9d1\U0001f3fb\U0000200d\U00002695\U0000fe0f',  # 🧑🏻‍⚕️
@@ -1809,14 +1820,15 @@
   u'\U0001f406',  # 🐆
   u'\U0001f39a\U0000fe0f',  # 🎚️
   u'\U0001f39a',  # 🎚
   u'\U0001fa75',  # 🩵
   u'\U0001f4a1',  # 💡
   u'\U0001f688',  # 🚈
   u'\U0001f3fb',  # 🏻
+  u'\U0001f34b\U0000200d\U0001f7e9',  # 🍋‍🟩
   u'\U0001f517',  # 🔗
   u'\U0001f587\U0000fe0f',  # 🖇️
   u'\U0001f587',  # 🖇
   u'\U0001f981',  # 🦁
   u'\U0001f484',  # 💄
   u'\U0001f6ae',  # 🚮
   u'\U0001f98e',  # 🦎
@@ -2156,20 +2168,44 @@
   u'\U0001f9d8\U0001f3fe\U0000200d\U00002642',  # 🧘🏾‍♂
   u'\U0001f9d8\U0001f3fc\U0000200d\U00002642\U0000fe0f',  # 🧘🏼‍♂️
   u'\U0001f9d8\U0001f3fc\U0000200d\U00002642',  # 🧘🏼‍♂
   u'\U0001f9d8\U0001f3fd\U0000200d\U00002642\U0000fe0f',  # 🧘🏽‍♂️
   u'\U0001f9d8\U0001f3fd\U0000200d\U00002642',  # 🧘🏽‍♂
   u'\U0001f468\U0000200d\U0001f9bd',  # 👨‍🦽
   u'\U0001f468\U0001f3ff\U0000200d\U0001f9bd',  # 👨🏿‍🦽
+  u'\U0001f468\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👨‍🦽‍➡️
+  u'\U0001f468\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👨‍🦽‍➡
+  u'\U0001f468\U0001f3ff\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👨🏿‍🦽‍➡️
+  u'\U0001f468\U0001f3ff\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👨🏿‍🦽‍➡
+  u'\U0001f468\U0001f3fb\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👨🏻‍🦽‍➡️
+  u'\U0001f468\U0001f3fb\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👨🏻‍🦽‍➡
+  u'\U0001f468\U0001f3fe\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👨🏾‍🦽‍➡️
+  u'\U0001f468\U0001f3fe\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👨🏾‍🦽‍➡
+  u'\U0001f468\U0001f3fc\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👨🏼‍🦽‍➡️
+  u'\U0001f468\U0001f3fc\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👨🏼‍🦽‍➡
+  u'\U0001f468\U0001f3fd\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👨🏽‍🦽‍➡️
+  u'\U0001f468\U0001f3fd\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👨🏽‍🦽‍➡
   u'\U0001f468\U0001f3fb\U0000200d\U0001f9bd',  # 👨🏻‍🦽
   u'\U0001f468\U0001f3fe\U0000200d\U0001f9bd',  # 👨🏾‍🦽
   u'\U0001f468\U0001f3fc\U0000200d\U0001f9bd',  # 👨🏼‍🦽
   u'\U0001f468\U0001f3fd\U0000200d\U0001f9bd',  # 👨🏽‍🦽
   u'\U0001f468\U0000200d\U0001f9bc',  # 👨‍🦼
   u'\U0001f468\U0001f3ff\U0000200d\U0001f9bc',  # 👨🏿‍🦼
+  u'\U0001f468\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👨‍🦼‍➡️
+  u'\U0001f468\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👨‍🦼‍➡
+  u'\U0001f468\U0001f3ff\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👨🏿‍🦼‍➡️
+  u'\U0001f468\U0001f3ff\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👨🏿‍🦼‍➡
+  u'\U0001f468\U0001f3fb\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👨🏻‍🦼‍➡️
+  u'\U0001f468\U0001f3fb\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👨🏻‍🦼‍➡
+  u'\U0001f468\U0001f3fe\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👨🏾‍🦼‍➡️
+  u'\U0001f468\U0001f3fe\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👨🏾‍🦼‍➡
+  u'\U0001f468\U0001f3fc\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👨🏼‍🦼‍➡️
+  u'\U0001f468\U0001f3fc\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👨🏼‍🦼‍➡
+  u'\U0001f468\U0001f3fd\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👨🏽‍🦼‍➡️
+  u'\U0001f468\U0001f3fd\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👨🏽‍🦼‍➡
   u'\U0001f468\U0001f3fb\U0000200d\U0001f9bc',  # 👨🏻‍🦼
   u'\U0001f468\U0001f3fe\U0000200d\U0001f9bc',  # 👨🏾‍🦼
   u'\U0001f468\U0001f3fc\U0000200d\U0001f9bc',  # 👨🏼‍🦼
   u'\U0001f468\U0001f3fd\U0000200d\U0001f9bc',  # 👨🏽‍🦼
   u'\U0001f9d6\U0000200d\U00002642\U0000fe0f',  # 🧖‍♂️
   u'\U0001f9d6\U0000200d\U00002642',  # 🧖‍♂
   u'\U0001f9d6\U0001f3ff\U0000200d\U00002642\U0000fe0f',  # 🧖🏿‍♂️
@@ -2218,14 +2254,38 @@
   u'\U0001f939\U0001f3fc\U0000200d\U00002642',  # 🤹🏼‍♂
   u'\U0001f939\U0001f3fd\U0000200d\U00002642\U0000fe0f',  # 🤹🏽‍♂️
   u'\U0001f939\U0001f3fd\U0000200d\U00002642',  # 🤹🏽‍♂
   u'\U0001f9ce\U0000200d\U00002642\U0000fe0f',  # 🧎‍♂️
   u'\U0001f9ce\U0000200d\U00002642',  # 🧎‍♂
   u'\U0001f9ce\U0001f3ff\U0000200d\U00002642\U0000fe0f',  # 🧎🏿‍♂️
   u'\U0001f9ce\U0001f3ff\U0000200d\U00002642',  # 🧎🏿‍♂
+  u'\U0001f9ce\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎‍♂️‍➡️
+  u'\U0001f9ce\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🧎‍♂‍➡️
+  u'\U0001f9ce\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🧎‍♂️‍➡
+  u'\U0001f9ce\U0000200d\U00002642\U0000200d\U000027a1',  # 🧎‍♂‍➡
+  u'\U0001f9ce\U0001f3ff\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎🏿‍♂️‍➡️
+  u'\U0001f9ce\U0001f3ff\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🧎🏿‍♂‍➡️
+  u'\U0001f9ce\U0001f3ff\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🧎🏿‍♂️‍➡
+  u'\U0001f9ce\U0001f3ff\U0000200d\U00002642\U0000200d\U000027a1',  # 🧎🏿‍♂‍➡
+  u'\U0001f9ce\U0001f3fb\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎🏻‍♂️‍➡️
+  u'\U0001f9ce\U0001f3fb\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🧎🏻‍♂‍➡️
+  u'\U0001f9ce\U0001f3fb\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🧎🏻‍♂️‍➡
+  u'\U0001f9ce\U0001f3fb\U0000200d\U00002642\U0000200d\U000027a1',  # 🧎🏻‍♂‍➡
+  u'\U0001f9ce\U0001f3fe\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎🏾‍♂️‍➡️
+  u'\U0001f9ce\U0001f3fe\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🧎🏾‍♂‍➡️
+  u'\U0001f9ce\U0001f3fe\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🧎🏾‍♂️‍➡
+  u'\U0001f9ce\U0001f3fe\U0000200d\U00002642\U0000200d\U000027a1',  # 🧎🏾‍♂‍➡
+  u'\U0001f9ce\U0001f3fc\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎🏼‍♂️‍➡️
+  u'\U0001f9ce\U0001f3fc\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🧎🏼‍♂‍➡️
+  u'\U0001f9ce\U0001f3fc\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🧎🏼‍♂️‍➡
+  u'\U0001f9ce\U0001f3fc\U0000200d\U00002642\U0000200d\U000027a1',  # 🧎🏼‍♂‍➡
+  u'\U0001f9ce\U0001f3fd\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎🏽‍♂️‍➡️
+  u'\U0001f9ce\U0001f3fd\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🧎🏽‍♂‍➡️
+  u'\U0001f9ce\U0001f3fd\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🧎🏽‍♂️‍➡
+  u'\U0001f9ce\U0001f3fd\U0000200d\U00002642\U0000200d\U000027a1',  # 🧎🏽‍♂‍➡
   u'\U0001f9ce\U0001f3fb\U0000200d\U00002642\U0000fe0f',  # 🧎🏻‍♂️
   u'\U0001f9ce\U0001f3fb\U0000200d\U00002642',  # 🧎🏻‍♂
   u'\U0001f9ce\U0001f3fe\U0000200d\U00002642\U0000fe0f',  # 🧎🏾‍♂️
   u'\U0001f9ce\U0001f3fe\U0000200d\U00002642',  # 🧎🏾‍♂
   u'\U0001f9ce\U0001f3fc\U0000200d\U00002642\U0000fe0f',  # 🧎🏼‍♂️
   u'\U0001f9ce\U0001f3fc\U0000200d\U00002642',  # 🧎🏼‍♂
   u'\U0001f9ce\U0001f3fd\U0000200d\U00002642\U0000fe0f',  # 🧎🏽‍♂️
@@ -2401,14 +2461,38 @@
   u'\U0001f6a3\U0001f3fc\U0000200d\U00002642',  # 🚣🏼‍♂
   u'\U0001f6a3\U0001f3fd\U0000200d\U00002642\U0000fe0f',  # 🚣🏽‍♂️
   u'\U0001f6a3\U0001f3fd\U0000200d\U00002642',  # 🚣🏽‍♂
   u'\U0001f3c3\U0000200d\U00002642\U0000fe0f',  # 🏃‍♂️
   u'\U0001f3c3\U0000200d\U00002642',  # 🏃‍♂
   u'\U0001f3c3\U0001f3ff\U0000200d\U00002642\U0000fe0f',  # 🏃🏿‍♂️
   u'\U0001f3c3\U0001f3ff\U0000200d\U00002642',  # 🏃🏿‍♂
+  u'\U0001f3c3\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃‍♂️‍➡️
+  u'\U0001f3c3\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🏃‍♂‍➡️
+  u'\U0001f3c3\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🏃‍♂️‍➡
+  u'\U0001f3c3\U0000200d\U00002642\U0000200d\U000027a1',  # 🏃‍♂‍➡
+  u'\U0001f3c3\U0001f3ff\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃🏿‍♂️‍➡️
+  u'\U0001f3c3\U0001f3ff\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🏃🏿‍♂‍➡️
+  u'\U0001f3c3\U0001f3ff\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🏃🏿‍♂️‍➡
+  u'\U0001f3c3\U0001f3ff\U0000200d\U00002642\U0000200d\U000027a1',  # 🏃🏿‍♂‍➡
+  u'\U0001f3c3\U0001f3fb\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃🏻‍♂️‍➡️
+  u'\U0001f3c3\U0001f3fb\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🏃🏻‍♂‍➡️
+  u'\U0001f3c3\U0001f3fb\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🏃🏻‍♂️‍➡
+  u'\U0001f3c3\U0001f3fb\U0000200d\U00002642\U0000200d\U000027a1',  # 🏃🏻‍♂‍➡
+  u'\U0001f3c3\U0001f3fe\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃🏾‍♂️‍➡️
+  u'\U0001f3c3\U0001f3fe\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🏃🏾‍♂‍➡️
+  u'\U0001f3c3\U0001f3fe\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🏃🏾‍♂️‍➡
+  u'\U0001f3c3\U0001f3fe\U0000200d\U00002642\U0000200d\U000027a1',  # 🏃🏾‍♂‍➡
+  u'\U0001f3c3\U0001f3fc\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃🏼‍♂️‍➡️
+  u'\U0001f3c3\U0001f3fc\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🏃🏼‍♂‍➡️
+  u'\U0001f3c3\U0001f3fc\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🏃🏼‍♂️‍➡
+  u'\U0001f3c3\U0001f3fc\U0000200d\U00002642\U0000200d\U000027a1',  # 🏃🏼‍♂‍➡
+  u'\U0001f3c3\U0001f3fd\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃🏽‍♂️‍➡️
+  u'\U0001f3c3\U0001f3fd\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🏃🏽‍♂‍➡️
+  u'\U0001f3c3\U0001f3fd\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🏃🏽‍♂️‍➡
+  u'\U0001f3c3\U0001f3fd\U0000200d\U00002642\U0000200d\U000027a1',  # 🏃🏽‍♂‍➡
   u'\U0001f3c3\U0001f3fb\U0000200d\U00002642\U0000fe0f',  # 🏃🏻‍♂️
   u'\U0001f3c3\U0001f3fb\U0000200d\U00002642',  # 🏃🏻‍♂
   u'\U0001f3c3\U0001f3fe\U0000200d\U00002642\U0000fe0f',  # 🏃🏾‍♂️
   u'\U0001f3c3\U0001f3fe\U0000200d\U00002642',  # 🏃🏾‍♂
   u'\U0001f3c3\U0001f3fc\U0000200d\U00002642\U0000fe0f',  # 🏃🏼‍♂️
   u'\U0001f3c3\U0001f3fc\U0000200d\U00002642',  # 🏃🏼‍♂
   u'\U0001f3c3\U0001f3fd\U0000200d\U00002642\U0000fe0f',  # 🏃🏽‍♂️
@@ -2539,14 +2623,38 @@
   u'\U0001f9db\U0001f3fc\U0000200d\U00002642',  # 🧛🏼‍♂
   u'\U0001f9db\U0001f3fd\U0000200d\U00002642\U0000fe0f',  # 🧛🏽‍♂️
   u'\U0001f9db\U0001f3fd\U0000200d\U00002642',  # 🧛🏽‍♂
   u'\U0001f6b6\U0000200d\U00002642\U0000fe0f',  # 🚶‍♂️
   u'\U0001f6b6\U0000200d\U00002642',  # 🚶‍♂
   u'\U0001f6b6\U0001f3ff\U0000200d\U00002642\U0000fe0f',  # 🚶🏿‍♂️
   u'\U0001f6b6\U0001f3ff\U0000200d\U00002642',  # 🚶🏿‍♂
+  u'\U0001f6b6\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶‍♂️‍➡️
+  u'\U0001f6b6\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🚶‍♂‍➡️
+  u'\U0001f6b6\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🚶‍♂️‍➡
+  u'\U0001f6b6\U0000200d\U00002642\U0000200d\U000027a1',  # 🚶‍♂‍➡
+  u'\U0001f6b6\U0001f3ff\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶🏿‍♂️‍➡️
+  u'\U0001f6b6\U0001f3ff\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🚶🏿‍♂‍➡️
+  u'\U0001f6b6\U0001f3ff\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🚶🏿‍♂️‍➡
+  u'\U0001f6b6\U0001f3ff\U0000200d\U00002642\U0000200d\U000027a1',  # 🚶🏿‍♂‍➡
+  u'\U0001f6b6\U0001f3fb\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶🏻‍♂️‍➡️
+  u'\U0001f6b6\U0001f3fb\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🚶🏻‍♂‍➡️
+  u'\U0001f6b6\U0001f3fb\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🚶🏻‍♂️‍➡
+  u'\U0001f6b6\U0001f3fb\U0000200d\U00002642\U0000200d\U000027a1',  # 🚶🏻‍♂‍➡
+  u'\U0001f6b6\U0001f3fe\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶🏾‍♂️‍➡️
+  u'\U0001f6b6\U0001f3fe\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🚶🏾‍♂‍➡️
+  u'\U0001f6b6\U0001f3fe\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🚶🏾‍♂️‍➡
+  u'\U0001f6b6\U0001f3fe\U0000200d\U00002642\U0000200d\U000027a1',  # 🚶🏾‍♂‍➡
+  u'\U0001f6b6\U0001f3fc\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶🏼‍♂️‍➡️
+  u'\U0001f6b6\U0001f3fc\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🚶🏼‍♂‍➡️
+  u'\U0001f6b6\U0001f3fc\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🚶🏼‍♂️‍➡
+  u'\U0001f6b6\U0001f3fc\U0000200d\U00002642\U0000200d\U000027a1',  # 🚶🏼‍♂‍➡
+  u'\U0001f6b6\U0001f3fd\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶🏽‍♂️‍➡️
+  u'\U0001f6b6\U0001f3fd\U0000200d\U00002642\U0000200d\U000027a1\U0000fe0f',  # 🚶🏽‍♂‍➡️
+  u'\U0001f6b6\U0001f3fd\U0000200d\U00002642\U0000fe0f\U0000200d\U000027a1',  # 🚶🏽‍♂️‍➡
+  u'\U0001f6b6\U0001f3fd\U0000200d\U00002642\U0000200d\U000027a1',  # 🚶🏽‍♂‍➡
   u'\U0001f6b6\U0001f3fb\U0000200d\U00002642\U0000fe0f',  # 🚶🏻‍♂️
   u'\U0001f6b6\U0001f3fb\U0000200d\U00002642',  # 🚶🏻‍♂
   u'\U0001f6b6\U0001f3fe\U0000200d\U00002642\U0000fe0f',  # 🚶🏾‍♂️
   u'\U0001f6b6\U0001f3fe\U0000200d\U00002642',  # 🚶🏾‍♂
   u'\U0001f6b6\U0001f3fc\U0000200d\U00002642\U0000fe0f',  # 🚶🏼‍♂️
   u'\U0001f6b6\U0001f3fc\U0000200d\U00002642',  # 🚶🏼‍♂
   u'\U0001f6b6\U0001f3fd\U0000200d\U00002642\U0000fe0f',  # 🚶🏽‍♂️
@@ -2574,14 +2682,26 @@
   u'\U0001f470\U0001f3fe\U0000200d\U00002642',  # 👰🏾‍♂
   u'\U0001f470\U0001f3fc\U0000200d\U00002642\U0000fe0f',  # 👰🏼‍♂️
   u'\U0001f470\U0001f3fc\U0000200d\U00002642',  # 👰🏼‍♂
   u'\U0001f470\U0001f3fd\U0000200d\U00002642\U0000fe0f',  # 👰🏽‍♂️
   u'\U0001f470\U0001f3fd\U0000200d\U00002642',  # 👰🏽‍♂
   u'\U0001f468\U0000200d\U0001f9af',  # 👨‍🦯
   u'\U0001f468\U0001f3ff\U0000200d\U0001f9af',  # 👨🏿‍🦯
+  u'\U0001f468\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👨‍🦯‍➡️
+  u'\U0001f468\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👨‍🦯‍➡
+  u'\U0001f468\U0001f3ff\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👨🏿‍🦯‍➡️
+  u'\U0001f468\U0001f3ff\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👨🏿‍🦯‍➡
+  u'\U0001f468\U0001f3fb\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👨🏻‍🦯‍➡️
+  u'\U0001f468\U0001f3fb\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👨🏻‍🦯‍➡
+  u'\U0001f468\U0001f3fe\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👨🏾‍🦯‍➡️
+  u'\U0001f468\U0001f3fe\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👨🏾‍🦯‍➡
+  u'\U0001f468\U0001f3fc\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👨🏼‍🦯‍➡️
+  u'\U0001f468\U0001f3fc\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👨🏼‍🦯‍➡
+  u'\U0001f468\U0001f3fd\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👨🏽‍🦯‍➡️
+  u'\U0001f468\U0001f3fd\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👨🏽‍🦯‍➡
   u'\U0001f468\U0001f3fb\U0000200d\U0001f9af',  # 👨🏻‍🦯
   u'\U0001f468\U0001f3fe\U0000200d\U0001f9af',  # 👨🏾‍🦯
   u'\U0001f468\U0001f3fc\U0000200d\U0001f9af',  # 👨🏼‍🦯
   u'\U0001f468\U0001f3fd\U0000200d\U0001f9af',  # 👨🏽‍🦯
   u'\U0001f9df\U0000200d\U00002642\U0000fe0f',  # 🧟‍♂️
   u'\U0001f9df\U0000200d\U00002642',  # 🧟‍♂
   u'\U0001f96d',  # 🥭
@@ -3047,20 +3167,44 @@
   u'\U0001f9d8\U0001f3ff',  # 🧘🏿
   u'\U0001f9d8\U0001f3fb',  # 🧘🏻
   u'\U0001f9d8\U0001f3fe',  # 🧘🏾
   u'\U0001f9d8\U0001f3fc',  # 🧘🏼
   u'\U0001f9d8\U0001f3fd',  # 🧘🏽
   u'\U0001f9d1\U0000200d\U0001f9bd',  # 🧑‍🦽
   u'\U0001f9d1\U0001f3ff\U0000200d\U0001f9bd',  # 🧑🏿‍🦽
+  u'\U0001f9d1\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 🧑‍🦽‍➡️
+  u'\U0001f9d1\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 🧑‍🦽‍➡
+  u'\U0001f9d1\U0001f3ff\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 🧑🏿‍🦽‍➡️
+  u'\U0001f9d1\U0001f3ff\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 🧑🏿‍🦽‍➡
+  u'\U0001f9d1\U0001f3fb\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 🧑🏻‍🦽‍➡️
+  u'\U0001f9d1\U0001f3fb\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 🧑🏻‍🦽‍➡
+  u'\U0001f9d1\U0001f3fe\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 🧑🏾‍🦽‍➡️
+  u'\U0001f9d1\U0001f3fe\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 🧑🏾‍🦽‍➡
+  u'\U0001f9d1\U0001f3fc\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 🧑🏼‍🦽‍➡️
+  u'\U0001f9d1\U0001f3fc\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 🧑🏼‍🦽‍➡
+  u'\U0001f9d1\U0001f3fd\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 🧑🏽‍🦽‍➡️
+  u'\U0001f9d1\U0001f3fd\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 🧑🏽‍🦽‍➡
   u'\U0001f9d1\U0001f3fb\U0000200d\U0001f9bd',  # 🧑🏻‍🦽
   u'\U0001f9d1\U0001f3fe\U0000200d\U0001f9bd',  # 🧑🏾‍🦽
   u'\U0001f9d1\U0001f3fc\U0000200d\U0001f9bd',  # 🧑🏼‍🦽
   u'\U0001f9d1\U0001f3fd\U0000200d\U0001f9bd',  # 🧑🏽‍🦽
   u'\U0001f9d1\U0000200d\U0001f9bc',  # 🧑‍🦼
   u'\U0001f9d1\U0001f3ff\U0000200d\U0001f9bc',  # 🧑🏿‍🦼
+  u'\U0001f9d1\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 🧑‍🦼‍➡️
+  u'\U0001f9d1\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 🧑‍🦼‍➡
+  u'\U0001f9d1\U0001f3ff\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 🧑🏿‍🦼‍➡️
+  u'\U0001f9d1\U0001f3ff\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 🧑🏿‍🦼‍➡
+  u'\U0001f9d1\U0001f3fb\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 🧑🏻‍🦼‍➡️
+  u'\U0001f9d1\U0001f3fb\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 🧑🏻‍🦼‍➡
+  u'\U0001f9d1\U0001f3fe\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 🧑🏾‍🦼‍➡️
+  u'\U0001f9d1\U0001f3fe\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 🧑🏾‍🦼‍➡
+  u'\U0001f9d1\U0001f3fc\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 🧑🏼‍🦼‍➡️
+  u'\U0001f9d1\U0001f3fc\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 🧑🏼‍🦼‍➡
+  u'\U0001f9d1\U0001f3fd\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 🧑🏽‍🦼‍➡️
+  u'\U0001f9d1\U0001f3fd\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 🧑🏽‍🦼‍➡
   u'\U0001f9d1\U0001f3fb\U0000200d\U0001f9bc',  # 🧑🏻‍🦼
   u'\U0001f9d1\U0001f3fe\U0000200d\U0001f9bc',  # 🧑🏾‍🦼
   u'\U0001f9d1\U0001f3fc\U0000200d\U0001f9bc',  # 🧑🏼‍🦼
   u'\U0001f9d1\U0001f3fd\U0000200d\U0001f9bc',  # 🧑🏽‍🦼
   u'\U0001f9d6',  # 🧖
   u'\U0001f9d6\U0001f3ff',  # 🧖🏿
   u'\U0001f9d6\U0001f3fb',  # 🧖🏻
@@ -3084,14 +3228,26 @@
   u'\U0001f939\U0001f3ff',  # 🤹🏿
   u'\U0001f939\U0001f3fb',  # 🤹🏻
   u'\U0001f939\U0001f3fe',  # 🤹🏾
   u'\U0001f939\U0001f3fc',  # 🤹🏼
   u'\U0001f939\U0001f3fd',  # 🤹🏽
   u'\U0001f9ce',  # 🧎
   u'\U0001f9ce\U0001f3ff',  # 🧎🏿
+  u'\U0001f9ce\U0000200d\U000027a1\U0000fe0f',  # 🧎‍➡️
+  u'\U0001f9ce\U0000200d\U000027a1',  # 🧎‍➡
+  u'\U0001f9ce\U0001f3ff\U0000200d\U000027a1\U0000fe0f',  # 🧎🏿‍➡️
+  u'\U0001f9ce\U0001f3ff\U0000200d\U000027a1',  # 🧎🏿‍➡
+  u'\U0001f9ce\U0001f3fb\U0000200d\U000027a1\U0000fe0f',  # 🧎🏻‍➡️
+  u'\U0001f9ce\U0001f3fb\U0000200d\U000027a1',  # 🧎🏻‍➡
+  u'\U0001f9ce\U0001f3fe\U0000200d\U000027a1\U0000fe0f',  # 🧎🏾‍➡️
+  u'\U0001f9ce\U0001f3fe\U0000200d\U000027a1',  # 🧎🏾‍➡
+  u'\U0001f9ce\U0001f3fc\U0000200d\U000027a1\U0000fe0f',  # 🧎🏼‍➡️
+  u'\U0001f9ce\U0001f3fc\U0000200d\U000027a1',  # 🧎🏼‍➡
+  u'\U0001f9ce\U0001f3fd\U0000200d\U000027a1\U0000fe0f',  # 🧎🏽‍➡️
+  u'\U0001f9ce\U0001f3fd\U0000200d\U000027a1',  # 🧎🏽‍➡
   u'\U0001f9ce\U0001f3fb',  # 🧎🏻
   u'\U0001f9ce\U0001f3fe',  # 🧎🏾
   u'\U0001f9ce\U0001f3fc',  # 🧎🏼
   u'\U0001f9ce\U0001f3fd',  # 🧎🏽
   u'\U0001f3cb\U0000fe0f',  # 🏋️
   u'\U0001f3cb',  # 🏋
   u'\U0001f3cb\U0001f3ff',  # 🏋🏿
@@ -3162,14 +3318,26 @@
   u'\U0001f6a3\U0001f3ff',  # 🚣🏿
   u'\U0001f6a3\U0001f3fb',  # 🚣🏻
   u'\U0001f6a3\U0001f3fe',  # 🚣🏾
   u'\U0001f6a3\U0001f3fc',  # 🚣🏼
   u'\U0001f6a3\U0001f3fd',  # 🚣🏽
   u'\U0001f3c3',  # 🏃
   u'\U0001f3c3\U0001f3ff',  # 🏃🏿
+  u'\U0001f3c3\U0000200d\U000027a1\U0000fe0f',  # 🏃‍➡️
+  u'\U0001f3c3\U0000200d\U000027a1',  # 🏃‍➡
+  u'\U0001f3c3\U0001f3ff\U0000200d\U000027a1\U0000fe0f',  # 🏃🏿‍➡️
+  u'\U0001f3c3\U0001f3ff\U0000200d\U000027a1',  # 🏃🏿‍➡
+  u'\U0001f3c3\U0001f3fb\U0000200d\U000027a1\U0000fe0f',  # 🏃🏻‍➡️
+  u'\U0001f3c3\U0001f3fb\U0000200d\U000027a1',  # 🏃🏻‍➡
+  u'\U0001f3c3\U0001f3fe\U0000200d\U000027a1\U0000fe0f',  # 🏃🏾‍➡️
+  u'\U0001f3c3\U0001f3fe\U0000200d\U000027a1',  # 🏃🏾‍➡
+  u'\U0001f3c3\U0001f3fc\U0000200d\U000027a1\U0000fe0f',  # 🏃🏼‍➡️
+  u'\U0001f3c3\U0001f3fc\U0000200d\U000027a1',  # 🏃🏼‍➡
+  u'\U0001f3c3\U0001f3fd\U0000200d\U000027a1\U0000fe0f',  # 🏃🏽‍➡️
+  u'\U0001f3c3\U0001f3fd\U0000200d\U000027a1',  # 🏃🏽‍➡
   u'\U0001f3c3\U0001f3fb',  # 🏃🏻
   u'\U0001f3c3\U0001f3fe',  # 🏃🏾
   u'\U0001f3c3\U0001f3fc',  # 🏃🏼
   u'\U0001f3c3\U0001f3fd',  # 🏃🏽
   u'\U0001f937',  # 🤷
   u'\U0001f937\U0001f3ff',  # 🤷🏿
   u'\U0001f937\U0001f3fb',  # 🤷🏻
@@ -3204,14 +3372,26 @@
   u'\U0001f481\U0001f3ff',  # 💁🏿
   u'\U0001f481\U0001f3fb',  # 💁🏻
   u'\U0001f481\U0001f3fe',  # 💁🏾
   u'\U0001f481\U0001f3fc',  # 💁🏼
   u'\U0001f481\U0001f3fd',  # 💁🏽
   u'\U0001f6b6',  # 🚶
   u'\U0001f6b6\U0001f3ff',  # 🚶🏿
+  u'\U0001f6b6\U0000200d\U000027a1\U0000fe0f',  # 🚶‍➡️
+  u'\U0001f6b6\U0000200d\U000027a1',  # 🚶‍➡
+  u'\U0001f6b6\U0001f3ff\U0000200d\U000027a1\U0000fe0f',  # 🚶🏿‍➡️
+  u'\U0001f6b6\U0001f3ff\U0000200d\U000027a1',  # 🚶🏿‍➡
+  u'\U0001f6b6\U0001f3fb\U0000200d\U000027a1\U0000fe0f',  # 🚶🏻‍➡️
+  u'\U0001f6b6\U0001f3fb\U0000200d\U000027a1',  # 🚶🏻‍➡
+  u'\U0001f6b6\U0001f3fe\U0000200d\U000027a1\U0000fe0f',  # 🚶🏾‍➡️
+  u'\U0001f6b6\U0001f3fe\U0000200d\U000027a1',  # 🚶🏾‍➡
+  u'\U0001f6b6\U0001f3fc\U0000200d\U000027a1\U0000fe0f',  # 🚶🏼‍➡️
+  u'\U0001f6b6\U0001f3fc\U0000200d\U000027a1',  # 🚶🏼‍➡
+  u'\U0001f6b6\U0001f3fd\U0000200d\U000027a1\U0000fe0f',  # 🚶🏽‍➡️
+  u'\U0001f6b6\U0001f3fd\U0000200d\U000027a1',  # 🚶🏽‍➡
   u'\U0001f6b6\U0001f3fb',  # 🚶🏻
   u'\U0001f6b6\U0001f3fe',  # 🚶🏾
   u'\U0001f6b6\U0001f3fc',  # 🚶🏼
   u'\U0001f6b6\U0001f3fd',  # 🚶🏽
   u'\U0001f473',  # 👳
   u'\U0001f473\U0001f3ff',  # 👳🏿
   u'\U0001f473\U0001f3fb',  # 👳🏻
@@ -3235,19 +3415,32 @@
   u'\U0001f470\U0001f3ff',  # 👰🏿
   u'\U0001f470\U0001f3fb',  # 👰🏻
   u'\U0001f470\U0001f3fe',  # 👰🏾
   u'\U0001f470\U0001f3fc',  # 👰🏼
   u'\U0001f470\U0001f3fd',  # 👰🏽
   u'\U0001f9d1\U0000200d\U0001f9af',  # 🧑‍🦯
   u'\U0001f9d1\U0001f3ff\U0000200d\U0001f9af',  # 🧑🏿‍🦯
+  u'\U0001f9d1\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 🧑‍🦯‍➡️
+  u'\U0001f9d1\U0000200d\U0001f9af\U0000200d\U000027a1',  # 🧑‍🦯‍➡
+  u'\U0001f9d1\U0001f3ff\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 🧑🏿‍🦯‍➡️
+  u'\U0001f9d1\U0001f3ff\U0000200d\U0001f9af\U0000200d\U000027a1',  # 🧑🏿‍🦯‍➡
+  u'\U0001f9d1\U0001f3fb\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 🧑🏻‍🦯‍➡️
+  u'\U0001f9d1\U0001f3fb\U0000200d\U0001f9af\U0000200d\U000027a1',  # 🧑🏻‍🦯‍➡
+  u'\U0001f9d1\U0001f3fe\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 🧑🏾‍🦯‍➡️
+  u'\U0001f9d1\U0001f3fe\U0000200d\U0001f9af\U0000200d\U000027a1',  # 🧑🏾‍🦯‍➡
+  u'\U0001f9d1\U0001f3fc\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 🧑🏼‍🦯‍➡️
+  u'\U0001f9d1\U0001f3fc\U0000200d\U0001f9af\U0000200d\U000027a1',  # 🧑🏼‍🦯‍➡
+  u'\U0001f9d1\U0001f3fd\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 🧑🏽‍🦯‍➡️
+  u'\U0001f9d1\U0001f3fd\U0000200d\U0001f9af\U0000200d\U000027a1',  # 🧑🏽‍🦯‍➡
   u'\U0001f9d1\U0001f3fb\U0000200d\U0001f9af',  # 🧑🏻‍🦯
   u'\U0001f9d1\U0001f3fe\U0000200d\U0001f9af',  # 🧑🏾‍🦯
   u'\U0001f9d1\U0001f3fc\U0000200d\U0001f9af',  # 🧑🏼‍🦯
   u'\U0001f9d1\U0001f3fd\U0000200d\U0001f9af',  # 🧑🏽‍🦯
   u'\U0001f9eb',  # 🧫
+  u'\U0001f426\U0000200d\U0001f525',  # 🐦‍🔥
   u'\U000026cf\U0000fe0f',  # ⛏️
   u'\U000026cf',  # ⛏
   u'\U0001f6fb',  # 🛻
   u'\U0001f967',  # 🥧
   u'\U0001f416',  # 🐖
   u'\U0001f437',  # 🐷
   u'\U0001f43d',  # 🐽
@@ -4235,20 +4428,44 @@
   u'\U0001f9d8\U0001f3fe\U0000200d\U00002640',  # 🧘🏾‍♀
   u'\U0001f9d8\U0001f3fc\U0000200d\U00002640\U0000fe0f',  # 🧘🏼‍♀️
   u'\U0001f9d8\U0001f3fc\U0000200d\U00002640',  # 🧘🏼‍♀
   u'\U0001f9d8\U0001f3fd\U0000200d\U00002640\U0000fe0f',  # 🧘🏽‍♀️
   u'\U0001f9d8\U0001f3fd\U0000200d\U00002640',  # 🧘🏽‍♀
   u'\U0001f469\U0000200d\U0001f9bd',  # 👩‍🦽
   u'\U0001f469\U0001f3ff\U0000200d\U0001f9bd',  # 👩🏿‍🦽
+  u'\U0001f469\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👩‍🦽‍➡️
+  u'\U0001f469\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👩‍🦽‍➡
+  u'\U0001f469\U0001f3ff\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👩🏿‍🦽‍➡️
+  u'\U0001f469\U0001f3ff\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👩🏿‍🦽‍➡
+  u'\U0001f469\U0001f3fb\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👩🏻‍🦽‍➡️
+  u'\U0001f469\U0001f3fb\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👩🏻‍🦽‍➡
+  u'\U0001f469\U0001f3fe\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👩🏾‍🦽‍➡️
+  u'\U0001f469\U0001f3fe\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👩🏾‍🦽‍➡
+  u'\U0001f469\U0001f3fc\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👩🏼‍🦽‍➡️
+  u'\U0001f469\U0001f3fc\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👩🏼‍🦽‍➡
+  u'\U0001f469\U0001f3fd\U0000200d\U0001f9bd\U0000200d\U000027a1\U0000fe0f',  # 👩🏽‍🦽‍➡️
+  u'\U0001f469\U0001f3fd\U0000200d\U0001f9bd\U0000200d\U000027a1',  # 👩🏽‍🦽‍➡
   u'\U0001f469\U0001f3fb\U0000200d\U0001f9bd',  # 👩🏻‍🦽
   u'\U0001f469\U0001f3fe\U0000200d\U0001f9bd',  # 👩🏾‍🦽
   u'\U0001f469\U0001f3fc\U0000200d\U0001f9bd',  # 👩🏼‍🦽
   u'\U0001f469\U0001f3fd\U0000200d\U0001f9bd',  # 👩🏽‍🦽
   u'\U0001f469\U0000200d\U0001f9bc',  # 👩‍🦼
   u'\U0001f469\U0001f3ff\U0000200d\U0001f9bc',  # 👩🏿‍🦼
+  u'\U0001f469\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👩‍🦼‍➡️
+  u'\U0001f469\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👩‍🦼‍➡
+  u'\U0001f469\U0001f3ff\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👩🏿‍🦼‍➡️
+  u'\U0001f469\U0001f3ff\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👩🏿‍🦼‍➡
+  u'\U0001f469\U0001f3fb\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👩🏻‍🦼‍➡️
+  u'\U0001f469\U0001f3fb\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👩🏻‍🦼‍➡
+  u'\U0001f469\U0001f3fe\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👩🏾‍🦼‍➡️
+  u'\U0001f469\U0001f3fe\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👩🏾‍🦼‍➡
+  u'\U0001f469\U0001f3fc\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👩🏼‍🦼‍➡️
+  u'\U0001f469\U0001f3fc\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👩🏼‍🦼‍➡
+  u'\U0001f469\U0001f3fd\U0000200d\U0001f9bc\U0000200d\U000027a1\U0000fe0f',  # 👩🏽‍🦼‍➡️
+  u'\U0001f469\U0001f3fd\U0000200d\U0001f9bc\U0000200d\U000027a1',  # 👩🏽‍🦼‍➡
   u'\U0001f469\U0001f3fb\U0000200d\U0001f9bc',  # 👩🏻‍🦼
   u'\U0001f469\U0001f3fe\U0000200d\U0001f9bc',  # 👩🏾‍🦼
   u'\U0001f469\U0001f3fc\U0000200d\U0001f9bc',  # 👩🏼‍🦼
   u'\U0001f469\U0001f3fd\U0000200d\U0001f9bc',  # 👩🏽‍🦼
   u'\U0001f9d6\U0000200d\U00002640\U0000fe0f',  # 🧖‍♀️
   u'\U0001f9d6\U0000200d\U00002640',  # 🧖‍♀
   u'\U0001f9d6\U0001f3ff\U0000200d\U00002640\U0000fe0f',  # 🧖🏿‍♀️
@@ -4297,14 +4514,38 @@
   u'\U0001f939\U0001f3fc\U0000200d\U00002640',  # 🤹🏼‍♀
   u'\U0001f939\U0001f3fd\U0000200d\U00002640\U0000fe0f',  # 🤹🏽‍♀️
   u'\U0001f939\U0001f3fd\U0000200d\U00002640',  # 🤹🏽‍♀
   u'\U0001f9ce\U0000200d\U00002640\U0000fe0f',  # 🧎‍♀️
   u'\U0001f9ce\U0000200d\U00002640',  # 🧎‍♀
   u'\U0001f9ce\U0001f3ff\U0000200d\U00002640\U0000fe0f',  # 🧎🏿‍♀️
   u'\U0001f9ce\U0001f3ff\U0000200d\U00002640',  # 🧎🏿‍♀
+  u'\U0001f9ce\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎‍♀️‍➡️
+  u'\U0001f9ce\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🧎‍♀‍➡️
+  u'\U0001f9ce\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🧎‍♀️‍➡
+  u'\U0001f9ce\U0000200d\U00002640\U0000200d\U000027a1',  # 🧎‍♀‍➡
+  u'\U0001f9ce\U0001f3ff\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎🏿‍♀️‍➡️
+  u'\U0001f9ce\U0001f3ff\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🧎🏿‍♀‍➡️
+  u'\U0001f9ce\U0001f3ff\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🧎🏿‍♀️‍➡
+  u'\U0001f9ce\U0001f3ff\U0000200d\U00002640\U0000200d\U000027a1',  # 🧎🏿‍♀‍➡
+  u'\U0001f9ce\U0001f3fb\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎🏻‍♀️‍➡️
+  u'\U0001f9ce\U0001f3fb\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🧎🏻‍♀‍➡️
+  u'\U0001f9ce\U0001f3fb\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🧎🏻‍♀️‍➡
+  u'\U0001f9ce\U0001f3fb\U0000200d\U00002640\U0000200d\U000027a1',  # 🧎🏻‍♀‍➡
+  u'\U0001f9ce\U0001f3fe\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎🏾‍♀️‍➡️
+  u'\U0001f9ce\U0001f3fe\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🧎🏾‍♀‍➡️
+  u'\U0001f9ce\U0001f3fe\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🧎🏾‍♀️‍➡
+  u'\U0001f9ce\U0001f3fe\U0000200d\U00002640\U0000200d\U000027a1',  # 🧎🏾‍♀‍➡
+  u'\U0001f9ce\U0001f3fc\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎🏼‍♀️‍➡️
+  u'\U0001f9ce\U0001f3fc\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🧎🏼‍♀‍➡️
+  u'\U0001f9ce\U0001f3fc\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🧎🏼‍♀️‍➡
+  u'\U0001f9ce\U0001f3fc\U0000200d\U00002640\U0000200d\U000027a1',  # 🧎🏼‍♀‍➡
+  u'\U0001f9ce\U0001f3fd\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🧎🏽‍♀️‍➡️
+  u'\U0001f9ce\U0001f3fd\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🧎🏽‍♀‍➡️
+  u'\U0001f9ce\U0001f3fd\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🧎🏽‍♀️‍➡
+  u'\U0001f9ce\U0001f3fd\U0000200d\U00002640\U0000200d\U000027a1',  # 🧎🏽‍♀‍➡
   u'\U0001f9ce\U0001f3fb\U0000200d\U00002640\U0000fe0f',  # 🧎🏻‍♀️
   u'\U0001f9ce\U0001f3fb\U0000200d\U00002640',  # 🧎🏻‍♀
   u'\U0001f9ce\U0001f3fe\U0000200d\U00002640\U0000fe0f',  # 🧎🏾‍♀️
   u'\U0001f9ce\U0001f3fe\U0000200d\U00002640',  # 🧎🏾‍♀
   u'\U0001f9ce\U0001f3fc\U0000200d\U00002640\U0000fe0f',  # 🧎🏼‍♀️
   u'\U0001f9ce\U0001f3fc\U0000200d\U00002640',  # 🧎🏼‍♀
   u'\U0001f9ce\U0001f3fd\U0000200d\U00002640\U0000fe0f',  # 🧎🏽‍♀️
@@ -4480,14 +4721,38 @@
   u'\U0001f6a3\U0001f3fc\U0000200d\U00002640',  # 🚣🏼‍♀
   u'\U0001f6a3\U0001f3fd\U0000200d\U00002640\U0000fe0f',  # 🚣🏽‍♀️
   u'\U0001f6a3\U0001f3fd\U0000200d\U00002640',  # 🚣🏽‍♀
   u'\U0001f3c3\U0000200d\U00002640\U0000fe0f',  # 🏃‍♀️
   u'\U0001f3c3\U0000200d\U00002640',  # 🏃‍♀
   u'\U0001f3c3\U0001f3ff\U0000200d\U00002640\U0000fe0f',  # 🏃🏿‍♀️
   u'\U0001f3c3\U0001f3ff\U0000200d\U00002640',  # 🏃🏿‍♀
+  u'\U0001f3c3\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃‍♀️‍➡️
+  u'\U0001f3c3\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🏃‍♀‍➡️
+  u'\U0001f3c3\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🏃‍♀️‍➡
+  u'\U0001f3c3\U0000200d\U00002640\U0000200d\U000027a1',  # 🏃‍♀‍➡
+  u'\U0001f3c3\U0001f3ff\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃🏿‍♀️‍➡️
+  u'\U0001f3c3\U0001f3ff\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🏃🏿‍♀‍➡️
+  u'\U0001f3c3\U0001f3ff\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🏃🏿‍♀️‍➡
+  u'\U0001f3c3\U0001f3ff\U0000200d\U00002640\U0000200d\U000027a1',  # 🏃🏿‍♀‍➡
+  u'\U0001f3c3\U0001f3fb\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃🏻‍♀️‍➡️
+  u'\U0001f3c3\U0001f3fb\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🏃🏻‍♀‍➡️
+  u'\U0001f3c3\U0001f3fb\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🏃🏻‍♀️‍➡
+  u'\U0001f3c3\U0001f3fb\U0000200d\U00002640\U0000200d\U000027a1',  # 🏃🏻‍♀‍➡
+  u'\U0001f3c3\U0001f3fe\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃🏾‍♀️‍➡️
+  u'\U0001f3c3\U0001f3fe\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🏃🏾‍♀‍➡️
+  u'\U0001f3c3\U0001f3fe\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🏃🏾‍♀️‍➡
+  u'\U0001f3c3\U0001f3fe\U0000200d\U00002640\U0000200d\U000027a1',  # 🏃🏾‍♀‍➡
+  u'\U0001f3c3\U0001f3fc\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃🏼‍♀️‍➡️
+  u'\U0001f3c3\U0001f3fc\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🏃🏼‍♀‍➡️
+  u'\U0001f3c3\U0001f3fc\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🏃🏼‍♀️‍➡
+  u'\U0001f3c3\U0001f3fc\U0000200d\U00002640\U0000200d\U000027a1',  # 🏃🏼‍♀‍➡
+  u'\U0001f3c3\U0001f3fd\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🏃🏽‍♀️‍➡️
+  u'\U0001f3c3\U0001f3fd\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🏃🏽‍♀‍➡️
+  u'\U0001f3c3\U0001f3fd\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🏃🏽‍♀️‍➡
+  u'\U0001f3c3\U0001f3fd\U0000200d\U00002640\U0000200d\U000027a1',  # 🏃🏽‍♀‍➡
   u'\U0001f3c3\U0001f3fb\U0000200d\U00002640\U0000fe0f',  # 🏃🏻‍♀️
   u'\U0001f3c3\U0001f3fb\U0000200d\U00002640',  # 🏃🏻‍♀
   u'\U0001f3c3\U0001f3fe\U0000200d\U00002640\U0000fe0f',  # 🏃🏾‍♀️
   u'\U0001f3c3\U0001f3fe\U0000200d\U00002640',  # 🏃🏾‍♀
   u'\U0001f3c3\U0001f3fc\U0000200d\U00002640\U0000fe0f',  # 🏃🏼‍♀️
   u'\U0001f3c3\U0001f3fc\U0000200d\U00002640',  # 🏃🏼‍♀
   u'\U0001f3c3\U0001f3fd\U0000200d\U00002640\U0000fe0f',  # 🏃🏽‍♀️
@@ -4618,14 +4883,38 @@
   u'\U0001f9db\U0001f3fc\U0000200d\U00002640',  # 🧛🏼‍♀
   u'\U0001f9db\U0001f3fd\U0000200d\U00002640\U0000fe0f',  # 🧛🏽‍♀️
   u'\U0001f9db\U0001f3fd\U0000200d\U00002640',  # 🧛🏽‍♀
   u'\U0001f6b6\U0000200d\U00002640\U0000fe0f',  # 🚶‍♀️
   u'\U0001f6b6\U0000200d\U00002640',  # 🚶‍♀
   u'\U0001f6b6\U0001f3ff\U0000200d\U00002640\U0000fe0f',  # 🚶🏿‍♀️
   u'\U0001f6b6\U0001f3ff\U0000200d\U00002640',  # 🚶🏿‍♀
+  u'\U0001f6b6\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶‍♀️‍➡️
+  u'\U0001f6b6\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🚶‍♀‍➡️
+  u'\U0001f6b6\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🚶‍♀️‍➡
+  u'\U0001f6b6\U0000200d\U00002640\U0000200d\U000027a1',  # 🚶‍♀‍➡
+  u'\U0001f6b6\U0001f3ff\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶🏿‍♀️‍➡️
+  u'\U0001f6b6\U0001f3ff\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🚶🏿‍♀‍➡️
+  u'\U0001f6b6\U0001f3ff\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🚶🏿‍♀️‍➡
+  u'\U0001f6b6\U0001f3ff\U0000200d\U00002640\U0000200d\U000027a1',  # 🚶🏿‍♀‍➡
+  u'\U0001f6b6\U0001f3fb\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶🏻‍♀️‍➡️
+  u'\U0001f6b6\U0001f3fb\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🚶🏻‍♀‍➡️
+  u'\U0001f6b6\U0001f3fb\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🚶🏻‍♀️‍➡
+  u'\U0001f6b6\U0001f3fb\U0000200d\U00002640\U0000200d\U000027a1',  # 🚶🏻‍♀‍➡
+  u'\U0001f6b6\U0001f3fe\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶🏾‍♀️‍➡️
+  u'\U0001f6b6\U0001f3fe\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🚶🏾‍♀‍➡️
+  u'\U0001f6b6\U0001f3fe\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🚶🏾‍♀️‍➡
+  u'\U0001f6b6\U0001f3fe\U0000200d\U00002640\U0000200d\U000027a1',  # 🚶🏾‍♀‍➡
+  u'\U0001f6b6\U0001f3fc\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶🏼‍♀️‍➡️
+  u'\U0001f6b6\U0001f3fc\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🚶🏼‍♀‍➡️
+  u'\U0001f6b6\U0001f3fc\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🚶🏼‍♀️‍➡
+  u'\U0001f6b6\U0001f3fc\U0000200d\U00002640\U0000200d\U000027a1',  # 🚶🏼‍♀‍➡
+  u'\U0001f6b6\U0001f3fd\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1\U0000fe0f',  # 🚶🏽‍♀️‍➡️
+  u'\U0001f6b6\U0001f3fd\U0000200d\U00002640\U0000200d\U000027a1\U0000fe0f',  # 🚶🏽‍♀‍➡️
+  u'\U0001f6b6\U0001f3fd\U0000200d\U00002640\U0000fe0f\U0000200d\U000027a1',  # 🚶🏽‍♀️‍➡
+  u'\U0001f6b6\U0001f3fd\U0000200d\U00002640\U0000200d\U000027a1',  # 🚶🏽‍♀‍➡
   u'\U0001f6b6\U0001f3fb\U0000200d\U00002640\U0000fe0f',  # 🚶🏻‍♀️
   u'\U0001f6b6\U0001f3fb\U0000200d\U00002640',  # 🚶🏻‍♀
   u'\U0001f6b6\U0001f3fe\U0000200d\U00002640\U0000fe0f',  # 🚶🏾‍♀️
   u'\U0001f6b6\U0001f3fe\U0000200d\U00002640',  # 🚶🏾‍♀
   u'\U0001f6b6\U0001f3fc\U0000200d\U00002640\U0000fe0f',  # 🚶🏼‍♀️
   u'\U0001f6b6\U0001f3fc\U0000200d\U00002640',  # 🚶🏼‍♀
   u'\U0001f6b6\U0001f3fd\U0000200d\U00002640\U0000fe0f',  # 🚶🏽‍♀️
@@ -4659,14 +4948,26 @@
   u'\U0001f470\U0001f3fe\U0000200d\U00002640',  # 👰🏾‍♀
   u'\U0001f470\U0001f3fc\U0000200d\U00002640\U0000fe0f',  # 👰🏼‍♀️
   u'\U0001f470\U0001f3fc\U0000200d\U00002640',  # 👰🏼‍♀
   u'\U0001f470\U0001f3fd\U0000200d\U00002640\U0000fe0f',  # 👰🏽‍♀️
   u'\U0001f470\U0001f3fd\U0000200d\U00002640',  # 👰🏽‍♀
   u'\U0001f469\U0000200d\U0001f9af',  # 👩‍🦯
   u'\U0001f469\U0001f3ff\U0000200d\U0001f9af',  # 👩🏿‍🦯
+  u'\U0001f469\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👩‍🦯‍➡️
+  u'\U0001f469\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👩‍🦯‍➡
+  u'\U0001f469\U0001f3ff\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👩🏿‍🦯‍➡️
+  u'\U0001f469\U0001f3ff\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👩🏿‍🦯‍➡
+  u'\U0001f469\U0001f3fb\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👩🏻‍🦯‍➡️
+  u'\U0001f469\U0001f3fb\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👩🏻‍🦯‍➡
+  u'\U0001f469\U0001f3fe\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👩🏾‍🦯‍➡️
+  u'\U0001f469\U0001f3fe\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👩🏾‍🦯‍➡
+  u'\U0001f469\U0001f3fc\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👩🏼‍🦯‍➡️
+  u'\U0001f469\U0001f3fc\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👩🏼‍🦯‍➡
+  u'\U0001f469\U0001f3fd\U0000200d\U0001f9af\U0000200d\U000027a1\U0000fe0f',  # 👩🏽‍🦯‍➡️
+  u'\U0001f469\U0001f3fd\U0000200d\U0001f9af\U0000200d\U000027a1',  # 👩🏽‍🦯‍➡
   u'\U0001f469\U0001f3fb\U0000200d\U0001f9af',  # 👩🏻‍🦯
   u'\U0001f469\U0001f3fe\U0000200d\U0001f9af',  # 👩🏾‍🦯
   u'\U0001f469\U0001f3fc\U0000200d\U0001f9af',  # 👩🏼‍🦯
   u'\U0001f469\U0001f3fd\U0000200d\U0001f9af',  # 👩🏽‍🦯
   u'\U0001f9df\U0000200d\U00002640\U0000fe0f',  # 🧟‍♀️
   u'\U0001f9df\U0000200d\U00002640',  # 🧟‍♀
   u'\U0001f462',  # 👢
```

### Comparing `ical-8.0.2/ical/parsing/parser.py` & `ical-8.1.0/ical/parsing/parser.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/parsing/property.py` & `ical-8.1.0/ical/parsing/property.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/parsing/unicode.py` & `ical-8.1.0/ical/parsing/unicode.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/recur_adapter.py` & `ical-8.1.0/ical/recur_adapter.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/store.py` & `ical-8.1.0/ical/store.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/timeline.py` & `ical-8.1.0/ical/timeline.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/timespan.py` & `ical-8.1.0/ical/timespan.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/timezone.py` & `ical-8.1.0/ical/timezone.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/todo.py` & `ical-8.1.0/ical/todo.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/__init__.py` & `ical-8.1.0/ical/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/boolean.py` & `ical-8.1.0/ical/types/boolean.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/cal_address.py` & `ical-8.1.0/ical/types/cal_address.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/data_types.py` & `ical-8.1.0/ical/types/data_types.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/date.py` & `ical-8.1.0/ical/types/date.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/date_time.py` & `ical-8.1.0/ical/types/date_time.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/duration.py` & `ical-8.1.0/ical/types/duration.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/geo.py` & `ical-8.1.0/ical/types/geo.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/integer.py` & `ical-8.1.0/ical/types/integer.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/parsing.py` & `ical-8.1.0/ical/types/parsing.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/period.py` & `ical-8.1.0/ical/types/period.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/priority.py` & `ical-8.1.0/ical/types/priority.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/recur.py` & `ical-8.1.0/ical/types/recur.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/relation.py` & `ical-8.1.0/ical/types/relation.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/request_status.py` & `ical-8.1.0/ical/types/request_status.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/text.py` & `ical-8.1.0/ical/types/text.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/uri.py` & `ical-8.1.0/ical/types/uri.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/types/utc_offset.py` & `ical-8.1.0/ical/types/utc_offset.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/tzif/model.py` & `ical-8.1.0/ical/tzif/model.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/tzif/timezoneinfo.py` & `ical-8.1.0/ical/tzif/timezoneinfo.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/tzif/tz_rule.py` & `ical-8.1.0/ical/tzif/tz_rule.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/tzif/tzif.py` & `ical-8.1.0/ical/tzif/tzif.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical/util.py` & `ical-8.1.0/ical/util.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/ical.egg-info/PKG-INFO` & `ical-8.1.0/ical.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ical
-Version: 8.0.2
+Version: 8.1.0
 Summary: Python iCalendar implementation (rfc 2445)
 Home-page: https://github.com/allenporter/ical
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `ical-8.0.2/ical.egg-info/SOURCES.txt` & `ical-8.1.0/ical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/pyproject.toml` & `ical-8.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/setup.cfg` & `ical-8.1.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ical
-version = 8.0.2
+version = 8.1.0
 description = Python iCalendar implementation (rfc 2445)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/ical
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `ical-8.0.2/tests/test_alarm.py` & `ical-8.1.0/tests/test_alarm.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_calendar.py` & `ical-8.1.0/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_calendar_stream.py` & `ical-8.1.0/tests/test_calendar_stream.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_component.py` & `ical-8.1.0/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_diagnostics.py` & `ical-8.1.0/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_event.py` & `ical-8.1.0/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_freebusy.py` & `ical-8.1.0/tests/test_freebusy.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_iter.py` & `ical-8.1.0/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_journal.py` & `ical-8.1.0/tests/test_journal.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_list.py` & `ical-8.1.0/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_store.py` & `ical-8.1.0/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_timeline.py` & `ical-8.1.0/tests/test_timeline.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_timezone.py` & `ical-8.1.0/tests/test_timezone.py`

 * *Files identical despite different names*

### Comparing `ical-8.0.2/tests/test_todo.py` & `ical-8.1.0/tests/test_todo.py`

 * *Files identical despite different names*

