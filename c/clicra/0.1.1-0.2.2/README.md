# Comparing `tmp/clicra-0.1.1.tar.gz` & `tmp/clicra-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clicra-0.1.1.tar", last modified: Thu May  9 13:18:55 2024, max compression
+gzip compressed data, was "clicra-0.2.2.tar", last modified: Sat May 11 01:40:09 2024, max compression
```

## Comparing `clicra-0.1.1.tar` & `clicra-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-09 13:18:55.202475 clicra-0.1.1/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     3167 2024-05-09 02:31:12.000000 clicra-0.1.1/.gitignore
--rw-r--r--   0 toshihiro  (1000) toshihiro  (1000)     2106 2024-05-09 13:18:55.202475 clicra-0.1.1/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1441 2024-05-09 08:49:04.000000 clicra-0.1.1/README.md
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-09 13:18:55.198475 clicra-0.1.1/clicra/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       25 2024-05-09 01:28:09.000000 clicra-0.1.1/clicra/__init__.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     7596 2024-05-09 08:39:51.000000 clicra-0.1.1/clicra/clicra.py
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-09 13:18:55.202475 clicra-0.1.1/clicra.egg-info/
--rw-r--r--   0 toshihiro  (1000) toshihiro  (1000)     2106 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/SOURCES.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/dependency_links.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       39 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/entry_points.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       63 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/requires.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        7 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/top_level.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      863 2024-05-09 08:03:46.000000 clicra-0.1.1/pyproject.toml
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2024-05-09 13:18:55.202475 clicra-0.1.1/setup.cfg
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-11 01:40:09.486089 clicra-0.2.2/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     3167 2024-05-09 02:31:12.000000 clicra-0.2.2/.gitignore
+-rw-r--r--   0 toshihiro  (1000) toshihiro  (1000)     2528 2024-05-11 01:40:09.486089 clicra-0.2.2/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1863 2024-05-11 01:24:18.000000 clicra-0.2.2/README.md
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-11 01:40:09.486089 clicra-0.2.2/clicra/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       25 2024-05-09 01:28:09.000000 clicra-0.2.2/clicra/__init__.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     8767 2024-05-11 01:30:58.000000 clicra-0.2.2/clicra/clicra.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-11 01:40:09.486089 clicra-0.2.2/clicra.egg-info/
+-rw-r--r--   0 toshihiro  (1000) toshihiro  (1000)     2528 2024-05-11 01:40:09.000000 clicra-0.2.2/clicra.egg-info/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2024-05-11 01:40:09.000000 clicra-0.2.2/clicra.egg-info/SOURCES.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2024-05-11 01:40:09.000000 clicra-0.2.2/clicra.egg-info/dependency_links.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       39 2024-05-11 01:40:09.000000 clicra-0.2.2/clicra.egg-info/entry_points.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       63 2024-05-11 01:40:09.000000 clicra-0.2.2/clicra.egg-info/requires.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        7 2024-05-11 01:40:09.000000 clicra-0.2.2/clicra.egg-info/top_level.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      863 2024-05-10 12:14:36.000000 clicra-0.2.2/pyproject.toml
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2024-05-11 01:40:09.486089 clicra-0.2.2/setup.cfg
```

### Comparing `clicra-0.1.1/.gitignore` & `clicra-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `clicra-0.1.1/PKG-INFO` & `clicra-0.2.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,8 @@
-Metadata-Version: 2.1
-Name: clicra
-Version: 0.1.1
-Summary: A LLM command-line crafter
-Author-email: Toshihiro Kamiya <kamiya@mbj.nifty.com>
-License: MIT LICENSE
-Project-URL: Souce, https://github.com/tos-kamiya/clicra
-Keywords: cli-tool,LLM
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Requires-Dist: ollama>=0.1.9
-Requires-Dist: pyperclip>=1.8.2
-Requires-Dist: termcolor>=2.4.0
-Requires-Dist: setuptools>=61
-
-### clicra: Command Line Crafter
+# clicra: Command Line Crafter
 
 `clicra` is a command-line tool that utilizes local large language models (LLMs) to generate and analyze command lines based on tasks provided by users.
 
 ## Installation
 
 `clicra` requires `Ollama` to be installed beforehand. Please follow the instructions on the official Ollama website.
 
@@ -40,27 +20,28 @@
 
 ```sh
 pipx uninstall clicra
 ```
 
 ## Usage
 
-To run `clicra`, use the following syntax:
+To run `clicra`, provide a description of the task you want to execute as a command-line argument:
 
 ```sh
 clicra [options] <task>
 ```
 
-- `<task>`: Description of the task you want to execute.
-
 ### Options
 
 - `-m, --model`: Specifies the LLM to use (default is `llama3`).
-- `-r, --run`: Generates and executes the command without confirmation and analyzes the outcome if there are errors.
 - `-f, --refer`: Executes a specified command and uses its output as additional context to improve the accuracy and relevance of task command generation.
+- `-M, --max-chars`: Specifies the maximum number of characters to include from the referred command's output in the prompt (default is `2000`).
+- `-r, --run`: Instead of copying the generated command to the clipboard, it executes the command immediately without confirmation, and analyzes the outcome if there are errors (non-zero exit code).
+- `-s, --script`: Generates a script instead of a command.
+- `--p, --prompt`: Ask for a prompt to describe the solution (**experimental feature**). `tot` for Tree-of-Thought. `sbs` for Step-by-Step.
 
 ### Examples
 
 To find source files containing TODO comments, you can provide the output of `ls` as context. This allows `clicra` to recognize the directory structure and file types:
 
 ```sh
 clicra "Find TODOs in source files" -f "ls"
