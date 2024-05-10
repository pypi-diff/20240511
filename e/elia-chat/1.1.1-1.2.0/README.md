# Comparing `tmp/elia_chat-1.1.1.tar.gz` & `tmp/elia_chat-1.2.0.tar.gz`

## Comparing `elia_chat-1.1.1.tar` & `elia_chat-1.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.1.1/.python-version
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 elia_chat-1.1.1/requirements-dev.lock
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 elia_chat-1.1.1/requirements.lock
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.1.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/__init__.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/__main__.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/app.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/chats_manager.py
--rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/config.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/constants.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/elia.scss
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/launch_args.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/locations.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/models.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/runtime_config.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/time_display.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/database/__init__.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/database/converters.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/database/database.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/database/import_chatgpt.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/database/models.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/screens/chat_details.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/screens/chat_screen.py
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/screens/help_screen.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/screens/home_screen.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/widgets/agent_is_typing.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/widgets/app_header.py
--rw-r--r--   0        0        0    10891 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/widgets/chat.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/widgets/chat_header.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/widgets/chat_list.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/widgets/chat_options.py
--rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/widgets/chatbox.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/widgets/prompt_input.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.1.1/elia_chat/widgets/token_analysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.1.1/.gitignore
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 elia_chat-1.1.1/README.md
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 elia_chat-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 elia_chat-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.2.0/.python-version
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 elia_chat-1.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 elia_chat-1.2.0/requirements.lock
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/__init__.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/__main__.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/app.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/chats_manager.py
+-rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/config.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/constants.py
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/elia.scss
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/launch_args.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/locations.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/models.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/runtime_config.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/time_display.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/database/__init__.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/database/converters.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/database/database.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/database/import_chatgpt.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/database/models.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/screens/chat_details.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/screens/chat_screen.py
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/screens/help_screen.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/screens/home_screen.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/agent_is_typing.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/app_header.py
+-rw-r--r--   0        0        0    10891 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/chat.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/chat_header.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/chat_list.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/chat_options.py
+-rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/chatbox.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/prompt_input.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/token_analysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.2.0/.gitignore
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 elia_chat-1.2.0/README.md
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 elia_chat-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 elia_chat-1.2.0/PKG-INFO
```

### Comparing `elia_chat-1.1.1/.pre-commit-config.yaml` & `elia_chat-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/requirements-dev.lock` & `elia_chat-1.2.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/requirements.lock` & `elia_chat-1.2.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/__main__.py` & `elia_chat-1.2.0/elia_chat/__main__.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/app.py` & `elia_chat-1.2.0/elia_chat/app.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/chats_manager.py` & `elia_chat-1.2.0/elia_chat/chats_manager.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/config.py` & `elia_chat-1.2.0/elia_chat/config.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/elia.scss` & `elia_chat-1.2.0/elia_chat/elia.scss`

 * *Files 8% similar despite different names*

```diff
@@ -48,18 +48,28 @@
     margin: 0 0;
   }
 }
 
 Toast {
   background: $background-darken-1;
   border-right: none;
-}
+  &.-information {
+    border-left: outer $main-lighten-1;
+    & .toast--title {
+      color: $main-lighten-2;
+    }
+  }
+
+  &.-error {
+    border-left: outer $main-lighten-1;
+    & .toast--title {
+      color: $main-lighten-2;
+    }
+  }
 
