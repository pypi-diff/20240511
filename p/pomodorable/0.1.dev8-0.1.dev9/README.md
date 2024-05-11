# Comparing `tmp/pomodorable-0.1.dev8.tar.gz` & `tmp/pomodorable-0.1.dev9.tar.gz`

## Comparing `pomodorable-0.1.dev8.tar` & `pomodorable-0.1.dev9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/Justfile
--rw-r--r--   0        0        0     6068 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/ruff_defaults.toml
--rwxr-xr-x   0        0        0   160840 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/readme_images/app-1.gif
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/__main__.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/app.tcss
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/app_config.py
--rw-r--r--   0        0        0    11494 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/app_data.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/app_utils.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/cli.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/mru_list.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/mru_screen.py
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/output_csv.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/output_md.py
--rw-r--r--   0        0        0     9524 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/settings_screen.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/timerbar.py
--rw-r--r--   0        0        0    14633 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/src/pomodorable/ui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/tests/__init__.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/tests/conftest.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/tests/test_app_config.py
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/tests/test_app_data.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/tests/test_cli.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/tests/test_mru_list.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/tests/test_ui.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/LICENSE.txt
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/README.md
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/pyproject.toml
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 pomodorable-0.1.dev8/PKG-INFO
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/Justfile
+-rw-r--r--   0        0        0     6068 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/ruff_defaults.toml
+-rwxr-xr-x   0        0        0   160840 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/readme_images/app-1.gif
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/__main__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/app.tcss
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/app_config.py
+-rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/app_data.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/app_utils.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/cli.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/mru_list.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/mru_screen.py
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/output_csv.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/output_md.py
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/settings_screen.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/timerbar.py
+-rw-r--r--   0        0        0    14633 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/src/pomodorable/ui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/tests/__init__.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/tests/conftest.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/tests/test_app_config.py
+-rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/tests/test_app_data.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/tests/test_cli.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/tests/test_mru_list.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/tests/test_ui.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/LICENSE.txt
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/README.md
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/pyproject.toml
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 pomodorable-0.1.dev9/PKG-INFO
```

### Comparing `pomodorable-0.1.dev8/Justfile` & `pomodorable-0.1.dev9/Justfile`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/ruff_defaults.toml` & `pomodorable-0.1.dev9/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/readme_images/app-1.gif` & `pomodorable-0.1.dev9/readme_images/app-1.gif`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/src/pomodorable/app.tcss` & `pomodorable-0.1.dev9/src/pomodorable/app.tcss`

 * *Files 5% similar despite different names*

```diff
@@ -119,44 +119,38 @@
 
 .paused #frm-paused {
     display: block;
 }
 
 SettingsScreen {
     ScrollableContainer {
+        border: solid gray;
+
         Input {
             width: 4fr;
         }
+
         Button {
             max-width: 10;
         }
     }
     #frm-buttons {
-        height: 1;
-    }
-    #btn-close {
-        background: green;
-        border: none;
-        dock: left;
+        align: center middle;
     }
 }
 
-SettingSwitch {
-    border: solid gray;
+SettingInput, SettingSwitch {
+    border-bottom: solid olive;
     margin: 0;
 
     #lbl-setting {
         padding: 0 1;
         text-align: left;
     }
 
-    #swt-setting {
-        margin: 0 2;
-    }
-
     #lbl-warn {
         color: yellow;
         display: none;
         padding: 0 3;
         text-align: center;
     }
 
@@ -168,39 +162,17 @@
         visibility: hidden;
     }
     #btn-undo.data-changed {
         visibility: visible;
     }
 }
 
