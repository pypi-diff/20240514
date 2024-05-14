# Comparing `tmp/habits_txt-0.1.2.tar.gz` & `tmp/habits_txt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habits_txt-0.1.2.tar", max compression
+gzip compressed data, was "habits_txt-0.1.3.tar", max compression
```

## Comparing `habits_txt-0.1.2.tar` & `habits_txt-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     2053 2024-05-11 15:48:56.511263 habits_txt-0.1.2/README.md
--rw-r--r--   0        0        0     9572 2024-05-11 15:56:18.089263 habits_txt-0.1.2/habits_txt/builder.py
--rw-r--r--   0        0        0     3419 2024-05-11 15:56:18.089263 habits_txt-0.1.2/habits_txt/cli.py
--rw-r--r--   0        0        0      111 2024-05-11 15:56:18.089263 habits_txt-0.1.2/habits_txt/defaults.py
--rw-r--r--   0        0        0     1563 2024-05-11 15:56:18.089263 habits_txt-0.1.2/habits_txt/directives.py
--rw-r--r--   0        0        0      194 2024-05-11 15:56:18.089263 habits_txt-0.1.2/habits_txt/exceptions.py
--rw-r--r--   0        0        0     4319 2024-05-11 15:56:18.089263 habits_txt-0.1.2/habits_txt/journal.py
--rw-r--r--   0        0        0     1537 2024-05-11 15:56:18.089263 habits_txt-0.1.2/habits_txt/models.py
--rw-r--r--   0        0        0     5939 2024-05-11 15:56:18.089263 habits_txt-0.1.2/habits_txt/parser.py
--rw-r--r--   0        0        0      595 2024-05-11 15:56:18.089263 habits_txt-0.1.2/habits_txt/utils.py
--rw-r--r--   0        0        0      243 2024-05-11 15:56:18.089263 habits_txt-0.1.2/main.py
--rw-r--r--   0        0        0      510 2024-05-11 15:56:18.089263 habits_txt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 habits_txt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2165 2024-05-14 18:39:14.295454 habits_txt-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/__init__.py
+-rw-r--r--   0        0        0    10111 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/builder.py
+-rw-r--r--   0        0        0     3419 2024-05-11 15:56:18.089263 habits_txt-0.1.3/habits_txt/cli.py
+-rw-r--r--   0        0        0      145 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/defaults.py
+-rw-r--r--   0        0        0     2030 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/directives.py
+-rw-r--r--   0        0        0      380 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/exceptions.py
+-rw-r--r--   0        0        0     3768 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/journal.py
+-rw-r--r--   0        0        0     1855 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/models.py
+-rw-r--r--   0        0        0     9233 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/parser.py
+-rw-r--r--   0        0        0      952 2024-05-14 18:39:14.295454 habits_txt-0.1.3/habits_txt/records_query.py
+-rw-r--r--   0        0        0      243 2024-05-11 15:56:18.089263 habits_txt-0.1.3/main.py
+-rw-r--r--   0        0        0      637 2024-05-14 18:39:44.895715 habits_txt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 habits_txt-0.1.3/PKG-INFO
```

### Comparing `habits_txt-0.1.2/README.md` & `habits_txt-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,68 +9,70 @@
 A habit is time-bound. It has a start date, and eventually an end date.
 It means with habits.txt, you can track habits for a specific period of time. When you want to stop tracking a habit, you can just stop tracking it.
 
 ### Frequency
 
 A habit is defined by a frequency, else it's called a task. The minimum frequency supported by habits.txt is daily (it doesn't support intra-day habits).
 
-### Boolean or Numeric
-
-A habit can be boolean or numeric. A boolean habit is either done or not done. A numeric habit is a value, like the number of pages read in a day.
+### Boolean or Measurable
 
+A habit can be boolean or measurable. A boolean habit is either done or not done. A measurable habit has a value.
 
 ## Format
 
 Habits are tracked in what I call a "journal" which is just a plain text file. A journal contains "directives".
 
 A directive is composed of a date, a directive type, a habit name, and other metadata specific to the directive type. For example, here is a sample directive:
 
 ```
-2024-01-01 track "Read 5 pages a day"
+2024-01-01 track "Read 5 pages a day" (* * *)
 ```
 
 You can comment lines in your journal by starting them with a `#` character.
 You can't add comments at the end of a line.
 
 ```
 # Start tracking a habit
-2024-01-01 track "Read 5 pages a day"
+2024-01-01 track "Read 5 pages a day" (* * *)
 ```
 