-Toast.information {
-  border-left: outer $main-lighten-1;
 }
 
 
 Chat {
   ChatHeader {
     width: 100%;
     height: auto;
```

### Comparing `elia_chat-1.1.1/elia_chat/locations.py` & `elia_chat-1.2.0/elia_chat/locations.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/models.py` & `elia_chat-1.2.0/elia_chat/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/time_display.py` & `elia_chat-1.2.0/elia_chat/time_display.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/database/converters.py` & `elia_chat-1.2.0/elia_chat/database/converters.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/database/database.py` & `elia_chat-1.2.0/elia_chat/database/database.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/database/import_chatgpt.py` & `elia_chat-1.2.0/elia_chat/database/import_chatgpt.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/database/models.py` & `elia_chat-1.2.0/elia_chat/database/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/screens/chat_details.py` & `elia_chat-1.2.0/elia_chat/screens/chat_details.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/screens/chat_screen.py` & `elia_chat-1.2.0/elia_chat/screens/chat_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/screens/help_screen.py` & `elia_chat-1.2.0/elia_chat/screens/help_screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,25 @@
 You may need to set some environment variables, depending on the model
 you wish to set.
 To use OpenAI models, the `OPENAI_API_KEY` env var must be set.
 To use Anthropic models, the `ANTHROPIC_API_KEY` env var must be set.
 
 To use a local model, see the instructions in the README:
 
-* https://github.com/darrenburns/elia/blob/master/README.md
+* https://github.com/darrenburns/elia/blob/main/README.md
 
 ### Config file and database
 
 The locations of the config file and the database can be found at the bottom
 of the options screen (`ctrl+o`).
 
 ### General navigation
 
+Elia has very strong mouse support. Most things can be clicked.
+
 Use `tab` and `shift+tab` to move between different widgets on screen.
 
 In some places you can make use of the arrow keys or Vim nav keys to move around.
 
 In general, pressing `esc` will move you "closer to home".
 Pay attention to the bar at the bottom to see where `esc` will take you.
 
@@ -127,14 +129,15 @@
 - `y,c`: Copy the raw Markdown of the message to the clipboard.
     - This requires terminal support. The default MacOS terminal is not supported.
 - `enter`: Enter _select mode_.
     - In this mode, you can move a cursor through the text, optionally holding
         `shift` to select text as you move.
     - Press `v` to toggle _visual mode_, allowing you to select without text without
         needing to hold `shift`.
+    - Press `u` to quickly select the next code block in the message.
     - With some text selected, press `y` or c` to copy.
 - `enter`: View more details about a message.
     - The amount of details available may vary depending on the model
         or provider being used.
 - `g`: Focus the first message.
 - `G`: Focus the latest message.
 - `m`: Move focus to the prompt box.
```

### Comparing `elia_chat-1.1.1/elia_chat/screens/home_screen.py` & `elia_chat-1.2.0/elia_chat/screens/home_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/widgets/app_header.py` & `elia_chat-1.2.0/elia_chat/widgets/app_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/widgets/chat.py` & `elia_chat-1.2.0/elia_chat/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/widgets/chat_header.py` & `elia_chat-1.2.0/elia_chat/widgets/chat_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/widgets/chat_list.py` & `elia_chat-1.2.0/elia_chat/widgets/chat_list.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/widgets/chat_options.py` & `elia_chat-1.2.0/elia_chat/widgets/chat_options.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/widgets/chatbox.py` & `elia_chat-1.2.0/elia_chat/widgets/chatbox.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 from __future__ import annotations
+import bisect
 from dataclasses import dataclass
 
 from rich.console import RenderableType
 from rich.markdown import Markdown
 from rich.syntax import Syntax
 from textual import on
 from textual.binding import Binding
 from textual.css.query import NoMatches
 from textual.geometry import Size
 from textual.message import Message
 from textual.reactive import reactive
 from textual.widget import Widget
 from textual.widgets import TextArea
 from textual.widgets.text_area import Selection
+from textual.document._syntax_aware_document import SyntaxAwareDocumentError
 
 from elia_chat.config import EliaChatModel
 from elia_chat.models import ChatMessage
 
 
 class SelectionTextArea(TextArea):
-    @dataclass
     class LeaveSelectionMode(Message):
-        pass
+        """Broadcast that the user wants to leave selection mode."""
+
+    @dataclass
+    class VisualModeToggled(Message):
+        """Sent when we enter/leave visual select mode."""
+
+        enabled: bool
 
     BINDINGS = [
         Binding(
             "escape",
             "leave_selection_mode",
             description="Exit selection mode",
             key_display="esc",
@@ -35,29 +42,30 @@
             "toggle_visual_mode",
             description="Toggle visual select",
             key_display="v",
         ),
         Binding(
             "y,c", "copy_to_clipboard", description="Copy selection", key_display="y"
         ),
+        Binding("u", "next_code_block", description="Next code block", key_display="u"),
     ]
 
     visual_mode = reactive(False, init=False)
 
     def action_toggle_visual_mode(self) -> None:
         self.visual_mode = not self.visual_mode
 
     def watch_visual_mode(self, value: bool) -> None:
+        self.post_message(self.VisualModeToggled(value))
         self.cursor_blink = not value
 
         if not value:
             self.selection = Selection.cursor(self.selection.end)
 
         self.set_class(value, "visual-mode")
-        print(self.classes)
 
     def action_cursor_up(self, select: bool = False) -> None:
         return super().action_cursor_up(self.visual_mode or select)
 
     def action_cursor_right(self, select: bool = False) -> None:
         return super().action_cursor_right(self.visual_mode or select)
 
@@ -88,14 +96,42 @@
             text_to_copy = self.text
             message = f"Copied message ({len(text_to_copy)} characters)."
             self.notify(message, title="Message copied")
 
         self.app.copy_to_clipboard(text_to_copy)
         self.visual_mode = False
 
+    def action_next_code_block(self) -> None:
+        try:
+            query = self.document.prepare_query(
+                "(fenced_code_block (code_fence_content) @code_block)"
+            )
+        except SyntaxAwareDocumentError:
+            self.app.notify(
+                "This feature requires tree-sitter, which isn't installed.",
+                severity="error",
+            )
+        else:
+            if query:
+                self.visual_mode = True
+                code_block_nodes = self.document.query_syntax_tree(query)
+                locations: list[tuple[tuple[int, int], tuple[int, int]]] = [
+                    (node.start_point, node.end_point)
+                    for (node, _name) in code_block_nodes
+                ]
+                end_locations = [end for _start, end in locations]
+                cursor_row, _cursor_column = self.cursor_location
+                search_start_location = cursor_row + 1, 0
+                insertion_index = bisect.bisect_left(
+                    end_locations, search_start_location
+                )
+                insertion_index %= len(end_locations)
+                start, end = locations[insertion_index]
+                self.selection = Selection(start, end)
+
     def action_leave_selection_mode(self) -> None:
         self.post_message(self.LeaveSelectionMode())
 
 
 class Chatbox(Widget, can_focus=True):
     BINDINGS = [
         Binding(key="up,k", action="up", description="Up", show=False),
@@ -165,15 +201,15 @@
             else:
                 message = "Unable to copy message"
                 self.notify(message, title="Clipboard error", severity="error")
 
     async def watch_selection_mode(self, value: bool) -> None:
         if value:
             async with self.batch():
-                self.border_subtitle = "[[white]c[/]] Copy selection"
+                self.border_subtitle = "SELECT"
                 content = self.message.message.get("content")
                 text_area = SelectionTextArea(
                     content if isinstance(content, str) else "",
                     read_only=True,
                     language="markdown",
                     classes="selection-mode",
                 )
@@ -200,14 +236,20 @@
             try:
                 child = self.query_one(SelectionTextArea)
             except NoMatches:
                 return None
             else:
                 child.focus()
 
+    @on(SelectionTextArea.VisualModeToggled)
+    def handle_visual_select(self, event: SelectionTextArea.VisualModeToggled) -> None:
+        self.border_subtitle = (
+            "[reverse] VISUAL SELECT [/]" if event.enabled else "SELECT"
+        )
+
     @property
     def markdown(self) -> Markdown:
         """Return the content as a Rich Markdown object."""
         content = self.message.message.get("content")
         if not isinstance(content, str):
             content = ""
         return Markdown(content)
```

### Comparing `elia_chat-1.1.1/elia_chat/widgets/prompt_input.py` & `elia_chat-1.2.0/elia_chat/widgets/prompt_input.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/elia_chat/widgets/token_analysis.py` & `elia_chat-1.2.0/elia_chat/widgets/token_analysis.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/.gitignore` & `elia_chat-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elia_chat-1.1.1/README.md` & `elia_chat-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 # only the `name` field is required here.
 [[models]]
 name = "ollama/llama3"
 
 # example of a model running on a local server, e.g. LocalAI
 [[models]]
 name = "openai/some-model"
-api_base = "http://localhost:8080/v1/chat/completions"
+api_base = "http://localhost:8080/v1"
 api_key = "api-key-if-required"
 
 # example of add a groq model, showing some other fields
 [[models]]
 name = "groq/llama2-70b-4096"
 display_name = "Llama 2 70B"  # appears in UI
 provider = "Groq"  # appears in UI
@@ -82,15 +82,15 @@
 name = "gpt-3.5-turbo"
 display_name = "GPT 3.5 Turbo (Work)"
 
 [[models]]
 id = "personal-gpt-3.5-turbo"
 name = "gpt-3.5-turbo"
 display_name = "GPT 3.5 Turbo (Personal)"
-
+```
 
 ### Import from ChatGPT
 
 Export your conversations to a JSON file using the ChatGPT UI, then import them using the `import` command.
 
 ```bash
 elia import 'path/to/conversations.json'
```

### Comparing `elia_chat-1.1.1/pyproject.toml` & `elia_chat-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "elia_chat"
-version = "1.1.1"
+version = "1.2.0"
 description = "A powerful terminal user interface for interacting with large language models."
 authors = [
     { name = "Darren Burns", email = "darrenb900@gmail.com" }
 ]
 dependencies = [
     "textual[syntax]==0.58.1",
     "sqlmodel>=0.0.9",
```

### Comparing `elia_chat-1.1.1/PKG-INFO` & `elia_chat-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: elia_chat
-Version: 1.1.1
+Version: 1.2.0
 Summary: A powerful terminal user interface for interacting with large language models.
 Author-email: Darren Burns <darrenb900@gmail.com>
 Requires-Python: >=3.11
 Requires-Dist: aiosqlite>=0.20.0
 Requires-Dist: click-default-group>=1.2.4
 Requires-Dist: click>=8.1.6
 Requires-Dist: greenlet>=3.0.3
@@ -78,15 +78,15 @@
 # only the `name` field is required here.
 [[models]]
 name = "ollama/llama3"
 
 # example of a model running on a local server, e.g. LocalAI
 [[models]]
 name = "openai/some-model"
-api_base = "http://localhost:8080/v1/chat/completions"
+api_base = "http://localhost:8080/v1"
 api_key = "api-key-if-required"
 
 # example of add a groq model, showing some other fields
 [[models]]
 name = "groq/llama2-70b-4096"
 display_name = "Llama 2 70B"  # appears in UI
 provider = "Groq"  # appears in UI
@@ -100,15 +100,15 @@
 name = "gpt-3.5-turbo"
 display_name = "GPT 3.5 Turbo (Work)"
 
 [[models]]
 id = "personal-gpt-3.5-turbo"
 name = "gpt-3.5-turbo"
 display_name = "GPT 3.5 Turbo (Personal)"
-
+```
 
 ### Import from ChatGPT
 
 Export your conversations to a JSON file using the ChatGPT UI, then import them using the `import` command.
 
 ```bash
 elia import 'path/to/conversations.json'
```

