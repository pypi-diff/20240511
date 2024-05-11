# Comparing `tmp/devon_agent-0.1.0.tar.gz` & `tmp/devon_agent-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devon_agent-0.1.0.tar", max compression
+gzip compressed data, was "devon_agent-0.1.1.tar", max compression
```

## Comparing `devon_agent-0.1.0.tar` & `devon_agent-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.1.0/LICENSE
--rw-r--r--   0        0        0     1463 2024-04-08 19:20:30.592278 devon_agent-0.1.0/README.md
--rw-r--r--   0        0        0      129 2024-05-08 17:03:00.214056 devon_agent-0.1.0/devon_agent/TODO
--rw-r--r--   0        0        0      768 2024-05-10 06:57:09.595864 devon_agent-0.1.0/devon_agent/__main__.py
--rw-r--r--   0        0        0     9669 2024-05-09 00:32:05.731574 devon_agent-0.1.0/devon_agent/agent.py
--rw-r--r--   0        0        0     2514 2024-05-10 05:23:48.883645 devon_agent-0.1.0/devon_agent/environment.py
--rw-r--r--   0        0        0     2196 2024-05-08 19:10:42.793826 devon_agent-0.1.0/devon_agent/model.py
--rw-r--r--   0        0        0    19895 2024-05-08 17:01:35.524177 devon_agent-0.1.0/devon_agent/prompt.py
--rw-r--r--   0        0        0     8161 2024-05-08 19:30:12.992344 devon_agent-0.1.0/devon_agent/server.py
--rw-r--r--   0        0        0    13910 2024-05-10 05:26:03.426818 devon_agent-0.1.0/devon_agent/session.py
--rw-r--r--   0        0        0      898 2024-05-08 17:28:06.948322 devon_agent-0.1.0/devon_agent/test/test_tools.py
--rw-r--r--   0        0        0    42372 2024-05-10 05:38:04.631959 devon_agent-0.1.0/devon_agent/tools.py
--rw-r--r--   0        0        0    29332 2024-05-08 18:15:48.650465 devon_agent-0.1.0/devon_agent/udiff.py
--rw-r--r--   0        0        0      727 2024-05-08 18:15:29.478903 devon_agent-0.1.0/devon_agent/utils.py
--rw-r--r--   0        0        0     1509 2024-05-08 18:15:29.478838 devon_agent-0.1.0/devon_agent/vgit.py
--rw-r--r--   0        0        0     1109 2024-05-10 07:33:38.576397 devon_agent-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 devon_agent-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1463 2024-04-08 19:20:30.592278 devon_agent-0.1.1/README.md
+-rw-r--r--   0        0        0      129 2024-05-10 17:13:36.831768 devon_agent-0.1.1/devon_agent/TODO
+-rw-r--r--   0        0        0      794 2024-05-10 17:13:36.832076 devon_agent-0.1.1/devon_agent/__main__.py
+-rw-r--r--   0        0        0     9751 2024-05-10 17:13:36.832377 devon_agent-0.1.1/devon_agent/agent.py
+-rw-r--r--   0        0        0     2512 2024-05-10 17:13:36.832634 devon_agent-0.1.1/devon_agent/environment.py
+-rw-r--r--   0        0        0     2195 2024-05-10 17:13:36.832781 devon_agent-0.1.1/devon_agent/model.py
+-rw-r--r--   0        0        0    19947 2024-05-10 17:13:36.833052 devon_agent-0.1.1/devon_agent/prompt.py
+-rw-r--r--   0        0        0     6312 2024-05-11 00:03:38.899715 devon_agent-0.1.1/devon_agent/server.py
+-rw-r--r--   0        0        0    14732 2024-05-11 00:03:38.900376 devon_agent-0.1.1/devon_agent/session.py
+-rw-r--r--   0        0        0     4607 2024-05-11 00:03:38.900486 devon_agent-0.1.1/devon_agent/telemetry.py
+-rw-r--r--   0        0        0      898 2024-05-10 17:13:36.833911 devon_agent-0.1.1/devon_agent/test/test_tools.py
+-rw-r--r--   0        0        0    42575 2024-05-11 00:03:38.900960 devon_agent-0.1.1/devon_agent/tools.py
+-rw-r--r--   0        0        0    29381 2024-05-10 23:28:51.716909 devon_agent-0.1.1/devon_agent/udiff.py
+-rw-r--r--   0        0        0      727 2024-05-10 17:13:36.835159 devon_agent-0.1.1/devon_agent/utils.py
+-rw-r--r--   0        0        0     1509 2024-05-10 17:13:36.835377 devon_agent-0.1.1/devon_agent/vgit.py
+-rw-r--r--   0        0        0     1127 2024-05-11 00:26:40.396257 devon_agent-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 devon_agent-0.1.1/PKG-INFO
```

### Comparing `devon_agent-0.1.0/LICENSE` & `devon_agent-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.0/README.md` & `devon_agent-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.0/devon_agent/__main__.py` & `devon_agent-0.1.1/devon_agent/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-
-
-
 import os
 import click
 from devon_agent.server import app
