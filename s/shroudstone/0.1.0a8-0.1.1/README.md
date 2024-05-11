# Comparing `tmp/shroudstone-0.1.0a8.tar.gz` & `tmp/shroudstone-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shroudstone-0.1.0a8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "shroudstone-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `shroudstone-0.1.0a8.tar` & `shroudstone-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,89 @@
--rw-r--r--   0        0        0       20 2024-02-24 10:29:15.326251 shroudstone-0.1.0a8/.gitignore
--rw-r--r--   0        0        0    32422 2024-02-24 10:29:15.326251 shroudstone-0.1.0a8/LICENSE
--rw-r--r--   0        0        0     2365 2024-02-24 12:34:23.934514 shroudstone-0.1.0a8/README.md
--rwxr-xr-x   0        0        0      297 2024-02-24 10:29:15.326251 shroudstone-0.1.0a8/codegen.sh
--rw-r--r--   0        0        0      723 2024-02-24 12:31:21.140159 shroudstone-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0       83 2024-02-24 13:15:37.006156 shroudstone-0.1.0a8/shroudstone/__init__.py
--rw-r--r--   0        0        0       28 2024-02-24 12:24:29.102030 shroudstone-0.1.0a8/shroudstone/__main__.py
--rw-r--r--   0        0        0     6088 2024-02-24 13:14:37.800475 shroudstone-0.1.0a8/shroudstone/cli.py
--rw-r--r--   0        0        0     1210 2024-02-24 12:12:08.196227 shroudstone-0.1.0a8/shroudstone/config.py
--rwxr-xr-x   0        0        0     9570 2024-02-24 12:25:57.857598 shroudstone-0.1.0a8/shroudstone/renamer.py
--rwxr-xr-x   0        0        0     2088 2024-02-24 10:29:15.330252 shroudstone-0.1.0a8/shroudstone/replay.py
--rw-r--r--   0        0        0     2121 2024-02-24 11:56:41.438150 shroudstone-0.1.0a8/shroudstone/stormgate_pb2.py
--rw-r--r--   0        0        0     1847 2024-02-24 11:56:41.442150 shroudstone-0.1.0a8/shroudstone/stormgate_pb2.pyi
--rwxr-xr-x   0        0        0      755 2024-02-24 10:29:15.334251 shroudstone-0.1.0a8/stormgate.proto
--rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 shroudstone-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0      957 2024-02-27 12:08:06.662709 shroudstone-0.1.1/.github/workflows/build-exe.yml
+-rw-r--r--   0        0        0       45 2024-02-28 11:05:03.022804 shroudstone-0.1.1/.gitignore
+-rw-r--r--   0        0        0    32422 2024-02-25 06:24:42.992531 shroudstone-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7244 2024-03-23 01:38:38.331578 shroudstone-0.1.1/README.md
+-rwxr-xr-x   0        0        0      514 2024-02-29 02:05:53.988528 shroudstone-0.1.1/api-client-codegen.sh
+-rwxr-xr-x   0        0        0      297 2024-02-25 06:24:42.992531 shroudstone-0.1.1/codegen.sh
+-rw-r--r--   0        0        0    90765 2024-03-07 06:03:55.756412 shroudstone-0.1.1/docs/example-screenshot.png
+-rw-r--r--   0        0        0      185 2024-03-23 01:38:38.331578 shroudstone-0.1.1/pyinstaller_build.bat
+-rw-r--r--   0        0        0      873 2024-03-23 01:38:38.331578 shroudstone-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-05-11 02:51:00.179901 shroudstone-0.1.1/shroudstone/__init__.py
+-rw-r--r--   0        0        0      373 2024-03-01 04:58:54.233893 shroudstone-0.1.1/shroudstone/__main__.py
+-rw-r--r--   0        0        0     7858 2024-05-11 01:09:56.591517 shroudstone-0.1.1/shroudstone/cli.py
+-rw-r--r--   0        0        0     2572 2024-03-23 01:38:38.331578 shroudstone-0.1.1/shroudstone/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:03:55.756412 shroudstone-0.1.1/shroudstone/gui/__init__.py
+-rw-r--r--   0        0        0       43 2024-02-27 12:08:06.666709 shroudstone-0.1.1/shroudstone/gui/__main__.py
+-rw-r--r--   0        0        0    15443 2024-05-11 01:09:56.591517 shroudstone-0.1.1/shroudstone/gui/app.py
+-rw-r--r--   0        0        0    16958 2024-02-27 12:08:06.666709 shroudstone-0.1.1/shroudstone/gui/assets/shroudstone.ico
+-rw-r--r--   0        0        0     2821 2024-02-27 12:08:06.666709 shroudstone-0.1.1/shroudstone/gui/assets/shroudstone.png
+-rw-r--r--   0        0        0     6363 2024-02-27 12:08:06.666709 shroudstone-0.1.1/shroudstone/gui/assets/shroudstone.svg
+-rw-r--r--   0        0        0      569 2024-03-23 01:38:38.331578 shroudstone-0.1.1/shroudstone/gui/fonts.py
+-rw-r--r--   0        0        0     2779 2024-03-07 04:57:52.650122 shroudstone-0.1.1/shroudstone/gui/jobs.py
+-rw-r--r--   0        0        0     3002 2024-03-23 01:38:38.331578 shroudstone-0.1.1/shroudstone/gui/logview.py
+-rw-r--r--   0        0        0      621 2024-03-23 01:38:38.331578 shroudstone-0.1.1/shroudstone/logging.py
+-rwxr-xr-x   0        0        0    21687 2024-03-23 01:38:38.331578 shroudstone-0.1.1/shroudstone/renamer.py
+-rwxr-xr-x   0        0        0    11462 2024-05-11 02:50:42.075928 shroudstone-0.1.1/shroudstone/replay.py
+-rw-r--r--   0        0        0      353 2024-02-28 10:42:52.460560 shroudstone-0.1.1/shroudstone/sgw_api.py
+-rw-r--r--   0        0        0     4463 2024-03-06 11:27:47.966810 shroudstone-0.1.1/shroudstone/stormgate_pb2.py
+-rw-r--r--   0        0        0     5462 2024-03-06 11:27:47.966810 shroudstone-0.1.1/shroudstone/stormgate_pb2.pyi
+-rw-r--r--   0        0        0     5374 2024-03-01 04:58:49.905816 shroudstone-0.1.1/shroudstone/stormgateworld/__init__.py
+-rw-r--r--   0        0        0      417 2024-03-01 04:58:49.913816 shroudstone-0.1.1/shroudstone/stormgateworld/api/__init__.py
+-rw-r--r--   0        0        0    12807 2024-03-01 04:58:49.917816 shroudstone-0.1.1/shroudstone/stormgateworld/api/leaderboard_entries_api.py
+-rw-r--r--   0        0        0    22652 2024-03-01 04:58:49.925816 shroudstone-0.1.1/shroudstone/stormgateworld/api/leaderboards_api.py
+-rw-r--r--   0        0        0    11844 2024-03-01 04:58:49.929816 shroudstone-0.1.1/shroudstone/stormgateworld/api/matches_api.py
+-rw-r--r--   0        0        0    64249 2024-03-01 04:58:49.937816 shroudstone-0.1.1/shroudstone/stormgateworld/api/players_api.py
+-rw-r--r--   0        0        0    43816 2024-03-01 04:58:49.941816 shroudstone-0.1.1/shroudstone/stormgateworld/api/statistics_api.py
+-rw-r--r--   0        0        0    25859 2024-03-01 04:58:49.945817 shroudstone-0.1.1/shroudstone/stormgateworld/api_client.py
+-rw-r--r--   0        0        0      652 2024-03-01 04:58:49.953817 shroudstone-0.1.1/shroudstone/stormgateworld/api_response.py
+-rw-r--r--   0        0        0    15400 2024-03-01 04:58:49.957817 shroudstone-0.1.1/shroudstone/stormgateworld/configuration.py
+-rw-r--r--   0        0        0     5968 2024-03-01 04:58:49.965817 shroudstone-0.1.1/shroudstone/stormgateworld/exceptions.py
+-rw-r--r--   0        0        0     4353 2024-03-01 04:58:49.969817 shroudstone-0.1.1/shroudstone/stormgateworld/models/__init__.py
+-rw-r--r--   0        0        0     3091 2024-03-01 04:58:49.977817 shroudstone-0.1.1/shroudstone/stormgateworld/models/activity_statistics.py
+-rw-r--r--   0        0        0     3379 2024-03-01 04:58:49.981817 shroudstone-0.1.1/shroudstone/stormgateworld/models/activity_statistics_activity.py
+-rw-r--r--   0        0        0     3113 2024-03-01 04:58:49.989817 shroudstone-0.1.1/shroudstone/stormgateworld/models/activity_statistics_entry.py
+-rw-r--r--   0        0        0      770 2024-03-01 04:58:49.997818 shroudstone-0.1.1/shroudstone/stormgateworld/models/aggregation.py
+-rw-r--r--   0        0        0     3263 2024-03-01 04:58:50.005818 shroudstone-0.1.1/shroudstone/stormgateworld/models/countries_statistics.py
+-rw-r--r--   0        0        0     3090 2024-03-01 04:58:50.009818 shroudstone-0.1.1/shroudstone/stormgateworld/models/countries_statistics_entry.py
+-rw-r--r--   0        0        0      731 2024-03-01 04:58:50.017818 shroudstone-0.1.1/shroudstone/stormgateworld/models/dump_format.py
+-rw-r--r--   0        0        0     2956 2024-03-01 04:58:50.021818 shroudstone-0.1.1/shroudstone/stormgateworld/models/error_response.py
+-rw-r--r--   0        0        0      784 2024-03-01 04:58:50.029818 shroudstone-0.1.1/shroudstone/stormgateworld/models/leaderboard.py
+-rw-r--r--   0        0        0     3274 2024-03-01 04:58:50.033818 shroudstone-0.1.1/shroudstone/stormgateworld/models/leaderboard_dump_response.py
+-rw-r--r--   0        0        0     3459 2024-03-01 04:58:50.037818 shroudstone-0.1.1/shroudstone/stormgateworld/models/leaderboard_entry_history.py
+-rw-r--r--   0        0        0     3172 2024-03-01 04:58:50.045818 shroudstone-0.1.1/shroudstone/stormgateworld/models/leaderboard_entry_history_row.py
+-rw-r--r--   0        0        0     6683 2024-03-01 04:58:50.049818 shroudstone-0.1.1/shroudstone/stormgateworld/models/leaderboard_entry_response.py
+-rw-r--r--   0        0        0      751 2024-03-01 04:58:50.053819 shroudstone-0.1.1/shroudstone/stormgateworld/models/leaderboard_order.py
+-rw-r--r--   0        0        0     3340 2024-03-01 04:58:50.061819 shroudstone-0.1.1/shroudstone/stormgateworld/models/leaderboard_response.py
+-rw-r--r--   0        0        0      843 2024-03-01 04:58:50.065819 shroudstone-0.1.1/shroudstone/stormgateworld/models/league.py
+-rw-r--r--   0        0        0     4124 2024-03-01 04:58:50.073819 shroudstone-0.1.1/shroudstone/stormgateworld/models/match_participant_player_leaderboard_entry_response.py
+-rw-r--r--   0        0        0     3287 2024-03-01 04:58:50.077819 shroudstone-0.1.1/shroudstone/stormgateworld/models/match_participant_player_response.py
+-rw-r--r--   0        0        0     6065 2024-03-01 04:58:50.081819 shroudstone-0.1.1/shroudstone/stormgateworld/models/match_participant_response.py
+-rw-r--r--   0        0        0     4510 2024-03-01 04:58:50.089819 shroudstone-0.1.1/shroudstone/stormgateworld/models/match_response.py
+-rw-r--r--   0        0        0      760 2024-03-01 04:58:50.093819 shroudstone-0.1.1/shroudstone/stormgateworld/models/match_result.py
+-rw-r--r--   0        0        0      745 2024-03-01 04:58:50.097819 shroudstone-0.1.1/shroudstone/stormgateworld/models/match_state.py
+-rw-r--r--   0        0        0     3279 2024-03-01 04:58:50.105820 shroudstone-0.1.1/shroudstone/stormgateworld/models/matches_response.py
+-rw-r--r--   0        0        0     4373 2024-03-01 04:58:50.109820 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_activity_stats.py
+-rw-r--r--   0        0        0     3575 2024-03-01 04:58:50.117820 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_activity_stats_race.py
+-rw-r--r--   0        0        0     3303 2024-03-01 04:58:50.121820 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_matches_response.py
+-rw-r--r--   0        0        0     3129 2024-03-01 04:58:50.125820 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_matchups_stats.py
+-rw-r--r--   0        0        0     4181 2024-03-01 04:58:50.133820 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_matchups_stats_entry.py
+-rw-r--r--   0        0        0     3643 2024-03-01 04:58:50.137820 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_matchups_stats_matchup.py
+-rw-r--r--   0        0        0     3297 2024-03-01 04:58:50.145820 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_opponents_stats.py
+-rw-r--r--   0        0        0     4240 2024-03-01 04:58:50.149820 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_opponents_stats_opponent.py
+-rw-r--r--   0        0        0     5174 2024-03-01 04:58:50.153820 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_response.py
+-rw-r--r--   0        0        0     4858 2024-03-01 04:58:50.161821 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_stats_entry.py
+-rw-r--r--   0        0        0     4625 2024-03-01 04:58:50.165820 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_stats_entry_aggregated.py
+-rw-r--r--   0        0        0     3704 2024-03-01 04:58:50.173821 shroudstone-0.1.1/shroudstone/stormgateworld/models/player_stats_entry_num_breakdown.py
+-rw-r--r--   0        0        0      753 2024-03-01 04:58:50.177821 shroudstone-0.1.1/shroudstone/stormgateworld/models/profile_privacy.py
+-rw-r--r--   0        0        0      731 2024-03-01 04:58:50.185821 shroudstone-0.1.1/shroudstone/stormgateworld/models/race.py
+-rw-r--r--   0        0        0      769 2024-03-01 04:58:50.189821 shroudstone-0.1.1/shroudstone/stormgateworld/models/resolution.py
+-rw-r--r--   0        0        0     3229 2024-03-01 04:58:50.193821 shroudstone-0.1.1/shroudstone/stormgateworld/models/servers_statistics.py
+-rw-r--r--   0        0        0     2660 2024-03-01 04:58:50.197821 shroudstone-0.1.1/shroudstone/stormgateworld/models/servers_statistics_entry.py
+-rw-r--r--   0        0        0     4183 2024-03-01 04:58:50.205821 shroudstone-0.1.1/shroudstone/stormgateworld/models/stats_by_time.py
+-rw-r--r--   0        0        0     3457 2024-03-01 04:58:50.209821 shroudstone-0.1.1/shroudstone/stormgateworld/models/stats_by_time_entry.py
+-rw-r--r--   0        0        0     5499 2024-03-01 04:58:50.213822 shroudstone-0.1.1/shroudstone/stormgateworld/models/stats_by_time_history_point.py
+-rw-r--r--   0        0        0     3390 2024-03-01 04:58:50.217821 shroudstone-0.1.1/shroudstone/stormgateworld/models/stats_by_time_match_length.py
+-rw-r--r--   0        0        0     4227 2024-03-01 04:58:50.225822 shroudstone-0.1.1/shroudstone/stormgateworld/models/stats_by_time_match_length_entry.py
+-rw-r--r--   0        0        0        0 2024-02-29 02:04:14.863124 shroudstone-0.1.1/shroudstone/stormgateworld/py.typed
+-rw-r--r--   0        0        0     9240 2024-03-01 04:58:50.229822 shroudstone-0.1.1/shroudstone/stormgateworld/rest.py
+-rwxr-xr-x   0        0        0     2668 2024-03-06 11:27:47.970810 shroudstone-0.1.1/stormgate.proto
+-rw-r--r--   0        0        0     8031 1970-01-01 00:00:00.000000 shroudstone-0.1.1/PKG-INFO
```

### Comparing `shroudstone-0.1.0a8/LICENSE` & `shroudstone-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.0a8/pyproject.toml` & `shroudstone-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,19 +10,25 @@
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Topic :: Games/Entertainment :: Real Time Strategy"
 ]
 keywords = ["Stormgate"]
 dynamic = ["version", "description"]
 dependencies = [
-    "pandas~=2.1",
+    "pandas~=2.0",
+    "pillow>=5.0",
     "protobuf~=4.23",
     "pydantic~=2.6",
+    "pystray~=0.19.5",
+    "python-dateutil>=2.8.2",
+    "pyyaml>=5",
     "typer[all]~=0.9.0",
+    "typing_extensions>=4.7.1",
+    "urllib3>=1.25.3",
 ]
 requires-python = "~=3.8"
 
 [project.urls]
 Source = "https://github.com/acarapetis/shroudstone"
 
 [project.scripts]
