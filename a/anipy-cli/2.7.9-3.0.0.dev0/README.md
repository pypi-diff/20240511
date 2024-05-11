# Comparing `tmp/anipy_cli-2.7.9.tar.gz` & `tmp/anipy_cli-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_cli-2.7.9.tar", last modified: Thu Mar  2 20:43:57 2023, max compression
+gzip compressed data, was "anipy_cli-3.0.0.dev0.tar", max compression
```

## Comparing `anipy_cli-2.7.9.tar` & `anipy_cli-3.0.0.dev0.tar`

### file list

```diff
@@ -1,57 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.846925 anipy_cli-2.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-03-02 20:43:57.846925 anipy_cli-2.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.842925 anipy_cli-2.7.9/anipy_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/arg_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.842925 anipy_cli-2.7.9/anipy_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.842925 anipy_cli-2.7.9/anipy_cli/cli/clis/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/base_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/binge_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/default_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/download_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/history_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/mal_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/seasonal_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.842925 anipy_cli-2.7.9/anipy_cli/cli/menus/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/menus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/menus/base_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/menus/mal_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/menus/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/menus/seasonal_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15799 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/mal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.846925 anipy_cli-2.7.9/anipy_cli/player/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.846925 anipy_cli-2.7.9/anipy_cli/player/players/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/mpv.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/mpv_contrl.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/syncplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/vlc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/run_anipy_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/seasonal.py
--rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/url_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.842925 anipy_cli-2.7.9/anipy_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 20:43:57.846925 anipy_cli-2.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/setup.py
+-rw-r--r--   0        0        0     1974 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/README.md
+-rw-r--r--   0        0        0      865 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0       53 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/__init__.py
+-rw-r--r--   0        0        0     5299 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/arg_parser.py
+-rw-r--r--   0        0        0     1922 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/cli.py
+-rw-r--r--   0        0        0      411 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/clis/__init__.py
+-rw-r--r--   0        0        0      609 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/clis/base_cli.py
+-rw-r--r--   0        0        0     2281 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/clis/binge_cli.py
+-rw-r--r--   0        0        0     2815 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/clis/default_cli.py
+-rw-r--r--   0        0        0     3197 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/clis/download_cli.py
+-rw-r--r--   0        0        0     2676 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/clis/history_cli.py
+-rw-r--r--   0        0        0     2260 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/clis/mal_cli.py
+-rw-r--r--   0        0        0      616 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/clis/seasonal_cli.py
+-rw-r--r--   0        0        0      916 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/colors.py
+-rw-r--r--   0        0        0    15404 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/config.py
+-rw-r--r--   0        0        0     1134 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/discord.py
+-rw-r--r--   0        0        0     6981 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/mal_proxy.py
+-rw-r--r--   0        0        0      185 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/menus/__init__.py
+-rw-r--r--   0        0        0     1140 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/menus/base_menu.py
+-rw-r--r--   0        0        0    24091 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/menus/mal_menu.py
+-rw-r--r--   0        0        0     6179 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/menus/menu.py
+-rw-r--r--   0        0        0     9097 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/menus/seasonal_menu.py
+-rw-r--r--   0        0        0     6989 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/prompts.py
+-rw-r--r--   0        0        0     7700 2024-05-11 00:42:50.177161 anipy_cli-3.0.0.dev0/src/anipy_cli/util.py
+-rw-r--r--   0        0        0     3080 1970-01-01 00:00:00.000000 anipy_cli-3.0.0.dev0/PKG-INFO
```

### Comparing `anipy_cli-2.7.9/anipy_cli/arg_parser.py` & `anipy_cli-3.0.0.dev0/src/anipy_cli/arg_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import argparse
-from pathlib import Path
 from dataclasses import dataclass
