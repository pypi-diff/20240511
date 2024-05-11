# Comparing `tmp/habits_txt-0.1.0.tar.gz` & `tmp/habits_txt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habits_txt-0.1.0.tar", max compression
+gzip compressed data, was "habits_txt-0.1.1.tar", max compression
```

## Comparing `habits_txt-0.1.0.tar` & `habits_txt-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2053 2024-05-11 15:07:21.133891 habits_txt-0.1.0/README.md
--rw-r--r--   0        0        0      236 2024-05-11 15:20:35.231382 habits_txt-0.1.0/main.py
--rw-r--r--   0        0        0      485 2024-05-11 15:20:01.114266 habits_txt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9551 2024-05-11 15:12:54.975231 habits_txt-0.1.0/src/builder.py
--rw-r--r--   0        0        0     3326 2024-05-11 15:12:54.975231 habits_txt-0.1.0/src/cli.py
--rw-r--r--   0        0        0      111 2024-05-11 15:12:54.975231 habits_txt-0.1.0/src/defaults.py
--rw-r--r--   0        0        0     1556 2024-05-11 15:12:54.975231 habits_txt-0.1.0/src/directives.py
--rw-r--r--   0        0        0      194 2024-05-11 15:07:11.397084 habits_txt-0.1.0/src/exceptions.py
--rw-r--r--   0        0        0     3814 2024-05-11 15:12:54.975231 habits_txt-0.1.0/src/journal.py
--rw-r--r--   0        0        0     1508 2024-05-11 15:12:54.975231 habits_txt-0.1.0/src/models.py
--rw-r--r--   0        0        0     5911 2024-05-11 15:12:54.975231 habits_txt-0.1.0/src/parser.py
--rw-r--r--   0        0        0      595 2024-05-11 15:12:54.975231 habits_txt-0.1.0/src/utils.py
--rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 habits_txt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2053 2024-05-11 15:48:56.511263 habits_txt-0.1.1/README.md
+-rw-r--r--   0        0        0      236 2024-05-11 15:49:37.955022 habits_txt-0.1.1/main.py
+-rw-r--r--   0        0        0      503 2024-05-11 15:52:58.483789 habits_txt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9551 2024-05-11 15:48:56.511263 habits_txt-0.1.1/src/builder.py
+-rw-r--r--   0        0        0     3405 2024-05-11 15:49:37.955022 habits_txt-0.1.1/src/cli.py
+-rw-r--r--   0        0        0      111 2024-05-11 15:48:56.511263 habits_txt-0.1.1/src/defaults.py
+-rw-r--r--   0        0        0     1556 2024-05-11 15:48:56.511263 habits_txt-0.1.1/src/directives.py
+-rw-r--r--   0        0        0      194 2024-05-11 15:48:56.511263 habits_txt-0.1.1/src/exceptions.py
+-rw-r--r--   0        0        0     4284 2024-05-11 15:49:37.955022 habits_txt-0.1.1/src/journal.py
+-rw-r--r--   0        0        0     1530 2024-05-11 15:49:37.955022 habits_txt-0.1.1/src/models.py
+-rw-r--r--   0        0        0     5911 2024-05-11 15:48:56.511263 habits_txt-0.1.1/src/parser.py
+-rw-r--r--   0        0        0      595 2024-05-11 15:48:56.511263 habits_txt-0.1.1/src/utils.py
+-rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 habits_txt-0.1.1/PKG-INFO
```

### Comparing `habits_txt-0.1.0/README.md` & `habits_txt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `habits_txt-0.1.0/src/builder.py` & `habits_txt-0.1.1/src/builder.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.1.0/src/cli.py` & `habits_txt-0.1.1/src/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,16 +63,19 @@
 
     def run_fill():
         records = journal.fill_day(
             args.file,
             dt.datetime.strptime(args.date, defaults.DATE_FMT).date(),
             args.interactive,
         )
-        records_str = "\n".join([str(record) for record in records])
-        output(args.file, records_str, args.write_top, args.write_bottom)
+        if records:
+            records_str = (
+                "\n".join([str(record) for record in records]) if records else ""
+            )
+            output(args.file, records_str, args.write_top, args.write_bottom)
 
     if not args.command:
         run_fill()
     if args.command == "fill":
         run_fill()
     if args.command == "filter":
         start_date = (
```

### Comparing `habits_txt-0.1.0/src/directives.py` & `habits_txt-0.1.1/src/directives.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.1.0/src/journal.py` & `habits_txt-0.1.1/src/journal.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime as dt
 import logging
-from functools import wraps
 
 import src.builder as builder
+import src.defaults as defaults
 import src.exceptions as exceptions
 import src.models as models
 import src.parser as parser
 
 
 def get_state_at_date(
     journal_file: str, date: dt.date
@@ -42,21 +42,31 @@
     :param journal_file: Path to the journal file.
     :param date: Date to fill.
     :param interactive: Interactive mode.
     :return: Journal file.
     """
     records_fill = []
     tracked_habits, records = get_state_at_date(journal_file, date)
+    if not tracked_habits:
+        logging.info(f"{defaults.COMMENT_CHAR} No habits tracked")
+        return []
     for habit in tracked_habits:
-        most_recent_and_completed_record = _get_most_recent_and_completed_record(
-            habit, records
-        )
-        next_due_date = habit.frequency.get_next_date(
-            most_recent_and_completed_record.date
-        )
+        habit_records = [
+            record for record in records if record.habit_name == habit.name
+        ]
+        if not habit_records:
+            # because we can have a record directive the day we start to track a habit
+            next_due_date = habit.frequency.get_next_date(date - dt.timedelta(days=1))
+        else:
+            most_recent_and_completed_record = _get_most_recent_and_completed_record(
+                habit, records
+            )
+            next_due_date = habit.frequency.get_next_date(
+                most_recent_and_completed_record.date
+            )
         if next_due_date <= date:
             if interactive:
                 value_is_valid = False
                 while not value_is_valid:
                     value = input(f"{habit.name} ({next_due_date}): ")
                     try:
                         parsed_value = parser._parse_value(value)
```

### Comparing `habits_txt-0.1.0/src/models.py` & `habits_txt-0.1.1/src/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,8 +66,9 @@
     value: bool | float | None
 
     @property
     def is_complete(self) -> bool:
         return bool(self.value)
 
     def __str__(self) -> str:
-        return f'{dt.datetime.strftime(self.date, defaults.DATE_FMT)} "{self.habit_name}" {self.value if self.value is not None else ""}'
+        return (f'{dt.datetime.strftime(self.date, defaults.DATE_FMT)} '
+                f'"{self.habit_name}" {self.value if self.value is not None else ""}')
```

### Comparing `habits_txt-0.1.0/src/parser.py` & `habits_txt-0.1.1/src/parser.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.1.0/src/utils.py` & `habits_txt-0.1.1/src/utils.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.1.0/PKG-INFO` & `habits_txt-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habits.txt
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: estebanthi
 Author-email: esteban.thilliez@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: croniter (>=2.0.5,<3.0.0)
```