-SettingInput {
-    border: solid gray;
-    margin: 0;
-
-    #lbl-setting {
-        padding: 0 1;
-        text-align: left;
-    }
-
-    #lbl-warn {
-        color: yellow;
-        display: none;
-        padding: 0 3;
-        text-align: center;
-    }
-
-    #lbl-warn.show-warnings {
-        display: block;
-    }
-
-    #btn-undo {
-        visibility: hidden;
-    }
-    #btn-undo.data-changed {
-        visibility: visible;
+SettingSwitch {
+    #swt-setting {
+        margin: 0 2;
     }
 }
 
 TimerBar {
     align: center bottom;
     content-align: center middle;
     height: 3;
```

### Comparing `pomodorable-0.1.dev8/src/pomodorable/app_config.py` & `pomodorable-0.1.dev9/src/pomodorable/app_config.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/src/pomodorable/app_data.py` & `pomodorable-0.1.dev9/src/pomodorable/app_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 
 import csv
 import logging
 import os
 import sys
 from dataclasses import dataclass
 from datetime import datetime
-from logging.handlers import TimedRotatingFileHandler
 from pathlib import Path
 
 import dotenv
 from platformdirs import user_config_path, user_data_path
 
-from pomodorable.app_config import AppConfig
+from pomodorable.app_config import LOG_RETENTION_MIN, AppConfig
 from pomodorable.app_utils import get_date_from_str, sec_to_hms
 from pomodorable.mru_list import MRUList
 from pomodorable.output_csv import write_to_daily_csv
 from pomodorable.output_md import write_to_daily_md
 
 APP_NAME = "pomodorable"
 APP_CONFIG_FILE = f"{APP_NAME}-config.toml"
 APP_OUTPUT_CSV = f"{APP_NAME}-data.csv"
-APP_LOG_FILE = f"{APP_NAME}.log"
 APP_DATA_VERSION = "1"
 
 
 @dataclass
 class AppDataRow:
     version: str = APP_DATA_VERSION
     date_time: datetime = None
@@ -72,24 +70,25 @@
                 APP_NAME, appauthor=False, ensure_exists=True
             )
 
         self.output_csv = self.data_path / APP_OUTPUT_CSV
 
         self._log_handler = None
         self._log_formatter = None
-        self.log_file = self.data_path / APP_LOG_FILE
+        log_name = f"{APP_NAME}-{datetime.now().strftime('%Y%m%d')}.log"
+        self.log_file = self.data_path / log_name
         self._init_logging()
 
         if init_app_config:
             self.config = init_app_config
         else:
             self.config = AppConfig(self.config_file)
             self.config.load()
 