-
 ## Directives
 
 ### track
 
-To start tracking a habit, you use the `track` directive and specify the frequency of the habit.
+To start tracking a habit, you use the `track` directive and specify the frequency of the habit enclosed in parentheses.
+Optionally, you can make the habit measurable by specifying the "measurable" keyword.
 
 The frequency follows a simplified [cron](https://en.wikipedia.org/wiki/Cron) syntax, omitting the minute and the hour.
 
 Example:
+
 ```
-2024-01-01 track "Read 5 pages a day" * * *
-2024-01-01 track "Exercise" * * 1,3,5
+2024-01-01 track "Read 5 pages a day" (* * *)
+2024-01-01 track "Exercise" (* * 1,3,5) measurable
 ```
 
 ### untrack
 
 To stop tracking a habit, you use the `untrack` directive.
 
 Example:
+
 ```
 2024-02-01 untrack "Read 5 pages a day"
 ```
 
 ### record
 
 To record a habit, you use the `record` directive and specify a value.
 
 The allowed values are `yes`, `no`, or a number. You should not mix boolean and numeric values for the same habit.
 
 You can write directives but omit the directive type, it will default to `record`.
 
 Example:
+
 ```
 2024-01-01 record "Read 5 pages a day" 5
 2024-01-01 record "Workout" yes
 2024-01-01 "Weight" 70.5
 ```
```

### Comparing `habits_txt-0.1.2/habits_txt/builder.py` & `habits_txt-0.1.3/habits_txt/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 import datetime as dt
+import typing
 
 import habits_txt.directives as directives
 import habits_txt.exceptions as exceptions
 import habits_txt.models as models
 
 
 def _sort_directives(
     directives_: list[directives.Directive],
 ) -> list[directives.Directive]:
     """
     Sort the directives by date.
 
-    :param directives: List of directives.
+    :param directives_: List of directives.
     :return: Sorted list of directives.
 
     Example:
     >>> directive1 = directives.RecordDirective(dt.datetime(2024, 1, 1), "Habit 1", False)
     >>> directive2 = directives.RecordDirective(dt.datetime(2024, 1, 2), "Habit 2", True)
     >>> sorted_directives = _sort_directives([directive2, directive1])
     >>> print(sorted_directives)
     [directive1, directive2]
     """
     return sorted(directives_, key=lambda directive_: directive_.date)
 
 
-"""
-checks:
-- each untrack directive has a corresponding track directive before it
-- each record directive has a corresponding track directive before it
-- there can't be several tracked habits with the same name
-- there can't be several records of the same habit on the same day
-"""
-
-
 def _get_tracked_habits_at_date(
     directives_: list[directives.Directive], date: dt.date
 ) -> set[models.Habit]:
     """
     Get the tracked habits at a given date.
 
     :param directives_: List of directives.
@@ -52,15 +44,15 @@
     [Habit 1, Habit 2]
     """
     directives_before_date = [
         directive for directive in directives_ if directive.date <= date
     ]
     sorted_directives = _sort_directives(directives_before_date)
 
-    current_state = set()
+    current_state: set[models.Habit] = set()
     for directive in sorted_directives:
         if isinstance(directive, directives.TrackDirective):
             _check_track_directive_is_valid(directive, current_state)
             current_state.add(_build_habit_from_track_directive(directive))
         elif isinstance(directive, directives.UntrackDirective):
             _check_untrack_directive_is_valid(directive, current_state)
             current_state = _remove_habit_from_state(
@@ -83,15 +75,16 @@
     >>> directive1 = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("*", "*", "*"))
     >>> directive2 = directives.TrackDirective(dt.datetime(2024, 1, 2), "Habit 2", models.Frequency("*", "*", "*"))
     >>> tracked_habits = {models.Habit("Habit 1", models.Frequency("*", "*", "*"))}
     >>> _check_track_directive_is_valid(directive2, tracked_habits)
     """
     if directive.habit_name in {habit.name for habit in tracked_habits}:
         raise exceptions.ConsistencyError(
-            f"Several tracked habits with the same name: {directive.habit_name}"
+            f"Several tracked habits with the same name: {directive.habit_name}",
+            directive,
         )
 
 
 def _check_untrack_directive_is_valid(
     directive: directives.UntrackDirective, tracked_habits: set[models.Habit]
 ):
     """
@@ -103,15 +96,16 @@
     Example:
     >>> directive = directives.UntrackDirective(dt.datetime(2024, 1, 1), "Habit 1")
     >>> tracked_habits = {models.Habit("Habit 1", models.Frequency("*", "*", "*"))}
     >>> _check_untrack_directive_is_valid(directive, tracked_habits)
     """
     if directive.habit_name not in {habit.name for habit in tracked_habits}:
         raise exceptions.ConsistencyError(
-            f"Untracked habit without a corresponding track directive: {directive.habit_name}"
+            f"Untracked habit without a corresponding track directive: {directive.habit_name}",
+            directive,
         )
 
 
 def _remove_habit_from_state(
     habit_name: str, tracked_habits: set[models.Habit]
 ) -> set[models.Habit]:
     """
@@ -142,15 +136,17 @@
 
     Example:
     >>> directive = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("*", "*", "*"))
     >>> habit = _build_habit_from_track_directive(directive)
     >>> print(habit)
     Habit 1
     """
-    return models.Habit(directive.habit_name, directive.frequency)
+    return models.Habit(
+        directive.habit_name, directive.frequency, directive.is_measurable
+    )
 
 
 def _build_habit_record_from_record_directive(
     directive: directives.RecordDirective,
 ) -> models.HabitRecord:
     """
     Build a habit record from a record directive.