-from typing import Union, Optional
-from anipy_cli.version import __version__
+from pathlib import Path
+from typing import Optional, Union
+
+from anipy_cli import __version__
 
 
 @dataclass(frozen=True)
 class CliArgs:
     download: bool
     binge: bool
     history: bool
     seasonal: bool
     mal: bool
     delete: bool
     quality: Optional[Union[str, int]]
     ffmpeg: bool
-    no_season_search: bool
     auto_update: bool
+    mal_sync_seasonals: bool
     optional_player: Optional[str]
+    search: Optional[str]
     location: Optional[Path]
     mal_password: Optional[str]
     config: bool
 
 
-def parse_args() -> CliArgs:
+def parse_args(override_args: Optional[list[str]] = None) -> CliArgs:
     parser = argparse.ArgumentParser(
-        description="Play Animes from gogoanime in local video-player or Download them.",
+        description="Play Animes from online anime providers locally or download them, and much more.",
         add_help=False,
     )
 
     # Workaround, so the Mutally Exclusive group can have a custom title+description
     actions_group = parser.add_argument_group(
         "Actions", "Different Actions and Modes of anipy-cli (only pick one)"
     )
@@ -93,55 +95,55 @@
         required=False,
         dest="delete",
         action="store_true",
         help="Delete your History.",
     )
 
     options_group.add_argument(
+        "-s",
+        "--search",
+        required=False,
+        dest="search",
+        action="store",
+        help="Provide a search term to the Download or Binge mode in this format: {query}:{episode range}:{dub/sub}. Examples: 'frieren:1-10:sub' or 'frieren:1:sub' or 'frieren:1-3 7-12:dub'",
+    )
+
+    options_group.add_argument(
         "-q",
         "--quality",
         action="store",
         required=False,
-        default="auto",
+        default="best",
+        type=lambda v: int(v) if v.isdigit() else v,
         help="Change the quality of the video, accepts: best, worst or 360, 480, 720 etc.  Default: best",
     )
 
     options_group.add_argument(
         "-f",
         "--ffmpeg",
         required=False,
         dest="ffmpeg",
         action="store_true",
         help="Use ffmpeg to download m3u8 playlists, may be more stable but is way slower than internal downloader",
     )
 
     options_group.add_argument(
-        "-o",
-        "--no-seas-search",
-        required=False,
-        dest="no_season_search",
-        action="store_true",
-        help="Turn off search in season. "
-        "Disables prompting if GoGoAnime is to be searched for anime in specific season.",
-    )
-
-    options_group.add_argument(
         "-a",
         "--auto-update",
         required=False,
         dest="auto_update",
         action="store_true",
-        help="Automatically update and download all Anime in seasonals list from start EP to newest.",
+        help="Automatically update and download all Anime in seasonals or mal mode from start EP to newest.",
     )
 
     options_group.add_argument(
         "-p",
         "--optional-player",
         required=False,
-        choices=["mpv", "vlc", "syncplay", "mpvnet"],
+        choices=["mpv", "vlc", "syncplay", "mpvnet", "mpv-controlled"],
         help="Override the player set in the config.",
     )
 
     options_group.add_argument(
         "-l",
         "--location",
         required=False,
@@ -156,22 +158,30 @@
         "--mal-password",
         required=False,
         dest="mal_password",
         action="store",
         help="Provide password for MAL login (overrides password set in config)",
     )
 
+    options_group.add_argument(
+        "--mal-sync-to-seasonals",
+        required=False,
+        dest="mal_sync_seasonals",
+        action="store_true",
+        help="Automatically sync myanimelist to seasonals (only works with `-M`)",
+    )
+
     info_group.add_argument(
         "-h", "--help", action="help", help="show this help message and exit"
     )
 
     info_group.add_argument("-v", "--version", action="version", version=__version__)
 
     info_group.add_argument(
         "--config-path",
         required=False,
         dest="config",
         action="store_true",
         help="Print path to the config file.",
     )
 