+
+
 @click.group()
 def cli():
     """Devon Agent CLI application."""
     pass
 
 
 @click.command()
-@click.option('--port', default=8000, help='Port number for the server.')
-@click.option('--key', required=False,default=None, help='API key for authentication.')
+@click.option("--port", default=8000, help="Port number for the server.")
+@click.option("--key", required=False, default=None, help="API key for authentication.")
 def server(port, key):
     """Start the Devon Agent server."""
     import uvicorn
 
     import sys
 
     if key is None:
-        if not os.environ.get('ANTHROPIC_API_KEY'):
-            print("Please set the ANTHROPIC_API_KEY environment variable to use the Devon Agent.")
+        if not os.environ.get("ANTHROPIC_API_KEY"):
+            print(
+                "Please set the ANTHROPIC_API_KEY environment variable to use the Devon Agent."
+            )
             sys.exit(1)
-    else:    
-        os.environ['ANTHROPIC_API_KEY'] = key
+    else:
+        os.environ["ANTHROPIC_API_KEY"] = key
     uvicorn.run(app, host="0.0.0.0", port=port)
 
 
-
-
 cli.add_command(server)
 
+
 def main():
-    cli()
+    cli()
```

### Comparing `devon_agent-0.1.0/devon_agent/agent.py` & `devon_agent-0.1.1/devon_agent/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,19 @@
         session: "Session",
     ) -> Tuple[str, str, str]:
         if self.interrupt:
             observation = observation + ". also " + self.interrupt
             self.interrupt = ""
 
         self.current_model = AnthropicModel(
-            args=ModelArguments(model_name=self.model, temperature=self.temperature, api_key=self.api_key)
+            args=ModelArguments(
+                model_name=self.model,
+                temperature=self.temperature,
+                api_key=self.api_key,
+            )
         )
         try:
             editor = self._convert_editor_to_view(
                 session.state.editor, session.state.PAGE_SIZE
             )
 
             self.chat_history.append(
@@ -124,15 +128,15 @@
                 self.current_model.args.temperature += (
                     0.2 if self.current_model.args.temperature < 0.8 else 0
                 )
             else:
                 history = history_to_bash_history(self.chat_history)
 
             last_user_prompt = last_user_prompt_template_v3(
-                task, history, editor, session.environment.get_cwd()
+                task, history, editor, session.environment.get_cwd(), session.base_path
             )
 
             messages = [{"role": "user", "content": last_user_prompt}]
 
             output = self.current_model.query(messages, system_message=system_prompt)
 
             # logger.debug(
```

### Comparing `devon_agent-0.1.0/devon_agent/environment.py` & `devon_agent-0.1.1/devon_agent/environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,38 +8,37 @@
 from typing import Optional, Protocol
 
 
 @dataclass(frozen=False)
 class EnvironmentModule(Protocol):
     # tools : list[]
 
-    def setup(self,**kwargs): ...
+    def setup(self, **kwargs): ...
 
-    def teardown(self,**kwargs): ...
+    def teardown(self, **kwargs): ...
 
     def __enter__(self):
         self.setup()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
-        self.teardown( exc_type, exc_value, traceback)
+        self.teardown(exc_type, exc_value, traceback)
 
     def execute(self, input: str, timeout_duration=25): ...
-    
 
 
 @dataclass(frozen=False)
 class LocalEnvironment:
     path: str
 
-    def setup(self,**kwargs):
+    def setup(self, **kwargs):
         self.old_dir = os.getcwd()
         os.chdir(self.path)
 
-    def teardown(self,**kwargs):
+    def teardown(self, **kwargs):
         os.chdir(self.old_dir)
 
     def get_cwd(self):
         return self.execute("pwd")[0]
 
     def communicate(self, input: str, timeout_duration=25):
         return self.execute(input, timeout_duration=timeout_duration)
@@ -86,8 +85,8 @@
         return output, process.returncode
 
     def __enter__(self):
         self.setup()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
-        self.teardown( exc_type, exc_value, traceback)
+        self.teardown(exc_type, exc_value, traceback)
```

### Comparing `devon_agent-0.1.0/devon_agent/model.py` & `devon_agent-0.1.1/devon_agent/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,29 +47,27 @@
     }
 
     def __init__(self, args: ModelArguments):
         self.args = args
         self.api_model = self.SHORTCUTS.get(args.model_name, args.model_name)
         self.model_metadata = self.MODELS[self.api_model]
 