-shroudstone = "shroudstone.cli:app"
+shroudstone = "shroudstone.__main__:main"
```

### Comparing `shroudstone-0.1.0a8/shroudstone/cli.py` & `shroudstone-0.1.1/shroudstone/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,127 @@
-"""The shroudstone CLI"""
+"""shroudstone is a tool for managing Stormgate replays.
+
+To get started renaming your replays, use [b]rename-replays --help[/b] to view
+options or [b]rename-replays[/b] to jump straight in."""
 
 import logging
 import os
 from pathlib import Path
 import platform
 import subprocess
-from typing import Annotated, Optional
+import sys
+from typing import Optional
+from typing_extensions import Annotated
 
-from rich.console import Console
-from rich.logging import RichHandler
 import typer
 
-from shroudstone import renamer, replay
-from shroudstone.config import Config, config_file, DEFAULT_FORMAT
+from shroudstone import __version__
+from shroudstone.config import DEFAULT_GENERIC_FORMAT, Config, config_file, DEFAULT_1v1_FORMAT, Strategy
+from shroudstone.logging import configure_logging
 
-app = typer.Typer()
+app = typer.Typer(rich_markup_mode="rich", help=sys.modules[__name__].__doc__)
 
-console = Console(stderr=True)
-logging.captureWarnings(True)
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(message)s",
-    handlers=[RichHandler(console=console)],
-)
 logger = logging.getLogger(__name__)
 
 