@@ -164,15 +160,15 @@
     >>> print(habit_record)
     HabitRecord(2024-01-01, Habit 1, False)
     """
     return models.HabitRecord(directive.date, directive.habit_name, directive.value)
 
 
 def _get_records_up_to_date(
-    directives_: list[directives.Directive], date: dt.datetime
+    directives_: list[directives.Directive], date: dt.date
 ) -> list[models.HabitRecord]:
     """
     Get the records up to a given date.
 
     :param directives_: List of directives.
     :param date: Date to check.
     :return: List of records.
@@ -186,15 +182,15 @@
     [HabitRecord(Habit 1, False), HabitRecord(Habit 2, True)]
     """
     directives_before_date = [
         directive for directive in directives_ if directive.date <= date
     ]
     sorted_directives = _sort_directives(directives_before_date)
 
-    records = []
+    records: list[models.HabitRecord] = []
     for directive in sorted_directives:
         if isinstance(directive, directives.RecordDirective):
             tracked_habits_at_date = _get_tracked_habits_at_date(
                 directives_, directive.date
             )
             _check_record_directive_is_valid(directive, tracked_habits_at_date, records)
             records.append(_build_habit_record_from_record_directive(directive))
@@ -218,29 +214,44 @@
     >>> directive = directives.RecordDirective(dt.datetime(2024, 1, 1), "Habit 1", False)
     >>> tracked_habits = {models.Habit("Habit 1", models.Frequency("*", "*", "*"))}
     >>> records = [models.HabitRecord(dt.datetime(2024, 1, 1), "Habit 2", True)]
     >>> _check_record_directive_is_valid(directive, tracked_habits, records)
     """
     if directive.habit_name not in {habit.name for habit in tracked_habits}:
         raise exceptions.ConsistencyError(
-            f"Recorded habit without a corresponding track directive: {directive.habit_name}"
+            f"Recorded habit without a corresponding track directive: {directive.habit_name}",
+            directive,
         )
 
     if any(
         record.date == directive.date and record.habit_name == directive.habit_name
         for record in records
     ):
         raise exceptions.ConsistencyError(
-            f"Several records of the same habit on the same day: {directive.habit_name}"
+            f"Several records of the same habit on the same day: {directive.habit_name}",
+            directive,
         )
 