```

### Comparing `clicra-0.1.1/clicra/clicra.py` & `clicra-0.2.2/clicra/clicra.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,96 @@
-from typing import Tuple, List, Optional
+from typing import Dict, Tuple, List, Optional
 from typing import IO, TextIO
 
 import argparse
+import re
 import subprocess
 import sys
 import threading
 
 import pyperclip
 from termcolor import colored
 
 try:
     import ollama
 except ImportError:
     exit("Install `ollama-python` by following the instruction on: https://github.com/ollama/ollama-python")
 
 
 import pkg_resources
-_version = pkg_resources.get_distribution('clicra').version
+
+_version = pkg_resources.get_distribution("clicra").version
 
 DEFAULT_LLM = "llama3"
+LARGER_LLM = "llama3:70b"
 DEFAULT_OUTPUT_MAX_CHARS = 2000
 
+PROMPTINGS : Dict[str, str] = {
+    "sbs": """(Let’s work this out in a step by step way to be sure we have the right answer.
+
+""",  # ref: https://arxiv.org/pdf/2211.01910
+    "tot": """magine three different experts are answering this question. All experts will write down 1 step of their thinking, then share it with the group.
+Then all experts will go on to the next step, etc. If any expert realises they're wrong at any point then they leave.
+
+""",  # ref: https://github.com/dave1010/tree-of-thought-prompting
+}
+
 
 def clip_text(text: str, max_chars: int) -> str:
     if len(text) == 0:
-        return ""
+        return "\n"
 
     snip_str = " ...(snip)... "
 
     newline_pos = text.find("\n")
     if newline_pos < 0 or newline_pos > max_chars:
         return text[:max_chars] + snip_str + "\n"
 
     while newline_pos >= 0:
         next_newline_pos = text.find("\n", newline_pos + 1)
         if next_newline_pos < 0 or next_newline_pos > max_chars:
-            return text[:newline_pos + 1] + snip_str + "\n"
+            return text[: newline_pos + 1] + snip_str + "\n"
         newline_pos = next_newline_pos
 
+    if not text.endswith("\n"):
+        text = text + "\n"
+    return text
 
-def stream_reader(
-    stream: IO, output: TextIO, output_list: List[str]
-) -> None:
+
+def stream_reader(stream: IO, output: TextIO, output_list: List[str]) -> None:
     for line in iter(stream.readline, b""):
         line = line.decode("utf-8")
         output_list.append(line)
 
 
-def stream_reader_thru(
-    stream: IO, output: TextIO, output_list: List[str]
-) -> None:
+def stream_reader_thru(stream: IO, output: TextIO, output_list: List[str]) -> None:
     for line in iter(stream.readline, b""):
         line = line.decode("utf-8")
         output_list.append(line)
         print(line, file=output, end="")
 
 
 def do_run_and_capture(code: str, thru_output=True) -> Tuple[int, str, str]:
     """Run the code and capture the standard out and standard error."""
 
     lines = []
