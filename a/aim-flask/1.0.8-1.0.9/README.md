# Comparing `tmp/aim_flask-1.0.8-py3-none-any.whl.zip` & `tmp/aim_flask-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 5205 bytes, number of entries: 7
--rw-r--r--  2.0 fat     1079 b- defN 80-Jan-01 00:00 aim_flask/__init__.py
--rw-r--r--  2.0 fat     8946 b- defN 80-Jan-01 00:00 aim_flask/main.py
--rw-r--r--  2.0 fat       38 b- defN 80-Jan-01 00:00 aim_flask-1.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 fat     1087 b- defN 80-Jan-01 00:00 aim_flask-1.0.8.dist-info/LICENSE
--rw-r--r--  2.0 fat      321 b- defN 80-Jan-01 00:00 aim_flask-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 aim_flask-1.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 fat      550 b- defN 16-Jan-01 00:00 aim_flask-1.0.8.dist-info/RECORD
-7 files, 12109 bytes uncompressed, 4231 bytes compressed:  65.1%
+Zip file size: 6685 bytes, number of entries: 9
+-rw-r--r--  2.0 fat     1324 b- defN 80-Jan-01 00:00 aim_flask/__init__.py
+-rw-r--r--  2.0 fat      214 b- defN 80-Jan-01 00:00 aim_flask/Interpreter/__init__.py
+-rw-r--r--  2.0 fat     1399 b- defN 80-Jan-01 00:00 aim_flask/Interpreter/interpreter.py
+-rw-r--r--  2.0 fat    10087 b- defN 80-Jan-01 00:00 aim_flask/main.py
+-rw-r--r--  2.0 fat       38 b- defN 80-Jan-01 00:00 aim_flask-1.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 fat     1087 b- defN 80-Jan-01 00:00 aim_flask-1.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 fat      321 b- defN 80-Jan-01 00:00 aim_flask-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 aim_flask-1.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 fat      733 b- defN 16-Jan-01 00:00 aim_flask-1.0.9.dist-info/RECORD
+9 files, 15291 bytes uncompressed, 5421 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -1,22 +1,28 @@
 Filename: aim_flask/__init__.py
 Comment: 
 
+Filename: aim_flask/Interpreter/__init__.py
+Comment: 
+
+Filename: aim_flask/Interpreter/interpreter.py
+Comment: 
+
 Filename: aim_flask/main.py
 Comment: 
 
-Filename: aim_flask-1.0.8.dist-info/entry_points.txt
+Filename: aim_flask-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: aim_flask-1.0.8.dist-info/LICENSE
+Filename: aim_flask-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: aim_flask-1.0.8.dist-info/METADATA
+Filename: aim_flask-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: aim_flask-1.0.8.dist-info/WHEEL
+Filename: aim_flask-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: aim_flask-1.0.8.dist-info/RECORD
+Filename: aim_flask-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aim_flask/__init__.py

```diff
@@ -1,16 +1,17 @@
 # __init__.py
 
-from .main import run_setup, run_feedback, run_help, run_version
+from .main import run_setup, run_feedback, run_help, run_version, run_preview
 import argparse
 import sys
+import aim_flask.Interpreter.interpreter as interpret_aim_command
 
 def main():
     parser = argparse.ArgumentParser(description="AIM CLI for environment setup and installation")
-    parser.add_argument("command", choices=[":cli", ":version", ":setup", ":feedback", ":help", ":verbose"], help="Command to execute")
+    parser.add_argument("command", choices=[":cli", ":version", ":setup", ":feedback", ":help", ":verbose", ":preview"], help="Command to execute")
     args = parser.parse_args()
     args.command == sys.argv[1] if len(sys.argv) > 1 else None
 
     if args.command == ":version":
         run_version()
     elif args.command == ":setup":
         run_setup(verbose=True)
@@ -18,14 +19,17 @@
         feedback_message = input("Enter your feedback message: ")
         run_feedback(feedback_message)
     elif args.command == ":help":
         run_help()
     elif args.command == ":verbose":
         print("Verbose mode enabled.")
         run_setup(verbose=True)
+    elif args.command == ":preview":
+        print("Verbose mode enabled.")
+        run_preview(verbose=True)
     
 
 if __name__ == "__main__":
     main()
 
 # Make sure only necessary functions are exported
-__all__ = ["run_setup", "run_feedback", "run_help", "run_version", "main"]
+__all__ = ["run_setup", "run_feedback", "run_help", "run_version", "main", "run_preview", "interpret_aim_command"]
```