+    for habit in tracked_habits:
+        if habit.name == directive.habit_name:
+            if habit.is_measurable and not isinstance(directive.value, float):
+                raise exceptions.ConsistencyError(
+                    f"Measurable habit with a non-float value: {directive.habit_name}",
+                    directive,
+                )
+            if not habit.is_measurable and not isinstance(directive.value, bool):
+                raise exceptions.ConsistencyError(
+                    f"Non-measurable habit with a non-bool value: {directive.habit_name}",
+                    directive,
+                )
+
 
 def get_state_at_date(
     directives_: list[directives.Directive], date: dt.date
-) -> (set[models.Habit], list[models.HabitRecord]):
+) -> typing.Tuple[set[models.Habit], list[models.HabitRecord]]:
     """
     Get the state of the habits at a given date.
 
     :param directives_: List of directives.
     :param date: Date to check.
     :return: List of tracked habits, list of records.
```

### Comparing `habits_txt-0.1.2/habits_txt/cli.py` & `habits_txt-0.1.3/habits_txt/cli.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.1.2/habits_txt/directives.py` & `habits_txt-0.1.3/habits_txt/directives.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,82 @@
 import datetime as dt
 from enum import Enum
 
+import habits_txt.defaults as defaults
 import habits_txt.models as models
 
 
 class DirectiveType(Enum):
     TRACK = "track"
     UNTRACK = "untrack"
     RECORD = "record"
 
 
 class Directive:
 
     directive_type: DirectiveType
 
-    def __init__(self, date: dt.date, habit_name: str):
+    def __init__(self, date: dt.date, habit_name: str, lineno: int):
         self.date = date
         self.habit_name = habit_name
+        self.lineno = lineno
 
     def __eq__(self, other):
         return self.date == other.date and self.habit_name == other.habit_name
 
     def __repr__(self):
         return f"{self.directive_type} {self.date} {self.habit_name}"
 
 
 class TrackDirective(Directive):
 
     directive_type = DirectiveType.TRACK
 
-    def __init__(self, date: dt.date, habit_name: str, frequency: models.Frequency):
-        super().__init__(date, habit_name)
+    def __init__(
+        self,
+        date: dt.date,
+        habit_name: str,
+        lineno: int,
+        frequency: models.Frequency,
+        is_measurable: bool,
+    ):
+        super().__init__(date, habit_name, lineno)
         self.frequency = frequency
+        self.is_measurable = is_measurable
 
     def __eq__(self, other):
-        return super().__eq__(other) and self.frequency == other.frequency
+        return (
+            super().__eq__(other)
+            and self.frequency == other.frequency
+            and self.is_measurable == other.is_measurable
+        )
 
     def __repr__(self):
-        return super().__repr__() + f" {self.frequency}"
+        return (
+            super().__repr__()
+            + f" {self.frequency} {defaults.MEASURABLE_KEYWORD if self.is_measurable else ''}"
+        )
 
 
 class UntrackDirective(Directive):
 
     directive_type = DirectiveType.UNTRACK
 
-    def __init__(self, date: dt.date, habit_name: str):
-        super().__init__(date, habit_name)
+    def __init__(self, date: dt.date, habit_name: str, lineno: int):
+        super().__init__(date, habit_name, lineno)
 
 
 class RecordDirective(Directive):
 
     directive_type = DirectiveType.RECORD
 
-    def __init__(self, date: dt.date, habit_name: str, value: bool | float):
-        super().__init__(date, habit_name)
+    def __init__(
+        self, date: dt.date, habit_name: str, lineno: int, value: bool | float
+    ):
+        super().__init__(date, habit_name, lineno)
         self.value = value
 
     def __eq__(self, other):
         return super().__eq__(other) and self.value == other.value
 
     def __repr__(self):
         return super().__repr__() + f" {self.value}"
```

### Comparing `habits_txt-0.1.2/habits_txt/models.py` & `habits_txt-0.1.3/habits_txt/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,18 +37,20 @@
 class Habit:
     """
     Habit tracked by the user.
 
     Example:
       name: "Sample habit"
       frequency: Frequency("*", "*", "*")