-        self._update_logging()
+        self._purge_log_files()
 
         self.mru_list = MRUList(self.data_path)
         self.mru_list.load()
 
     def _init_logging(self) -> None:
         """Add a file handler to the root logger. Do this before loading
         configuration so any errors in that process are logged.
@@ -99,32 +98,26 @@
         logger = logging.getLogger()
         logger.setLevel(logging.INFO)
         self._log_handler = logging.FileHandler(self.log_file)
         self._log_formatter = logging.Formatter("%(asctime)s %(message)s")
         self._log_handler.setFormatter(self._log_formatter)
         logger.addHandler(self._log_handler)
 
-    def _update_logging(self) -> None:
-        """Update logging after configuration is loaded. Replace the FileHandler
-        with a TimedRotatingFileHandler that rotates based on the configured
-        log retention days.
-        """
-        if not self.log_file:
+    def _purge_log_files(self) -> None:
+        """Purge log files older than the configured retention period."""
+
+        if self.config.log_retention_days < LOG_RETENTION_MIN:
+            logging.error("Log retention days is less than the minimum.")
             return
-        logger = logging.getLogger()
-        if self._log_handler:
-            logger.removeHandler(self._log_handler)
-        self._log_handler = TimedRotatingFileHandler(
-            self.log_file,
-            interval=1,
-            when="D",
-            backupCount=self.config.log_retention_days,
-        )
-        self._log_handler.setFormatter(self._log_formatter)
-        logger.addHandler(self._log_handler)
+
+        # Purge based on distinct dates in filenames (not by date range).
+        log_files = sorted(self.log_file.parent.glob(f"{APP_NAME}-*.log"))
+        if len(log_files) > self.config.log_retention_days:
+            for file in log_files[: -self.config.log_retention_days]:
+                file.unlink()
 
     def _append_data_csv(self, data_row: AppDataRow) -> None:
         """Append a line to the CSV file."""
         csv_str = (
             f"{data_row.version},{self._csv_date_time(data_row.date_time)},"
             f'"{data_row.action}","{data_row.message}",'
             f'"{data_row.duration}","{data_row.notes}"'
```

### Comparing `pomodorable-0.1.dev8/src/pomodorable/app_utils.py` & `pomodorable-0.1.dev9/src/pomodorable/app_utils.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/src/pomodorable/cli.py` & `pomodorable-0.1.dev9/src/pomodorable/cli.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/src/pomodorable/mru_list.py` & `pomodorable-0.1.dev9/src/pomodorable/mru_list.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/src/pomodorable/mru_screen.py` & `pomodorable-0.1.dev9/src/pomodorable/mru_screen.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/src/pomodorable/output_csv.py` & `pomodorable-0.1.dev9/src/pomodorable/output_csv.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/src/pomodorable/output_md.py` & `pomodorable-0.1.dev9/src/pomodorable/output_md.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/src/pomodorable/settings_screen.py` & `pomodorable-0.1.dev9/src/pomodorable/settings_screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 from textual import on
 from textual.app import ComposeResult  # noqa: TCH002
 from textual.containers import Horizontal, ScrollableContainer
 from textual.screen import Screen
 from textual.validation import Function, Integer
-from textual.widgets import Button, Footer, Header, Input, Label, Static, Switch
+from textual.widgets import Button, Header, Input, Label, Static, Switch
 
 from pomodorable.app_config import LOG_RETENTION_MIN, AppConfig
 
 
 class SettingSwitch(Static):
     def __init__(self, *args, **kwargs) -> None:
         self.initial_value = None
@@ -128,29 +128,29 @@
 class SettingsScreen(Screen[str]):
     def __init__(self, app_config: AppConfig) -> None:
         self.app_config = app_config
         super().__init__()
 
     def compose(self) -> ComposeResult:
         yield Header()
-        yield Footer()
-        yield Horizontal(
-            Button("Close", id="btn-close"),
-            id="frm-buttons",
-        )
         yield ScrollableContainer(
             SettingInput(id="set-minutes"),
             SettingInput(id="set-csv-dir"),
             SettingInput(id="set-md-dir"),
             SettingInput(id="set-md-heading"),
             SettingSwitch(id="set-md-append"),
             SettingInput(id="set-log-ret"),
         )
+        yield Horizontal(
+            Button("Close", id="btn-close"),
+            id="frm-buttons",
+        )
 
     def on_mount(self) -> None:
+        self.title = "Settings"
         set_minutes = self.query_one("#set-minutes")
         set_minutes.initialize(
             "Session Minutes",
             str(self.app_config.session_minutes),
             [
                 Integer(
                     minimum=1,
```

### Comparing `pomodorable-0.1.dev8/src/pomodorable/timerbar.py` & `pomodorable-0.1.dev9/src/pomodorable/timerbar.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/src/pomodorable/ui.py` & `pomodorable-0.1.dev9/src/pomodorable/ui.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/tests/conftest.py` & `pomodorable-0.1.dev9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/tests/test_app_config.py` & `pomodorable-0.1.dev9/tests/test_app_config.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/tests/test_app_data.py` & `pomodorable-0.1.dev9/tests/test_app_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from csv import DictReader
 from datetime import datetime, timedelta
 from pathlib import Path
 
 import pytest
 
+from pomodorable.app_config import AppConfig
 from pomodorable.app_data import AppData
 from pomodorable.app_utils import get_date_from_str
 from pomodorable.output_md import write_to_daily_md
 
 
 def test_data_csv_fields(app_data_with_four_test_sessions):
     app_data, start_times = app_data_with_four_test_sessions
@@ -210,7 +211,34 @@
 
     s = md_file.read_text()
     assert s.startswith(a)
     assert s.endswith(b)
     assert "Test session 1" in s
     assert "Test session 2" in s
     assert "Test session 3" in s
+
+
+def test_purge_log_files(tmp_path):
+    config_file = tmp_path / "pomodorable-config.toml"
+    app_config = AppConfig(config_file)
+    app_data = AppData(init_app_config=app_config, init_data_path=tmp_path)
+
+    # Make 8 fake log files.
+    for i in range(8):
+        p = tmp_path / f"pomodorable-2024010{i+1}.log"
+        p.write_text("")
+
+    # Should create a new log file.
+    assert app_data.log_file.exists()
+
+    # Default retention days is 30. Change it to 5.
+    app_data.config.log_retention_days = 5
+
+    # Run the private method to purge older log files.
+    app_data._purge_log_files()  # noqa: SLF001
+
+    # Check that all but 5 most recent were purged.
+    log_files = sorted(tmp_path.glob("*.log"))
+    assert len(log_files) == 5
+    assert log_files[0].name == "pomodorable-20240105.log"
+    assert log_files[-2].name == "pomodorable-20240108.log"
+    assert log_files[-1].name == app_data.log_file.name
```

### Comparing `pomodorable-0.1.dev8/tests/test_cli.py` & `pomodorable-0.1.dev9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/tests/test_mru_list.py` & `pomodorable-0.1.dev9/tests/test_mru_list.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/tests/test_ui.py` & `pomodorable-0.1.dev9/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/LICENSE.txt` & `pomodorable-0.1.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/README.md` & `pomodorable-0.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/pyproject.toml` & `pomodorable-0.1.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pomodorable-0.1.dev8/PKG-INFO` & `pomodorable-0.1.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pomodorable
-Version: 0.1.dev8
+Version: 0.1.dev9
 Summary: A pomodoro timer implemented as a Textual app
 Project-URL: Source, https://github.com/wmelvin/pomodorable
 Project-URL: Documentation, https://github.com/wmelvin/pomodorable#readme
 Author-email: Bill Melvin <bill@billmelvin.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: Textual,pomodoro
```