-    return CliArgs(**vars(parser.parse_args()))
+    return CliArgs(**vars(parser.parse_args(args=override_args)))
```

### Comparing `anipy_cli-2.7.9/anipy_cli/cli/clis/mal_cli.py` & `anipy_cli-3.0.0.dev0/src/anipy_cli/clis/seasonal_cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-from anipy_cli.arg_parser import CliArgs
-from anipy_cli.cli.menus import MALMenu
-from anipy_cli.cli.clis.base_cli import CliBase
+from typing import TYPE_CHECKING
+from anipy_cli.menus import SeasonalMenu
+from anipy_cli.clis.base_cli import CliBase
 
+if TYPE_CHECKING:
+    from anipy_cli.arg_parser import CliArgs
 
-class MalCli(CliBase):
-    def __init__(self, options: CliArgs, rpc_client=None):
-        super().__init__(options, rpc_client)
+
+class SeasonalCli(CliBase):
+    def __init__(self, options: "CliArgs"):
+        super().__init__(options)
 
     def print_header(self):
         pass
 
     def take_input(self):
         pass
 
     def process(self):
         pass
 
     def show(self):
         pass
 
     def post(self):
-        menu = MALMenu(options=self.options, rpc_client=self.rpc_client)
+        menu = SeasonalMenu(self.options)
+
         if self.options.auto_update:
-            menu.download(mode="all")
+            menu.download_latest()
         else:
             menu.run()
```

### Comparing `anipy_cli-2.7.9/anipy_cli/cli/menus/base_menu.py` & `anipy_cli-3.0.0.dev0/src/anipy_cli/menus/base_menu.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import sys
+import os
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Callable, List
-from abc import ABC, abstractmethod
 
-from anipy_cli.misc import error, clear_console
-from anipy_cli.colors import colors, color
+from anipy_cli.colors import color, colors
+from anipy_cli.util import error
 
 
 @dataclass(frozen=True)
 class MenuOption:
     info: str
     callback: Callable
     trigger: str
@@ -16,20 +16,18 @@
     def __repr__(self):
         return color(colors.GREEN, f"[{self.trigger}] ") + self.info
 
 
 class MenuBase(ABC):
     @property
     @abstractmethod
-    def menu_options(self) -> List[MenuOption]:
-        pass
+    def menu_options(self) -> List[MenuOption]: ...
 
     @abstractmethod
-    def print_header(self):
-        pass
+    def print_header(self): ...
 
     def run(self):
         self.print_options()
         self.take_input()
 
     def take_input(self):
         while True:
@@ -40,14 +38,12 @@
                 error("invalid input")
                 continue
 
             op.callback()
 
     def print_options(self, clear_screen=True):
         if clear_screen:
-            clear_console()
+            os.system("cls" if os.name == "nt" else "clear")
+
         self.print_header()
         for op in self.menu_options:
             print(op)
-
-    def quit(self):
-        sys.exit()
```

### Comparing `anipy_cli-2.7.9/anipy_cli/colors.py` & `anipy_cli-3.0.0.dev0/src/anipy_cli/colors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 class colors:
-    """
-    Just a class for colors
-    """
+    """Just a class for colors."""
 
     GREEN = "\033[92m"
     ERROR = "\033[93m"
     BLUE = "\u001b[34m"
     YELLOW = "\u001b[33m"
     MAGENTA = "\u001b[35m"
     CYAN = "\u001b[36m"
     RED = "\u001b[31m"
     END = "\x1b[0m"
+    BOLD = "\033[1m"
+    UNDERLINE = "\033[4m"
+    RESET = "\033[0m"
 
 
 def color(*values, sep: str = "") -> str:
     """Decorate a string with color codes.
+
     Basically just ensures that the color doesn't "leak"
     from the text.
-    format: color(color1, text1, color2, text2...)"""
+    format: color(color1, text1, color2, text2...)
+    """
     return sep.join(map(str, values)) + colors.END
 
 
 def cinput(*prompt, input_color: str = "") -> str:
     """An input function that handles coloring input."""
     inp = input(color(*prompt) + input_color)
     print(colors.END, end="")
```

