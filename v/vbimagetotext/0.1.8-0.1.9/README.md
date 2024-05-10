# Comparing `tmp/vbimagetotext-0.1.8.tar.gz` & `tmp/vbimagetotext-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbimagetotext-0.1.8.tar", max compression
+gzip compressed data, was "vbimagetotext-0.1.9.tar", max compression
```

## Comparing `vbimagetotext-0.1.8.tar` & `vbimagetotext-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.8/README.md
--rw-r--r--   0        0        0      588 2024-05-06 14:15:50.855574 vbimagetotext-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.8/vbimagetotext/__init__.py
--rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.8/vbimagetotext/__main__.py
--rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.8/vbimagetotext/choice_option.py
--rw-r--r--   0        0        0     1518 2024-05-01 23:15:21.290644 vbimagetotext-0.1.8/vbimagetotext/copyprompt.py
--rw-r--r--   0        0        0     5136 2024-05-06 14:15:44.767344 vbimagetotext-0.1.8/vbimagetotext/functions.py
--rw-r--r--   0        0        0     2776 2024-04-26 07:27:12.309253 vbimagetotext-0.1.8/vbimagetotext/geminivision.py
--rw-r--r--   0        0        0     1611 2024-05-06 14:15:09.868118 vbimagetotext-0.1.8/vbimagetotext/gptvision.py
--rw-r--r--   0        0        0      428 2024-05-01 23:23:16.539392 vbimagetotext-0.1.8/vbimagetotext/main.py
--rw-r--r--   0        0        0     9081 2024-05-06 13:57:13.429263 vbimagetotext-0.1.8/vbimagetotext/prompts.py
--rw-r--r--   0        0        0     1070 2024-05-02 11:19:07.184507 vbimagetotext-0.1.8/vbimagetotext/solution.py
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.9/README.md
+-rw-r--r--   0        0        0      588 2024-05-09 09:52:29.841868 vbimagetotext-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.9/vbimagetotext/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.9/vbimagetotext/__main__.py
+-rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.9/vbimagetotext/choice_option.py
+-rw-r--r--   0        0        0     1606 2024-05-09 09:52:07.857054 vbimagetotext-0.1.9/vbimagetotext/copyprompt.py
+-rw-r--r--   0        0        0     5212 2024-05-09 09:49:07.076656 vbimagetotext-0.1.9/vbimagetotext/functions.py
+-rw-r--r--   0        0        0     2800 2024-05-09 09:35:15.765295 vbimagetotext-0.1.9/vbimagetotext/geminivision.py
+-rw-r--r--   0        0        0     1635 2024-05-09 09:35:05.777867 vbimagetotext-0.1.9/vbimagetotext/gptvision.py
+-rw-r--r--   0        0        0      469 2024-05-09 09:43:29.258649 vbimagetotext-0.1.9/vbimagetotext/main.py
+-rw-r--r--   0        0        0     9901 2024-05-09 09:34:47.511588 vbimagetotext-0.1.9/vbimagetotext/prompts.py
+-rw-r--r--   0        0        0     1070 2024-05-02 11:19:07.184507 vbimagetotext-0.1.9/vbimagetotext/solution.py
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.9/PKG-INFO
```

### Comparing `vbimagetotext-0.1.8/pyproject.toml` & `vbimagetotext-0.1.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vbimagetotext"
-version = "0.1.8"
+version = "0.1.9"
 description = "A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API"
 authors = ["vaibhavblayer <vaibhavblayer@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 click = "^8.1.7"
```

### Comparing `vbimagetotext-0.1.8/vbimagetotext/choice_option.py` & `vbimagetotext-0.1.9/vbimagetotext/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.8/vbimagetotext/copyprompt.py` & `vbimagetotext-0.1.9/vbimagetotext/copyprompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .prompts import prompt_assertion_reason, prompt_mcq, prompt_mcq_solution, prompt_subjective, prompt_match, prompt_comprehension, prompt_answer, prompt_solution
+from .prompts import prompt_assertion_reason, prompt_mcq, prompt_mcq_list, prompt_mcq_solution, prompt_subjective, prompt_match, prompt_comprehension, prompt_answer, prompt_solution
 
 import click
 import pyperclip
 from .choice_option import ChoiceOption
 
 
 @click.command(
@@ -34,14 +34,16 @@
     """
     Copy the prompt to the clipboard.
     """
     if prompt == "assertion_reason":
         pyperclip.copy(prompt_assertion_reason)
     elif prompt == "mcq":
         pyperclip.copy(prompt_mcq)
+    elif prompt == "mcq_list":
+        pyperclip.copy(prompt_mcq_list)
     elif prompt == "mcq_solution":
         pyperclip.copy(prompt_mcq_solution)
     elif prompt == "subjective":
         pyperclip.copy(prompt_subjective)
     elif prompt == "match":
         pyperclip.copy(prompt_match)
     elif prompt == "comprehension":
```

### Comparing `vbimagetotext-0.1.8/vbimagetotext/functions.py` & `vbimagetotext-0.1.9/vbimagetotext/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,21 +101,21 @@
         console.print(
             f"Error: API request failed with status code {response.status_code}.", style="bold red")
         return f"Error: API request failed with status code {response.status_code}."
 
     pattern = r"```latex(.*?)```"
     matches = re.findall(pattern, message, re.DOTALL)
 
-    Console().print(message, style="deep_pink3")
-
     if matches:
         pyperclip.copy(matches[0])
+        subprocess.run(["pbpaste", "|", "bat", "-l", "latex"])
         return matches[0]
     else:
         pyperclip.copy(message)
+        subprocess.run(["pbpaste", "|", "bat", "-l", "latex"])
         return message
 
 
 def process_text(input_file: str, prompt: str, api_key: str, max_tokens: int) -> str:
     """
     Processes text using OpenAI's GPT-4, extracts LaTeX code from the response,
     copies the first match to the clipboard, and prints the message in deep pink color.
```

### Comparing `vbimagetotext-0.1.8/vbimagetotext/geminivision.py` & `vbimagetotext-0.1.9/vbimagetotext/geminivision.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "-p",
     "--prompt",
     cls=ChoiceOption,
     type=click.Choice(
         [
             "assertion_reason",
             "mcq",
+            "mcq_list",
             "mcq_solution",
             "subjective",
             "match",
             "comprehension",
             "answer",
             "prompt",
         ],
```

### Comparing `vbimagetotext-0.1.8/vbimagetotext/gptvision.py` & `vbimagetotext-0.1.9/vbimagetotext/gptvision.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "-p",
     "--prompt",
     cls=ChoiceOption,
     type=click.Choice(
         [
             "assertion_reason",
             "mcq",
+            "mcq_list",
             "mcq_solution",
             "subjective",
             "match",
             "comprehension",
             "answer",
             "prompt",
         ],
```

### Comparing `vbimagetotext-0.1.8/vbimagetotext/prompts.py` & `vbimagetotext-0.1.9/vbimagetotext/prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,35 @@
 \begin{enumerate}
     \item[1. Assertion:] This is an assertion.
     \item[Reason:] This is a reason.
 \end{enumerate}
 Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
-
 prompt_mcq = r"""
+Please analyze the image provided and extract text from it and format it into latex. For question use \item , if there are any diagrams present, place it after \item part. For the options use tasks environment.
+Use this code as reference for multiple-choice questions
+    \item This is a question.
+        \begin{center}
+            \begin{tikzpicture}
+                \node at (0, 0) {Diagram};
+            \end{tikzpicture}
+        \end{center}
+        \begin{tasks}(2)
+            \task Shorter Option 1
+            \task Shorter Option 2
+            \task Shorter Option 3\ans
+            \task Shorter Option 4
+        \end{tasks}
+
+Please provide only the part above formatted of the LaTeX file, not the whole LaTeX document.
+"""
+
+
+prompt_mcq_list = r"""
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only, in the center environment. If there are any multiple-choice questions, please put the options in a tasks environment.
 Use this code as reference for multiple-choice questions
 \begin{enumerate}
     \item This is a question.
         \begin{tasks}(2)
             \task Shorter Option 1
             \task Shorter Option 2
@@ -153,14 +172,16 @@
 
 
 def switch_prompt(value):
     if value == "match":
         return prompt_match
     elif value == "mcq":
         return prompt_mcq
+    elif value == "mcq_list":
+        return prompt_mcq_list
     elif value == "mcq_solution":
         return prompt_mcq_solution
     elif value == "subjective":
         return prompt_subjective
     elif value == "comprension":
         return prompt_comprehension
     elif value == "assertion_reason":
```

### Comparing `vbimagetotext-0.1.8/vbimagetotext/solution.py` & `vbimagetotext-0.1.9/vbimagetotext/solution.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.8/PKG-INFO` & `vbimagetotext-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbimagetotext
-Version: 0.1.8
+Version: 0.1.9
 Summary: A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API
 Author: vaibhavblayer
 Author-email: vaibhavblayer@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