-@app.command()
+def version(value: bool):
+    if value:
+        typer.echo(f"Shroudstone v{__version__}")
+        raise typer.Exit()
+
+
+@app.callback()
+def callback(
+    ctx: typer.Context,
+    version: Annotated[
+        bool,
+        typer.Option(
+            "--version",
+            help="Show version information for your shroudstone installation",
+            callback=version,
+        ),
+    ] = False,
+    debug: bool = False,
+):
+    configure_logging(debug=debug)
+
+
+@app.command(rich_help_panel="Tools for nerds")
 def get_replay_info(replay_file: typer.FileBinaryRead):
     """Extract information from a replay, outputting it in JSON format."""
-    typer.echo(replay.get_match_info(replay_file).model_dump_json(indent=2))
+    from shroudstone.replay import summarize_replay
+
+    typer.echo(summarize_replay(replay_file).model_dump_json(indent=2))
 
 
-@app.command()
+@app.command(rich_help_panel="Tools for nerds")
 def split_replay(replay_file: typer.FileBinaryRead, output_directory: Path):
     """Extract a stormgate replay into a directory containing individual protoscope messages."""
+    from shroudstone.replay import split_replay
+
     output_directory.mkdir(exist_ok=True, parents=True)
     i = 0
-    for i, chunk in enumerate(replay.split_replay(replay_file)):
+    for i, chunk in enumerate(split_replay(replay_file)):
         (output_directory / f"{i:07d}.binpb").write_bytes(chunk)
     typer.echo(
         f"Wrote {i+1} replay messages in protoscope wire format to {output_directory}/."
     )
 
 