-
         if args.api_key is not None:
             self.api = Anthropic(api_key=args.api_key)
         else:
             self.api = Anthropic(api_key=os.getenv("ANTHROPIC_API_KEY"))
 
     def query(self, messages: list[dict[str, str]], system_message: str = "") -> str:
-
         response = (
             self.api.messages.create(
                 messages=messages,
                 max_tokens=self.model_metadata["max_tokens"],
                 model=self.api_model,
                 temperature=self.args.temperature,
                 system=system_message,
                 stop_sequences=["</COMMAND>"],
             )
             .content[0]
             .text
         )
 
-        return response + "</COMMAND>"
+        return response + "</COMMAND>"
```

### Comparing `devon_agent-0.1.0/devon_agent/prompt.py` & `devon_agent-0.1.1/devon_agent/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -418,56 +418,54 @@
 </SETTING>
 <EDITOR>
 Currently open files will be listed here. Close unused files. Use open files to understand code structure and flow.
 </EDITOR>
 <COMMANDS>
 {command_docs} 
 </COMMANDS>
-<RESPONSE FORMAT>
+<RESPONSE FORMAT>s
 Shell prompt format: <cwd> $
 Required fields for each response:
 <THOUGHT>
 Your reflection, planning, and justification goes here
 </THOUGHT>
 <COMMAND>
-A single executable command goes here
+A single executable command goes here, you also have access to all non-interactive bash commands
 </COMMAND>
 </RESPONSE FORMAT>
 """
 
 
-def last_user_prompt_template_v3(issue, history, editor, working_dir):
+def last_user_prompt_template_v3(issue, history, editor, cwd, root_dir):
     return f"""
-<SETTING> 
-Current task: <TASK>{issue}</TASK>
+<SETTING>
+
+Current objective: {issue}
 
 Instructions:
 
 Edit necessary files and run checks/tests
-Submit changes with 'submit' command when ready
+Submit changes with 'submit' command when you think the task has been completed
 Interactive session commands (e.g. python, vim) NOT supported
 Write and run scripts instead (e.g. 'python script.py')
 </SETTING>
 <CONSTRAINTS>
 - Execute ONLY ONE command at a time
 - Wait for feedback after each command
 - Avoid repeating failed commands, reconsider approach instead
 - Use files currently open in editor for information
 - Locate code elements with 'find_class' or 'find_function', not 'search'
 - 'no_op' command available to allow for more thinking time 
 - The title or first line of the issue describes the issue succintly
 </CONSTRAINTS>
 <RESPONSE FORMAT>
 <THOUGHT>
-
-**Am I overthinking?**
-Yes, I am overthinking, I should just make the change that fixes all cases of this type.
-
+Reflect on previous actions here. Feel free to use the no_op command if you need to think more.
 </THOUGHT>
-<COMMAND> 
+<COMMAND>
 Single executable command here
 </COMMAND>
 </RESPONSE FORMAT>
 <WORKSPACE>
 <EDITOR>
 {editor}
 </EDITOR>