-    for L in code.split('\n'):
+    for L in code.split("\n"):
         if L.startswith("$ "):
             L = L[2:]
         lines.append(L)
 
-    process = subprocess.Popen(
-        ["bash", "-c", "\n".join(lines)], stdout=subprocess.PIPE, stderr=subprocess.PIPE
-    )
+    process = subprocess.Popen(["bash", "-c", "\n".join(lines)], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
     stdout_list = []
     stderr_list = []
 
     sr = stream_reader_thru if thru_output else stream_reader
 
-    stdout_thread = threading.Thread(
-        target=sr, args=(process.stdout, sys.stdout, stdout_list)
-    )
-    stderr_thread = threading.Thread(
-        target=sr, args=(process.stderr, sys.stderr, stderr_list)
-    )
+    stdout_thread = threading.Thread(target=sr, args=(process.stdout, sys.stdout, stdout_list))
+    stderr_thread = threading.Thread(target=sr, args=(process.stderr, sys.stderr, stderr_list))
 
     stdout_thread.start()
     stderr_thread.start()
 
     process.wait()
 
     stdout_thread.join()
@@ -91,49 +98,58 @@
 
     stdout = "".join(stdout_list).rstrip()
     stderr = "".join(stderr_list).rstrip()
 
     return process.returncode, stdout, stderr
 
 
-def highlight_and_extract_code(text: str) -> Tuple[str, str]:
+def highlight_and_extract_command(text: str) -> Tuple[str, str]:
     """Extract the first code block enclosed by "```" and add highlights to the text."""
 
     lines = text.splitlines()
     in_code_block = False
     highlighted_lines = []
     code_block = []
+    pat_code_block_start = re.compile("^```")
+    pat_code_block_end = re.compile("^```")
+
     for line in lines:
         if in_code_block:
-            if line.startswith("```"):
+            if pat_code_block_start.match(line):
                 highlighted_lines.append(line)
                 in_code_block = False
             else:
                 code_block.append(line)
                 highlighted_lines.append(colored(line, "green", attrs=["bold"]))
         else:
             highlighted_lines.append(line)
-            if not code_block and line.startswith("```"):
+            if not code_block and pat_code_block_end.match(line):
                 in_code_block = True
+
     return "\n".join(highlighted_lines), "\n".join(code_block)
 
 
-def format_command_generation_prompt(task: str, context: Optional[str], generate_script: bool = False) -> str:
+def format_command_generation_prompt(
+    task: str, context: Optional[str], generate_script: bool = False, prompting: Optional[str] = None
+) -> str:
+    p = PROMPTINGS.get(prompting, "") if prompting is not None else ""
     if generate_script:
-        p = f"Please provide a script to accomplish the following task."
+        p += f"Please provide a script to accomplish the following task."
     else:
-        p = f"Please provide a command line to accomplish the following task."
+        p += f"Please provide a command line to accomplish the following task."
     if task:
         p += f"\n## TASK\n{task}\n"
     if context:
         p += f"\n## CONTEXT\n{context}\n"
     return p
 
 
-def format_analysis_prompt(code: str, task: Optional[str], context: Optional[str], stdout: Optional[str], stderr: Optional[str]) -> str:
+def format_analysis_prompt(
+    code: str, task: Optional[str], context: Optional[str], stdout: Optional[str], stderr: Optional[str]
+) -> str:
     p = f"Analyze the result of the command.\n"
     if task:
         p += f"\n## TASK\n{task}\n"
     if context:
         p += f"\n## CONTEXT\n{context}\n"
     p += f"\n## COMMAND\n```\n{code}\n```\n"
     if stdout:
@@ -156,94 +172,103 @@
         r.append(f"EXIT CODE: {exit_code}")
     r.append("```")
     context = "\n".join(r)
     return context
 
 
 def main() -> None:
-    parser = argparse.ArgumentParser(
-        description="Generate command line from task description"
-    )
+    parser = argparse.ArgumentParser(description="Generate command line from task description")
     parser.add_argument("task", nargs="*", help="description of the task to perform")
-    parser.add_argument(
-        "-r", "--run", action="store_true", help="generate command, run it, and then analyze the result."
+    g = parser.add_mutually_exclusive_group()
+    g.add_argument("-r", "--run", action="store_true", help="generate command, run it, and then analyze the result.")
+    g.add_argument(
+        "-s",
+        "--script",
+        action="store_true",
+        help="ask to generate a script (instead of a command line).",
+    )
+    g.add_argument(
+        "-p",
+        "--prompt",
+        choices=["tot", "sbs"],
+        help="ask for a prompt to describe the solution (**experimental feature**). `tot` for Tree-of-Thought. `sbs` for Step-by-Step.",
     )
     parser.add_argument(
         "-f",
         "--refer",
         help="provide a command to execute and use its output as additional context.",
     )
     parser.add_argument(
         "-m",
         "--model",
         default=DEFAULT_LLM,
         help="LLM name to use.",
     )
     parser.add_argument(
-        "-s",
-        "--script",
-        action="store_true",
-        help="ask to generate a script (instead of a command line).",
-    )
-    parser.add_argument(
         "-M",
         "--max-chars",
         type=int,
         default=DEFAULT_OUTPUT_MAX_CHARS,
         help="max characters of command execution results.",
     )
-    parser.add_argument(
-        "-v", "--verbose", action="store_true"
-    )
-    parser.add_argument("--version", action="version",
-                        version=f"%(prog)s {_version}")
+    parser.add_argument("-v", "--verbose", action="store_true")
+    parser.add_argument("--version", action="version", version=f"%(prog)s {_version}")
     args = parser.parse_args()
 
     if not args.task:
         exit("Error: no task is given. Option `-h` for help.")
-    if args.run and args.script:
-        exit("Error: options --generate-script and --run are mutually exclusive.")
     task = " ".join(args.task)
 
+    if args.verbose:
+        print(colored(f"Model: {args.model}", attrs=["dark"]) + "\n", file=sys.stderr)
+
     def chat(prompt: str) -> str:
         response = ollama.chat(
             model=args.model,
             messages=[{"role": "user", "content": prompt}],
         )
         return response["message"]["content"]
 
     context = build_reference_context(args.refer, args.max_chars) if args.refer else None
 
-    p = format_command_generation_prompt(task, context, generate_script=args.script)
+    p = format_command_generation_prompt(
+        task,
+        context,
+        generate_script=args.script,
+        prompting=args.prompt,
+    )
     if args.verbose:
         for L in p.split("\n"):
             print(colored(L, attrs=["dark"]), file=sys.stderr)
-    command = chat(p)
+    response = chat(p)
 
-    highlighted_text, code = highlight_and_extract_code(command)
+    if args.prompt:
+        highlighted_text = response
+        command = None
+    else:
+        highlighted_text, command = highlight_and_extract_command(response)
     print(highlighted_text)
 
-    if code:
+    if command:
         if args.run:
             ht_run = colored(f"-- RUN", "yellow", attrs=["bold"])
-            print(f"\n{ht_run}: {code}\n")
-            exit_code, stdout, stderr = do_run_and_capture(code)
+            print(f"\n{ht_run}: {command}\n")
+            exit_code, stdout, stderr = do_run_and_capture(command)
             if exit_code != 0:
                 print("\n" + colored("-- DEBUG", "yellow", attrs=["bold"]) + "\n")
                 p = format_analysis_prompt(
-                    code, task, context,
-                    clip_text(stdout, args.max_chars), clip_text(stderr, args.max_chars)
+                    command, task, context, clip_text(stdout, args.max_chars), clip_text(stderr, args.max_chars)
                 )
                 if args.verbose:
                     for L in p.split("\n"):
                         print(colored(L, attrs=["dark"]), file=sys.stderr)
                 analysis = chat(p)
                 print(analysis)
             exit(exit_code)
         else:
-            pyperclip.copy(code)
+            pyperclip.copy(command)
             ht_copied = colored(f"-- COPIED THE HIGHLIGHTED CODE TO CLIPBOARD", "yellow", attrs=["bold"])
             print(f"\n{ht_copied}\n")
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clicra-0.1.1/pyproject.toml` & `clicra-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Operating System :: POSIX :: Linux",
 ]
-version = "0.1.1"
+version = "0.2.2"
 
 [project.scripts]
 clicra = "clicra:main"
 
 [project.urls]
 Souce = "https://github.com/tos-kamiya/clicra"
```