-@app.command()
-def edit_config():
-    """Open the shroudstone configuration file in your default text editor."""
+@app.command(rich_help_panel="Tools for nerds")
+def dump_replay(replay_file: typer.FileBinaryRead):
+    """Decode a replay and print a human-readable-ish representation of its contents."""
+    from shroudstone.replay import split_replay
+    from shroudstone.stormgate_pb2 import ReplayChunk
+
+    for bytestring in split_replay(replay_file):
+        chunk = ReplayChunk.FromString(bytestring)
+        print(chunk.timestamp, chunk.client_id, chunk.inner.content)
+
+
+@app.command(rich_help_panel="Tools for nerds")
+def config_path():
+    """Print the real path to the shroudstone configuration file."""
     if not config_file.exists():
         Config().save()
+    typer.echo(config_file.resolve())
+
+
+@app.command(rich_help_panel="Tools for nerds")
+def edit_config(xdg_open: bool = False):
+    """Open the shroudstone configuration file in your default text editor."""
+    from shroudstone import renamer
+
+    if not config_file.exists():
+        logger.info("No config file found, doing our best to auto-generate one.")
+        cfg = Config()
+        # Prefill this path if possible:
+        cfg.replay_dir = renamer.guess_replay_dir()
+        cfg.save()
+
+    realpath = config_file.resolve()
     if platform.system() == "Windows":
         # .resolve() is crucial when python is installed from the microsoft store