@@ -475,18 +473,18 @@
 <HISTORY>
 {history}
 </HISTORY>
 <EDITING TIPS>
 - Use 'no_op' periodically to pause and think
 - Focus on matching the source lines precisely, to do this make sure you identify the desired source lines first
 - Always scroll to the lines you want to change
-- If making a one line change, only include that line
 - Only make one change at a time
 - When changing functions, always make sure to search for and update references
-- You only have access to code contained in {working_dir}
+- You only have access to code contained in {root_dir}
+- Your current working directory is {cwd}
 </EDITING TIPS>"""
 
 
 def parse_response(response):
     thought = response.split("<THOUGHT>")[1].split("</THOUGHT>")[0]
     action = response.split("<COMMAND>")[1].split("</COMMAND>")[0]
```

### Comparing `devon_agent-0.1.0/devon_agent/server.py` & `devon_agent-0.1.1/devon_agent/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,107 +10,41 @@
     Event,
     Session,
     SessionArguments,
 )
 from fastapi.middleware.cors import CORSMiddleware
 
 
-# persistence
-# sqlite
-# - sessions
-# - events
-# from fastapi import FastAPI
 from fastapi.responses import StreamingResponse
-# from sqlalchemy import create_engine, text
 
 # API
 # SESSION
 # - get sessions
 # - create session
 # - start session
 # repond session
 # interrupt session
 # stop session
 # delete session
 # get session event history
 # get session event stream
 
 
-# DATABASE_PATH = "./devon_environment.db"
-# DATABASE_URL = "sqlite:///" + DATABASE_PATH
-
 origins = [
     "http://localhost:3000",
     "http://127.0.0.1:3000",
 ]
 
 sessions: Dict[str, Session] = {}
 
-add_or_update_sessions_sql = """
-INSERT INTO sessions (name, JSON_STATE) VALUES (:name, :JSON_STATE)
-ON CONFLICT(name) DO UPDATE SET JSON_STATE = excluded.JSON_STATE
-"""
-
-delete_session_sql = """
-DELETE FROM sessions WHERE name = :name
-"""
-
-get_session_sql = """
-SELECT * FROM sessions WHERE name = :name
-"""
-
-get_sessions_sql = """
-SELECT * FROM sessions
-"""
 
 API_KEY = None
 
-# @asynccontextmanager
-# async def lifespan(app: FastAPI):
-#     print("lifespan")
-#     engine = create_engine(DATABASE_URL, echo=True)
-
-#     # session table SQL DDL
-#     session_table_sql = """
-
-#     CREATE TABLE IF NOT EXISTS sessions (
-#         name TEXT PRIMARY KEY,
-#         JSON_STATE TEXT NOT NULL
-#     );
-#     """
-
-#     # run the SQL DDL statement
-#     with engine.connect() as conn:
-#         conn.execute(text(session_table_sql))
-
-#     # get all sessions and load them into sessions dictionary
-#     with engine.connect() as conn:
-#         ses = conn.execute(text(get_sessions_sql)).fetchall()
-#         for session in ses:
-#             print(session)
-#             state = json.loads(session[1])
-#             state["user_input"] = lambda: get_user_input(session[0])
-#             sessions[session[0]] = Session.from_dict(state)
-#     print("statup done")
-#     yield
-#     print("cleanup")
-#     session_states = [(name, session.to_dict()) for name, session in sessions.items()]
-#     with engine.connect() as conn:
-#         for name, state in session_states:
-#             conn.execute(
-#                 text(add_or_update_sessions_sql),
-#                 {"name": name, "JSON_STATE": json.dumps(state)},
-#             )
-#         conn.commit()
-#     print("cleanup done")
-
 
-app = fastapi.FastAPI(
-    # lifespan=lifespan,
-)
+app = fastapi.FastAPI()
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=origins,
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
@@ -157,15 +91,18 @@
         name="Devon",
         model="claude-opus",
         temperature=0.0,
         api_key=API_KEY,
     )
     sessions[session] = Session(
         SessionArguments(
-            path, environment="local", user_input=lambda: get_user_input(session)
+            path,
+            environment="local",
+            user_input=lambda: get_user_input(session),
+            name=session,
         ),
         agent,
     )
 
     return session