## aim_flask/main.py

```diff
@@ -1,16 +1,17 @@
 import argparse
 import os
 import subprocess
 import platform
 import logging
+from aim_flask.Interpreter.interpreter import interpret_aim_command
 
 # aim_flask.py
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 current_dir = os.getcwd()
 
 # Configure logging
 logging.basicConfig(filename=f'{current_dir}/setup.log', level=logging.INFO, format='%(asctime)s - %(levelname)s: %(message)s')
 logger = logging.getLogger(__name__)
 
@@ -228,14 +229,35 @@
     if not is_git_installed():
         setup_git(verbose=verbose)
     else:
         log("Git is already installed.")
 
     log("Setup completed successfully.")
 
+def run_preview(verbose=False):
+    # Read AIM commands from .aim file
+    # Specify the directory name
+    directory_name = "com.aim"
+
+    # Construct the full path
+    directory_path = os.path.join(f"{current_dir}\\app", directory_name)
+
+    # Check if the directory exists
+    if os.path.exists(f"{current_dir}\\app") and os.path.exists(directory_path):
+        log(f"Directory path for 'com.aim': {directory_path}")
+        with open(directory_path, 'r') as file:
+            aim_commands = file.readlines()
+
+        # Interpret each AIM command and execute corresponding action
+        for aim_command in aim_commands:
+            result = interpret_aim_command(aim_command.strip())
+            print(result)
+    else:
+        print("Directory 'com.aim' does not exist or is not a directory. PATH: ", directory_path)
+
 def run_feedback(message):
     log("Saving feedback to file...")
     with open(f"{current_dir}/feedback.txt", "a") as f:
         f.write(message + "\n")
     log("Feedback saved successfully.")
 
     log("Pushing feedback to GitHub...")
@@ -250,19 +272,20 @@
 def run_help():
     log("Usage: aim <command>")
     log("Commands:")
     log("  version    : Version AIM environment")
     log("  setup    : Setup AIM environment")
     log("  feedback : Send feedback")
     log("  help     : Display this help message")
+    log("  preview     : Display design in browser")
     
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description="AIM CLI for environment setup and installation")
-    parser.add_argument("command", choices=[":cli", ":version", ":setup", ":feedback", ":help", ":verbose"], help="Command to execute")
+    parser = argparse.ArgumentParser(description="AIM CLI")
+    parser.add_argument("command", choices=[":cli", ":version", ":setup", ":feedback", ":help", ":verbose", ":preview"], help="Command to execute")
     args = parser.parse_args()
 
     if args.command == ":version":
         run_version()
     elif args.command == ":setup":
         run_setup(verbose=True)
     elif args.command == ":feedback":
@@ -272,7 +295,13 @@
         run_help()
     elif args.command == ":verbose":
         print("Verbose mode enabled.")
         run_setup(verbose=True)
     elif args.command == ":cli":
         print("Verbose mode enabled.")
         cli(verbose=True)
+    elif args.command == ":preview":
+        print("Verbose mode enabled.")
+        run_preview(verbose=True)
+
+# Make sure only necessary functions are exported
+__all__ = ["interpret_aim_command"]
```

## Comparing `aim_flask-1.0.8.dist-info/LICENSE` & `aim_flask-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