+      is_measurable: False
     """
 
     name: str
     frequency: Frequency
+    is_measurable: bool = False
 
     def __hash__(self):
         return hash(self.name)
 
 
 @dataclass
 class HabitRecord:
@@ -66,9 +68,20 @@
     value: bool | float | None
 
     @property
     def is_complete(self) -> bool:
         return bool(self.value)
 
     def __str__(self) -> str:
-        return (f'{dt.datetime.strftime(self.date, defaults.DATE_FMT)} '
-                f'"{self.habit_name}" {self.value if self.value is not None else ""}')
+        return (
+            f"{dt.datetime.strftime(self.date, defaults.DATE_FMT)} "
+            f'"{self.habit_name}" {self._str_value()}'
+        )
+
+    def _str_value(self) -> str:
+        if self.value is True:
+            return defaults.BOOLEAN_TRUE
+        elif self.value is False:
+            return defaults.BOOLEAN_FALSE
+        elif self.value is None:
+            return ""
+        return str(self.value)
```

### Comparing `habits_txt-0.1.2/PKG-INFO` & `habits_txt-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: habits.txt
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: estebanthi
 Author-email: esteban.thilliez@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: croniter (>=2.0.5,<3.0.0)
+Requires-Dist: types-croniter (>=2.0.0.20240423,<3.0.0.0)
 Description-Content-Type: text/markdown
 
 # habits.txt
 
 habits.txt is a plain text habit tracker.
 
 ## Concepts
@@ -21,69 +22,71 @@
 A habit is time-bound. It has a start date, and eventually an end date.
 It means with habits.txt, you can track habits for a specific period of time. When you want to stop tracking a habit, you can just stop tracking it.
 
 ### Frequency
 
 A habit is defined by a frequency, else it's called a task. The minimum frequency supported by habits.txt is daily (it doesn't support intra-day habits).
 
-### Boolean or Numeric
-
-A habit can be boolean or numeric. A boolean habit is either done or not done. A numeric habit is a value, like the number of pages read in a day.
+### Boolean or Measurable
 
+A habit can be boolean or measurable. A boolean habit is either done or not done. A measurable habit has a value.
 
 ## Format
 
 Habits are tracked in what I call a "journal" which is just a plain text file. A journal contains "directives".
 
 A directive is composed of a date, a directive type, a habit name, and other metadata specific to the directive type. For example, here is a sample directive:
 
 ```
-2024-01-01 track "Read 5 pages a day"
+2024-01-01 track "Read 5 pages a day" (* * *)
 ```
 
 You can comment lines in your journal by starting them with a `#` character.
 You can't add comments at the end of a line.
 
 ```
 # Start tracking a habit
-2024-01-01 track "Read 5 pages a day"
+2024-01-01 track "Read 5 pages a day" (* * *)
 ```
 
-
 ## Directives
 
 ### track
 
-To start tracking a habit, you use the `track` directive and specify the frequency of the habit.
+To start tracking a habit, you use the `track` directive and specify the frequency of the habit enclosed in parentheses.
+Optionally, you can make the habit measurable by specifying the "measurable" keyword.
 
 The frequency follows a simplified [cron](https://en.wikipedia.org/wiki/Cron) syntax, omitting the minute and the hour.
 
 Example:
+
 ```
-2024-01-01 track "Read 5 pages a day" * * *
-2024-01-01 track "Exercise" * * 1,3,5
+2024-01-01 track "Read 5 pages a day" (* * *)
+2024-01-01 track "Exercise" (* * 1,3,5) measurable
 ```
 
 ### untrack
 
 To stop tracking a habit, you use the `untrack` directive.
 
 Example:
+
 ```
 2024-02-01 untrack "Read 5 pages a day"
 ```
 
 ### record
 
 To record a habit, you use the `record` directive and specify a value.
 
 The allowed values are `yes`, `no`, or a number. You should not mix boolean and numeric values for the same habit.
 
 You can write directives but omit the directive type, it will default to `record`.
 
 Example:
+
 ```
 2024-01-01 record "Read 5 pages a day" 5
 2024-01-01 record "Workout" yes
 2024-01-01 "Weight" 70.5
 ```
```

