# Comparing `tmp/chaiverse-1.9.8.tar.gz` & `tmp/chaiverse-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaiverse-1.9.8.tar", last modified: Thu Feb 22 18:58:02 2024, max compression
+gzip compressed data, was "chaiverse-1.9.9.tar", last modified: Thu Feb 22 20:00:30 2024, max compression
```

## Comparing `chaiverse-1.9.8.tar` & `chaiverse-1.9.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:58:02.720183 chaiverse-1.9.8/
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-22 18:57:52.000000 chaiverse-1.9.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4818 2024-02-22 18:58:02.720183 chaiverse-1.9.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4569 2024-02-22 18:57:52.000000 chaiverse-1.9.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      681 2024-02-22 18:57:52.000000 chaiverse-1.9.8/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:58:02.719183 chaiverse-1.9.8/chaiverse.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4818 2024-02-22 18:58:02.000000 chaiverse-1.9.8/chaiverse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1294 2024-02-22 18:58:02.000000 chaiverse-1.9.8/chaiverse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 18:58:02.000000 chaiverse-1.9.8/chaiverse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-02-22 18:58:02.000000 chaiverse-1.9.8/chaiverse.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 18:58:02.000000 chaiverse-1.9.8/chaiverse.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       71 2024-02-22 18:58:02.000000 chaiverse-1.9.8/chaiverse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-22 18:58:02.000000 chaiverse-1.9.8/chaiverse.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5961 2024-02-22 18:57:52.000000 chaiverse-1.9.8/chat.py
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-02-22 18:57:52.000000 chaiverse-1.9.8/competition_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-22 18:57:52.000000 chaiverse-1.9.8/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3387 2024-02-22 18:57:52.000000 chaiverse-1.9.8/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4526 2024-02-22 18:57:52.000000 chaiverse-1.9.8/feedback.py
--rw-rw-rw-   0 root         (0) root         (0)     2215 2024-02-22 18:57:52.000000 chaiverse-1.9.8/formatters.py
--rw-rw-rw-   0 root         (0) root         (0)     2296 2024-02-22 18:57:52.000000 chaiverse-1.9.8/http_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:58:02.713183 chaiverse-1.9.8/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 18:57:53.000000 chaiverse-1.9.8/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-02-22 18:57:52.000000 chaiverse-1.9.8/lib/binomial_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2024-02-22 18:57:52.000000 chaiverse-1.9.8/lib/date_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2024-02-22 18:57:52.000000 chaiverse-1.9.8/login_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:58:02.715183 chaiverse-1.9.8/metrics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 18:57:53.000000 chaiverse-1.9.8/metrics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2024-02-22 18:57:52.000000 chaiverse-1.9.8/metrics/conversation_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3374 2024-02-22 18:57:52.000000 chaiverse-1.9.8/metrics/feedback_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2024-02-22 18:57:52.000000 chaiverse-1.9.8/metrics/leaderboard_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2024-02-22 18:57:52.000000 chaiverse-1.9.8/metrics/leaderboard_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2740 2024-02-22 18:57:52.000000 chaiverse-1.9.8/metrics/leaderboard_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-02-22 18:57:52.000000 chaiverse-1.9.8/metrics/submission_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-22 18:57:52.000000 chaiverse-1.9.8/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:58:02.709183 chaiverse-1.9.8/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:58:02.717183 chaiverse-1.9.8/resources/bot_config/
--rw-rw-rw-   0 root         (0) root         (0)     1332 2024-02-22 18:57:54.000000 chaiverse-1.9.8/resources/bot_config/blade.json
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-02-22 18:57:54.000000 chaiverse-1.9.8/resources/bot_config/captain_wyatt.json
--rw-rw-rw-   0 root         (0) root         (0)     2031 2024-02-22 18:57:53.000000 chaiverse-1.9.8/resources/bot_config/coffee_shop_girl.json
--rw-rw-rw-   0 root         (0) root         (0)     1305 2024-02-22 18:57:54.000000 chaiverse-1.9.8/resources/bot_config/filbert.json
--rw-rw-rw-   0 root         (0) root         (0)     1050 2024-02-22 18:57:54.000000 chaiverse-1.9.8/resources/bot_config/leo.json
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-02-22 18:57:54.000000 chaiverse-1.9.8/resources/bot_config/levi.json
--rw-rw-rw-   0 root         (0) root         (0)     1821 2024-02-22 18:57:53.000000 chaiverse-1.9.8/resources/bot_config/mr_wilson.json
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-02-22 18:57:54.000000 chaiverse-1.9.8/resources/bot_config/nerd_girl.json
--rw-rw-rw-   0 root         (0) root         (0)     2205 2024-02-22 18:57:53.000000 chaiverse-1.9.8/resources/bot_config/scaramouche.json
--rw-rw-rw-   0 root         (0) root         (0)     1386 2024-02-22 18:57:54.000000 chaiverse-1.9.8/resources/bot_config/story_teller.json
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-02-22 18:57:53.000000 chaiverse-1.9.8/resources/bot_config/vampire_queen.json
--rw-rw-rw-   0 root         (0) root         (0)     2246 2024-02-22 18:57:53.000000 chaiverse-1.9.8/resources/bot_config/wednesday_addams.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:58:02.718183 chaiverse-1.9.8/schemas/
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-02-22 18:57:52.000000 chaiverse-1.9.8/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2801 2024-02-22 18:57:52.000000 chaiverse-1.9.8/schemas/competition_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2024-02-22 18:57:52.000000 chaiverse-1.9.8/schemas/date_range_schema.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-22 18:58:02.720183 chaiverse-1.9.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1761 2024-02-22 18:57:52.000000 chaiverse-1.9.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     7883 2024-02-22 18:57:52.000000 chaiverse-1.9.8/submit.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-22 18:57:52.000000 chaiverse-1.9.8/test_requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     5230 2024-02-22 18:57:52.000000 chaiverse-1.9.8/utils.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-22 18:57:55.000000 chaiverse-1.9.8/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 20:00:30.418048 chaiverse-1.9.9/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-22 20:00:20.000000 chaiverse-1.9.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4818 2024-02-22 20:00:30.417048 chaiverse-1.9.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2024-02-22 20:00:20.000000 chaiverse-1.9.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      681 2024-02-22 20:00:20.000000 chaiverse-1.9.9/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 20:00:30.417048 chaiverse-1.9.9/chaiverse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4818 2024-02-22 20:00:30.000000 chaiverse-1.9.9/chaiverse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-02-22 20:00:30.000000 chaiverse-1.9.9/chaiverse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 20:00:30.000000 chaiverse-1.9.9/chaiverse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-02-22 20:00:30.000000 chaiverse-1.9.9/chaiverse.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 20:00:30.000000 chaiverse-1.9.9/chaiverse.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       71 2024-02-22 20:00:30.000000 chaiverse-1.9.9/chaiverse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-02-22 20:00:30.000000 chaiverse-1.9.9/chaiverse.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5965 2024-02-22 20:00:20.000000 chaiverse-1.9.9/chat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2024-02-22 20:00:20.000000 chaiverse-1.9.9/competition_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-22 20:00:20.000000 chaiverse-1.9.9/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3387 2024-02-22 20:00:20.000000 chaiverse-1.9.9/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2024-02-22 20:00:20.000000 chaiverse-1.9.9/feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)     2215 2024-02-22 20:00:20.000000 chaiverse-1.9.9/formatters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2296 2024-02-22 20:00:20.000000 chaiverse-1.9.9/http_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 20:00:30.412048 chaiverse-1.9.9/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 20:00:20.000000 chaiverse-1.9.9/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-02-22 20:00:20.000000 chaiverse-1.9.9/lib/binomial_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2024-02-22 20:00:20.000000 chaiverse-1.9.9/lib/date_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2024-02-22 20:00:20.000000 chaiverse-1.9.9/login_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 20:00:30.413048 chaiverse-1.9.9/metrics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 20:00:20.000000 chaiverse-1.9.9/metrics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2024-02-22 20:00:20.000000 chaiverse-1.9.9/metrics/conversation_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3374 2024-02-22 20:00:20.000000 chaiverse-1.9.9/metrics/feedback_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2024-02-22 20:00:20.000000 chaiverse-1.9.9/metrics/leaderboard_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2024-02-22 20:00:20.000000 chaiverse-1.9.9/metrics/leaderboard_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2024-02-22 20:00:20.000000 chaiverse-1.9.9/metrics/leaderboard_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-02-22 20:00:20.000000 chaiverse-1.9.9/metrics/submission_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-22 20:00:20.000000 chaiverse-1.9.9/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 20:00:30.408048 chaiverse-1.9.9/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 20:00:30.415048 chaiverse-1.9.9/resources/bot_config/
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/blade.json
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/captain_wyatt.json
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/coffee_shop_girl.json
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/filbert.json
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/leo.json
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/levi.json
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/mr_wilson.json
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/nerd_girl.json
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/scaramouche.json
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/story_teller.json
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/vampire_queen.json
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2024-02-22 20:00:21.000000 chaiverse-1.9.9/resources/bot_config/wednesday_addams.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 20:00:30.416048 chaiverse-1.9.9/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-02-22 20:00:20.000000 chaiverse-1.9.9/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2801 2024-02-22 20:00:20.000000 chaiverse-1.9.9/schemas/competition_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2024-02-22 20:00:20.000000 chaiverse-1.9.9/schemas/date_range_schema.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-22 20:00:30.418048 chaiverse-1.9.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2024-02-22 20:00:20.000000 chaiverse-1.9.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     7883 2024-02-22 20:00:20.000000 chaiverse-1.9.9/submit.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-22 20:00:20.000000 chaiverse-1.9.9/test_requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5230 2024-02-22 20:00:20.000000 chaiverse-1.9.9/utils.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-02-22 20:00:22.000000 chaiverse-1.9.9/version.txt
```

### Comparing `chaiverse-1.9.8/PKG-INFO` & `chaiverse-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaiverse
-Version: 1.9.8
+Version: 1.9.9
 Summary: Chaiverse
 Home-page: https://www.chaiverse.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chaiverse-1.9.8/README.md` & `chaiverse-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/__init__.py` & `chaiverse-1.9.9/__init__.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/chaiverse.egg-info/PKG-INFO` & `chaiverse-1.9.9/chaiverse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaiverse
-Version: 1.9.8
+Version: 1.9.9
 Summary: Chaiverse
 Home-page: https://www.chaiverse.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chaiverse-1.9.8/chaiverse.egg-info/SOURCES.txt` & `chaiverse-1.9.9/chaiverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/chat.py` & `chaiverse-1.9.9/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,16 +69,16 @@
 
     def _print_greetings_header(self, bot_config):
         print_color(f'\nChatting with {bot_config.bot_label}, reply "exit" to quit.\n', 'yellow')
         print_color(f'{bot_config.bot_label}: {bot_config.first_message}', 'green')
 
     def _print_bot_response(self, bot_config, response, show_model_input):
         bot_response = response['model_output']
-        model_input = response['model_input']
         if show_model_input:
+            model_input = response['model_input']
             print_color('<Begin model input>', 'yellow')
             print_color(model_input, 'cyan')
             print_color('<End model input>', 'yellow')
         print_color(f"{bot_config.bot_label}: {bot_response}", 'green')
 
 
 @dataclass
```

### Comparing `chaiverse-1.9.8/competition_cli.py` & `chaiverse-1.9.9/competition_cli.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/config.py` & `chaiverse-1.9.9/config.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/constants.py` & `chaiverse-1.9.9/constants.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/feedback.py` & `chaiverse-1.9.9/feedback.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/formatters.py` & `chaiverse-1.9.9/formatters.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/http_client.py` & `chaiverse-1.9.9/http_client.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/lib/date_tools.py` & `chaiverse-1.9.9/lib/date_tools.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/login_cli.py` & `chaiverse-1.9.9/login_cli.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/metrics/conversation_metrics.py` & `chaiverse-1.9.9/metrics/conversation_metrics.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/metrics/feedback_metrics.py` & `chaiverse-1.9.9/metrics/feedback_metrics.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/metrics/leaderboard_api.py` & `chaiverse-1.9.9/metrics/leaderboard_api.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/metrics/leaderboard_cli.py` & `chaiverse-1.9.9/metrics/leaderboard_cli.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/metrics/leaderboard_formatter.py` & `chaiverse-1.9.9/metrics/leaderboard_formatter.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/metrics/submission_metrics.py` & `chaiverse-1.9.9/metrics/submission_metrics.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/blade.json` & `chaiverse-1.9.9/resources/bot_config/blade.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/captain_wyatt.json` & `chaiverse-1.9.9/resources/bot_config/captain_wyatt.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/coffee_shop_girl.json` & `chaiverse-1.9.9/resources/bot_config/coffee_shop_girl.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/filbert.json` & `chaiverse-1.9.9/resources/bot_config/filbert.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/leo.json` & `chaiverse-1.9.9/resources/bot_config/leo.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/levi.json` & `chaiverse-1.9.9/resources/bot_config/levi.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/mr_wilson.json` & `chaiverse-1.9.9/resources/bot_config/mr_wilson.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/nerd_girl.json` & `chaiverse-1.9.9/resources/bot_config/nerd_girl.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/scaramouche.json` & `chaiverse-1.9.9/resources/bot_config/scaramouche.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/story_teller.json` & `chaiverse-1.9.9/resources/bot_config/story_teller.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/vampire_queen.json` & `chaiverse-1.9.9/resources/bot_config/vampire_queen.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/resources/bot_config/wednesday_addams.json` & `chaiverse-1.9.9/resources/bot_config/wednesday_addams.json`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/schemas/competition_schema.py` & `chaiverse-1.9.9/schemas/competition_schema.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/schemas/date_range_schema.py` & `chaiverse-1.9.9/schemas/date_range_schema.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/setup.py` & `chaiverse-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/submit.py` & `chaiverse-1.9.9/submit.py`

 * *Files identical despite different names*

### Comparing `chaiverse-1.9.8/utils.py` & `chaiverse-1.9.9/utils.py`

 * *Files identical despite different names*