```

### Comparing `devon_agent-0.1.0/devon_agent/session.py` & `devon_agent-0.1.1/devon_agent/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import inspect
 import json
 import logging
+import os
 import traceback
 from dataclasses import dataclass
 from typing import Any, List
 from devon_agent.agent import TaskAgent
 from devon_agent.environment import LocalEnvironment
+from devon_agent.telemetry import Posthog, SessionEventEvent, SessionStartEvent
 from devon_agent.tools import (
     ask_user,
     close_file,
     create_file,
     delete_file,
     edit_file,
     exit,
@@ -35,14 +37,15 @@
 
 
 @dataclass(frozen=False)
 class SessionArguments:
     path: str
     environment: str
     user_input: Any
+    name: str
 
 
 """
 The Event System
 
 To generalize over several things that can happen. We have decided to use an event log to communicate every "event" that happens in the system. The following are a type of some events.
 
@@ -89,26 +92,43 @@
     User --> UserRequest
     ModelResponse --> [*]: Stop
 ```
 
 """
 
 
+def get_git_root(fpath=None):
+    path = fpath
+
+    if path is None:
+        path = os.getcwd()
+
+    while True:
+        if os.path.exists(os.path.join(path, ".git")):
+            return path
+        parent_dir = os.path.dirname(path)
+        if parent_dir == path:
+            return fpath
+        path = parent_dir
+
+
 class Session:
     def __init__(self, args: SessionArguments, agent):
         logger = logging.getLogger(__name__)
 
         self.state = DotDict({})
         self.state.PAGE_SIZE = 200
         self.logger = logger
         self.agent: TaskAgent = agent
-        self.base_path = args.path
+        self.base_path = get_git_root(args.path)
         self.event_log: List[Event] = []
         self.event_index = 0
         self.get_user_input = args.user_input
+        self.telemetry_client = Posthog()
+        self.name = args.name
 
         self.state.editor = {}
 
         self.path = args.path
         self.environment_type = args.environment
 
         if args.environment == "local":
@@ -199,14 +219,21 @@
     def step_event(self):
         if self.event_index == len(self.event_log):
             return "No more events to process", True
         event = self.event_log[self.event_index]
         self.logger.info(f"Event: {event}")
         self.logger.info(f"State: {self.state.editor}")
 
+        # Collect only event name and content only in case of error
+        telemetry_event = SessionEventEvent(
+            event_type=event["type"],
+            message="" if not event["type"] == "Error" else event["content"],
+        )
+        self.telemetry_client.capture(telemetry_event)
+
         if event["type"] == "ModelRequest":
             thought, action, output = self.agent.predict(
                 self.get_last_task(), event["content"], self
             )
             self.event_log.append(
                 {
                     "type": "ModelResponse",
@@ -401,26 +428,24 @@
                     ctx.logger.error(traceback.print_exc())
                     raise e
             elif fn_name in fn_names:
                 for fn in self.tools:
                     if fn.__name__ == fn_name:
                         return fn(ctx, *args), False
             else:
-                try:
-                    output, rc = ctx.environment.communicate(
-                        fn_name + " " + " ".join(args)
-                    )
-                    if rc != 0:
-                        raise Exception(output)
-                    return output, False
-                except Exception as e:
-                    ctx.logger.error(
-                        f"Failed to execute bash command '{fn_name}': {str(e)}"
-                    )
-                    return "Failed to execute bash command", False
+                # try:
+                output, rc = ctx.environment.communicate(fn_name + " " + " ".join(args))
+                if rc != 0:
+                    raise Exception(output)
+                return output, False
+                # except Exception as e:
+                #     ctx.logger.error(
+                #         f"Failed to execute bash command '{fn_name}': {str(e)}"
+                #     )
+                #     return "Failed to execute bash command", False
         except Exception as e:
             ctx.logger.error(traceback.print_exc())
             return e.args[0], False
 
     def get_available_actions(self) -> list[str]:
         return [fn.__name__ for fn in self.tools]
 
@@ -437,11 +462,12 @@
             code = inspect.getsource(func)
             sig, docstring = extract_signature_and_docstring(code)
             docs[name] = {"signature": sig, "docstring": docstring}
 
         return docs
 
     def enter(self):
+        self.telemetry_client.capture(SessionStartEvent(self.name))
         self.environment.setup()
 
     def exit(self):
         self.environment.teardown()
```

### Comparing `devon_agent-0.1.0/devon_agent/test/test_tools.py` & `devon_agent-0.1.1/devon_agent/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.0/devon_agent/tools.py` & `devon_agent-0.1.1/devon_agent/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,22 +48,25 @@
 #     state: DotDict
 
 
 # class ToolModule(Protocol):
 
 #     def setup(self, ctx : ToolContext):
 #         pass
-    
+
 #     def __call__(self, ctx : ToolContext, **kwargs):
 #         pass
 
 #     def cleanup(self, ctx : ToolContext):
 #         pass
 
 
+ToolContext = Any
+
+
 def normalize_path(path, specified_path):
     if path == os.sep:
         return specified_path
     elif os.path.isabs(path):
         if path.startswith(specified_path):
             path = Path(path)
             return path.absolute().as_posix()
@@ -73,15 +76,14 @@
             path = os.sep + os.path.join(*path_components)
             path = Path(path)
             return path.absolute().as_posix()
     else:
         path = Path(specified_path) / Path(path)
         return path.absolute().as_posix()
 
-ToolContext = Any
 
 def make_abs_path(ctx, fpath: str) -> str:
     """
     Converts relative paths to absolute paths based on the container's root directory.
 
     Args:
         fpath (str): The file path to convert.
@@ -412,20 +414,20 @@
     if abs_path not in ctx.state.editor:
         raise Exception(f"Could not scroll in file, file is not open: {abs_path}")
 
     lines = ctx.state.editor[abs_path]["lines"].splitlines()
     total_lines = len(lines)
     line_number = int(line_number)
 
-    if line_number < 1 or line_number > total_lines:
+    if line_number < 0 or line_number > total_lines:
         raise Exception(
             f"Invalid line number: {line_number}. Line number should be between 1 and {total_lines}."
         )
 
-    window_number = (line_number - 1) // ctx.state.PAGE_SIZE
+    window_number = (line_number) // ctx.state.PAGE_SIZE
     ctx.state.editor[abs_path]["page"] = window_number
 
     window_start_line = window_number * ctx.state.PAGE_SIZE + 1
     return f"Scrolled to window containing line {line_number} in file {abs_path}. Window starts at line {window_start_line}."
 
 
 def close_file(ctx, file_path: str) -> bool:
@@ -754,40 +756,46 @@
                     file_content=success[2],
                     src_file=success[0],
                     tgt_file=success[0],
                 )
 
     if len(failures) == 0:
         file_paths = []
+        diff_results = []
         for result in successes:
             # This will overwrite if the tgt files are the same, but doesnt really matter in this case because its usually only one diff
 
-            try:
-                compile(result[1], "<string>", "exec")
-            except Exception as e:
-                return "Error applying diff: \n" + repr(e)
-
             target_path = result[0]
 
+            if target_path.endswith(".py"):
+                try:
+                    compile(result[1], "<string>", "exec")
+                    before_results = check_lint(
+                        ctx, read_file(ctx, target_path), target_path
+                    )
+                except Exception as e:
+                    return "Error applying diff: \n" + repr(e)
+
             old_editor_code = "\n".join(ctx.state.editor[target_path]["lines"])
-            before_results = check_lint(ctx, read_file(ctx, target_path), target_path)
 
             write_file(ctx, file_path=target_path, content=result[1])
             file_paths.append(target_path)
 
             new_editor_code = "\n".join(ctx.state.editor[target_path]["lines"])
-            after_results = check_lint(ctx, result[1], target_path)
 
             assert old_editor_code != new_editor_code
 
-            diff_results = [
-                x
-                for x in after_results
-                if not check_lint_entry_in_list(x, before_results)
-            ]
+            if target_path.endswith(".py"):
+                after_results = check_lint(ctx, result[1], target_path)
+
+                diff_results = [
+                    x
+                    for x in after_results
+                    if not check_lint_entry_in_list(x, before_results)
+                ]
 
         paths = ", ".join(file_paths)
 
         if diff_results:
             lint_error_message = ""
             for rst in diff_results:
                 lint_error_message += f"{rst['type']}: {rst['message']} on line {rst['line']} column {rst['column']}. Line {result[1].splitlines()[int(rst['line'])-1]} \n"
@@ -1363,16 +1371,16 @@
 
     SYNOPSIS
         exit
     """
     pass
 
 
-def set_task(ctx : ToolContext, task):
+def set_task(ctx: ToolContext, task):
     """
     NAME
         set_task - set the current task
 
     SYNOPSIS
         set_task TASK
     """
-    pass
+    pass
```

### Comparing `devon_agent-0.1.0/devon_agent/udiff.py` & `devon_agent-0.1.1/devon_agent/udiff.py`

 * *Files 0% similar despite different names*

```diff
@@ -631,14 +631,17 @@
     start_indents = [get_indent(line[1], indent_size) for line in start_code_fence]
     # stop_indents = [get_indent(line[1],indent_size) for line in stop_code_fence]
     # print(start_indents)
     # print(stop_indents)
     # print(new_lines)
 
     new_indents = [get_indent(line, indent_size) for line in new_lines]
+
+    if not new_indents:
+        return new_lines
     # print(new_indents)
 
     # print(relative_indents)
     base = start_indents[0] - new_indents[0]
 
     line_no_base = start_code_fence_start
 
@@ -829,15 +832,14 @@
         else:
             failed.extend(errors)
 
     # should return files with new code to write
     return {"success": succeeded, "fail": failed}
 
 
-
 def apply_multi_file_context_diff(file_content, diff, original_change_count):
     # By the time we get here we have correctly captured a single command
 
     failures = []
 
     try:
         all_diffs, total_new_changed = extract_all_diffs(diff)
```

### Comparing `devon_agent-0.1.0/devon_agent/utils.py` & `devon_agent-0.1.1/devon_agent/utils.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.0/devon_agent/vgit.py` & `devon_agent-0.1.1/devon_agent/vgit.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.0/pyproject.toml` & `devon_agent-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "devon-agent"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["killind-dev <61808204+killind-dev@users.noreply.github.com>","mihir1003 <mihir1003@gmail.com>"]
 readme = "README.md"
 exclude = [
     "devon_tui",
 ]
 
-
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 openai = "^1.14.1"
 anthropic = "^0.20.0"
 pydantic = "^2.5.0"
 xmltodict = "^0.13.0"
 astroid = "^3.1.0"
@@ -28,14 +27,15 @@
 sqlalchemy = "^2.0.30"
 tenacity = "^8.2.2"
 simple-parsing = {version = "^0.1.5", optional = true}
 swebench = {version = "1.0.1", optional = true}
 gymnasium = {version = "^0.29.1", optional = true}
 datasets = {version = ">=2.14.6,<2.15.0", optional = true}
 click = "^8.1.7"
+posthog = "^3.5.0"
 
 [tool.poetry.extras]
 swebench = ["swebench", "datasets", "gymnasium"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.3"
```

### Comparing `devon_agent-0.1.0/PKG-INFO` & `devon_agent-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devon-agent
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: killind-dev
 Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -17,14 +17,15 @@
 Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: fastapi (>=0.110.3,<0.111.0)
 Requires-Dist: ghapi (>=1.0.5,<2.0.0)
 Requires-Dist: gitpython (>=3.1.42,<4.0.0)
 Requires-Dist: gymnasium (>=0.29.1,<0.30.0) ; extra == "swebench"
 Requires-Dist: networkx (>=3.3,<4.0)
 Requires-Dist: openai (>=1.14.1,<2.0.0)
+Requires-Dist: posthog (>=3.5.0,<4.0.0)
 Requires-Dist: pydantic (>=2.5.0,<3.0.0)
 Requires-Dist: pylint (>=3.1.0,<4.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: pytest-json-report (>=1.5.0,<2.0.0)
 Requires-Dist: simple-parsing (>=0.1.5,<0.2.0)
 Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
 Requires-Dist: swebench (==1.0.1) ; extra == "swebench"
```