-        realpath = config_file.resolve()
         subprocess.run(["cmd", "/c", f"start {realpath}"])
     else:
-        editor = os.environ.get("VISUAL", os.environ.get("EDITOR", "nano"))
-        subprocess.run([editor, config_file.resolve()])
+        if xdg_open:
+            editor = "xdg-open"
+        else:
+            editor = os.environ.get("VISUAL", os.environ.get("EDITOR", "nano"))
+        subprocess.run([editor, realpath])
 
 
-@app.command()
+@app.command(rich_help_panel="Replay renaming")
+def gui():
+    from shroudstone.gui import app
+
+    app.run()
+
+
+@app.command(rich_help_panel="Replay renaming")
 def create_rename_replays_shortcut():
     """Create a desktop icon to launch the rename-replays script."""
     if platform.system() != "Windows":
         logger.error("This subcommand is only currently available on Windows.")
     else:
         batch = (
             Path(os.environ["USERPROFILE"]) / "Desktop" / "Rename Stormgate Replays.bat"
@@ -78,97 +137,90 @@
                 file=f,
             )
         logger.info(
             f"Batch file created at {batch} - should be visible on your desktop :)"
         )
 
 
-@app.command()
+@app.command(rich_help_panel="Replay renaming")
 def rename_replays(
     replay_dir: Annotated[
         Optional[Path],
         typer.Option(file_okay=False, dir_okay=True, exists=True, readable=True),
     ] = None,
-    my_player_id: Optional[str] = None,
-    format: Annotated[
-        Optional[str], typer.Option(help=f"Format string for new replay filenames\n(e.g. '{DEFAULT_FORMAT}')")
+    format_1v1: Annotated[
+        Optional[str],
+        typer.Option(
+            help=f"Format string for 1v1 replays \n(e.g. '{DEFAULT_1v1_FORMAT}')"
+        ),
+    ] = None,
+    format_generic: Annotated[
+        Optional[str],
+        typer.Option(
+            help=f"Format string for other replays \n(e.g. '{DEFAULT_GENERIC_FORMAT}')"
+        ),
     ] = None,
     backup: bool = True,
     dry_run: bool = False,
     reprocess: Annotated[
         bool, typer.Option(help="Reprocess old replays that have already been renamed")
     ] = False,
-    check_nicknames: Annotated[
+    clear_cache: Annotated[
         bool,
         typer.Option(
-            help="Check that nicknames in the replay match those from stormgateworld"
+            help="Clear the local match cache and re-retrieve all data from Stormgate World."
         ),
-    ] = True,
+    ] = False,
+    duration_strategy: Strategy = Strategy.prefer_stormgateworld,
+    result_strategy: Strategy = Strategy.prefer_stormgateworld,
 ):
-    """Automatically rename your replay files (including player nicknames, races, map name, duration, result)"""
+    """Automatically rename your replay files.
+
+    The first time you run this, you will be asked for your replay directory if
+    we can not find it automatically. This value is then stored in the
+    configuration file for future runs.
+
+    To customize the naming of your replays, you can provide a python format
+    string in the --format option, or (preferably) edit the format string in
+    your config file (see the [b]edit-config[/b] command).
+
+    Format strings can use the following values:
+
+    * us: Your nickname (as it appeared in the replay)
+    * them: Opponent nickname (as it appeared in the replay)
+    * f1: Faction/Race you played (Vanguard or Infernals or Maloc or Blockade)
+    * f2: Faction/Race opponent played
+    * time (datetime): Creation time of match
+    * duration: Game duration (e.g. "15m10s")
+    * result: Your game result (Win, Loss, Undecided)
+    * map_name (str): Name of the map on which the game was played (extracted from replay file)
+    * build_number (int): Build number of Stormgate version on which the game was played (extracted from replay file)
+    """
+    from shroudstone import renamer
+
     config = Config.load()
     if replay_dir is None:
         replay_dir = get_replay_dir(config)
-    if my_player_id is None:
-        my_player_id = get_player_id(config)
+    if clear_cache:
+        renamer.clear_cached_matches()
     renamer.rename_replays(
         replay_dir=replay_dir,
-        my_player_id=my_player_id,
         dry_run=dry_run,
         backup=backup,
         reprocess=reprocess,
-        check_nicknames=check_nicknames,
-        format=format or config.replay_name_format,
+        format_1v1=format_1v1 or config.replay_name_format_1v1,
+        format_generic=format_generic or config.replay_name_format_generic,
+        duration_strategy=duration_strategy,
+        result_strategy=result_strategy,
     )
 
 
-def get_player_id(config: Config) -> str:
-    if config.my_player_id is None:
-        typer.echo(
-            "You have not yet configured your player ID. To find it:\n"
-            "1. visit https://stormgateworld.com/leaderboards/ranked_1v1 and search for your in-game nickname.\n"
-            "2. find your account in the results and click on it.\n"
-            "3. click the characters next to the '#' icon to copy your player ID.\n"
-            "4. paste it below and press enter :)"
-        )
-        config.my_player_id = typer.prompt("Player ID")
-    config.save()
-    return config.my_player_id
-
-
-def guess_replay_dir() -> Optional[Path]:
-    if platform.system() == "Windows":
-        # Should be easy, just look in the current user's local app data
-        appdata = os.environ["LOCALAPPDATA"]
-        paths = [Path(appdata) / "Stormgate" / "Saved" / "Replays"]
-    else:
-        # If this script is running on Linux and Stormgate is installed using
-        # Steam+Proton, look in the steam compatdata:
-        steammnt = (
-            Path("~").expanduser()
-            / ".steam/root/steamapps/compatdata/2012510/pfx/dosdevices"
-        )
-
-        # If this script is running on the Windows Subsystem for Linux, we can
-        # find the Windows drives mounted in /mnt:
-        wslmnt = Path("/mnt")
-
-        tail = "AppData/Local/Stormgate/Saved/Replays"
-        paths = [
-            *steammnt.glob(f"*/users/steamuser/{tail}"),
-            *wslmnt.glob(f"*/Users/*/{tail}"),
-            *wslmnt.glob(f"*/Documents and Settings/*/{tail}"),
-        ]
-
-    for path in paths:
-        if path.is_dir():
-            return path
-
-
 def get_replay_dir(config: Config) -> Path:
+    from shroudstone.renamer import guess_replay_dir
+
     if config.replay_dir is None:
         config.replay_dir = guess_replay_dir()
         if config.replay_dir is None:
             typer.echo("Couldn't automatically determine your replay directory!")
             typer.echo(
                 "It normally lives in your user directory under "
                 r"AppData\Local\Stormgate\Saved\Replays."
```

