# Comparing `tmp/applang-0.0.1a3.tar.gz` & `tmp/applang-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "applang-0.0.1a3.tar", last modified: Sat May  4 18:59:59 2024, max compression
+gzip compressed data, was "applang-0.0.1a4.tar", last modified: Sat May 11 08:56:17 2024, max compression
```

## Comparing `applang-0.0.1a3.tar` & `applang-0.0.1a4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1087 2024-05-04 18:41:49.554879 applang-0.0.1a3/LICENSE
--rw-r--r--   0        0        0    17094 2024-05-04 18:51:56.444639 applang-0.0.1a3/README.md
--rw-r--r--   0        0        0     2787 2024-05-04 18:59:59.087001 applang-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0     6707 2024-05-04 18:41:49.600881 applang-0.0.1a3/src/appl/__init__.py
--rw-r--r--   0        0        0     1005 2024-05-04 18:41:49.601881 applang-0.0.1a3/src/appl/cli/vis_trace.py
--rw-r--r--   0        0        0    11825 2024-05-04 18:41:49.601881 applang-0.0.1a3/src/appl/compositor.py
--rw-r--r--   0        0        0      316 2024-05-04 18:41:49.602877 applang-0.0.1a3/src/appl/const.py
--rw-r--r--   0        0        0      695 2024-05-04 18:41:49.602877 applang-0.0.1a3/src/appl/core/__init__.py
--rw-r--r--   0        0        0    12488 2024-05-04 18:41:49.603880 applang-0.0.1a3/src/appl/core/compile.py
--rw-r--r--   0        0        0     2100 2024-05-04 18:41:49.603880 applang-0.0.1a3/src/appl/core/config.py
--rw-r--r--   0        0        0     4556 2024-05-04 18:41:49.603880 applang-0.0.1a3/src/appl/core/context.py
--rw-r--r--   0        0        0     7323 2024-05-04 18:41:49.604881 applang-0.0.1a3/src/appl/core/function.py
--rw-r--r--   0        0        0     7897 2024-05-04 18:41:49.604881 applang-0.0.1a3/src/appl/core/generation.py
--rw-r--r--   0        0        0      510 2024-05-04 18:41:49.605879 applang-0.0.1a3/src/appl/core/globals.py
--rw-r--r--   0        0        0     2197 2024-05-04 18:41:49.605879 applang-0.0.1a3/src/appl/core/io.py
--rw-r--r--   0        0        0    12755 2024-05-04 18:41:49.606878 applang-0.0.1a3/src/appl/core/message.py
--rw-r--r--   0        0        0     6341 2024-05-04 18:41:49.606878 applang-0.0.1a3/src/appl/core/modifiers.py
--rw-r--r--   0        0        0    12389 2024-05-04 18:41:49.606878 applang-0.0.1a3/src/appl/core/printer.py
--rw-r--r--   0        0        0      162 2024-05-04 18:41:49.607877 applang-0.0.1a3/src/appl/core/promptable/__init__.py
--rw-r--r--   0        0        0      565 2024-05-04 18:41:49.607877 applang-0.0.1a3/src/appl/core/promptable/base.py
--rw-r--r--   0        0        0     2899 2024-05-04 18:41:49.608878 applang-0.0.1a3/src/appl/core/promptable/definition.py
--rw-r--r--   0        0        0     1149 2024-05-04 18:41:49.608878 applang-0.0.1a3/src/appl/core/promptable/formatter.py
--rw-r--r--   0        0        0     9062 2024-05-04 18:41:49.608878 applang-0.0.1a3/src/appl/core/response.py
--rw-r--r--   0        0        0     3017 2024-05-04 18:41:49.609877 applang-0.0.1a3/src/appl/core/runtime.py
--rw-r--r--   0        0        0     6626 2024-05-04 18:41:49.609877 applang-0.0.1a3/src/appl/core/server.py
--rw-r--r--   0        0        0     7519 2024-05-04 18:41:49.610876 applang-0.0.1a3/src/appl/core/tool.py
--rw-r--r--   0        0        0     4879 2024-05-04 18:41:49.610876 applang-0.0.1a3/src/appl/core/trace.py
--rw-r--r--   0        0        0      232 2024-05-04 18:41:49.611876 applang-0.0.1a3/src/appl/core/types/__init__.py
--rw-r--r--   0        0        0     1091 2024-05-04 18:41:49.611876 applang-0.0.1a3/src/appl/core/types/basic.py
--rw-r--r--   0        0        0     2726 2024-05-04 18:41:49.611876 applang-0.0.1a3/src/appl/core/types/content.py
--rw-r--r--   0        0        0      395 2024-05-04 18:41:49.612877 applang-0.0.1a3/src/appl/core/types/custom.py
--rw-r--r--   0        0        0     7468 2024-05-04 18:41:49.612877 applang-0.0.1a3/src/appl/core/types/futures.py
--rw-r--r--   0        0        0     2006 2024-05-04 18:41:49.613878 applang-0.0.1a3/src/appl/core/types/role.py
--rw-r--r--   0        0        0     2340 2024-05-04 18:41:49.613878 applang-0.0.1a3/src/appl/default_configs.yaml
--rw-r--r--   0        0        0    15934 2024-05-04 18:41:49.614878 applang-0.0.1a3/src/appl/func.py
--rw-r--r--   0        0        0        0 2024-05-04 18:41:49.614878 applang-0.0.1a3/src/appl/py.typed
--rw-r--r--   0        0        0     2735 2024-05-04 18:41:49.614878 applang-0.0.1a3/src/appl/role_changer.py
--rw-r--r--   0        0        0       65 2024-05-04 18:41:49.615878 applang-0.0.1a3/src/appl/servers/__init__.py
--rw-r--r--   0        0        0     7304 2024-05-04 18:41:49.615878 applang-0.0.1a3/src/appl/servers/api.py
--rw-r--r--   0        0        0     2652 2024-05-04 18:41:49.616879 applang-0.0.1a3/src/appl/servers/manager.py
--rw-r--r--   0        0        0       93 2024-05-04 18:41:49.616879 applang-0.0.1a3/src/appl/tracing/__init__.py
--rw-r--r--   0        0        0     6168 2024-05-04 18:41:49.617878 applang-0.0.1a3/src/appl/tracing/engine.py
--rw-r--r--   0        0        0      622 2024-05-04 18:41:49.617878 applang-0.0.1a3/src/appl/tracing/header.html
--rw-r--r--   0        0        0     9271 2024-05-04 18:41:49.618878 applang-0.0.1a3/src/appl/tracing/printer.py
--rw-r--r--   0        0        0      575 2024-05-04 18:41:49.618878 applang-0.0.1a3/src/appl/types.py
--rw-r--r--   0        0        0     4377 2024-05-04 18:41:49.618878 applang-0.0.1a3/src/appl/utils.py
--rw-r--r--   0        0        0     2748 2024-05-04 18:41:49.619878 applang-0.0.1a3/tests/test_func.py
--rw-r--r--   0        0        0     1674 2024-05-04 18:41:49.620880 applang-0.0.1a3/tests/test_gen.py
--rw-r--r--   0        0        0     6601 2024-05-04 18:41:49.620880 applang-0.0.1a3/tests/test_message.py
--rw-r--r--   0        0        0     2002 2024-05-04 18:41:49.621879 applang-0.0.1a3/tests/test_openai.py
--rw-r--r--   0        0        0     1155 2024-05-04 18:41:49.621879 applang-0.0.1a3/tests/test_parallel.py
--rw-r--r--   0        0        0     5238 2024-05-04 18:41:49.622879 applang-0.0.1a3/tests/test_prompt.py
--rw-r--r--   0        0        0     2650 2024-05-04 18:41:49.622879 applang-0.0.1a3/tests/test_prompt_helpers.py
--rw-r--r--   0        0        0     1701 2024-05-04 18:41:49.623879 applang-0.0.1a3/tests/test_stringfuture.py
--rw-r--r--   0        0        0     5368 2024-05-04 18:41:49.623879 applang-0.0.1a3/tests/test_tool.py
--rw-r--r--   0        0        0    18241 1970-01-01 00:00:00.000000 applang-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-11 08:41:27.250801 applang-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0    16779 2024-05-11 08:41:27.251715 applang-0.0.1a4/README.md
+-rw-r--r--   0        0        0     2787 2024-05-11 08:56:17.937427 applang-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     6537 2024-05-11 08:48:06.483769 applang-0.0.1a4/src/appl/__init__.py
+-rw-r--r--   0        0        0      979 2024-05-11 08:41:27.294900 applang-0.0.1a4/src/appl/cli/vis_trace.py
+-rw-r--r--   0        0        0    11354 2024-05-11 08:41:27.295358 applang-0.0.1a4/src/appl/compositor.py
+-rw-r--r--   0        0        0      297 2024-05-11 08:41:27.295699 applang-0.0.1a4/src/appl/const.py
+-rw-r--r--   0        0        0      673 2024-05-11 08:41:27.296218 applang-0.0.1a4/src/appl/core/__init__.py
+-rw-r--r--   0        0        0    12144 2024-05-11 08:41:27.296786 applang-0.0.1a4/src/appl/core/compile.py
+-rw-r--r--   0        0        0     2034 2024-05-11 08:41:27.297164 applang-0.0.1a4/src/appl/core/config.py
+-rw-r--r--   0        0        0     4432 2024-05-11 08:41:27.313500 applang-0.0.1a4/src/appl/core/context.py
+-rw-r--r--   0        0        0     7141 2024-05-11 08:41:27.314001 applang-0.0.1a4/src/appl/core/function.py
+-rw-r--r--   0        0        0     7681 2024-05-11 08:41:27.314532 applang-0.0.1a4/src/appl/core/generation.py
+-rw-r--r--   0        0        0      490 2024-05-11 08:41:27.314877 applang-0.0.1a4/src/appl/core/globals.py
+-rw-r--r--   0        0        0     2114 2024-05-11 08:41:27.315268 applang-0.0.1a4/src/appl/core/io.py
+-rw-r--r--   0        0        0    12387 2024-05-11 08:41:27.315768 applang-0.0.1a4/src/appl/core/message.py
+-rw-r--r--   0        0        0     6162 2024-05-11 08:41:27.316276 applang-0.0.1a4/src/appl/core/modifiers.py
+-rw-r--r--   0        0        0    12048 2024-05-11 08:41:27.316785 applang-0.0.1a4/src/appl/core/printer.py
+-rw-r--r--   0        0        0      159 2024-05-11 08:41:27.317599 applang-0.0.1a4/src/appl/core/promptable/__init__.py
+-rw-r--r--   0        0        0      544 2024-05-11 08:41:27.318258 applang-0.0.1a4/src/appl/core/promptable/base.py
+-rw-r--r--   0        0        0     2800 2024-05-11 08:41:27.318791 applang-0.0.1a4/src/appl/core/promptable/definition.py
+-rw-r--r--   0        0        0     1106 2024-05-11 08:41:27.319270 applang-0.0.1a4/src/appl/core/promptable/formatter.py
+-rw-r--r--   0        0        0     8824 2024-05-11 08:41:27.319769 applang-0.0.1a4/src/appl/core/response.py
+-rw-r--r--   0        0        0     2933 2024-05-11 08:41:27.320182 applang-0.0.1a4/src/appl/core/runtime.py
+-rw-r--r--   0        0        0     6440 2024-05-11 08:41:27.320637 applang-0.0.1a4/src/appl/core/server.py
+-rw-r--r--   0        0        0     7315 2024-05-11 08:41:27.321064 applang-0.0.1a4/src/appl/core/tool.py
+-rw-r--r--   0        0        0     4707 2024-05-11 08:41:27.321454 applang-0.0.1a4/src/appl/core/trace.py
+-rw-r--r--   0        0        0      222 2024-05-11 08:41:27.321934 applang-0.0.1a4/src/appl/core/types/__init__.py
+-rw-r--r--   0        0        0     1046 2024-05-11 08:41:27.322878 applang-0.0.1a4/src/appl/core/types/basic.py
+-rw-r--r--   0        0        0     2645 2024-05-11 08:41:27.323151 applang-0.0.1a4/src/appl/core/types/content.py
+-rw-r--r--   0        0        0      379 2024-05-11 08:41:27.323383 applang-0.0.1a4/src/appl/core/types/custom.py
+-rw-r--r--   0        0        0     7234 2024-05-11 08:41:27.323750 applang-0.0.1a4/src/appl/core/types/futures.py
+-rw-r--r--   0        0        0     1935 2024-05-11 08:41:27.324043 applang-0.0.1a4/src/appl/core/types/role.py
+-rw-r--r--   0        0        0     2286 2024-05-11 08:41:27.324340 applang-0.0.1a4/src/appl/default_configs.yaml
+-rw-r--r--   0        0        0    15495 2024-05-11 08:41:27.324789 applang-0.0.1a4/src/appl/func.py
+-rw-r--r--   0        0        0        0 2024-05-11 08:41:27.325037 applang-0.0.1a4/src/appl/py.typed
+-rw-r--r--   0        0        0     2651 2024-05-11 08:41:27.325381 applang-0.0.1a4/src/appl/role_changer.py
+-rw-r--r--   0        0        0       63 2024-05-11 08:41:27.325846 applang-0.0.1a4/src/appl/servers/__init__.py
+-rw-r--r--   0        0        0     7101 2024-05-11 08:47:37.242145 applang-0.0.1a4/src/appl/servers/api.py
+-rw-r--r--   0        0        0     2570 2024-05-11 08:41:27.326533 applang-0.0.1a4/src/appl/servers/manager.py
+-rw-r--r--   0        0        0       91 2024-05-11 08:41:27.326977 applang-0.0.1a4/src/appl/tracing/__init__.py
+-rw-r--r--   0        0        0     6001 2024-05-11 08:41:27.327333 applang-0.0.1a4/src/appl/tracing/engine.py
+-rw-r--r--   0        0        0      609 2024-05-11 08:41:27.327612 applang-0.0.1a4/src/appl/tracing/header.html
+-rw-r--r--   0        0        0     9051 2024-05-11 08:41:27.327979 applang-0.0.1a4/src/appl/tracing/printer.py
+-rw-r--r--   0        0        0      558 2024-05-11 08:41:27.328330 applang-0.0.1a4/src/appl/types.py
+-rw-r--r--   0        0        0     4252 2024-05-11 08:41:27.328722 applang-0.0.1a4/src/appl/utils.py
+-rw-r--r--   0        0        0     2590 2024-05-11 08:41:27.329210 applang-0.0.1a4/tests/test_func.py
+-rw-r--r--   0        0        0     1610 2024-05-11 08:41:27.329461 applang-0.0.1a4/tests/test_gen.py
+-rw-r--r--   0        0        0     6346 2024-05-11 08:41:27.329797 applang-0.0.1a4/tests/test_message.py
+-rw-r--r--   0        0        0     1923 2024-05-11 08:41:27.330155 applang-0.0.1a4/tests/test_openai.py
+-rw-r--r--   0        0        0     1095 2024-05-11 08:41:27.330429 applang-0.0.1a4/tests/test_parallel.py
+-rw-r--r--   0        0        0     5001 2024-05-11 08:41:27.330772 applang-0.0.1a4/tests/test_prompt.py
+-rw-r--r--   0        0        0     2541 2024-05-11 08:41:27.331105 applang-0.0.1a4/tests/test_prompt_helpers.py
+-rw-r--r--   0        0        0     1622 2024-05-11 08:41:27.331340 applang-0.0.1a4/tests/test_stringfuture.py
+-rw-r--r--   0        0        0     5179 2024-05-11 08:41:27.331638 applang-0.0.1a4/tests/test_tool.py
+-rw-r--r--   0        0        0    18244 1970-01-01 00:00:00.000000 applang-0.0.1a4/PKG-INFO
```

### Comparing `applang-0.0.1a3/README.md` & `applang-0.0.1a4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,318 +1,318 @@
-# 🍎APPL: A Prompt Programming Language
-
-[![python](https://img.shields.io/badge/Python-3.9%2B-blue.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://mit-license.org/)
-
-
-**APPL** is A Prompt Programming Language that extends Python to provide a Natural, Intuitive, Convenient, and Efficient (NICE) way to utilize Large Language Models (LLMs) such as GPT in your program.
-
-![APPL](https://raw.githubusercontent.com/appl-team/appl/main/docs/_assets/appl_runtime.png)
-
-## Key Features
-- **Readability and maintainability via seamless integration with Python.**  APPL seamlessly embeds natural language prompts into Python programs, maintaining prompts' readability while inheriting modularity, reusability, dynamism and the ecosystem from the host programming language.
-- **Flexible prompt engineering.**  Except for allowing the utilization of Python control flows and the modularized decomposition of prompts, APPL offers prompt coding helpers to facilitate programming prompts in a modularized and maintainable way.
-- **Automatic parallelization via asynchronous computation.**  APPL schedules LLM calls asynchronously, leveraging potential independence among them to facilitate efficient parallelization. This offloads the burden of users to manage synchronization manually, with almost no extra work.
-- **Smooth tool calling integration.**  APPL provides intuitive ways to transform Python functions into tools that can be called by LLMs, making it easy for users to integrate existing Python libraries and functions with LLMs.
-- **Tracing and Failure Recovery.** APPL traces the execution of LLM calls and supports recovery from failures, which is essential for debugging and error handling in the LLM programming paradigm.
-- **More Features.** APPL also provides a unified interface for multiple LLM backends using [`litellm`](https://docs.litellm.ai/docs/), structured generations using [`instructor`](https://python.useinstructor.com/), and many other features.
-
-<!-- TODO: RoadMap -->
-
-## Quick Start
-
-### Installation
-You can simply install APPL from PyPI using pip:
-```bash
-pip install -U appl
-```
-More installation options can be found in the [installation guide](https://appl-team.github.io/appl/install).
-
-### Setup
-You need to set up API keys or your own LLM backends to interact with LLMs.
-
-In this guide, we use OpenAI API as the default backend.
-You can set your OpenAI API key in the `.env` file in the root directory of your project:
-```
-OPENAI_API_KEY=<your openai api key>
-```
-or export it as an environment variable:
-```bash
-export OPENAI_API_KEY=<your openai api key>
-```
-
-For setting up other backends, enabling tracing and recovering from traces, please refer to the [setup guide](https://appl-team.github.io/appl/setup).
-
-### Hello World
-
-To begin, let's create a simple function that uses LLM to respond to a greeting.
-
-```python
-import appl
-from appl import gen, ppl
-
-appl.init()  # initialize APPL
-
-@ppl  # the @ppl decorator marks the function as an `APPL function`
-def greeting(name: str):
-    f"Hello World! My name is {name}."  # Add text to the prompt
-    return gen()  # call the default LLM with the current prompt
-
-print(greeting("APPL"))  # call `greeting` as a normal Python function
-```
-
-The prompt for the generation is:
-```
-Hello World! My name is APPL.
-```
-
-The output will look like
-```
-Nice to meet you, APPL!
-```
-
-In this example, the `@ppl` decorator (`@` stands for `a` here) marks the `hello_world` function as an *APPL function*. Within such a function, the standalone string `f"Hello World! My name is {name}."` is added to the prompt, and the `gen()` function calls LLM to generate responses using the current prompt.
-
-### Question Answering
-
-Let's then implement a question-answering system using APPL. In this example, the APPL program answers multiple questions about a quotation by first extracting the author's name (inspired by [this cookbook](https://cookbook.openai.com/articles/how_to_work_with_large_language_models)). [Here](https://colab.research.google.com/drive/1khZcleOrdLOWtUB4EMEQCjGA1vBaARI9) is a runnable Colab notebook of this example.
-
-```python linenums="1" hl_lines="9 14 15 17"
-import appl
-from appl import AIRole, gen, ppl
-from appl.const import NEWLINE
-
-appl.init()
-
-@ppl(ctx="copy")  # copy the context from caller
-def get_answer(question: str):
-    question  # append to the prompt
-    return gen()  # return as a future object
-
-@ppl  # marks APPL function
-def answer_questions(quotation: str, questions: list[str]):
-    "Extract the name of the author from the quotation below and answer questions."
-    quotation  # append to the prompt
-    with AIRole():  # assistant message
-        f"The name of the author is {gen(stop=NEWLINE)}"  # specify the prefix
-    return [get_answer(q) for q in questions]  # parallelize calls
-
-quotation = '"Simplicity is the ultimate sophistication." -- Leonardo da Vinci'
-questions = [
-    "In what era did the author live?",
-    # more questions can be added here
-]
-for ans in answer_questions(quotation, questions):
-    print(ans)
-```
-
-The resulting conversation for the first question would look like (generated responses are in **bold**):
-
-| Role        | Message                                                                                                                                            |
-| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
-| *User*      | Extract the name of the author from the quotation below and answer questions.<br>"Simplicity is the ultimate sophistication." -- Leonardo da Vinci |
-| *Assistant* | The name of the author is **Leonardo da Vinci.**                                                                                                   |
-| *User*      | In what era did the author live?                                                                                                                   |
-| *Assistant* | **Leonardo da Vinci lived during the Renaissance era.**                                                                                            |
-
-In *APPL functions*, [expression statements](https://docs.python.org/3/reference/simple_stmts.html#expression-statements) are captured as prompts based on the type of its value. <!-- TODO: link to the language explanation doc-->
-Notably, the f-string is processed part by part, so the `gen` function inside the f-string intuitively uses the contents before that. In this example, `The name of the author is ` serves as a prefix to guide the completion of the author's name.
-
-After the author's name is extracted, the `get_answer` function is called multiple times in parallel to answer the questions, with the context being copied (detailed in [context-management](#context-management)), demonstrating the automatic parallelization feature of APPL.
-
-## Usage by Examples
-We provide a series of examples to demonstrate the usage of APPL. Some examples in this section are simplified for demonstration purposes. See runnable examples in the [examples](examples/basic) directory.
-
-### Context Management
-Each *APPL function* has a **context**, which contains the prompts captured in the function. There are four different ways to pass the context when calling another *APPL function* (the callee) in an *APPL function* (the caller): **new**, **copy**, **same**, and **resume**.
-
-![Context Management](https://raw.githubusercontent.com/appl-team/appl/main/docs/_assets/context.png)
-
-1. **new**: The default behavior, create a new empty context.
-2. **copy**: This is similar to *call by value* in programming languages. The callee's context is a copy of the caller's context, therefore the changes in the callee's context won't affect the caller's context.
-3. **same**: This is similar to *call by reference* in programming languages. The callee's context is the same as the caller's context, therefore the changes in the callee's context will affect the caller's context.
-4. **resume**: This resumes the context of the function each time it is called, i.e., the context is preserved across calls, making the function stateful. It copies the caller's context for the first call as the initial context. It is useful when you want to continue the conversation from the last call.
-
-In the following example, we illustrate the usage of the first three context management methods and ways to decompose long prompts into smaller pieces using *APPL functions*. 
-
-```python
-import appl
-from appl import convo, gen, ppl, records
-
-appl.init()
-
-@ppl  # use empty context
-def intro():
-    f"Today is 2024/02/29."
-    return records()
-
-@ppl(ctx="same")  # same as the caller's context
-def addon():
-    f"Dates should be in the format of YYYY/MM/DD."
-    # The newly captured prompt will influence the caller's context
-
-@ppl(ctx="copy")  # copy the caller's context
-def query(question: str):
-    # the prompts here will not influence the caller's context
-    f"Q: {question}"
-    f"A: "
-    # print(convo())  # display the conversation used for the generation
-    return gen()
-
-@ppl
-def ask_questions(questions: list[str]):
-    # long prompt can be decomposed into several smaller `appl functions`
-    # method 1 (recommended): build the sub-prompts in an empty context
-    intro()  # returns prompt records, will be captured in this context
-    # method 2: use the same context and modify it in the function
-    addon()  # returns None, not captured, but the context is modified inside
-    return [query(q) for q in questions]
- 
-questions = [
-    "What's the date tomorrow?",
-    "What's the date yesterday?",
-    "How many dates passed since 2024/02/02?",
-]
-for res in ask_questions(questions):
-    print(res)
-```
-
-Three queries are independent and run in parallel, where the prompts and possible responses of the generations are shown below:
-
-<table>
-  <tr>
-    <th>First query</th>
-    <th>Second query</th>
-    <th>Third query</th>
-  </tr>
-  <tr>
-    <td colspan="3">
-    Today is 2024/02/29.<br>
-    Dates should be in the format of YYYY/MM/DD.
-    </td>
-  </tr>
-  <tr>
-    <td>Q: What's the date tomorrow?</td>
-    <td>Q: What's the date yesterday?</td>
-    <td>Q: How many dates passed since 2024/02/02?</td>
-  </tr>
-  <tr>
-    <td>A: <strong>2024/03/01</strong></td>
-    <td>A: <strong>2024/02/28</strong></td>
-    <td>A: <strong>27 dates have passed since 2024/02/02.</strong></td>
-  </tr>
-</table>
-
-Note the `records()` function retrieves the prompt records captured in the current function, and the `convo()` function retrieves the full conversation in the context. They are analogous to the `locals()` and `globals()` functions in Python.
-
-### Concurrent Execution
-
-The parallelization of multiple queries in the last example is achieved using [asynchronous computation](https://docs.python.org/3/library/concurrent.futures.html). In APPL, the `gen` function automatically starts a new thread (or process) and does not block the main thread. The generation result is not synchronized (waited) until its value is needed, making the execution of multiple independent LLM calls easily concurrent.
-
-Many prompt engineering techniques like [Self-Consistency (CoT-SC)](https://arxiv.org/abs/2203.11171) and [Tree of Thoughts (ToT)](https://arxiv.org/abs/2305.10601) involve non-sequential LLM calls such as branching and gathering. The following example demonstrates how to use APPL to naturally exploit the independence among the reasoning paths in CoT-SC to parallelize the execution.
-
-```python
-def get_mode(answers: list[str]):
-    """Get the mode of the answers"""
-    return max(set(answers), key=answers.count)
-
-def marginalize(results: list):
-    """Get the answer from the results and get the mode of the answers"""
-    
-    # explicitly syncronize the results using str()
-    answers = [parse_answer(str(res)) for res in results]
-    # detailed implementation of `parse_answer` are omitted here
-
-    return get_mode(answers)
-
-@ppl
-def cot_consistency(cot_examples: list[str], question: str, num_trials: int):
-    cot_examples # the list of examples are captured into prompt one-by-one
-    question
-    results = [gen() for _ in range(num_trials)] # concurrent generation
-    return marginalize(results) # marginalize the reasoning paths to get the answer
-```
-
-### LLM Tool Calling
-
-Integrating tools significantly enhances the capabilities of LLMs. APPL introduces a seamless method to transform Python functions into tools accessible by LLMs (provided the backend LLM supports tool calls). When the `gen` function is provided with Python functions, APPL automatically transforms them into tools by extracting information from the signature and docstring of the functions. Such integration facilitates leveraging existing Python libraries and functions directly within LLMs.
-
-Consider the example below, where we transform a Python function, `is_lucky`, into a callable tool. During execution, `gpt-3.5-turbo` smartly invokes the `is_lucky` tool with the appropriate arguments. Subsequently, the function executes with these arguments and the result is returned.
-
-```python
-import sympy
-
-import appl
-from appl import Generation, as_tool, gen, ppl, records
-
-appl.init()
-
-def is_lucky(x: int) -> bool:
-    """Determine whether the input number is a lucky number.
-
-    Args:
-        x (int): The input number to be checked.
-
-    Returns:
-        bool: True if the number is a lucky number, False otherwise.
-    """
-    return sympy.isprime(x + 3)
-
-@ppl
-def func(x):
-    f"Is {x} a lucky number?"
-
-    # Initiate the generation with tool `unique_number``,
-    # which is built into a tool by automatically extracting
-    # information from the function signature and docstring.
-    # And then store the tool call messages into the prompt
-    (actions := gen(tools=[is_lucky]))
-
-    # Execute the tool calls and retrieve the results.
-    results = actions.run_tool_calls()  # results is a list of ToolMessage
-
-    # Return the first result from the tool execution.
-    return results[0].get_content()
-```
-
-### Prompt Coding Helpers
-
-We provide two types of helpers, `Compositor` and `Definition`, to facilitate coding prompts in a modularized and maintainable way. These helpers were originally designed in [PromptCoder](https://github.com/dhh1995/PromptCoder) and have been used to develop prompts in the [ToolEmu](https://github.com/ryoungj/ToolEmu) project with more than 20k tokens in total. By leveraging Python's idiomatic features, we have enhanced the usability and flexibility of these helpers.
-
-The `Compositor` organizes the prompts within its context into a structured prompt. For example, the `NumberedList` would compose a list of text into a numbered list:
-```python
-with NumberedList():
-    f"First item"
-    f"Second item"
->>> composed into >>>
-1. First item
-2. Second item
-```
-You can also nest the compositors to create more complex structures.
-
-The `Definition` class provides a standardized way to define concepts and refer to them in the prompts. Once a concept is defined by subclassing `Definition`, you can refer to it in the prompts by using the class name. Meanwhile, you need to include the concept's description somewhere in the prompt by instantiating the class with the description as an argument. This design ensures the consistency of the concept's definition and usage in the prompts.
-
-Please see the [example](examples/basic) for more details.
-
-## Cookbook
-For more detailed usage and examples, please refer to the [cookbook](https://appl-team.github.io/appl/cookbook).
-
-## Citation and Acknowledgment
-If you find APPL helpful, please consider citing our paper:
-```bibtex
-<to be added>
-```
-
-We would like to thank the open-source community for their contributions, where we learned from or used these libraries in our project, including
-[instructor](https://github.com/jxnl/instructor),
-[LiteLLM](https://github.com/BerriAI/litellm),
-[LMQL](https://github.com/eth-sri/lmql),
-[Guidance](https://github.com/guidance-ai/guidance),
-[SGLang](https://github.com/sgl-project/sglang) and
-[autogen](https://github.com/microsoft/autogen).
-
-## License
-This project is licensed under the terms of the MIT License.
+# 🍎APPL: A Prompt Programming Language
+
+[![python](https://img.shields.io/badge/Python-3.9%2B-blue.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://mit-license.org/)
+
+
+**APPL** is A Prompt Programming Language that extends Python to provide a Natural, Intuitive, Convenient, and Efficient (NICE) way to utilize Large Language Models (LLMs) such as GPT in your program.
+
+![APPL](https://raw.githubusercontent.com/appl-team/appl/main/docs/_assets/appl_runtime.png)
+
+## Key Features
+- **Readability and maintainability via seamless integration with Python.**  APPL seamlessly embeds natural language prompts into Python programs, maintaining prompts' readability while inheriting modularity, reusability, dynamism and the ecosystem from the host programming language.
+- **Flexible prompt engineering.**  Except for allowing the utilization of Python control flows and the modularized decomposition of prompts, APPL offers prompt coding helpers to facilitate programming prompts in a modularized and maintainable way.
+- **Automatic parallelization via asynchronous computation.**  APPL schedules LLM calls asynchronously, leveraging potential independence among them to facilitate efficient parallelization. This offloads the burden of users to manage synchronization manually, with almost no extra work.
+- **Smooth tool calling integration.**  APPL provides intuitive ways to transform Python functions into tools that can be called by LLMs, making it easy for users to integrate existing Python libraries and functions with LLMs.
+- **Tracing and Failure Recovery.** APPL traces the execution of LLM calls and supports recovery from failures, which is essential for debugging and error handling in the LLM programming paradigm.
+- **More Features.** APPL also provides a unified interface for multiple LLM backends using [`litellm`](https://docs.litellm.ai/docs/), structured generations using [`instructor`](https://python.useinstructor.com/), and many other features.
+
+<!-- TODO: RoadMap -->
+
+## Quick Start
+
+### Installation
+You can simply install APPL from PyPI using pip:
+```bash
+pip install -U applang
+```
+More installation options can be found in the [installation guide](https://appl-team.github.io/appl/install).
+
+### Setup
+You need to set up API keys or your own LLM backends to interact with LLMs.
+
+In this guide, we use OpenAI API as the default backend.
+You can set your OpenAI API key in the `.env` file in the root directory of your project:
+```
+OPENAI_API_KEY=<your openai api key>
+```
+or export it as an environment variable:
+```bash
+export OPENAI_API_KEY=<your openai api key>
+```
+
+For setting up other backends, enabling tracing and recovering from traces, please refer to the [setup guide](https://appl-team.github.io/appl/setup).
+
+### Hello World
+
+To begin, let's create a simple function that uses LLM to respond to a greeting.
+
+```python
+import appl
+from appl import gen, ppl
+
+appl.init()  # initialize APPL
+
+@ppl  # the @ppl decorator marks the function as an `APPL function`
+def greeting(name: str):
+    f"Hello World! My name is {name}."  # Add text to the prompt
+    return gen()  # call the default LLM with the current prompt
+
+print(greeting("APPL"))  # call `greeting` as a normal Python function
+```
+
+The prompt for the generation is:
+```
+Hello World! My name is APPL.
+```
+
+The output will look like
+```
+Nice to meet you, APPL!
+```
+
+In this example, the `@ppl` decorator (`@` stands for `a` here) marks the `hello_world` function as an *APPL function*. Within such a function, the standalone string `f"Hello World! My name is {name}."` is added to the prompt, and the `gen()` function calls LLM to generate responses using the current prompt.
+
+### Question Answering
+
+Let's then implement a question-answering system using APPL. In this example, the APPL program answers multiple questions about a quotation by first extracting the author's name (inspired by [this cookbook](https://cookbook.openai.com/articles/how_to_work_with_large_language_models)). [Here](https://colab.research.google.com/drive/1khZcleOrdLOWtUB4EMEQCjGA1vBaARI9) is a runnable Colab notebook of this example.
+
+```python linenums="1" hl_lines="9 14 15 17"
+import appl
+from appl import AIRole, gen, ppl
+from appl.const import NEWLINE
+
+appl.init()
+
+@ppl(ctx="copy")  # copy the context from caller
+def get_answer(question: str):
+    question  # append to the prompt
+    return gen()  # return as a future object
+
+@ppl  # marks APPL function
+def answer_questions(quotation: str, questions: list[str]):
+    "Extract the name of the author from the quotation below and answer questions."
+    quotation  # append to the prompt
+    with AIRole():  # assistant message
+        f"The name of the author is {gen(stop=NEWLINE)}"  # specify the prefix
+    return [get_answer(q) for q in questions]  # parallelize calls
+
+quotation = '"Simplicity is the ultimate sophistication." -- Leonardo da Vinci'
+questions = [
+    "In what era did the author live?",
+    # more questions can be added here
+]
+for ans in answer_questions(quotation, questions):
+    print(ans)
+```
+
+The resulting conversation for the first question would look like (generated responses are in **bold**):
+
+| Role        | Message                                                                                                                                            |
+| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
+| *User*      | Extract the name of the author from the quotation below and answer questions.<br>"Simplicity is the ultimate sophistication." -- Leonardo da Vinci |
+| *Assistant* | The name of the author is **Leonardo da Vinci.**                                                                                                   |
+| *User*      | In what era did the author live?                                                                                                                   |
+| *Assistant* | **Leonardo da Vinci lived during the Renaissance era.**                                                                                            |
+
+In *APPL functions*, [expression statements](https://docs.python.org/3/reference/simple_stmts.html#expression-statements) are captured as prompts based on the type of its value. <!-- TODO: link to the language explanation doc-->
+Notably, the f-string is processed part by part, so the `gen` function inside the f-string intuitively uses the contents before that. In this example, `The name of the author is ` serves as a prefix to guide the completion of the author's name.
+
+After the author's name is extracted, the `get_answer` function is called multiple times in parallel to answer the questions, with the context being copied (detailed in [context-management](#context-management)), demonstrating the automatic parallelization feature of APPL.
+
+## Usage by Examples
+We provide a series of examples to demonstrate the usage of APPL. Some examples in this section are simplified for demonstration purposes. See runnable examples in the [examples](examples/basic) directory.
+
+### Context Management
+Each *APPL function* has a **context**, which contains the prompts captured in the function. There are four different ways to pass the context when calling another *APPL function* (the callee) in an *APPL function* (the caller): **new**, **copy**, **same**, and **resume**.
+
+![Context Management](https://raw.githubusercontent.com/appl-team/appl/main/docs/_assets/context.png)
+
+1. **new**: The default behavior, create a new empty context.
+2. **copy**: This is similar to *call by value* in programming languages. The callee's context is a copy of the caller's context, therefore the changes in the callee's context won't affect the caller's context.
+3. **same**: This is similar to *call by reference* in programming languages. The callee's context is the same as the caller's context, therefore the changes in the callee's context will affect the caller's context.
+4. **resume**: This resumes the context of the function each time it is called, i.e., the context is preserved across calls, making the function stateful. It copies the caller's context for the first call as the initial context. It is useful when you want to continue the conversation from the last call.
+
+In the following example, we illustrate the usage of the first three context management methods and ways to decompose long prompts into smaller pieces using *APPL functions*. 
+
+```python
+import appl
+from appl import convo, gen, ppl, records
+
+appl.init()
+
+@ppl  # use empty context
+def intro():
+    f"Today is 2024/02/29."
+    return records()
+
+@ppl(ctx="same")  # same as the caller's context
+def addon():
+    f"Dates should be in the format of YYYY/MM/DD."
+    # The newly captured prompt will influence the caller's context
+
+@ppl(ctx="copy")  # copy the caller's context
+def query(question: str):
+    # the prompts here will not influence the caller's context
+    f"Q: {question}"
+    f"A: "
+    # print(convo())  # display the conversation used for the generation
+    return gen()
+
+@ppl
+def ask_questions(questions: list[str]):
+    # long prompt can be decomposed into several smaller `appl functions`
+    # method 1 (recommended): build the sub-prompts in an empty context
+    intro()  # returns prompt records, will be captured in this context
+    # method 2: use the same context and modify it in the function
+    addon()  # returns None, not captured, but the context is modified inside
+    return [query(q) for q in questions]
+ 
+questions = [
+    "What's the date tomorrow?",
+    "What's the date yesterday?",
+    "How many dates passed since 2024/02/02?",
+]
+for res in ask_questions(questions):
+    print(res)
+```
+
+Three queries are independent and run in parallel, where the prompts and possible responses of the generations are shown below:
+
+<table>
+  <tr>
+    <th>First query</th>
+    <th>Second query</th>
+    <th>Third query</th>
+  </tr>
+  <tr>
+    <td colspan="3">
+    Today is 2024/02/29.<br>
+    Dates should be in the format of YYYY/MM/DD.
+    </td>
+  </tr>
+  <tr>
+    <td>Q: What's the date tomorrow?</td>
+    <td>Q: What's the date yesterday?</td>
+    <td>Q: How many dates passed since 2024/02/02?</td>
+  </tr>
+  <tr>
+    <td>A: <strong>2024/03/01</strong></td>
+    <td>A: <strong>2024/02/28</strong></td>
+    <td>A: <strong>27 dates have passed since 2024/02/02.</strong></td>
+  </tr>
+</table>
+
+Note the `records()` function retrieves the prompt records captured in the current function, and the `convo()` function retrieves the full conversation in the context. They are analogous to the `locals()` and `globals()` functions in Python.
+
+### Concurrent Execution
+
+The parallelization of multiple queries in the last example is achieved using [asynchronous computation](https://docs.python.org/3/library/concurrent.futures.html). In APPL, the `gen` function automatically starts a new thread (or process) and does not block the main thread. The generation result is not synchronized (waited) until its value is needed, making the execution of multiple independent LLM calls easily concurrent.
+
+Many prompt engineering techniques like [Self-Consistency (CoT-SC)](https://arxiv.org/abs/2203.11171) and [Tree of Thoughts (ToT)](https://arxiv.org/abs/2305.10601) involve non-sequential LLM calls such as branching and gathering. The following example demonstrates how to use APPL to naturally exploit the independence among the reasoning paths in CoT-SC to parallelize the execution.
+
+```python
+def get_mode(answers: list[str]):
+    """Get the mode of the answers"""
+    return max(set(answers), key=answers.count)
+
+def marginalize(results: list):
+    """Get the answer from the results and get the mode of the answers"""
+    
+    # explicitly syncronize the results using str()
+    answers = [parse_answer(str(res)) for res in results]
+    # detailed implementation of `parse_answer` are omitted here
+
+    return get_mode(answers)
+
+@ppl
+def cot_consistency(cot_examples: list[str], question: str, num_trials: int):
+    cot_examples # the list of examples are captured into prompt one-by-one
+    question
+    results = [gen() for _ in range(num_trials)] # concurrent generation
+    return marginalize(results) # marginalize the reasoning paths to get the answer
+```
+
+### LLM Tool Calling
+
+Integrating tools significantly enhances the capabilities of LLMs. APPL introduces a seamless method to transform Python functions into tools accessible by LLMs (provided the backend LLM supports tool calls). When the `gen` function is provided with Python functions, APPL automatically transforms them into tools by extracting information from the signature and docstring of the functions. Such integration facilitates leveraging existing Python libraries and functions directly within LLMs.
+
+Consider the example below, where we transform a Python function, `is_lucky`, into a callable tool. During execution, `gpt-3.5-turbo` smartly invokes the `is_lucky` tool with the appropriate arguments. Subsequently, the function executes with these arguments and the result is returned.
+
+```python
+import sympy
+
+import appl
+from appl import Generation, as_tool, gen, ppl, records
+
+appl.init()
+
+def is_lucky(x: int) -> bool:
+    """Determine whether the input number is a lucky number.
+
+    Args:
+        x (int): The input number to be checked.
+
+    Returns:
+        bool: True if the number is a lucky number, False otherwise.
+    """
+    return sympy.isprime(x + 3)
+
+@ppl
+def func(x):
+    f"Is {x} a lucky number?"
+
+    # Initiate the generation with tool `unique_number``,
+    # which is built into a tool by automatically extracting
+    # information from the function signature and docstring.
+    # And then store the tool call messages into the prompt
+    (actions := gen(tools=[is_lucky]))
+
+    # Execute the tool calls and retrieve the results.
+    results = actions.run_tool_calls()  # results is a list of ToolMessage
+
+    # Return the first result from the tool execution.
+    return results[0].get_content()
+```
+
+### Prompt Coding Helpers
+
+We provide two types of helpers, `Compositor` and `Definition`, to facilitate coding prompts in a modularized and maintainable way. These helpers were originally designed in [PromptCoder](https://github.com/dhh1995/PromptCoder) and have been used to develop prompts in the [ToolEmu](https://github.com/ryoungj/ToolEmu) project with more than 20k tokens in total. By leveraging Python's idiomatic features, we have enhanced the usability and flexibility of these helpers.
+
+The `Compositor` organizes the prompts within its context into a structured prompt. For example, the `NumberedList` would compose a list of text into a numbered list:
+```python
+with NumberedList():
+    f"First item"
+    f"Second item"
+>>> composed into >>>
+1. First item
+2. Second item
+```
+You can also nest the compositors to create more complex structures.
+
+The `Definition` class provides a standardized way to define concepts and refer to them in the prompts. Once a concept is defined by subclassing `Definition`, you can refer to it in the prompts by using the class name. Meanwhile, you need to include the concept's description somewhere in the prompt by instantiating the class with the description as an argument. This design ensures the consistency of the concept's definition and usage in the prompts.
+
+Please see the [example](examples/basic) for more details.
+
+## Cookbook
+For more detailed usage and examples, please refer to the [cookbook](https://appl-team.github.io/appl/cookbook).
+
+## Citation and Acknowledgment
+If you find APPL helpful, please consider citing our paper:
+```bibtex
+<to be added>
+```
+
+We would like to thank the open-source community for their contributions, where we learned from or used these libraries in our project, including
+[instructor](https://github.com/jxnl/instructor),
+[LiteLLM](https://github.com/BerriAI/litellm),
+[LMQL](https://github.com/eth-sri/lmql),
+[Guidance](https://github.com/guidance-ai/guidance),
+[SGLang](https://github.com/sgl-project/sglang) and
+[autogen](https://github.com/microsoft/autogen).
+
+## License
+This project is licensed under the terms of the MIT License.
```

### Comparing `applang-0.0.1a3/pyproject.toml` & `applang-0.0.1a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "applang"
-version = "0.0.1-a3"
+version = "0.0.1-a4"
 description = "A Prompt Programming Language"
 authors = [
     { name = "Honghua Dong", email = "dhh19951@gmail.com" },
     { name = "QiDong Su", email = "soodoshll@gmail.com" },
     { name = "Jim Gao", email = "ybgao@cs.toronto.edu" },
 ]
 dependencies = [
```

### Comparing `applang-0.0.1a3/src/appl/__init__.py` & `applang-0.0.1a4/src/appl/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-"""appl - A Prompt Programming Language."""
-
-from __future__ import annotations
-
-import datetime
-import inspect
-import os
-import sys
-
-import pendulum
-import yaml
-from dotenv import load_dotenv
-from loguru import logger
-
-logger.remove()  # Remove default handler
-logger.add(sys.stderr, level="INFO")  # set to INFO
-
-from .compositor import ApplStr as Str
-from .compositor import iter
-from .core import (
-    BracketedDefinition,
-    CompletionResponse,
-    Definition,
-    Generation,
-    Image,
-    Indexing,
-    Promptable,
-    PromptPrinter,
-    PromptRecords,
-    Tool,
-)
-from .core import appl_compile as compile
-from .core import appl_execute as execute
-from .core import appl_format as format
-from .core import appl_with_ctx as with_ctx
-from .core.config import Configs, configs, load_config
-from .core.globals import global_vars
-from .core.io import dump_file, load_file
-from .core.message import (
-    AIMessage,
-    Conversation,
-    SystemMessage,
-    ToolMessage,
-    UserMessage,
-)
-from .core.promptable import define, define_bracketed, promptify
-from .func import (
-    as_func,
-    as_str,
-    as_tool,
-    as_tool_choice,
-    call,
-    convo,
-    gen,
-    need_ctx,
-    openai_tool_schema,
-    partial,
-    ppl,
-    records,
-)
-from .role_changer import AIRole, SystemRole, ToolRole, UserRole
-from .servers import server_manager
-from .tracing import TraceEngine
-from .types import *
-from .utils import LoguruFormatter, find_dotenv, find_files, get_folder, get_meta_file
-
-APPL_DIR = os.path.dirname(os.path.abspath(__file__))
-PROJECT_FILE = os.path.join(APPL_DIR, "..", "..", "pyproject.toml")
-PROJECT_INFO = load_file(PROJECT_FILE)
-__version__ = PROJECT_INFO["project"]["version"]
-
-
-def _get_loguru_format():
-    return LoguruFormatter(
-        max_length=configs.getattrs("settings.logging.max_length"),
-        suffix_length=configs.getattrs("settings.logging.suffix_length"),
-    ).loguru_format
-
-
-logger.remove()  # Remove default handler
-# update default handler for the loguru logger
-logger.add(sys.stderr, level="INFO", format=_get_loguru_format())  # default
-global_vars.initialized = False
-
-
-def init(
-    resume_cache: Optional[str] = None,
-    update_config_hook: Optional[Callable] = None,
-) -> None:
-    """Initialize APPL with dotenv and config files.
-
-    Args:
-        resume_cache: Path to the trace file used as resume cache. Defaults to None.
-        update_config_hook: A hook to update the configs. Defaults to None.
-    """
-    with global_vars.lock:
-        # only initialize once
-        if global_vars.initialized:
-            logger.warning("APPL has already been initialized, ignore")
-            return
-        global_vars.initialized = True
-
-    now = pendulum.instance(datetime.datetime.now())
-    # Get the previous frame in the stack, i.e., the one calling this function
-    frame = inspect.currentframe()
-    if frame and frame.f_back:
-        caller_path = frame.f_back.f_code.co_filename  # Get file_path of the caller
-        caller_basename = os.path.basename(caller_path).split(".")[0]
-        caller_folder = os.path.dirname(caller_path)  # Get folder of the caller
-        caller_folder = get_folder(caller_folder)
-        dotenvs = find_files(caller_folder, [".env"])
-        appl_config_files = find_files(
-            caller_folder, ["appl.yaml", "appl.yml", "appl.json", "appl.toml"]
-        )
-        # load dotenvs and appl configs from outer to inner with override
-        for dotenv in dotenvs[::-1]:
-            load_dotenv(dotenv, override=True)
-            logger.info("Loaded dotenv from {}".format(dotenv))
-        for config_file in appl_config_files[::-1]:
-            override_configs = load_config(config_file)
-            logger.info("Loaded configs from {}".format(config_file))
-            configs.update(override_configs)
-            logger.info(f"update configs:\n{yaml.dump(override_configs.to_dict())}")
-    else:
-        caller_basename, dotenvs, appl_config_files = "appl", [], []
-        logger.error(
-            "Cannot find the caller of appl.init(), fail to load .env and appl configs"
-        )
-
-    if update_config_hook:
-        update_config_hook(configs)
-    log_format = configs.getattrs("settings.logging.format")
-    log_level = configs.getattrs("settings.logging.log_level")
-    log_file = configs.getattrs("settings.logging.log_file")
-    # set logger level for loguru
-    logger.remove()  # Remove default handler
-    logger.add(sys.stderr, level=log_level, format=_get_loguru_format())
-    if log_file.get("enabled", False):
-        if (log_file_format := log_file.get("path_format", None)) is not None:
-            log_file_path = (
-                f"{log_file_format.format(basename=caller_basename, time=now)}.log"
-            )
-            log_file.path = log_file_path
-            file_log_level = log_file.get("log_level", None) or log_level
-            logger.info(f"Logging to file: {log_file_path} with level {file_log_level}")
-            # no need to overwrite the default format when writing to file
-            logger.add(log_file_path, level=file_log_level, format=log_format)
-
-    configs["info"] = Configs(
-        {
-            "start_time": now.format("YYYY-MM-DD HH:mm:ss"),
-            "dotenvs": dotenvs,
-            "appl_configs": appl_config_files,
-        }
-    )
-    if configs.getattrs("settings.logging.display.configs"):
-        logger.info(f"Using configs:\n{yaml.dump(configs.to_dict())}")
-
-    tracing = configs.getattrs("settings.tracing")
-    strict_match = tracing.get("strict_match", True)
-    if tracing.get("enabled", False):
-        if (trace_file_format := tracing.get("path_format", None)) is not None:
-            prefix = trace_file_format.format(basename=caller_basename, time=now)
-            trace_file_path = f"{prefix}.pkl"
-            meta_file = f"{prefix}_meta.json"
-            tracing.trace_file = trace_file_path
-            logger.info(f"Tracing file: {trace_file_path}")
-            dump_file(configs.to_dict(), meta_file)
-            global_vars.trace_engine = TraceEngine(
-                trace_file_path, mode="write", strict=strict_match
-            )
-        else:
-            logger.warning("Tracing is enabled but no trace file is specified")
-
-    resume_cache = resume_cache or os.environ.get("APPL_RESUME_TRACE", None)
-    if resume_cache:
-        global_vars.resume_cache = resume_cache
-        logger.info(f"Using resume cache: {resume_cache}")
-        global_vars.resume_cache = TraceEngine(
-            resume_cache, mode="read", strict=strict_match
-        )
+"""appl - A Prompt Programming Language."""
+
+from __future__ import annotations
+
+import datetime
+import inspect
+import os
+import sys
+
+import pendulum
+import toml
+import yaml
+from dotenv import load_dotenv
+from loguru import logger
+
+logger.remove()  # Remove default handler
+logger.add(sys.stderr, level="INFO")  # set to INFO
+APPL_DIR = os.path.dirname(os.path.abspath(__file__))
+PROJECT_FILE = os.path.join(APPL_DIR, "..", "..", "pyproject.toml")
+PROJECT_INFO = toml.load(PROJECT_FILE)
+__version__ = PROJECT_INFO["project"]["version"]
+
+from .compositor import ApplStr as Str
+from .compositor import iter
+from .core import (
+    BracketedDefinition,
+    CompletionResponse,
+    Definition,
+    Generation,
+    Image,
+    Indexing,
+    Promptable,
+    PromptPrinter,
+    PromptRecords,
+    Tool,
+)
+from .core import appl_compile as compile
+from .core import appl_execute as execute
+from .core import appl_format as format
+from .core import appl_with_ctx as with_ctx
+from .core.config import Configs, configs, load_config
+from .core.globals import global_vars
+from .core.io import dump_file, load_file
+from .core.message import (
+    AIMessage,
+    Conversation,
+    SystemMessage,
+    ToolMessage,
+    UserMessage,
+)
+from .core.promptable import define, define_bracketed, promptify
+from .func import (
+    as_func,
+    as_str,
+    as_tool,
+    as_tool_choice,
+    call,
+    convo,
+    gen,
+    need_ctx,
+    openai_tool_schema,
+    partial,
+    ppl,
+    records,
+)
+from .role_changer import AIRole, SystemRole, ToolRole, UserRole
+from .servers import server_manager
+from .tracing import TraceEngine
+from .types import *
+from .utils import LoguruFormatter, find_dotenv, find_files, get_folder, get_meta_file
+
+
+def _get_loguru_format():
+    return LoguruFormatter(
+        max_length=configs.getattrs("settings.logging.max_length"),
+        suffix_length=configs.getattrs("settings.logging.suffix_length"),
+    ).loguru_format
+
+
+logger.remove()  # Remove default handler
+# update default handler for the loguru logger
+logger.add(sys.stderr, level="INFO", format=_get_loguru_format())  # default
+global_vars.initialized = False
+
+
+def init(
+    resume_cache: Optional[str] = None,
+    update_config_hook: Optional[Callable] = None,
+) -> None:
+    """Initialize APPL with dotenv and config files.
+
+    Args:
+        resume_cache: Path to the trace file used as resume cache. Defaults to None.
+        update_config_hook: A hook to update the configs. Defaults to None.
+    """
+    with global_vars.lock:
+        # only initialize once
+        if global_vars.initialized:
+            logger.warning("APPL has already been initialized, ignore")
+            return
+        global_vars.initialized = True
+
+    now = pendulum.instance(datetime.datetime.now())
+    # Get the previous frame in the stack, i.e., the one calling this function
+    frame = inspect.currentframe()
+    if frame and frame.f_back:
+        caller_path = frame.f_back.f_code.co_filename  # Get file_path of the caller
+        caller_basename = os.path.basename(caller_path).split(".")[0]
+        caller_folder = os.path.dirname(caller_path)  # Get folder of the caller
+        caller_folder = get_folder(caller_folder)
+        dotenvs = find_files(caller_folder, [".env"])
+        appl_config_files = find_files(
+            caller_folder, ["appl.yaml", "appl.yml", "appl.json", "appl.toml"]
+        )
+        # load dotenvs and appl configs from outer to inner with override
+        for dotenv in dotenvs[::-1]:
+            load_dotenv(dotenv, override=True)
+            logger.info("Loaded dotenv from {}".format(dotenv))
+        for config_file in appl_config_files[::-1]:
+            override_configs = load_config(config_file)
+            logger.info("Loaded configs from {}".format(config_file))
+            configs.update(override_configs)
+            logger.info(f"update configs:\n{yaml.dump(override_configs.to_dict())}")
+    else:
+        caller_basename, dotenvs, appl_config_files = "appl", [], []
+        logger.error(
+            "Cannot find the caller of appl.init(), fail to load .env and appl configs"
+        )
+
+    if update_config_hook:
+        update_config_hook(configs)
+    log_format = configs.getattrs("settings.logging.format")
+    log_level = configs.getattrs("settings.logging.log_level")
+    log_file = configs.getattrs("settings.logging.log_file")
+    # set logger level for loguru
+    logger.remove()  # Remove default handler
+    logger.add(sys.stderr, level=log_level, format=_get_loguru_format())
+    if log_file.get("enabled", False):
+        if (log_file_format := log_file.get("path_format", None)) is not None:
+            log_file_path = (
+                f"{log_file_format.format(basename=caller_basename, time=now)}.log"
+            )
+            log_file.path = log_file_path
+            file_log_level = log_file.get("log_level", None) or log_level
+            logger.info(f"Logging to file: {log_file_path} with level {file_log_level}")
+            # no need to overwrite the default format when writing to file
+            logger.add(log_file_path, level=file_log_level, format=log_format)
+
+    configs["info"] = Configs(
+        {
+            "start_time": now.format("YYYY-MM-DD HH:mm:ss"),
+            "dotenvs": dotenvs,
+            "appl_configs": appl_config_files,
+        }
+    )
+    if configs.getattrs("settings.logging.display.configs"):
+        logger.info(f"Using configs:\n{yaml.dump(configs.to_dict())}")
+
+    tracing = configs.getattrs("settings.tracing")
+    strict_match = tracing.get("strict_match", True)
+    if tracing.get("enabled", False):
+        if (trace_file_format := tracing.get("path_format", None)) is not None:
+            prefix = trace_file_format.format(basename=caller_basename, time=now)
+            trace_file_path = f"{prefix}.pkl"
+            meta_file = f"{prefix}_meta.json"
+            tracing.trace_file = trace_file_path
+            logger.info(f"Tracing file: {trace_file_path}")
+            dump_file(configs.to_dict(), meta_file)
+            global_vars.trace_engine = TraceEngine(
+                trace_file_path, mode="write", strict=strict_match
+            )
+        else:
+            logger.warning("Tracing is enabled but no trace file is specified")
+
+    resume_cache = resume_cache or os.environ.get("APPL_RESUME_TRACE", None)
+    if resume_cache:
+        global_vars.resume_cache = resume_cache
+        logger.info(f"Using resume cache: {resume_cache}")
+        global_vars.resume_cache = TraceEngine(
+            resume_cache, mode="read", strict=strict_match
+        )
```

### Comparing `applang-0.0.1a3/src/appl/cli/vis_trace.py` & `applang-0.0.1a4/src/appl/cli/vis_trace.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import os
-
-from appl import dump_file, load_config, load_file
-from appl.tracing import TraceEngine, TraceHTMLPrinter, TraceProfilePrinter
-from appl.utils import get_meta_file
-
-if __name__ == "__main__":
-    import argparse
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("trace", type=str)
-    parser.add_argument("--output", "-o", type=str, default="./dumps/trace.html")
-    args = parser.parse_args()
-
-    trace_path = args.trace
-    if not os.path.exists(trace_path):
-        trace_path += ".pkl"
-    if not os.path.exists(trace_path):
-        raise FileNotFoundError(f"Trace file not found: {args.trace}")
-    meta_file_path = get_meta_file(trace_path)
-    configs = load_config(meta_file_path)
-    trace = TraceEngine(trace_path, mode="read")
-    print(f"Outputting to {args.output}")
-    is_html = args.output.endswith(".html")
-    printer = TraceHTMLPrinter() if is_html else TraceProfilePrinter()
-    dump_file(printer.print(trace, configs), args.output)
+import os
+
+from appl import dump_file, load_config, load_file
+from appl.tracing import TraceEngine, TraceHTMLPrinter, TraceProfilePrinter
+from appl.utils import get_meta_file
+
+if __name__ == "__main__":
+    import argparse
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument("trace", type=str)
+    parser.add_argument("--output", "-o", type=str, default="./dumps/trace.html")
+    args = parser.parse_args()
+
+    trace_path = args.trace
+    if not os.path.exists(trace_path):
+        trace_path += ".pkl"
+    if not os.path.exists(trace_path):
+        raise FileNotFoundError(f"Trace file not found: {args.trace}")
+    meta_file_path = get_meta_file(trace_path)
+    configs = load_config(meta_file_path)
+    trace = TraceEngine(trace_path, mode="read")
+    print(f"Outputting to {args.output}")
+    is_html = args.output.endswith(".html")
+    printer = TraceHTMLPrinter() if is_html else TraceProfilePrinter()
+    dump_file(printer.print(trace, configs), args.output)
```

### Comparing `applang-0.0.1a3/src/appl/compositor.py` & `applang-0.0.1a4/src/appl/compositor.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,471 +1,471 @@
-"""Containg the compositor classes.
-
-All examples shows the composed prompt in APPL functions.
-"""
-
-from __future__ import annotations
-
-from appl.types import Any, Dict
-
-from .const import INDENT4 as INDENT
-from .core import ApplStr, Compositor, Indexing, PromptContext
-from .func import need_ctx
-from .types import *
-
-
-class LineSeparated(Compositor):
-    r"""The line separated compositor.
-
-    Attributes:
-        _sep: The class default separator is "\n".
-
-    Example:
-        ```py
-        >>> with LineSeparated():
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        item1
-        item2
-        ```
-    """
-
-    _sep = "\n"
-
-
-class DoubleLineSeparated(Compositor):
-    r"""The double line separated compositor.
-
-    Attributes:
-        _sep: The class default separator is "\n\n".
-
-    Example:
-        ```py
-        >>> with DoubleLineSeparated():
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        item1
-
-        item2
-        ```
-    """
-
-    _sep = "\n\n"
-
-
-class FreshLine(LineSeparated):
-    """Create a fresh line with no indent.
-
-    Attributes:
-        _inc_indent: The class default indentation is "".
-
-    Example:
-        ```py
-        >>> with FreshLine():
-        ...     EMPTY
-        <<< The prompt will be:
-        [indicates an empty line]
-        ```
-    """
-
-    _new_indent = ""
-
-
-class IndentedList(LineSeparated):
-    """The indented list compositor.
-
-    Attributes:
-        _inc_indent: The class default indentation is INDENT.
-
-    Example:
-        ```py
-        >>> "BEGIN"
-        ... with IndentedList():
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        BEGIN
-            item1
-            item2
-        ```
-    """
-
-    _inc_indent = INDENT
-
-
-class NumberedList(LineSeparated):
-    """The number list compositor.
-
-    Attributes:
-        _indexing: The class default indexing mode is "number".
-
-    Example:
-        ```py
-        >>> with NumberedList():
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        1. item1
-        2. item2
-        ```
-    """
-
-    _indexing = Indexing("number")
-
-
-class LowerLetterList(LineSeparated):
-    """The lower letter list compositor.
-
-    Attributes:
-        _indexing: The class default indexing mode is "lower".
-
-    Example:
-        ```py
-        >>> with LowerLetterList():
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        a. item1
-        b. item2
-        ```
-    """
-
-    _indexing = Indexing("lower")
-
-
-class UpperLetterList(LineSeparated):
-    """The upper letter list compositor.
-
-    Attributes:
-        _indexing: The class default indexing mode is "upper".
-
-    Example:
-        ```py
-        >>> with UpperLetterList():
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        A. item1
-        B. item2
-        ```
-    """
-
-    _indexing = Indexing("upper")
-
-
-class LowerRomanList(LineSeparated):
-    """The lower roman list compositor.
-
-    Attributes:
-        _indexing: The class default indexing mode is "roman".
-
-    Example:
-        ```py
-        >>> with LowerRomanList():
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        i. item1
-        ii. item2
-        ```
-    """
-
-    _indexing = Indexing("roman")
-
-
-class UpperRomanList(LineSeparated):
-    """The upper roman list compositor.
-
-    Attributes:
-        _indexing: The class default indexing mode is "Roman".
-
-    Example:
-        ```py
-        >>> with UpperRomanList():
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        I. item1
-        II. item2
-        ```
-    """
-
-    _indexing = Indexing("Roman")
-
-
-class DashList(LineSeparated):
-    """The dash list compositor.
-
-    Attributes:
-        _indexing: The class default indexing mode is "dash".
-
-    Example:
-        ```py
-        >>> with DashList():
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        - item1
-        - item2
-        ```
-    """
-
-    _indexing = Indexing("dash")
-
-
-class StarList(LineSeparated):
-    """The star list compositor.
-
-    Attributes:
-        _indexing: The class default indexing mode is "star".
-
-    Example:
-        ```py
-        >>> with StarList():
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        * item1
-        * item2
-        ```
-    """
-
-    _indexing = Indexing("star")
-
-
-LetterList = UpperLetterList
-"""The alias of UpperLetterList."""
-RomanList = UpperRomanList
-"""The alias of UpperRomanList."""
-
-
-class Logged(LineSeparated):
-    """The logged compositor, which is used to wrap the content with logs.
-
-    Note the indent will also apply to the prolog and epilog.
-
-    Attributes:
-        _indent_inside:
-            The class default indentation inside prolog and epilog is "".
-
-    Example:
-        ```py
-        >>> with Logged(prolog="BEGIN", epilog="END"):
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        BEGIN
-        item1
-        item2
-        END
-    """
-
-    _indent_inside: Optional[str] = ""
-
-    def __init__(
-        self,
-        *args: Any,
-        prolog: str,
-        epilog: str,
-        indent_inside: Union[str, int, None] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize the logged compositor.
-
-        Args:
-            *args: The arguments.
-            prolog: The prolog string.
-            epilog: The epilog string.
-            indent_inside: The indentation inside the prolog and epilog.
-            **kwargs: The keyword arguments.
-        """
-        self._prolog = prolog
-        self._epilog = epilog
-        if isinstance(indent_inside, int):
-            indent_inside = " " * indent_inside
-        if indent_inside is not None:
-            if self._indent_inside is None:
-                raise ValueError(
-                    "Indentation inside is not allowed for this compositor."
-                )
-            self._indent_inside = indent_inside
-        outer_indent = kwargs.pop("indent", None)
-        super().__init__(indent=outer_indent, _ctx=kwargs.get("_ctx"))
-        kwargs = self._get_kwargs_for_inner(kwargs)
-        # The arguments are passed to the inner compositor
-        self._indent_compositor = LineSeparated(*args, **kwargs)
-
-    @property
-    def prolog(self) -> str:
-        """The prolog string."""
-        return self._prolog
-
-    @property
-    def epilog(self) -> str:
-        """The epilog string."""
-        return self._epilog
-
-    def _get_kwargs_for_inner(self, kwargs: Dict[str, Any]) -> Dict[str, Any]:
-        kwargs["indent"] = self._indent_inside
-        return kwargs
-
-    def _enter(self) -> None:
-        super()._enter()
-        if self._ctx is not None:
-            self._ctx.add_string(self.prolog)
-            self._indent_compositor.__enter__()
-
-    def _exit(
-        self,
-        _exc_type: Optional[type[BaseException]],
-        _exc_value: Optional[BaseException],
-        _traceback: Optional[TracebackType],
-    ) -> Optional[bool]:
-        if not _exc_type:
-            if self._ctx is not None:
-                self._indent_compositor.__exit__(None, None, None)
-                self._ctx.add_string(self.epilog)
-        else:
-            if self._ctx is not None:
-                self._indent_compositor.__exit__(_exc_type, _exc_value, _traceback)
-        return super()._exit(_exc_type, _exc_value, _traceback)
-
-
-class Tagged(Logged):
-    """The tagged compositor, which is used to wrap the content with a tag.
-
-    Note the indent will also applyt to the tag indicator.
-
-    Attributes:
-        _indent_inside:
-            The class default indentation inside prolog and epilog is 4 spaces.
-
-    Example:
-        ```py
-        >>> with Tagged("div"):
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        <div>
-            item1
-            item2
-        </div>
-        ```
-    """
-
-    _indent_inside: Optional[str] = INDENT
-
-    def __init__(
-        self,
-        tag: str,
-        *args: Any,
-        attrs: Optional[Dict[str, str]] = None,
-        tag_begin: str = "<{}{}>",
-        tag_end: str = "</{}>",
-        indent_inside: Union[str, int, None] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize the tagged compositor.
-
-        Args:
-            tag: The tag name.
-            *args: The arguments.
-            attrs: The attributes of the tag.
-            tag_begin: The format of tag begin string.
-            tag_end: The format of tag end string.
-            indent_inside: The indentation inside the tag.
-            **kwargs: The keyword arguments.
-        """
-        self._tag = tag
-        self._attrs = attrs
-        self._tag_begin = tag_begin
-        self._tag_end = tag_end
-        prolog = tag_begin.format(tag, self.formated_attrs)
-        epilog = tag_end.format(tag)
-        super().__init__(
-            *args, prolog=prolog, epilog=epilog, indent_inside=indent_inside, **kwargs
-        )
-
-    @property
-    def formated_attrs(self) -> str:
-        """The formatted attributes of the tag."""
-        if self._attrs is None:
-            return ""
-        return " " + " ".join(f'{k}="{v}"' for k, v in self._attrs.items())
-
-
-class InlineTagged(Tagged):
-    """The inline tagged compositor, which is used to wrap the content with a tag.
-
-    Attributes:
-        _sep: The class default separator is "".
-        _indexing: The class default indexing mode is no indexing.
-        _new_indent: The class default indentation is "".
-        _is_inline: The class default is True.
-        _indent_inside: This class does not support indentation inside.
-
-    Example:
-        ```py
-        >>> with InlineTagged("div", sep=","):
-        ...     "item1"
-        ...     "item2"
-        <<< The prompt will be:
-        <div>item1,item2</div>
-        ```
-    """
-
-    def _get_kwargs_for_inner(self, kwargs: Dict[str, Any]) -> Dict[str, Any]:
-        # pass the arguments to the inner compositor
-        kwargs["sep"] = kwargs.get("sep", self._sep)
-        kwargs["indexing"] = kwargs.get("indexing", self._indexing)
-        kwargs["new_indent"] = self._new_indent
-        kwargs["is_inline"] = self._is_inline
-        return kwargs
-
-    _sep = ""
-    _indexing = Indexing()
-    _new_indent = ""
-    _is_inline = True
-    _indent_inside: Optional[str] = None
-
-
-@need_ctx
-def iter(
-    lst: Iterable,
-    comp: Optional[Compositor] = None,
-    _ctx: Optional[PromptContext] = None,
-) -> Iterable:
-    """Iterate over the iterable list with the compositor.
-
-    Example:
-        ```py
-        >>> items = ["item1", "item2"]
-        >>> for i in iter(items, NumberedList()):
-        ...     i
-        <<< The prompt will be:
-        1. item1
-        2. item2
-        ```
-    """
-    # support tqdm-like context manager
-    if comp is None:
-        comp = NumberedList(_ctx=_ctx)
-
-    entered = False
-    try:
-        for i in lst:
-            if not entered:
-                entered = True
-                comp.__enter__()
-            yield i
-    except Exception as e:
-        # TODO: check the impl here
-        if entered:
-            if not comp.__exit__(type(e), e, e.__traceback__):
-                raise e
-        else:
-            raise e
-    finally:
-        if entered:
-            comp.__exit__(None, None, None)
+"""Containg the compositor classes.
+
+All examples shows the composed prompt in APPL functions.
+"""
+
+from __future__ import annotations
+
+from appl.types import Any, Dict
+
+from .const import INDENT4 as INDENT
+from .core import ApplStr, Compositor, Indexing, PromptContext
+from .func import need_ctx
+from .types import *
+
+
+class LineSeparated(Compositor):
+    r"""The line separated compositor.
+
+    Attributes:
+        _sep: The class default separator is "\n".
+
+    Example:
+        ```py
+        >>> with LineSeparated():
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        item1
+        item2
+        ```
+    """
+
+    _sep = "\n"
+
+
+class DoubleLineSeparated(Compositor):
+    r"""The double line separated compositor.
+
+    Attributes:
+        _sep: The class default separator is "\n\n".
+
+    Example:
+        ```py
+        >>> with DoubleLineSeparated():
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        item1
+
+        item2
+        ```
+    """
+
+    _sep = "\n\n"
+
+
+class FreshLine(LineSeparated):
+    """Create a fresh line with no indent.
+
+    Attributes:
+        _inc_indent: The class default indentation is "".
+
+    Example:
+        ```py
+        >>> with FreshLine():
+        ...     EMPTY
+        <<< The prompt will be:
+        [indicates an empty line]
+        ```
+    """
+
+    _new_indent = ""
+
+
+class IndentedList(LineSeparated):
+    """The indented list compositor.
+
+    Attributes:
+        _inc_indent: The class default indentation is INDENT.
+
+    Example:
+        ```py
+        >>> "BEGIN"
+        ... with IndentedList():
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        BEGIN
+            item1
+            item2
+        ```
+    """
+
+    _inc_indent = INDENT
+
+
+class NumberedList(LineSeparated):
+    """The number list compositor.
+
+    Attributes:
+        _indexing: The class default indexing mode is "number".
+
+    Example:
+        ```py
+        >>> with NumberedList():
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        1. item1
+        2. item2
+        ```
+    """
+
+    _indexing = Indexing("number")
+
+
+class LowerLetterList(LineSeparated):
+    """The lower letter list compositor.
+
+    Attributes:
+        _indexing: The class default indexing mode is "lower".
+
+    Example:
+        ```py
+        >>> with LowerLetterList():
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        a. item1
+        b. item2
+        ```
+    """
+
+    _indexing = Indexing("lower")
+
+
+class UpperLetterList(LineSeparated):
+    """The upper letter list compositor.
+
+    Attributes:
+        _indexing: The class default indexing mode is "upper".
+
+    Example:
+        ```py
+        >>> with UpperLetterList():
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        A. item1
+        B. item2
+        ```
+    """
+
+    _indexing = Indexing("upper")
+
+
+class LowerRomanList(LineSeparated):
+    """The lower roman list compositor.
+
+    Attributes:
+        _indexing: The class default indexing mode is "roman".
+
+    Example:
+        ```py
+        >>> with LowerRomanList():
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        i. item1
+        ii. item2
+        ```
+    """
+
+    _indexing = Indexing("roman")
+
+
+class UpperRomanList(LineSeparated):
+    """The upper roman list compositor.
+
+    Attributes:
+        _indexing: The class default indexing mode is "Roman".
+
+    Example:
+        ```py
+        >>> with UpperRomanList():
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        I. item1
+        II. item2
+        ```
+    """
+
+    _indexing = Indexing("Roman")
+
+
+class DashList(LineSeparated):
+    """The dash list compositor.
+
+    Attributes:
+        _indexing: The class default indexing mode is "dash".
+
+    Example:
+        ```py
+        >>> with DashList():
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        - item1
+        - item2
+        ```
+    """
+
+    _indexing = Indexing("dash")
+
+
+class StarList(LineSeparated):
+    """The star list compositor.
+
+    Attributes:
+        _indexing: The class default indexing mode is "star".
+
+    Example:
+        ```py
+        >>> with StarList():
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        * item1
+        * item2
+        ```
+    """
+
+    _indexing = Indexing("star")
+
+
+LetterList = UpperLetterList
+"""The alias of UpperLetterList."""
+RomanList = UpperRomanList
+"""The alias of UpperRomanList."""
+
+
+class Logged(LineSeparated):
+    """The logged compositor, which is used to wrap the content with logs.
+
+    Note the indent will also apply to the prolog and epilog.
+
+    Attributes:
+        _indent_inside:
+            The class default indentation inside prolog and epilog is "".
+
+    Example:
+        ```py
+        >>> with Logged(prolog="BEGIN", epilog="END"):
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        BEGIN
+        item1
+        item2
+        END
+    """
+
+    _indent_inside: Optional[str] = ""
+
+    def __init__(
+        self,
+        *args: Any,
+        prolog: str,
+        epilog: str,
+        indent_inside: Union[str, int, None] = None,
+        **kwargs: Any,
+    ) -> None:
+        """Initialize the logged compositor.
+
+        Args:
+            *args: The arguments.
+            prolog: The prolog string.
+            epilog: The epilog string.
+            indent_inside: The indentation inside the prolog and epilog.
+            **kwargs: The keyword arguments.
+        """
+        self._prolog = prolog
+        self._epilog = epilog
+        if isinstance(indent_inside, int):
+            indent_inside = " " * indent_inside
+        if indent_inside is not None:
+            if self._indent_inside is None:
+                raise ValueError(
+                    "Indentation inside is not allowed for this compositor."
+                )
+            self._indent_inside = indent_inside
+        outer_indent = kwargs.pop("indent", None)
+        super().__init__(indent=outer_indent, _ctx=kwargs.get("_ctx"))
+        kwargs = self._get_kwargs_for_inner(kwargs)
+        # The arguments are passed to the inner compositor
+        self._indent_compositor = LineSeparated(*args, **kwargs)
+
+    @property
+    def prolog(self) -> str:
+        """The prolog string."""
+        return self._prolog
+
+    @property
+    def epilog(self) -> str:
+        """The epilog string."""
+        return self._epilog
+
+    def _get_kwargs_for_inner(self, kwargs: Dict[str, Any]) -> Dict[str, Any]:
+        kwargs["indent"] = self._indent_inside
+        return kwargs
+
+    def _enter(self) -> None:
+        super()._enter()
+        if self._ctx is not None:
+            self._ctx.add_string(self.prolog)
+            self._indent_compositor.__enter__()
+
+    def _exit(
+        self,
+        _exc_type: Optional[type[BaseException]],
+        _exc_value: Optional[BaseException],
+        _traceback: Optional[TracebackType],
+    ) -> Optional[bool]:
+        if not _exc_type:
+            if self._ctx is not None:
+                self._indent_compositor.__exit__(None, None, None)
+                self._ctx.add_string(self.epilog)
+        else:
+            if self._ctx is not None:
+                self._indent_compositor.__exit__(_exc_type, _exc_value, _traceback)
+        return super()._exit(_exc_type, _exc_value, _traceback)
+
+
+class Tagged(Logged):
+    """The tagged compositor, which is used to wrap the content with a tag.
+
+    Note the indent will also applyt to the tag indicator.
+
+    Attributes:
+        _indent_inside:
+            The class default indentation inside prolog and epilog is 4 spaces.
+
+    Example:
+        ```py
+        >>> with Tagged("div"):
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        <div>
+            item1
+            item2
+        </div>
+        ```
+    """
+
+    _indent_inside: Optional[str] = INDENT
+
+    def __init__(
+        self,
+        tag: str,
+        *args: Any,
+        attrs: Optional[Dict[str, str]] = None,
+        tag_begin: str = "<{}{}>",
+        tag_end: str = "</{}>",
+        indent_inside: Union[str, int, None] = None,
+        **kwargs: Any,
+    ) -> None:
+        """Initialize the tagged compositor.
+
+        Args:
+            tag: The tag name.
+            *args: The arguments.
+            attrs: The attributes of the tag.
+            tag_begin: The format of tag begin string.
+            tag_end: The format of tag end string.
+            indent_inside: The indentation inside the tag.
+            **kwargs: The keyword arguments.
+        """
+        self._tag = tag
+        self._attrs = attrs
+        self._tag_begin = tag_begin
+        self._tag_end = tag_end
+        prolog = tag_begin.format(tag, self.formated_attrs)
+        epilog = tag_end.format(tag)
+        super().__init__(
+            *args, prolog=prolog, epilog=epilog, indent_inside=indent_inside, **kwargs
+        )
+
+    @property
+    def formated_attrs(self) -> str:
+        """The formatted attributes of the tag."""
+        if self._attrs is None:
+            return ""
+        return " " + " ".join(f'{k}="{v}"' for k, v in self._attrs.items())
+
+
+class InlineTagged(Tagged):
+    """The inline tagged compositor, which is used to wrap the content with a tag.
+
+    Attributes:
+        _sep: The class default separator is "".
+        _indexing: The class default indexing mode is no indexing.
+        _new_indent: The class default indentation is "".
+        _is_inline: The class default is True.
+        _indent_inside: This class does not support indentation inside.
+
+    Example:
+        ```py
+        >>> with InlineTagged("div", sep=","):
+        ...     "item1"
+        ...     "item2"
+        <<< The prompt will be:
+        <div>item1,item2</div>
+        ```
+    """
+
+    def _get_kwargs_for_inner(self, kwargs: Dict[str, Any]) -> Dict[str, Any]:
+        # pass the arguments to the inner compositor
+        kwargs["sep"] = kwargs.get("sep", self._sep)
+        kwargs["indexing"] = kwargs.get("indexing", self._indexing)
+        kwargs["new_indent"] = self._new_indent
+        kwargs["is_inline"] = self._is_inline
+        return kwargs
+
+    _sep = ""
+    _indexing = Indexing()
+    _new_indent = ""
+    _is_inline = True
+    _indent_inside: Optional[str] = None
+
+
+@need_ctx
+def iter(
+    lst: Iterable,
+    comp: Optional[Compositor] = None,
+    _ctx: Optional[PromptContext] = None,
+) -> Iterable:
+    """Iterate over the iterable list with the compositor.
+
+    Example:
+        ```py
+        >>> items = ["item1", "item2"]
+        >>> for i in iter(items, NumberedList()):
+        ...     i
+        <<< The prompt will be:
+        1. item1
+        2. item2
+        ```
+    """
+    # support tqdm-like context manager
+    if comp is None:
+        comp = NumberedList(_ctx=_ctx)
+
+    entered = False
+    try:
+        for i in lst:
+            if not entered:
+                entered = True
+                comp.__enter__()
+            yield i
+    except Exception as e:
+        # TODO: check the impl here
+        if entered:
+            if not comp.__exit__(type(e), e, e.__traceback__):
+                raise e
+        else:
+            raise e
+    finally:
+        if entered:
+            comp.__exit__(None, None, None)
```

### Comparing `applang-0.0.1a3/src/appl/core/__init__.py` & `applang-0.0.1a4/src/appl/core/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from .compile import appl_compile
-from .config import configs
-from .context import PromptContext
-from .function import PromptFunc
-from .generation import Generation
-from .globals import global_vars
-from .io import *
-from .message import *
-from .modifiers import ApplStr, Compositor
-from .printer import (
-    Indexing,
-    PrinterPop,
-    PrinterPush,
-    PrinterState,
-    PromptPrinter,
-    PromptRecords,
-)
-from .promptable import BracketedDefinition, Definition, Promptable, define, promptify
-from .response import CompletionResponse
-from .runtime import appl_execute, appl_format, appl_with_ctx
-from .server import BaseServer, GenArgs
-from .tool import BaseTool, Tool
+from .compile import appl_compile
+from .config import configs
+from .context import PromptContext
+from .function import PromptFunc
+from .generation import Generation
+from .globals import global_vars
+from .io import *
+from .message import *
+from .modifiers import ApplStr, Compositor
+from .printer import (
+    Indexing,
+    PrinterPop,
+    PrinterPush,
+    PrinterState,
+    PromptPrinter,
+    PromptRecords,
+)
+from .promptable import BracketedDefinition, Definition, Promptable, define, promptify
+from .response import CompletionResponse
+from .runtime import appl_execute, appl_format, appl_with_ctx
+from .server import BaseServer, GenArgs
+from .tool import BaseTool, Tool
```

### Comparing `applang-0.0.1a3/src/appl/core/compile.py` & `applang-0.0.1a4/src/appl/core/compile.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,344 +1,344 @@
-from __future__ import annotations
-
-import ast
-import inspect
-import linecache
-import sys
-import textwrap
-import traceback
-from ast import (
-    AST,
-    Assign,
-    Attribute,
-    Call,
-    Constant,
-    Expr,
-    FormattedValue,
-    FunctionDef,
-    JoinedStr,
-    Load,
-    Name,
-    NamedExpr,
-    NodeTransformer,
-    Store,
-    With,
-    stmt,
-)
-
-from .context import PromptContext
-from .types import *
-
-GLOBALS_KEYWORD = ast.keyword(
-    arg="_globals",
-    value=Call(func=Name(id="globals", ctx=Load()), args=[], keywords=[]),
-)
-LOCALS_KEYWORD = ast.keyword(
-    arg="_locals",
-    value=Call(func=Name(id="locals", ctx=Load()), args=[], keywords=[]),
-)
-CTX_KEYWORD = ast.keyword(arg="_ctx", value=Name(id="_ctx", ctx=Load()))
-CTX_ARG = ast.arg(arg="_ctx", annotation=Name(id="PromptContext", ctx=Load()))
-
-
-def _has_arg(args: Union[List[ast.arg], List[ast.keyword]], name: str) -> bool:
-    return any(
-        isinstance(arg, (ast.arg, ast.keyword)) and arg.arg == name for arg in args
-    )
-
-
-class ApplNodeTransformer(NodeTransformer):
-    """A base class for AST node transformers in APPL."""
-
-    def __init__(self, compile_info: Dict, *args: Any, **kwargs: Any) -> None:
-        """Initialize the transformer with compile info."""
-        super().__init__(*args, **kwargs)
-        self._compile_info = compile_info
-
-    def _raise_syntax_error(self, lineno: int, col_offset: int, msg: str) -> None:
-        file = self._compile_info["sourcefile"]
-        lineno = lineno + self._compile_info["lineno"] - 1
-        text = linecache.getline(file, lineno)
-        raise SyntaxError(msg, (file, lineno, col_offset, text))
-
-
-class RemoveApplDecorator(ApplNodeTransformer):
-    """An AST node transformer that removes the ppl decorator."""
-
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
-        """Initialize the transformer with the outmost flag."""
-        super().__init__(*args, **kwargs)
-        self._outmost = True
-
-    def _is_ppl_decorator(self, decorator: AST) -> bool:
-        if isinstance(decorator, Name):
-            return decorator.id == "ppl"
-        elif isinstance(decorator, Call):
-            if isinstance(func := decorator.func, Name):
-                return func.id == "ppl"
-        return False  # pragma: no cover
-
-    def visit_FunctionDef(self, node):
-        """Remove the ppl decorator from the function definition."""
-        if node.decorator_list:
-            for decorator in node.decorator_list:
-                if self._is_ppl_decorator(decorator):
-                    if not self._outmost:
-                        self._raise_syntax_error(
-                            decorator.lineno,
-                            decorator.col_offset,
-                            "Nested ppl decorator is not allowed yet for APPL.",
-                        )
-            # all decorators should be removed
-            node.decorator_list = []
-        if self._outmost:
-            self._outmost = False
-        self.generic_visit(node)
-        return node
-
-
-class SplitString(ApplNodeTransformer):
-    """An AST node transformer that splits the f-string into multiple parts."""
-
-    def _add_formatted_value(self, node: FormattedValue) -> Iterable[stmt]:
-        format_args = [node.value]
-        if node.format_spec is not None:
-            format_args.append(node.format_spec)
-        format_keywords = []
-        if node.conversion != -1:
-            # add conversion
-            format_keywords.append(
-                ast.keyword(arg="conversion", value=Constant(node.conversion))
-            )
-        expr = Call(
-            func=Attribute(
-                value=Name(id="appl", ctx=Load()),
-                attr="format",
-                ctx=Load(),
-            ),
-            args=format_args,
-            keywords=format_keywords,
-        )
-        # converted to `appl.format(value, format_spec)`
-        default_result: Iterable[stmt] = [Expr(expr)]
-        if isinstance(node.value, NamedExpr):
-            return default_result
-
-        if spec := node.format_spec:
-            spec_str = ast.unparse(spec)
-            # logger.debug(spec_str)
-            if spec_str and spec_str[2] == "=":  # f"= ..."
-                self._raise_syntax_error(
-                    node.lineno,
-                    node.col_offset,
-                    "Not supported format of named expression inside f-string. "
-                    "To use named expression, please add brackets around "
-                    f"`{ast.unparse(node)[3:-2]}`.",
-                )
-        return default_result
-
-    def visit_Expr(self, node: Expr) -> stmt:
-        """Split the f-string into multiple parts, so that we can add appl.execute wrapper to each part."""
-        if isinstance(node.value, JoinedStr):
-            fstring = node.value
-            # logger.debug(f"For joined string: {fstring}")
-            body: List[stmt] = []
-            for value in fstring.values:
-                if isinstance(value, Constant):
-                    body.append(Expr(value))
-                elif isinstance(value, FormattedValue):
-                    body.extend(self._add_formatted_value(value))
-                else:
-                    raise ValueError(
-                        f"Unknown value type in a JoinedStr: {type(value)}"
-                    )
-            if len(body) == 0:  # empty string
-                return node
-            if len(body) == 1:  # single string
-                return body[0]
-            return With(
-                items=[
-                    ast.withitem(
-                        context_expr=Call(
-                            func=Attribute(
-                                value=Name(id="appl", ctx=Load()),
-                                attr="Str",
-                                ctx=Load(),
-                            ),
-                            args=[],
-                            keywords=[],
-                        )
-                    )
-                ],
-                body=body,
-            )
-        return node
-
-
-class CallWithContext(ApplNodeTransformer):
-    """An AST node transformer provides the context to function calls."""
-
-    def visit_Call(self, node: Call) -> Call:
-        """Provide context (_ctx) to function calls that needs ctx."""
-        self.generic_visit(node)
-        # logger.debug(f"visit Call: {ast.dump(node, indent=4)}")
-        # * use appl.with_ctx as wrapper for all functions,
-        # * pass _ctx to the function annotated with @need_ctx
-        new_node = Call(
-            Attribute(
-                value=Name(id="appl", ctx=Load()),
-                attr="with_ctx",
-                ctx=Load(),
-            ),
-            node.args,
-            node.keywords,
-        )
-        new_node.keywords.append(ast.keyword(arg="_func", value=node.func))
-        # add _ctx to kwargs if not present
-        if not _has_arg(node.keywords, "_ctx"):
-            new_node.keywords.append(CTX_KEYWORD)
-        new_node.keywords.append(GLOBALS_KEYWORD)
-        new_node.keywords.append(LOCALS_KEYWORD)
-        return new_node
-
-
-class AddCtxToArgs(ApplNodeTransformer):
-    """An AST node transformer that adds _ctx to the function arguments."""
-
-    def visit_FunctionDef(self, node: FunctionDef) -> FunctionDef:
-        """Add _ctx to the function arguments if not present."""
-        # ! only add _ctx to outermost function def, not call generic_visit here.
-        # self.generic_visit(node) # !! do not call
-        args = node.args
-        # add _ctx to kwargs if not present
-        if not _has_arg(args.args, "_ctx") and not _has_arg(args.kwonlyargs, "_ctx"):
-            args.kwonlyargs.append(CTX_ARG)
-            # PromptContext() as default
-            args.kw_defaults.append(
-                Call(func=Name(id="PromptContext", ctx=Load()), args=[], keywords=[])
-            )
-        for var in self._compile_info["freevars"]:
-            args.kwonlyargs.append(ast.arg(arg=var))
-            args.kw_defaults.append(ast.Name(id=var, ctx=Load()))
-            logger.debug(f"add freevar {var} to function {node.name} args.")
-        return node
-
-
-class AddExecuteWrapper(ApplNodeTransformer):
-    """An AST node transformer that adds the appl.execute wrapper to expression statements."""
-
-    def visit_Expr(self, node: Expr) -> Expr:
-        """Add appl.execute wrapper to expression statements."""
-        return Expr(
-            Call(
-                func=Attribute(
-                    value=Name(id="appl", ctx=Load()),
-                    attr="execute",
-                    ctx=Load(),
-                ),
-                args=[node.value],
-                keywords=[CTX_KEYWORD],  # , GLOBALS_KEYWORD, LOCALS_KEYWORD],
-            )
-        )
-
-
-class APPLCompiled:
-    """A compiled APPL function that can be called with context."""
-
-    def __init__(
-        self, code: CodeType, ast: AST, original_func: Callable, compile_info: Dict
-    ):
-        """Initialize the compiled function.
-
-        Args:
-            code: The compiled code object.
-            ast: The AST of the compiled code.
-            original_func: The original function.
-            compile_info: The compile information.
-        """
-        self._code = code
-        self._ast = ast
-        self._name = original_func.__name__
-        self._original_func = original_func
-        self._compile_info = compile_info
-
-    @property
-    def freevars(self) -> Tuple[str, ...]:
-        """Get the free variables of the compiled function."""
-        if "freevars" in self._compile_info:
-            return self._compile_info["freevars"]
-        return self._original_func.__code__.co_freevars
-
-    def __call__(
-        self,
-        *args: Any,
-        _globals: Optional[Dict] = None,
-        _locals: Dict = {},
-        **kwargs: Any,
-    ) -> Any:
-        """Call the compiled function."""
-        _globals = _globals or self._original_func.__globals__
-        local_vars = {"PromptContext": PromptContext}
-        # get closure variables from locals
-        for name in self.freevars:
-            if name in _locals:
-                # set the closure variables to local_vars
-                local_vars[name] = _locals[name]
-            else:
-                raise ValueError(
-                    f"Freevar '{name}' not found. If you are using closure variables, "
-                    "please provide their values in the _locals argument. "
-                    "For example, assume the function is `func`, use `func(..., _locals=locals())`. "
-                    "Alternatively, you can first use the `appl.as_func` to convert the "
-                    "function within the current scope (automatically feeding the locals)."
-                )
-
-        exec(self._code, _globals, local_vars)
-        func = local_vars[self._name]
-        return func(*args, **kwargs)
-
-    def __repr__(self):
-        return f"APPLCompiled({self._name})"
-
-
-def appl_compile(func: Callable) -> APPLCompiled:
-    """Compile an APPL function."""
-    sourcefile = inspect.getsourcefile(func)
-    lines, lineno = inspect.getsourcelines(func)
-    source = textwrap.dedent(inspect.getsource(func))
-    key = f"<appl-compiled:{sourcefile}:{lineno}>"
-    linecache.cache[key] = (
-        len(source),
-        None,
-        [line + "\n" for line in source.splitlines()],
-        key,
-    )
-
-    parsed_ast = ast.parse(source)
-    logger.debug(
-        f"\n{'-'*20} code BEFORE appl compile {'-'*20}\n{ast.unparse(parsed_ast)}"
-    )
-
-    transformers = [
-        RemoveApplDecorator,
-        SplitString,
-        CallWithContext,
-        AddCtxToArgs,
-        AddExecuteWrapper,
-    ]
-    compile_info = {
-        "source": source,
-        "sourcefile": sourcefile,
-        "lineno": lineno,
-        "func_name": func.__name__,
-        "freevars": func.__code__.co_freevars,
-    }
-    for transformer in transformers:
-        parsed_ast = transformer(compile_info).visit(parsed_ast)
-
-    parsed_ast = ast.fix_missing_locations(parsed_ast)
-    compiled_ast = compile(parsed_ast, filename=key, mode="exec")
-    logger.debug(
-        f"\n{'-'*20} code AFTER appl compile {'-'*20}\n{ast.unparse(parsed_ast)}"
-    )
-
-    return APPLCompiled(compiled_ast, parsed_ast, func, compile_info)
+from __future__ import annotations
+
+import ast
+import inspect
+import linecache
+import sys
+import textwrap
+import traceback
+from ast import (
+    AST,
+    Assign,
+    Attribute,
+    Call,
+    Constant,
+    Expr,
+    FormattedValue,
+    FunctionDef,
+    JoinedStr,
+    Load,
+    Name,
+    NamedExpr,
+    NodeTransformer,
+    Store,
+    With,
+    stmt,
+)
+
+from .context import PromptContext
+from .types import *
+
+GLOBALS_KEYWORD = ast.keyword(
+    arg="_globals",
+    value=Call(func=Name(id="globals", ctx=Load()), args=[], keywords=[]),
+)
+LOCALS_KEYWORD = ast.keyword(
+    arg="_locals",
+    value=Call(func=Name(id="locals", ctx=Load()), args=[], keywords=[]),
+)
+CTX_KEYWORD = ast.keyword(arg="_ctx", value=Name(id="_ctx", ctx=Load()))
+CTX_ARG = ast.arg(arg="_ctx", annotation=Name(id="PromptContext", ctx=Load()))
+
+
+def _has_arg(args: Union[List[ast.arg], List[ast.keyword]], name: str) -> bool:
+    return any(
+        isinstance(arg, (ast.arg, ast.keyword)) and arg.arg == name for arg in args
+    )
+
+
+class ApplNodeTransformer(NodeTransformer):
+    """A base class for AST node transformers in APPL."""
+
+    def __init__(self, compile_info: Dict, *args: Any, **kwargs: Any) -> None:
+        """Initialize the transformer with compile info."""
+        super().__init__(*args, **kwargs)
+        self._compile_info = compile_info
+
+    def _raise_syntax_error(self, lineno: int, col_offset: int, msg: str) -> None:
+        file = self._compile_info["sourcefile"]
+        lineno = lineno + self._compile_info["lineno"] - 1
+        text = linecache.getline(file, lineno)
+        raise SyntaxError(msg, (file, lineno, col_offset, text))
+
+
+class RemoveApplDecorator(ApplNodeTransformer):
+    """An AST node transformer that removes the ppl decorator."""
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        """Initialize the transformer with the outmost flag."""
+        super().__init__(*args, **kwargs)
+        self._outmost = True
+
+    def _is_ppl_decorator(self, decorator: AST) -> bool:
+        if isinstance(decorator, Name):
+            return decorator.id == "ppl"
+        elif isinstance(decorator, Call):
+            if isinstance(func := decorator.func, Name):
+                return func.id == "ppl"
+        return False  # pragma: no cover
+
+    def visit_FunctionDef(self, node):
+        """Remove the ppl decorator from the function definition."""
+        if node.decorator_list:
+            for decorator in node.decorator_list:
+                if self._is_ppl_decorator(decorator):
+                    if not self._outmost:
+                        self._raise_syntax_error(
+                            decorator.lineno,
+                            decorator.col_offset,
+                            "Nested ppl decorator is not allowed yet for APPL.",
+                        )
+            # all decorators should be removed
+            node.decorator_list = []
+        if self._outmost:
+            self._outmost = False
+        self.generic_visit(node)
+        return node
+
+
+class SplitString(ApplNodeTransformer):
+    """An AST node transformer that splits the f-string into multiple parts."""
+
+    def _add_formatted_value(self, node: FormattedValue) -> Iterable[stmt]:
+        format_args = [node.value]
+        if node.format_spec is not None:
+            format_args.append(node.format_spec)
+        format_keywords = []
+        if node.conversion != -1:
+            # add conversion
+            format_keywords.append(
+                ast.keyword(arg="conversion", value=Constant(node.conversion))
+            )
+        expr = Call(
+            func=Attribute(
+                value=Name(id="appl", ctx=Load()),
+                attr="format",
+                ctx=Load(),
+            ),
+            args=format_args,
+            keywords=format_keywords,
+        )
+        # converted to `appl.format(value, format_spec)`
+        default_result: Iterable[stmt] = [Expr(expr)]
+        if isinstance(node.value, NamedExpr):
+            return default_result
+
+        if spec := node.format_spec:
+            spec_str = ast.unparse(spec)
+            # logger.debug(spec_str)
+            if spec_str and spec_str[2] == "=":  # f"= ..."
+                self._raise_syntax_error(
+                    node.lineno,
+                    node.col_offset,
+                    "Not supported format of named expression inside f-string. "
+                    "To use named expression, please add brackets around "
+                    f"`{ast.unparse(node)[3:-2]}`.",
+                )
+        return default_result
+
+    def visit_Expr(self, node: Expr) -> stmt:
+        """Split the f-string into multiple parts, so that we can add appl.execute wrapper to each part."""
+        if isinstance(node.value, JoinedStr):
+            fstring = node.value
+            # logger.debug(f"For joined string: {fstring}")
+            body: List[stmt] = []
+            for value in fstring.values:
+                if isinstance(value, Constant):
+                    body.append(Expr(value))
+                elif isinstance(value, FormattedValue):
+                    body.extend(self._add_formatted_value(value))
+                else:
+                    raise ValueError(
+                        f"Unknown value type in a JoinedStr: {type(value)}"
+                    )
+            if len(body) == 0:  # empty string
+                return node
+            if len(body) == 1:  # single string
+                return body[0]
+            return With(
+                items=[
+                    ast.withitem(
+                        context_expr=Call(
+                            func=Attribute(
+                                value=Name(id="appl", ctx=Load()),
+                                attr="Str",
+                                ctx=Load(),
+                            ),
+                            args=[],
+                            keywords=[],
+                        )
+                    )
+                ],
+                body=body,
+            )
+        return node
+
+
+class CallWithContext(ApplNodeTransformer):
+    """An AST node transformer provides the context to function calls."""
+
+    def visit_Call(self, node: Call) -> Call:
+        """Provide context (_ctx) to function calls that needs ctx."""
+        self.generic_visit(node)
+        # logger.debug(f"visit Call: {ast.dump(node, indent=4)}")
+        # * use appl.with_ctx as wrapper for all functions,
+        # * pass _ctx to the function annotated with @need_ctx
+        new_node = Call(
+            Attribute(
+                value=Name(id="appl", ctx=Load()),
+                attr="with_ctx",
+                ctx=Load(),
+            ),
+            node.args,
+            node.keywords,
+        )
+        new_node.keywords.append(ast.keyword(arg="_func", value=node.func))
+        # add _ctx to kwargs if not present
+        if not _has_arg(node.keywords, "_ctx"):
+            new_node.keywords.append(CTX_KEYWORD)
+        new_node.keywords.append(GLOBALS_KEYWORD)
+        new_node.keywords.append(LOCALS_KEYWORD)
+        return new_node
+
+
+class AddCtxToArgs(ApplNodeTransformer):
+    """An AST node transformer that adds _ctx to the function arguments."""
+
+    def visit_FunctionDef(self, node: FunctionDef) -> FunctionDef:
+        """Add _ctx to the function arguments if not present."""
+        # ! only add _ctx to outermost function def, not call generic_visit here.
+        # self.generic_visit(node) # !! do not call
+        args = node.args
+        # add _ctx to kwargs if not present
+        if not _has_arg(args.args, "_ctx") and not _has_arg(args.kwonlyargs, "_ctx"):
+            args.kwonlyargs.append(CTX_ARG)
+            # PromptContext() as default
+            args.kw_defaults.append(
+                Call(func=Name(id="PromptContext", ctx=Load()), args=[], keywords=[])
+            )
+        for var in self._compile_info["freevars"]:
+            args.kwonlyargs.append(ast.arg(arg=var))
+            args.kw_defaults.append(ast.Name(id=var, ctx=Load()))
+            logger.debug(f"add freevar {var} to function {node.name} args.")
+        return node
+
+
+class AddExecuteWrapper(ApplNodeTransformer):
+    """An AST node transformer that adds the appl.execute wrapper to expression statements."""
+
+    def visit_Expr(self, node: Expr) -> Expr:
+        """Add appl.execute wrapper to expression statements."""
+        return Expr(
+            Call(
+                func=Attribute(
+                    value=Name(id="appl", ctx=Load()),
+                    attr="execute",
+                    ctx=Load(),
+                ),
+                args=[node.value],
+                keywords=[CTX_KEYWORD],  # , GLOBALS_KEYWORD, LOCALS_KEYWORD],
+            )
+        )
+
+
+class APPLCompiled:
+    """A compiled APPL function that can be called with context."""
+
+    def __init__(
+        self, code: CodeType, ast: AST, original_func: Callable, compile_info: Dict
+    ):
+        """Initialize the compiled function.
+
+        Args:
+            code: The compiled code object.
+            ast: The AST of the compiled code.
+            original_func: The original function.
+            compile_info: The compile information.
+        """
+        self._code = code
+        self._ast = ast
+        self._name = original_func.__name__
+        self._original_func = original_func
+        self._compile_info = compile_info
+
+    @property
+    def freevars(self) -> Tuple[str, ...]:
+        """Get the free variables of the compiled function."""
+        if "freevars" in self._compile_info:
+            return self._compile_info["freevars"]
+        return self._original_func.__code__.co_freevars
+
+    def __call__(
+        self,
+        *args: Any,
+        _globals: Optional[Dict] = None,
+        _locals: Dict = {},
+        **kwargs: Any,
+    ) -> Any:
+        """Call the compiled function."""
+        _globals = _globals or self._original_func.__globals__
+        local_vars = {"PromptContext": PromptContext}
+        # get closure variables from locals
+        for name in self.freevars:
+            if name in _locals:
+                # set the closure variables to local_vars
+                local_vars[name] = _locals[name]
+            else:
+                raise ValueError(
+                    f"Freevar '{name}' not found. If you are using closure variables, "
+                    "please provide their values in the _locals argument. "
+                    "For example, assume the function is `func`, use `func(..., _locals=locals())`. "
+                    "Alternatively, you can first use the `appl.as_func` to convert the "
+                    "function within the current scope (automatically feeding the locals)."
+                )
+
+        exec(self._code, _globals, local_vars)
+        func = local_vars[self._name]
+        return func(*args, **kwargs)
+
+    def __repr__(self):
+        return f"APPLCompiled({self._name})"
+
+
+def appl_compile(func: Callable) -> APPLCompiled:
+    """Compile an APPL function."""
+    sourcefile = inspect.getsourcefile(func)
+    lines, lineno = inspect.getsourcelines(func)
+    source = textwrap.dedent(inspect.getsource(func))
+    key = f"<appl-compiled:{sourcefile}:{lineno}>"
+    linecache.cache[key] = (
+        len(source),
+        None,
+        [line + "\n" for line in source.splitlines()],
+        key,
+    )
+
+    parsed_ast = ast.parse(source)
+    logger.debug(
+        f"\n{'-'*20} code BEFORE appl compile {'-'*20}\n{ast.unparse(parsed_ast)}"
+    )
+
+    transformers = [
+        RemoveApplDecorator,
+        SplitString,
+        CallWithContext,
+        AddCtxToArgs,
+        AddExecuteWrapper,
+    ]
+    compile_info = {
+        "source": source,
+        "sourcefile": sourcefile,
+        "lineno": lineno,
+        "func_name": func.__name__,
+        "freevars": func.__code__.co_freevars,
+    }
+    for transformer in transformers:
+        parsed_ast = transformer(compile_info).visit(parsed_ast)
+
+    parsed_ast = ast.fix_missing_locations(parsed_ast)
+    compiled_ast = compile(parsed_ast, filename=key, mode="exec")
+    logger.debug(
+        f"\n{'-'*20} code AFTER appl compile {'-'*20}\n{ast.unparse(parsed_ast)}"
+    )
+
+    return APPLCompiled(compiled_ast, parsed_ast, func, compile_info)
```

### Comparing `applang-0.0.1a3/src/appl/core/config.py` & `applang-0.0.1a4/src/appl/core/config.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import os
-
-import addict
-import yaml
-
-from .io import get_ext, load_file
-from .types import *
-
-DIR = os.path.dirname(os.path.abspath(__file__))
-DEFAULT_CONFIG_FILE = os.path.join(DIR, "..", "default_configs.yaml")
-
-
-class Configs(addict.Dict):
-    """A Dictionary class that allows for dot notation access to nested dictionaries."""
-
-    def getattrs(self, key: str, default: Any = None) -> Any:
-        """Get a value from a nested dictionary using a dot-separated key string."""
-        if "." in key:
-            keys = key.split(".")
-        else:
-            keys = [key]
-        prefix = "."
-        v = self
-        try:
-            for k in keys:
-                v = getattr(v, k)
-                prefix += k + "."
-            return v
-        except KeyError as e:
-            msg = f"{e} not found in prefix '{prefix}'"
-
-            if default is None:  # check if key exists in default configs
-                try:
-                    # fallback to default configs
-                    default = DEFAULT_CONFIGS.getattrs(key)
-                except Exception:
-                    pass
-
-            if default is not None:
-                logger.warning(f"{msg}, using default: {default}")
-                return default
-            logger.error(msg)
-            raise e
-
-    def to_yaml(self) -> str:
-        """Convert the Configs object to a YAML string."""
-        return yaml.dump(self.to_dict())
-
-    def __missing__(self, key: str) -> None:
-        raise KeyError(key)
-
-
-def load_config(file: str, *args: Any, **kwargs: Any) -> Configs:
-    """Load a config file and return the data as a dictionary."""
-    ext = get_ext(file)
-    if ext not in [".json", ".yaml", ".yml", ".toml"]:
-        raise ValueError(f"Unsupported config file type {ext}")
-    content = load_file(file, *args, **kwargs)
-    return Configs(content)
-
-
-DEFAULT_CONFIGS = load_config(DEFAULT_CONFIG_FILE)
-"""The static default configs loaded from the default config file."""
-# singleton
-configs = DEFAULT_CONFIGS.deepcopy()
-"""The global configs"""
+import os
+
+import addict
+import yaml
+
+from .io import get_ext, load_file
+from .types import *
+
+DIR = os.path.dirname(os.path.abspath(__file__))
+DEFAULT_CONFIG_FILE = os.path.join(DIR, "..", "default_configs.yaml")
+
+
+class Configs(addict.Dict):
+    """A Dictionary class that allows for dot notation access to nested dictionaries."""
+
+    def getattrs(self, key: str, default: Any = None) -> Any:
+        """Get a value from a nested dictionary using a dot-separated key string."""
+        if "." in key:
+            keys = key.split(".")
+        else:
+            keys = [key]
+        prefix = "."
+        v = self
+        try:
+            for k in keys:
+                v = getattr(v, k)
+                prefix += k + "."
+            return v
+        except KeyError as e:
+            msg = f"{e} not found in prefix '{prefix}'"
+
+            if default is None:  # check if key exists in default configs
+                try:
+                    # fallback to default configs
+                    default = DEFAULT_CONFIGS.getattrs(key)
+                except Exception:
+                    pass
+
+            if default is not None:
+                logger.warning(f"{msg}, using default: {default}")
+                return default
+            logger.error(msg)
+            raise e
+
+    def to_yaml(self) -> str:
+        """Convert the Configs object to a YAML string."""
+        return yaml.dump(self.to_dict())
+
+    def __missing__(self, key: str) -> None:
+        raise KeyError(key)
+
+
+def load_config(file: str, *args: Any, **kwargs: Any) -> Configs:
+    """Load a config file and return the data as a dictionary."""
+    ext = get_ext(file)
+    if ext not in [".json", ".yaml", ".yml", ".toml"]:
+        raise ValueError(f"Unsupported config file type {ext}")
+    content = load_file(file, *args, **kwargs)
+    return Configs(content)
+
+
+DEFAULT_CONFIGS = load_config(DEFAULT_CONFIG_FILE)
+"""The static default configs loaded from the default config file."""
+# singleton
+configs = DEFAULT_CONFIGS.deepcopy()
+"""The global configs"""
```

### Comparing `applang-0.0.1a3/src/appl/core/function.py` & `applang-0.0.1a4/src/appl/core/function.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-from __future__ import annotations
-
-import inspect
-import sys
-import time
-import traceback
-
-from . import trace
-from .compile import appl_compile
-from .context import PromptContext
-from .modifiers import Compositor
-from .types import *
-
-
-class PromptFunc:
-    """A wrapper for an APPL function, can be called as a normal function.
-
-    The function contains a prompt context, which could be same as or
-    copied from its caller function, or created from scratch, or resumed
-    from the last run.
-    """
-
-    def __init__(
-        self,
-        func: Callable,
-        ctx_method: str = "new",
-        comp: Optional[Compositor] = None,
-        default_return: Optional[Literal["prompt"]] = None,
-        exclude_first_str: bool = False,
-        new_ctx_func: Callable = PromptContext,
-        # default_sep: Optional[str] = None,
-        # ? set the default printer behavior for the prompt function?
-    ):
-        """Initialize the PromptFunc.
-
-        Args:
-            func (Callable): the function being wrapped
-            ctx_method (str):
-                the method to deal with the child context, available methods includes:
-
-                - (default) "new" or "new_ctx": create a brand new context.
-                - "copy" or "copy_ctx":
-                    copy from the parent's context, the change will not
-                    affect the parent's context.
-                - "same" or "same_ctx":
-                    use the same context as the parent's, the change will
-                    affect the parent's context.
-                - "resume" or "resume_ctx":
-                    resume its own context from the last run.
-                    For the first run, it will copy the parent's context.
-
-            comp (Compositor, optional):
-                the default compositor to be used. Defaults to None.
-            default_return (str, optional):
-                The default return value, "prompt" means return the prompt within
-                the function. Defaults to None.
-            exclude_first_str (bool, optional):
-                set to True to exclude the first string (liekly the docstring)
-                from the prompt. Defaults to False.
-            new_ctx_func (Callable, optional):
-                the function to create a new context. Defaults to PromptContext.
-        """
-        self._func = appl_compile(func)
-        self._signature = inspect.signature(func)
-        self._doc = func.__doc__
-        self._name = func.__name__
-        self._default_ctx_method = self._process_ctx_method(ctx_method)
-        self._default_compositor = comp
-        if default_return is not None and default_return != "prompt":
-            raise NotImplementedError("Only support default_return='prompt' now.")
-        self._default_return = default_return
-        self._exclude_first_str = exclude_first_str
-        self._new_ctx_func = new_ctx_func
-        self._persist_ctx: Optional[PromptContext] = None
-        self._run_cnt = 0
-        # self._default_sep = default_sep
-
-    @property
-    def compiled_func(self):
-        """The compiled function."""
-        return self._func
-
-    def _process_ctx_method(self, ctx_method: str) -> str:
-        available_methods = ["new", "copy", "same", "resume"]
-        alias = [m + "_ctx" for m in available_methods]
-        res = ctx_method
-        if res in alias:
-            res = available_methods[alias.index(ctx_method)]
-        if res not in available_methods:
-            raise ValueError(f"Unknown ctx_method: {ctx_method}")
-        return res
-
-    def _run(
-        self,
-        parent_ctx: PromptContext,
-        child_ctx: PromptContext,
-        *args: Any,
-        **kwargs: Any,
-    ) -> Any:
-        """Run the prompt function with desired context, deal with the exception."""
-        if parent_ctx.is_outmost:
-            exc = None
-            try:
-                results = self._func(_ctx=child_ctx, *args, **kwargs)
-            except Exception:
-                # if parent_ctx.is_outmost:  # only print the trace in outmost appl function
-                traceback.print_exc()
-                print()  # empty line
-                exc = sys.exc_info()
-
-            if exc is not None:  # the outmost appl function
-                _, e_instance, e_traceback = exc
-                # already printed above, clean up the traceback
-                if e_instance and e_traceback:
-                    e_traceback.tb_next = None
-                    raise e_instance.with_traceback(e_traceback)
-        else:  # run normally, capture the exception at the outmost appl function
-            results = self._func(_ctx=child_ctx, *args, **kwargs)
-        return results
-
-    def _call(
-        self, *args: Any, _ctx: Optional[PromptContext] = None, **kwargs: Any
-    ) -> Any:
-        """Call the prompt function."""
-        parent_ctx = _ctx or self._new_ctx_func()
-        is_class_method = kwargs.pop("_is_class_method", False)
-        ctx_method = kwargs.pop("ctx_method", self._default_ctx_method)
-        if ctx_method == "new":
-            child_ctx = self._new_ctx_func()
-        elif ctx_method == "copy":
-            child_ctx = parent_ctx.copy()
-        elif ctx_method == "same":
-            child_ctx = parent_ctx.inherit()
-        elif ctx_method == "resume":
-            if is_class_method:
-                self_or_cls = args[0]  # is it guaranteed? need double check
-                var_name = f"{self._name}_appl_ctx_"
-                # try to retrieve the context from the class
-                if (ctx := getattr(self_or_cls, var_name, None)) is None:
-                    # copy the parent context if not exist
-                    child_ctx = parent_ctx.copy()
-                    setattr(self_or_cls, var_name, child_ctx)
-                else:
-                    # resume from the last run, but with clean locals
-                    child_ctx = ctx.inherit()
-            else:
-                if self._persist_ctx is None:
-                    self._persist_ctx = parent_ctx
-                child_ctx = self._persist_ctx.inherit()
-        else:
-            raise ValueError(f"Unknown ctx_method: {ctx_method}")
-        child_ctx.is_outmost = False
-        child_ctx._exclude_first_str = self._exclude_first_str  # set in the context
-
-        compositor: Optional[Compositor] = kwargs.pop(
-            "compositor", self._default_compositor
-        )
-        # push the compositor
-        if compositor is not None:
-            child_ctx.push_printer(compositor.push_args)
-
-        # run the function
-        results = self._run(parent_ctx, child_ctx, *args, **kwargs)
-        if results is None and self._default_return == "prompt":
-            results = child_ctx.records  # the default return result
-
-        # pop the compositor
-        if compositor is not None:
-            child_ctx.pop_printer()
-
-        if ctx_method == "same":
-            parent_ctx.add_records(child_ctx.records, write_to_prompt=False)
-
-        return results
-
-    __call__ = _call
-
-    def __repr__(self):
-        res = f"[PromptFunc]{self._name}{self._signature}"
-        if self._doc is not None:
-            res += f": {self._doc}"
-        return res
+from __future__ import annotations
+
+import inspect
+import sys
+import time
+import traceback
+
+from . import trace
+from .compile import appl_compile
+from .context import PromptContext
+from .modifiers import Compositor
+from .types import *
+
+
+class PromptFunc:
+    """A wrapper for an APPL function, can be called as a normal function.
+
+    The function contains a prompt context, which could be same as or
+    copied from its caller function, or created from scratch, or resumed
+    from the last run.
+    """
+
+    def __init__(
+        self,
+        func: Callable,
+        ctx_method: str = "new",
+        comp: Optional[Compositor] = None,
+        default_return: Optional[Literal["prompt"]] = None,
+        exclude_first_str: bool = False,
+        new_ctx_func: Callable = PromptContext,
+        # default_sep: Optional[str] = None,
+        # ? set the default printer behavior for the prompt function?
+    ):
+        """Initialize the PromptFunc.
+
+        Args:
+            func (Callable): the function being wrapped
+            ctx_method (str):
+                the method to deal with the child context, available methods includes:
+
+                - (default) "new" or "new_ctx": create a brand new context.
+                - "copy" or "copy_ctx":
+                    copy from the parent's context, the change will not
+                    affect the parent's context.
+                - "same" or "same_ctx":
+                    use the same context as the parent's, the change will
+                    affect the parent's context.
+                - "resume" or "resume_ctx":
+                    resume its own context from the last run.
+                    For the first run, it will copy the parent's context.
+
+            comp (Compositor, optional):
+                the default compositor to be used. Defaults to None.
+            default_return (str, optional):
+                The default return value, "prompt" means return the prompt within
+                the function. Defaults to None.
+            exclude_first_str (bool, optional):
+                set to True to exclude the first string (liekly the docstring)
+                from the prompt. Defaults to False.
+            new_ctx_func (Callable, optional):
+                the function to create a new context. Defaults to PromptContext.
+        """
+        self._func = appl_compile(func)
+        self._signature = inspect.signature(func)
+        self._doc = func.__doc__
+        self._name = func.__name__
+        self._default_ctx_method = self._process_ctx_method(ctx_method)
+        self._default_compositor = comp
+        if default_return is not None and default_return != "prompt":
+            raise NotImplementedError("Only support default_return='prompt' now.")
+        self._default_return = default_return
+        self._exclude_first_str = exclude_first_str
+        self._new_ctx_func = new_ctx_func
+        self._persist_ctx: Optional[PromptContext] = None
+        self._run_cnt = 0
+        # self._default_sep = default_sep
+
+    @property
+    def compiled_func(self):
+        """The compiled function."""
+        return self._func
+
+    def _process_ctx_method(self, ctx_method: str) -> str:
+        available_methods = ["new", "copy", "same", "resume"]
+        alias = [m + "_ctx" for m in available_methods]
+        res = ctx_method
+        if res in alias:
+            res = available_methods[alias.index(ctx_method)]
+        if res not in available_methods:
+            raise ValueError(f"Unknown ctx_method: {ctx_method}")
+        return res
+
+    def _run(
+        self,
+        parent_ctx: PromptContext,
+        child_ctx: PromptContext,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Any:
+        """Run the prompt function with desired context, deal with the exception."""
+        if parent_ctx.is_outmost:
+            exc = None
+            try:
+                results = self._func(_ctx=child_ctx, *args, **kwargs)
+            except Exception:
+                # if parent_ctx.is_outmost:  # only print the trace in outmost appl function
+                traceback.print_exc()
+                print()  # empty line
+                exc = sys.exc_info()
+
+            if exc is not None:  # the outmost appl function
+                _, e_instance, e_traceback = exc
+                # already printed above, clean up the traceback
+                if e_instance and e_traceback:
+                    e_traceback.tb_next = None
+                    raise e_instance.with_traceback(e_traceback)
+        else:  # run normally, capture the exception at the outmost appl function
+            results = self._func(_ctx=child_ctx, *args, **kwargs)
+        return results
+
+    def _call(
+        self, *args: Any, _ctx: Optional[PromptContext] = None, **kwargs: Any
+    ) -> Any:
+        """Call the prompt function."""
+        parent_ctx = _ctx or self._new_ctx_func()
+        is_class_method = kwargs.pop("_is_class_method", False)
+        ctx_method = kwargs.pop("ctx_method", self._default_ctx_method)
+        if ctx_method == "new":
+            child_ctx = self._new_ctx_func()
+        elif ctx_method == "copy":
+            child_ctx = parent_ctx.copy()
+        elif ctx_method == "same":
+            child_ctx = parent_ctx.inherit()
+        elif ctx_method == "resume":
+            if is_class_method:
+                self_or_cls = args[0]  # is it guaranteed? need double check
+                var_name = f"{self._name}_appl_ctx_"
+                # try to retrieve the context from the class
+                if (ctx := getattr(self_or_cls, var_name, None)) is None:
+                    # copy the parent context if not exist
+                    child_ctx = parent_ctx.copy()
+                    setattr(self_or_cls, var_name, child_ctx)
+                else:
+                    # resume from the last run, but with clean locals
+                    child_ctx = ctx.inherit()
+            else:
+                if self._persist_ctx is None:
+                    self._persist_ctx = parent_ctx
+                child_ctx = self._persist_ctx.inherit()
+        else:
+            raise ValueError(f"Unknown ctx_method: {ctx_method}")
+        child_ctx.is_outmost = False
+        child_ctx._exclude_first_str = self._exclude_first_str  # set in the context
+
+        compositor: Optional[Compositor] = kwargs.pop(
+            "compositor", self._default_compositor
+        )
+        # push the compositor
+        if compositor is not None:
+            child_ctx.push_printer(compositor.push_args)
+
+        # run the function
+        results = self._run(parent_ctx, child_ctx, *args, **kwargs)
+        if results is None and self._default_return == "prompt":
+            results = child_ctx.records  # the default return result
+
+        # pop the compositor
+        if compositor is not None:
+            child_ctx.pop_printer()
+
+        if ctx_method == "same":
+            parent_ctx.add_records(child_ctx.records, write_to_prompt=False)
+
+        return results
+
+    __call__ = _call
+
+    def __repr__(self):
+        res = f"[PromptFunc]{self._name}{self._signature}"
+        if self._doc is not None:
+            res += f": {self._doc}"
+        return res
```

### Comparing `applang-0.0.1a3/src/appl/core/generation.py` & `applang-0.0.1a4/src/appl/core/generation.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-from __future__ import annotations
-
-import json
-import time
-
-from . import trace
-from .config import configs
-from .context import PromptContext
-from .globals import inc_global
-from .message import AIMessage, BaseMessage, ToolMessage
-from .promptable import Promptable
-from .response import CompletionResponse
-from .server import BaseServer, GenArgs
-from .tool import BaseTool, ToolCall
-from .trace import GenerationInitEvent, add_to_trace
-from .types import *
-
-
-class Generation:
-    """Represents a generation call to the model."""
-
-    def __init__(
-        self,
-        server: BaseServer,
-        args: GenArgs,
-        *,
-        mock_response: Optional[Union[CompletionResponse, str]] = None,
-        lazy_eval: bool = False,
-        _ctx: Optional[PromptContext] = None,
-        **kwargs: Any,
-        # kwargs used for extra args for the create method
-    ) -> None:
-        """Initialize the Generation object.
-
-        Args:
-            server: An LLM server where the generation request will be sent.
-            args: The arguments of the generation call.
-            mock_response: A mock response for the generation call.
-            lazy_eval: If True, the generation call will be evaluated lazily.
-            _ctx: The prompt context filled automatically by the APPL function.
-            **kwargs: Extra arguments for the generation call.
-        """
-        # name needs to be unique and ordered, so it has to be generated in the main thread
-        self._id = inc_global("gen_cnt") - 1  # take the value before increment
-
-        self._server = server
-        self._args = args
-        self._ctx = _ctx
-        self._extra_args = kwargs
-
-        add_to_trace(GenerationInitEvent(name=self.id))
-        if isinstance(mock_response, CompletionResponse):
-            self._call = lambda: mock_response
-        else:
-            if mock_response:
-                # use litellm's mock response
-                kwargs.update({"mock_response": mock_response})
-            # TODO: supports custom postprocessing messages
-            self._call = CallFuture(
-                self._server.create,
-                lazy_eval=lazy_eval,
-                args=args,
-                gen_id=self.id,
-                **kwargs,
-            )
-
-        # tools
-        self._tools: Sequence[BaseTool] = args.tools
-        self._name2tools = {tool.name: tool for tool in self._tools}
-
-    @property
-    def id(self) -> str:
-        """The unique ID of the generation."""
-        return f"@gen_{self._id}"
-
-    def __call__(self):
-        """Get the response of the generation call."""
-        return self._call()
-
-    @property
-    def response(self) -> CompletionResponse:
-        """The response of the generation call."""
-        # NOTE: the result of the call will be cached in the CallFuture
-        return self._call()
-
-    @property
-    def response_type(self) -> ResponseType:
-        """The type of the response."""
-        return self.response.type
-
-    @property
-    def is_message(self) -> bool:
-        """Whether the response is a text message."""
-        return self.response_type == ResponseType.TEXT
-
-    @property
-    def is_tool_call(self) -> bool:
-        """Whether the response is a tool call."""
-        return self.response_type == ResponseType.TOOL_CALL
-
-    @property
-    def is_obj(self) -> bool:
-        """Whether the response is an object."""
-        return self.response_type == ResponseType.OBJECT
-
-    @property
-    def message(self) -> Optional[str]:
-        """The message of the response."""
-        return self.response.message
-
-    @property
-    def tool_calls(self) -> List[ToolCall]:
-        """The tool calls of the response."""
-        return self.response.tool_calls
-
-    @property
-    def response_obj(self) -> Any:
-        """The object of the response."""
-        return self.response.response_obj
-
-    @property
-    def results(self) -> Any:
-        """The results of the response."""
-        return self.response.results
-
-    def _call_tool(
-        self, name: str, args: str, parallel: bool = False, use_process: bool = False
-    ) -> Any:
-        try:
-            kwargs = json.loads(args)
-        except json.JSONDecodeError as e:
-            raise ValueError(f"Error parsing args: {args}") from e
-        args_str = ", ".join([f"{k}={v}" for k, v in kwargs.items()])
-        if configs.getattrs("settings.logging.display.tool_calls"):
-            logger.info(f"Running tool call: {name}({args_str})")
-
-        if name not in self._name2tools:
-            raise ValueError(f"Error: Tool {name} not found")
-        tool = self._name2tools[name]
-        try:
-            if parallel:
-                res = CallFuture(tool, use_process=use_process, **kwargs)
-            else:
-                res = tool(**kwargs)
-        except Exception as e:
-            raise RuntimeError(f"Error running tool call: {name}({args_str})") from e
-
-        return res
-
-    def run_tool_calls(
-        self,
-        filter_fn: Optional[Callable[[List[ToolCall]], List[ToolCall]]] = None,
-        parallel: bool = False,
-        use_process: bool = False,
-        log_results: Optional[bool] = None,
-    ) -> List[ToolMessage]:
-        """Run all tool calls in the generation and return the results.
-
-        Args:
-            filter_fn:
-                A function that takes a list of ToolCall objects and returns
-                a filtered list of ToolCall objects. This function can be
-                used to filter the tool calls that will be run.
-            parallel: If True, run the tool calls in parallel. Default to False.
-            use_process:
-                If True, run the tool calls in separate processes,
-                effective when parallel is True. Default to False.
-            log_results:
-                If True, log the results of the tool calls. Note This will wait for
-                the results to be ready. Default to use the setting in configs.
-
-        Returns:
-            A list of ToolMessage objects.
-        """
-        if not self.is_tool_call:
-            raise ValueError("Error: The Generation is not a tool call")
-        if log_results is None:
-            log_results = configs.getattrs("settings.logging.display.tool_results")
-        tool_calls = self.tool_calls
-        if filter_fn:
-            tool_calls = filter_fn(tool_calls)
-        messages = []
-        for tc in tool_calls:
-            role = MessageRole(TOOL, tc.name)
-            try:
-                tool_result = self._call_tool(
-                    tc.name, tc.args, parallel=parallel, use_process=use_process
-                )
-                msg = ToolMessage(
-                    tool_result, role=role, tool_call_id=tc.id, has_error=False
-                )
-            except Exception as e:
-                logger.error(f"Error running tool call: {tc.name}({tc.args})")
-                logger.error(e)
-                msg = ToolMessage(str(e), role=role, tool_call_id=tc.id, has_error=True)
-            messages.append(msg)
-        if log_results:  # this will wait for the results to be ready
-            for msg in messages:
-                logger.info(f"Tool call result: {msg}")
-        return messages
-
-    def as_prompt(self) -> Union[AIMessage, StringFuture]:
-        """Get the response of the generation as a promptable object."""
-        if self._args.tools:
-            if self.is_tool_call:
-                return AIMessage(tool_calls=self.tool_calls)
-        return StringFuture(self._call)
-
-    def __getattr__(self, name: str) -> Any:
-        return getattr(self.response, name)
-
-    def __str__(self) -> str:
-        return str(self.response.results)
-
-    def __repr__(self) -> str:
-        return repr(str(self))
+from __future__ import annotations
+
+import json
+import time
+
+from . import trace
+from .config import configs
+from .context import PromptContext
+from .globals import inc_global
+from .message import AIMessage, BaseMessage, ToolMessage
+from .promptable import Promptable
+from .response import CompletionResponse
+from .server import BaseServer, GenArgs
+from .tool import BaseTool, ToolCall
+from .trace import GenerationInitEvent, add_to_trace
+from .types import *
+
+
+class Generation:
+    """Represents a generation call to the model."""
+
+    def __init__(
+        self,
+        server: BaseServer,
+        args: GenArgs,
+        *,
+        mock_response: Optional[Union[CompletionResponse, str]] = None,
+        lazy_eval: bool = False,
+        _ctx: Optional[PromptContext] = None,
+        **kwargs: Any,
+        # kwargs used for extra args for the create method
+    ) -> None:
+        """Initialize the Generation object.
+
+        Args:
+            server: An LLM server where the generation request will be sent.
+            args: The arguments of the generation call.
+            mock_response: A mock response for the generation call.
+            lazy_eval: If True, the generation call will be evaluated lazily.
+            _ctx: The prompt context filled automatically by the APPL function.
+            **kwargs: Extra arguments for the generation call.
+        """
+        # name needs to be unique and ordered, so it has to be generated in the main thread
+        self._id = inc_global("gen_cnt") - 1  # take the value before increment
+
+        self._server = server
+        self._args = args
+        self._ctx = _ctx
+        self._extra_args = kwargs
+
+        add_to_trace(GenerationInitEvent(name=self.id))
+        if isinstance(mock_response, CompletionResponse):
+            self._call = lambda: mock_response
+        else:
+            if mock_response:
+                # use litellm's mock response
+                kwargs.update({"mock_response": mock_response})
+            # TODO: supports custom postprocessing messages
+            self._call = CallFuture(
+                self._server.create,
+                lazy_eval=lazy_eval,
+                args=args,
+                gen_id=self.id,
+                **kwargs,
+            )
+
+        # tools
+        self._tools: Sequence[BaseTool] = args.tools
+        self._name2tools = {tool.name: tool for tool in self._tools}
+
+    @property
+    def id(self) -> str:
+        """The unique ID of the generation."""
+        return f"@gen_{self._id}"
+
+    def __call__(self):
+        """Get the response of the generation call."""
+        return self._call()
+
+    @property
+    def response(self) -> CompletionResponse:
+        """The response of the generation call."""
+        # NOTE: the result of the call will be cached in the CallFuture
+        return self._call()
+
+    @property
+    def response_type(self) -> ResponseType:
+        """The type of the response."""
+        return self.response.type
+
+    @property
+    def is_message(self) -> bool:
+        """Whether the response is a text message."""
+        return self.response_type == ResponseType.TEXT
+
+    @property
+    def is_tool_call(self) -> bool:
+        """Whether the response is a tool call."""
+        return self.response_type == ResponseType.TOOL_CALL
+
+    @property
+    def is_obj(self) -> bool:
+        """Whether the response is an object."""
+        return self.response_type == ResponseType.OBJECT
+
+    @property
+    def message(self) -> Optional[str]:
+        """The message of the response."""
+        return self.response.message
+
+    @property
+    def tool_calls(self) -> List[ToolCall]:
+        """The tool calls of the response."""
+        return self.response.tool_calls
+
+    @property
+    def response_obj(self) -> Any:
+        """The object of the response."""
+        return self.response.response_obj
+
+    @property
+    def results(self) -> Any:
+        """The results of the response."""
+        return self.response.results
+
+    def _call_tool(
+        self, name: str, args: str, parallel: bool = False, use_process: bool = False
+    ) -> Any:
+        try:
+            kwargs = json.loads(args)
+        except json.JSONDecodeError as e:
+            raise ValueError(f"Error parsing args: {args}") from e
+        args_str = ", ".join([f"{k}={v}" for k, v in kwargs.items()])
+        if configs.getattrs("settings.logging.display.tool_calls"):
+            logger.info(f"Running tool call: {name}({args_str})")
+
+        if name not in self._name2tools:
+            raise ValueError(f"Error: Tool {name} not found")
+        tool = self._name2tools[name]
+        try:
+            if parallel:
+                res = CallFuture(tool, use_process=use_process, **kwargs)
+            else:
+                res = tool(**kwargs)
+        except Exception as e:
+            raise RuntimeError(f"Error running tool call: {name}({args_str})") from e
+
+        return res
+
+    def run_tool_calls(
+        self,
+        filter_fn: Optional[Callable[[List[ToolCall]], List[ToolCall]]] = None,
+        parallel: bool = False,
+        use_process: bool = False,
+        log_results: Optional[bool] = None,
+    ) -> List[ToolMessage]:
+        """Run all tool calls in the generation and return the results.
+
+        Args:
+            filter_fn:
+                A function that takes a list of ToolCall objects and returns
+                a filtered list of ToolCall objects. This function can be
+                used to filter the tool calls that will be run.
+            parallel: If True, run the tool calls in parallel. Default to False.
+            use_process:
+                If True, run the tool calls in separate processes,
+                effective when parallel is True. Default to False.
+            log_results:
+                If True, log the results of the tool calls. Note This will wait for
+                the results to be ready. Default to use the setting in configs.
+
+        Returns:
+            A list of ToolMessage objects.
+        """
+        if not self.is_tool_call:
+            raise ValueError("Error: The Generation is not a tool call")
+        if log_results is None:
+            log_results = configs.getattrs("settings.logging.display.tool_results")
+        tool_calls = self.tool_calls
+        if filter_fn:
+            tool_calls = filter_fn(tool_calls)
+        messages = []
+        for tc in tool_calls:
+            role = MessageRole(TOOL, tc.name)
+            try:
+                tool_result = self._call_tool(
+                    tc.name, tc.args, parallel=parallel, use_process=use_process
+                )
+                msg = ToolMessage(
+                    tool_result, role=role, tool_call_id=tc.id, has_error=False
+                )
+            except Exception as e:
+                logger.error(f"Error running tool call: {tc.name}({tc.args})")
+                logger.error(e)
+                msg = ToolMessage(str(e), role=role, tool_call_id=tc.id, has_error=True)
+            messages.append(msg)
+        if log_results:  # this will wait for the results to be ready
+            for msg in messages:
+                logger.info(f"Tool call result: {msg}")
+        return messages
+
+    def as_prompt(self) -> Union[AIMessage, StringFuture]:
+        """Get the response of the generation as a promptable object."""
+        if self._args.tools:
+            if self.is_tool_call:
+                return AIMessage(tool_calls=self.tool_calls)
+        return StringFuture(self._call)
+
+    def __getattr__(self, name: str) -> Any:
+        return getattr(self.response, name)
+
+    def __str__(self) -> str:
+        return str(self.response.results)
+
+    def __repr__(self) -> str:
+        return repr(str(self))
```

### Comparing `applang-0.0.1a3/src/appl/core/io.py` & `applang-0.0.1a4/src/appl/core/io.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import json
-import os
-
-import addict
-import toml
-import yaml
-
-from .types import *
-
-# from importlib import import_module # read python
-PLAIN_TEXT_FILES = [".txt", ".log", ".md", ".html"]
-
-
-def makedirs(file: str) -> None:
-    """Make the directory of the file if it does not exist."""
-    if folder := os.path.dirname(file):
-        os.makedirs(folder, exist_ok=True)
-
-
-def get_ext(file: str) -> str:
-    """Get the extension of a file."""
-    return os.path.splitext(file)[1]
-
-
-def dump_file(
-    data: Any,
-    file: str,
-    mode: str = "w",
-    ensure_folder_exists: bool = True,
-    file_type: Optional[str] = None,
-    *args: Any,
-    **kwargs: Any,
-) -> None:
-    """Write the data to a file based on the file extension."""
-    if file_type is None:
-        file_type = get_ext(file)
-    if ensure_folder_exists:
-        makedirs(file)
-
-    if file_type == ".json":
-        dump_func: Callable = json.dump
-    elif file_type in [".yaml", ".yml"]:
-        dump_func = yaml.dump
-    elif file_type == ".toml":
-        dump_func = toml.dump
-    elif file_type in PLAIN_TEXT_FILES:
-
-        def dump_func(data, f, *args, **kwargs):
-            f.write(data)
-
-    else:
-        raise ValueError(f"Unsupported file type {file_type}")
-    with open(file, mode) as f:
-        dump_func(data, f, *args, **kwargs)
-
-
-def load_file(
-    file: str,
-    mode: str = "r",
-    file_type: Optional[str] = None,
-    *args: Any,
-    **kwargs: Any,
-) -> Any:
-    """Load a file based on the file extension and return the data."""
-    if file_type is None:
-        file_type = get_ext(file)
-    if file_type == ".json":
-        load_func: Callable = json.load
-    elif file_type in [".yaml", ".yml"]:
-        load_func = yaml.safe_load
-    elif file_type == ".toml":
-        load_func = toml.load
-    # elif file_type == ".py":
-    #     load_func = import_module
-    elif file_type in PLAIN_TEXT_FILES:
-
-        def load_func(f, *args, **kwargs):
-            return f.read()
-
-    else:
-        raise ValueError(f"Unsupported file type {file_type}")
-    with open(file, mode) as f:
-        return load_func(f, *args, **kwargs)
+import json
+import os
+
+import addict
+import toml
+import yaml
+
+from .types import *
+
+# from importlib import import_module # read python
+PLAIN_TEXT_FILES = [".txt", ".log", ".md", ".html"]
+
+
+def makedirs(file: str) -> None:
+    """Make the directory of the file if it does not exist."""
+    if folder := os.path.dirname(file):
+        os.makedirs(folder, exist_ok=True)
+
+
+def get_ext(file: str) -> str:
+    """Get the extension of a file."""
+    return os.path.splitext(file)[1]
+
+
+def dump_file(
+    data: Any,
+    file: str,
+    mode: str = "w",
+    ensure_folder_exists: bool = True,
+    file_type: Optional[str] = None,
+    *args: Any,
+    **kwargs: Any,
+) -> None:
+    """Write the data to a file based on the file extension."""
+    if file_type is None:
+        file_type = get_ext(file)
+    if ensure_folder_exists:
+        makedirs(file)
+
+    if file_type == ".json":
+        dump_func: Callable = json.dump
+    elif file_type in [".yaml", ".yml"]:
+        dump_func = yaml.dump
+    elif file_type == ".toml":
+        dump_func = toml.dump
+    elif file_type in PLAIN_TEXT_FILES:
+
+        def dump_func(data, f, *args, **kwargs):
+            f.write(data)
+
+    else:
+        raise ValueError(f"Unsupported file type {file_type}")
+    with open(file, mode) as f:
+        dump_func(data, f, *args, **kwargs)
+
+
+def load_file(
+    file: str,
+    mode: str = "r",
+    file_type: Optional[str] = None,
+    *args: Any,
+    **kwargs: Any,
+) -> Any:
+    """Load a file based on the file extension and return the data."""
+    if file_type is None:
+        file_type = get_ext(file)
+    if file_type == ".json":
+        load_func: Callable = json.load
+    elif file_type in [".yaml", ".yml"]:
+        load_func = yaml.safe_load
+    elif file_type == ".toml":
+        load_func = toml.load
+    # elif file_type == ".py":
+    #     load_func = import_module
+    elif file_type in PLAIN_TEXT_FILES:
+
+        def load_func(f, *args, **kwargs):
+            return f.read()
+
+    else:
+        raise ValueError(f"Unsupported file type {file_type}")
+    with open(file, mode) as f:
+        return load_func(f, *args, **kwargs)
```

### Comparing `applang-0.0.1a3/src/appl/core/message.py` & `applang-0.0.1a4/src/appl/core/message.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,368 +1,368 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-
-from pydantic import model_validator
-from termcolor import colored
-
-from appl.core.types import Dict
-
-from .tool import ToolCall
-from .types import *
-
-
-class BaseMessage(BaseModel, ABC):
-    """The base class for messages."""
-
-    content: Any = Field(..., description="The content of the message")
-    role: Optional[MessageRole] = Field(
-        None, description="The role of the messages owner"
-    )
-    info: Optional[Dict] = Field(
-        {}, description="Additional information for the message"
-    )
-
-    def __init__(self, content: Any = None, *args: Any, **kwargs: Any) -> None:
-        """Create a message with content and extra arguments.
-
-        Provides a more flexible way to create a message.
-        """
-        super().__init__(content=content, *args, **kwargs)
-
-    @property
-    def is_system(self) -> bool:
-        """Whether the message is a system message."""
-        return self.role is not None and self.role.is_system
-
-    @property
-    def is_user(self) -> bool:
-        """Whether the message is a user message."""
-        return self.role is not None and self.role.is_user
-
-    @property
-    def is_ai(self) -> bool:
-        """Whether the message is an assistant message."""
-        return self.role is not None and self.role.is_assistant
-
-    @property
-    def is_tool(self) -> bool:
-        """Whether the message is a tool message."""
-        return self.role is not None and self.role.is_tool
-
-    def validate_role(self, target_role: MessageRole) -> None:
-        """Validate the role of the message, fill the role if not provided."""
-        target_type = target_role.type
-        if target_type is None:
-            raise ValueError("Target role type must be provided.")
-        if self.role is None:
-            self.role = target_role
-        elif self.role.type is None:
-            # fill the role type as the target type
-            self.role = MessageRole(type=target_type, name=self.role.name)
-        elif self.role.type != target_type:
-            raise ValueError(f"Invalid role for {target_type} message: {self.role}")
-
-    def should_merge(self, other: "BaseMessage") -> bool:
-        """Whether the message should be merged with the other message."""
-        if self.is_tool or other.is_tool:
-            # not merge tool messages
-            return False
-        if self.content is None or other.content is None:
-            return False
-        return self.role == other.role
-
-    def get_content(self, as_str: bool = False) -> Any:
-        """Get the content of the message.
-
-        Materialize the content if it is a FutureValue.
-        """
-        content = self.content
-        if content is not None:
-            if isinstance(content, ContentList):
-                return content.get_contents()  # return a list of dict
-            if isinstance(content, FutureValue):
-                # materialize the content
-                content = content.val
-            if as_str:  # not apply to ContentList
-                content = str(content)
-        return content
-
-    def get_dict(self, default_role: Optional[MessageRole] = None) -> Dict[str, Any]:
-        """Return a dict representation of the message."""
-        # materialize the content using str()
-        role = self.role or default_role
-        if role is None:
-            raise ValueError("Role or default role must be provided.")
-        if role.type is None:
-            if default_role and default_role.type:
-                role = MessageRole(type=default_role.type, name=role.name)
-            else:
-                raise ValueError("Role type must be provided.")
-        data = {"content": self.get_content(as_str=True), **role.get_dict()}
-        return data
-
-    def merge(self: "Message", other: "BaseMessage") -> Optional["Message"]:
-        """Merge the message with another message."""
-        if self.should_merge(other):
-            # merge the content
-            res = self.model_copy()
-            if isinstance(other.content, ContentList) and not isinstance(
-                res.content, ContentList
-            ):
-                res.content = ContentList(contents=[res.content])
-            res.content += other.content
-            return res
-        return None
-
-    def __repr__(self) -> str:
-        if self.role is None:
-            return f"Message({self.content})"
-        return f"{self.role}: {self.content}"
-
-    def __str__(self) -> str:
-        if self.role is None:
-            return str(self.content)
-        return self.__repr__()
-
-
-Message = TypeVar("Message", bound=BaseMessage)
-
-
-class ChatMessage(BaseMessage):
-    """A message in the chat conversation."""
-
-    def __init__(
-        self,
-        content: Any = None,
-        *,
-        role: Optional[MessageRole] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Create a chat message with content and extra arguments."""
-        super().__init__(content=content, role=role, **kwargs)
-
-
-class SystemMessage(BaseMessage):
-    """A system message in the conversation."""
-
-    def __init__(
-        self,
-        content: Any = None,
-        *,
-        role: Optional[MessageRole] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Create a system message with content and extra arguments."""
-        super().__init__(content=content, role=role, **kwargs)
-        self.validate_role(SYSTEM_ROLE)
-
-
-class UserMessage(BaseMessage):
-    """A user message in the conversation."""
-
-    def __init__(
-        self,
-        content: Any = None,
-        *,
-        role: Optional[MessageRole] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Create a user message with content and extra arguments."""
-        super().__init__(content=content, role=role, **kwargs)
-        self.validate_role(USER_ROLE)
-
-
-class AIMessage(BaseMessage):
-    """An assistant message in the conversation."""
-
-    tool_calls: List[ToolCall] = Field(
-        [], description="The tool calls generated by the model."
-    )
-
-    def __init__(
-        self,
-        content: Any = None,
-        *,
-        role: Optional[MessageRole] = None,
-        tool_calls: Optional[List[ToolCall]] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Create an assistant message with content and extra arguments."""
-        if tool_calls is None:
-            tool_calls = []
-        super().__init__(content=content, role=role, tool_calls=tool_calls, **kwargs)
-        self.validate_role(ASSISTANT_ROLE)
-
-    def __repr__(self) -> str:
-        s = f"{self.role}:"
-        if self.content is not None:
-            s += f" {self.content}"
-        if len(self.tool_calls):
-            s += f" {self.tool_calls}"
-        return s
-
-    def get_dict(self, default_role: Optional[MessageRole] = None) -> Dict[str, Any]:
-        """Return a dict representation of the message."""
-        data = super().get_dict(default_role)
-        if len(self.tool_calls):
-            data["tool_calls"] = [call.get_dict() for call in self.tool_calls]
-        return data
-
-
-class ToolMessage(BaseMessage):
-    """A tool message in the conversation."""
-
-    tool_call_id: str = Field(
-        ..., description="Tool call that this message is responding to."
-    )
-    has_error: bool = Field(
-        False, description="Whether the message is an error message."
-    )
-
-    def __init__(
-        self,
-        content: Any = None,
-        *,
-        role: Optional[MessageRole] = None,
-        **kwargs: Any,
-    ) -> None:
-        """Create a tool message with content and extra arguments."""
-        super().__init__(content=content, role=role, **kwargs)
-        self.validate_role(TOOL_ROLE)
-
-    def get_dict(self, *args: Any, **kwargs: Any) -> Dict[str, Any]:
-        """Return a dict representation of the message."""
-        data = super().get_dict(*args, **kwargs)
-        data["tool_call_id"] = self.tool_call_id
-        return data
-
-
-MESSAGE_CLASS_DICT = {
-    None: ChatMessage,
-    SYSTEM: SystemMessage,
-    USER: UserMessage,
-    ASSISTANT: AIMessage,
-    TOOL: ToolMessage,
-}
-
-
-def as_message(
-    role: Optional[MessageRole],
-    content: StrOrImg,
-    *args: Any,
-    **kwargs: Any,
-) -> BaseMessage:
-    """Create a message with role, content and extra arguments."""
-    role_type = role.type if role else None
-    if role_type not in MESSAGE_CLASS_DICT:
-        raise ValueError(f"Unknown role: {role}")
-    cls = MESSAGE_CLASS_DICT[role_type]
-    if isinstance(content, Image):
-        content = ContentList(contents=[content])  # type: ignore
-    return cls(content=content, role=role, *args, **kwargs)
-
-
-def collapse_messages(messages: List[Message]) -> List[Message]:
-    """Collapse a list of the messages by merging the messages with the same sender."""
-    res = []
-    msg: Optional[Message] = None
-    for m in messages:
-        if msg is None:
-            msg = m
-        else:
-            if (tmp := msg.merge(m)) is not None:
-                # merge success, update the msg
-                msg = tmp
-            else:
-                # merge failed, append the old message to the list
-                res.append(msg)
-                # a new message starts
-                msg = m
-    if msg is not None:
-        res.append(msg)
-    return res
-
-
-class Conversation(BaseModel):
-    """A conversation containing messages."""
-
-    system_messages: List[SystemMessage] = Field([], description="The system messages")
-    messages: List[BaseMessage] = Field(
-        [], description="The messages in the conversation"
-    )
-
-    def collapse(self) -> None:
-        """Collapse the messages in the conversation."""
-        self.system_messages = collapse_messages(self.system_messages)
-        if len(self.system_messages) > 1:
-            raise ValueError("System messages cannot be fully collapsed.")
-        self.messages = collapse_messages(self.messages)
-
-    def materialize(self) -> None:
-        """Materialize the messages in the conversation."""
-        str(self)
-
-    def __repr__(self) -> str:
-        return f"Conversation({self.system_messages}, {self.messages})"
-
-    def __str__(self) -> str:
-        self.collapse()
-        res = "\n".join(str(m) for m in self.system_messages)
-        res += "\n".join(str(m) for m in self.messages)
-        return res
-
-    def __iter__(self) -> Iterator[BaseMessage]:  # type: ignore
-        """Iterate over messages, excluding the system message."""
-        return iter(self.messages)
-
-    def __getitem__(self, index: int) -> BaseMessage:
-        """Get message by index, excluding the system message."""
-        return self.messages[index]
-
-    def __len__(self) -> int:
-        """Length of the conversation, excluding the system message."""
-        return len(self.messages)
-
-    def set_system_messages(self, messages: List[SystemMessage]) -> None:
-        """Set the system messages."""
-        if len(self.system_messages):
-            logger.warning("Overwriting system message.")
-        self.system_messages = messages
-
-    def append(self, message: Message) -> None:
-        """Append a message to the conversation."""
-        if message.is_system:
-            if len(self.messages):
-                # NOTE: Now allow appending system message after other messages
-                # raise ValueError("Cannot append system message after other messages.")
-
-                # Added a warning instead
-                logger.warning(
-                    "Modifying system message after other types of messages."
-                )
-            self.system_messages.append(message)  # type: ignore
-        else:
-            self.messages.append(message)
-
-    def extend(self, other: "Conversation") -> None:
-        """Extend the conversation with another conversation."""
-        for sys_m in other.system_messages:
-            self.append(sys_m)
-        for m in other.messages:
-            self.append(m)
-
-    def as_list(
-        self, default_role: Optional[MessageRole] = USER_ROLE
-    ) -> List[Dict[str, str]]:
-        """Return a list of dict representation of the conversation."""
-        self.collapse()
-        res = [m.get_dict() for m in self.system_messages]
-        res += [m.get_dict(default_role) for m in self.messages]
-        return res
-
-    def make_copy(self):
-        """Make a copy of the conversation."""
-        return Conversation(
-            system_messages=self.system_messages.copy(),
-            messages=self.messages.copy(),
-        )
+from __future__ import annotations
+
+from dataclasses import dataclass
+
+from pydantic import model_validator
+from termcolor import colored
+
+from appl.core.types import Dict
+
+from .tool import ToolCall
+from .types import *
+
+
+class BaseMessage(BaseModel, ABC):
+    """The base class for messages."""
+
+    content: Any = Field(..., description="The content of the message")
+    role: Optional[MessageRole] = Field(
+        None, description="The role of the messages owner"
+    )
+    info: Optional[Dict] = Field(
+        {}, description="Additional information for the message"
+    )
+
+    def __init__(self, content: Any = None, *args: Any, **kwargs: Any) -> None:
+        """Create a message with content and extra arguments.
+
+        Provides a more flexible way to create a message.
+        """
+        super().__init__(content=content, *args, **kwargs)
+
+    @property
+    def is_system(self) -> bool:
+        """Whether the message is a system message."""
+        return self.role is not None and self.role.is_system
+
+    @property
+    def is_user(self) -> bool:
+        """Whether the message is a user message."""
+        return self.role is not None and self.role.is_user
+
+    @property
+    def is_ai(self) -> bool:
+        """Whether the message is an assistant message."""
+        return self.role is not None and self.role.is_assistant
+
+    @property
+    def is_tool(self) -> bool:
+        """Whether the message is a tool message."""
+        return self.role is not None and self.role.is_tool
+
+    def validate_role(self, target_role: MessageRole) -> None:
+        """Validate the role of the message, fill the role if not provided."""
+        target_type = target_role.type
+        if target_type is None:
+            raise ValueError("Target role type must be provided.")
+        if self.role is None:
+            self.role = target_role
+        elif self.role.type is None:
+            # fill the role type as the target type
+            self.role = MessageRole(type=target_type, name=self.role.name)
+        elif self.role.type != target_type:
+            raise ValueError(f"Invalid role for {target_type} message: {self.role}")
+
+    def should_merge(self, other: "BaseMessage") -> bool:
+        """Whether the message should be merged with the other message."""
+        if self.is_tool or other.is_tool:
+            # not merge tool messages
+            return False
+        if self.content is None or other.content is None:
+            return False
+        return self.role == other.role
+
+    def get_content(self, as_str: bool = False) -> Any:
+        """Get the content of the message.
+
+        Materialize the content if it is a FutureValue.
+        """
+        content = self.content
+        if content is not None:
+            if isinstance(content, ContentList):
+                return content.get_contents()  # return a list of dict
+            if isinstance(content, FutureValue):
+                # materialize the content
+                content = content.val
+            if as_str:  # not apply to ContentList
+                content = str(content)
+        return content
+
+    def get_dict(self, default_role: Optional[MessageRole] = None) -> Dict[str, Any]:
+        """Return a dict representation of the message."""
+        # materialize the content using str()
+        role = self.role or default_role
+        if role is None:
+            raise ValueError("Role or default role must be provided.")
+        if role.type is None:
+            if default_role and default_role.type:
+                role = MessageRole(type=default_role.type, name=role.name)
+            else:
+                raise ValueError("Role type must be provided.")
+        data = {"content": self.get_content(as_str=True), **role.get_dict()}
+        return data
+
+    def merge(self: "Message", other: "BaseMessage") -> Optional["Message"]:
+        """Merge the message with another message."""
+        if self.should_merge(other):
+            # merge the content
+            res = self.model_copy()
+            if isinstance(other.content, ContentList) and not isinstance(
+                res.content, ContentList
+            ):
+                res.content = ContentList(contents=[res.content])
+            res.content += other.content
+            return res
+        return None
+
+    def __repr__(self) -> str:
+        if self.role is None:
+            return f"Message({self.content})"
+        return f"{self.role}: {self.content}"
+
+    def __str__(self) -> str:
+        if self.role is None:
+            return str(self.content)
+        return self.__repr__()
+
+
+Message = TypeVar("Message", bound=BaseMessage)
+
+
+class ChatMessage(BaseMessage):
+    """A message in the chat conversation."""
+
+    def __init__(
+        self,
+        content: Any = None,
+        *,
+        role: Optional[MessageRole] = None,
+        **kwargs: Any,
+    ) -> None:
+        """Create a chat message with content and extra arguments."""
+        super().__init__(content=content, role=role, **kwargs)
+
+
+class SystemMessage(BaseMessage):
+    """A system message in the conversation."""
+
+    def __init__(
+        self,
+        content: Any = None,
+        *,
+        role: Optional[MessageRole] = None,
+        **kwargs: Any,
+    ) -> None:
+        """Create a system message with content and extra arguments."""
+        super().__init__(content=content, role=role, **kwargs)
+        self.validate_role(SYSTEM_ROLE)
+
+
+class UserMessage(BaseMessage):
+    """A user message in the conversation."""
+
+    def __init__(
+        self,
+        content: Any = None,
+        *,
+        role: Optional[MessageRole] = None,
+        **kwargs: Any,
+    ) -> None:
+        """Create a user message with content and extra arguments."""
+        super().__init__(content=content, role=role, **kwargs)
+        self.validate_role(USER_ROLE)
+
+
+class AIMessage(BaseMessage):
+    """An assistant message in the conversation."""
+
+    tool_calls: List[ToolCall] = Field(
+        [], description="The tool calls generated by the model."
+    )
+
+    def __init__(
+        self,
+        content: Any = None,
+        *,
+        role: Optional[MessageRole] = None,
+        tool_calls: Optional[List[ToolCall]] = None,
+        **kwargs: Any,
+    ) -> None:
+        """Create an assistant message with content and extra arguments."""
+        if tool_calls is None:
+            tool_calls = []
+        super().__init__(content=content, role=role, tool_calls=tool_calls, **kwargs)
+        self.validate_role(ASSISTANT_ROLE)
+
+    def __repr__(self) -> str:
+        s = f"{self.role}:"
+        if self.content is not None:
+            s += f" {self.content}"
+        if len(self.tool_calls):
+            s += f" {self.tool_calls}"
+        return s
+
+    def get_dict(self, default_role: Optional[MessageRole] = None) -> Dict[str, Any]:
+        """Return a dict representation of the message."""
+        data = super().get_dict(default_role)
+        if len(self.tool_calls):
+            data["tool_calls"] = [call.get_dict() for call in self.tool_calls]
+        return data
+
+
+class ToolMessage(BaseMessage):
+    """A tool message in the conversation."""
+
+    tool_call_id: str = Field(
+        ..., description="Tool call that this message is responding to."
+    )
+    has_error: bool = Field(
+        False, description="Whether the message is an error message."
+    )
+
+    def __init__(
+        self,
+        content: Any = None,
+        *,
+        role: Optional[MessageRole] = None,
+        **kwargs: Any,
+    ) -> None:
+        """Create a tool message with content and extra arguments."""
+        super().__init__(content=content, role=role, **kwargs)
+        self.validate_role(TOOL_ROLE)
+
+    def get_dict(self, *args: Any, **kwargs: Any) -> Dict[str, Any]:
+        """Return a dict representation of the message."""
+        data = super().get_dict(*args, **kwargs)
+        data["tool_call_id"] = self.tool_call_id
+        return data
+
+
+MESSAGE_CLASS_DICT = {
+    None: ChatMessage,
+    SYSTEM: SystemMessage,
+    USER: UserMessage,
+    ASSISTANT: AIMessage,
+    TOOL: ToolMessage,
+}
+
+
+def as_message(
+    role: Optional[MessageRole],
+    content: StrOrImg,
+    *args: Any,
+    **kwargs: Any,
+) -> BaseMessage:
+    """Create a message with role, content and extra arguments."""
+    role_type = role.type if role else None
+    if role_type not in MESSAGE_CLASS_DICT:
+        raise ValueError(f"Unknown role: {role}")
+    cls = MESSAGE_CLASS_DICT[role_type]
+    if isinstance(content, Image):
+        content = ContentList(contents=[content])  # type: ignore
+    return cls(content=content, role=role, *args, **kwargs)
+
+
+def collapse_messages(messages: List[Message]) -> List[Message]:
+    """Collapse a list of the messages by merging the messages with the same sender."""
+    res = []
+    msg: Optional[Message] = None
+    for m in messages:
+        if msg is None:
+            msg = m
+        else:
+            if (tmp := msg.merge(m)) is not None:
+                # merge success, update the msg
+                msg = tmp
+            else:
+                # merge failed, append the old message to the list
+                res.append(msg)
+                # a new message starts
+                msg = m
+    if msg is not None:
+        res.append(msg)
+    return res
+
+
+class Conversation(BaseModel):
+    """A conversation containing messages."""
+
+    system_messages: List[SystemMessage] = Field([], description="The system messages")
+    messages: List[BaseMessage] = Field(
+        [], description="The messages in the conversation"
+    )
+
+    def collapse(self) -> None:
+        """Collapse the messages in the conversation."""
+        self.system_messages = collapse_messages(self.system_messages)
+        if len(self.system_messages) > 1:
+            raise ValueError("System messages cannot be fully collapsed.")
+        self.messages = collapse_messages(self.messages)
+
+    def materialize(self) -> None:
+        """Materialize the messages in the conversation."""
+        str(self)
+
+    def __repr__(self) -> str:
+        return f"Conversation({self.system_messages}, {self.messages})"
+
+    def __str__(self) -> str:
+        self.collapse()
+        res = "\n".join(str(m) for m in self.system_messages)
+        res += "\n".join(str(m) for m in self.messages)
+        return res
+
+    def __iter__(self) -> Iterator[BaseMessage]:  # type: ignore
+        """Iterate over messages, excluding the system message."""
+        return iter(self.messages)
+
+    def __getitem__(self, index: int) -> BaseMessage:
+        """Get message by index, excluding the system message."""
+        return self.messages[index]
+
+    def __len__(self) -> int:
+        """Length of the conversation, excluding the system message."""
+        return len(self.messages)
+
+    def set_system_messages(self, messages: List[SystemMessage]) -> None:
+        """Set the system messages."""
+        if len(self.system_messages):
+            logger.warning("Overwriting system message.")
+        self.system_messages = messages
+
+    def append(self, message: Message) -> None:
+        """Append a message to the conversation."""
+        if message.is_system:
+            if len(self.messages):
+                # NOTE: Now allow appending system message after other messages
+                # raise ValueError("Cannot append system message after other messages.")
+
+                # Added a warning instead
+                logger.warning(
+                    "Modifying system message after other types of messages."
+                )
+            self.system_messages.append(message)  # type: ignore
+        else:
+            self.messages.append(message)
+
+    def extend(self, other: "Conversation") -> None:
+        """Extend the conversation with another conversation."""
+        for sys_m in other.system_messages:
+            self.append(sys_m)
+        for m in other.messages:
+            self.append(m)
+
+    def as_list(
+        self, default_role: Optional[MessageRole] = USER_ROLE
+    ) -> List[Dict[str, str]]:
+        """Return a list of dict representation of the conversation."""
+        self.collapse()
+        res = [m.get_dict() for m in self.system_messages]
+        res += [m.get_dict(default_role) for m in self.messages]
+        return res
+
+    def make_copy(self):
+        """Make a copy of the conversation."""
+        return Conversation(
+            system_messages=self.system_messages.copy(),
+            messages=self.messages.copy(),
+        )
```

### Comparing `applang-0.0.1a3/src/appl/core/modifiers.py` & `applang-0.0.1a4/src/appl/core/modifiers.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-from __future__ import annotations
-
-import copy
-import traceback
-from abc import ABC, abstractmethod
-from contextlib import AbstractContextManager
-
-from .context import PromptContext
-from .printer import Indexing, PrinterPop, PrinterPush, PromptPrinter, PromptRecords
-from .types import *
-from .types import override
-
-
-class PrinterModifier(AbstractContextManager):
-    """The contextual compositor of the prompt printer.
-
-    Controls the behavior of the prompt printer within the context manager.
-    Should only be used within the APPL function.
-    """
-
-    __need_ctx__: bool = True
-
-    def __init__(self, _ctx: Optional[PromptContext] = None):
-        """Initialize the PrinterModifier object.
-
-        Args:
-            _ctx: The prompt context filled automatically by the APPL function.
-        """
-        self._ctx = _ctx
-
-    @property
-    def push_args(self) -> PrinterPush:
-        """The arguments to push to the printer."""
-        raise NotImplementedError
-
-    def _enter(self) -> None:
-        if self._ctx is None:
-            raise ValueError(
-                "Context is not provided, did you forget mark your function with @ppl?"
-            )
-        self._ctx.push_printer(self.push_args)
-
-    def _exit(
-        self,
-        _exc_type: Optional[type[BaseException]],
-        _exc_value: Optional[BaseException],
-        _traceback: Optional[TracebackType],
-    ) -> Optional[bool]:
-        if _exc_type:
-            # logger.debug(f"Exception occurred: {__exc_value}")
-            traceback.print_tb(_traceback)
-            return False
-        if self._ctx is not None:
-            self._ctx.pop_printer()
-        return None
-
-    def __enter__(self) -> "PrinterModifier":
-        self._enter()
-        return self
-
-    def __exit__(
-        self,
-        __exc_type: Optional[type[BaseException]],
-        __exc_value: Optional[BaseException],
-        __traceback: Optional[TracebackType],
-    ) -> Optional[bool]:
-        return self._exit(__exc_type, __exc_value, __traceback)
-
-
-class Compositor(PrinterModifier):
-    """The contextual compositor of the prompts.
-
-    This class represents a contextual compositor that modifies the behavior of the printer.
-    It provides various options for customizing the output format of the prompts within this context manager.
-
-    Attributes:
-        _sep: The class default separator string is None, indicating inherit from the parent.
-        _indexing: The class default indexing mode is empty indexing.
-        _inc_indent: The class default indentation string is empty string.
-        _new_indent: The class default new indentation string is None, indicating not overwrite the indent.
-        _is_inline: The class default inline flag is False.
-        _new_role: The class default role of the modifier is None, indicating not overwrite the role.
-    """
-
-    # The default value of the printer modifier
-    _sep: Optional[str] = None  # Default: inherit from the parent
-    _indexing: Indexing = Indexing()  # Default: empty indexing
-    _inc_indent: str = ""  # Default: no delta indent
-    _new_indent: Optional[str] = None  # Default: not overwrite the indent
-    _is_inline: bool = False  # Default: not inline
-    _new_role: Optional[MessageRole] = None  # Default: not overwrite the role
-
-    def __init__(
-        self,
-        sep: Optional[str] = None,
-        indexing: Union[Indexing, Optional[str]] = None,
-        indent: Optional[Union[str, int]] = None,
-        new_indent: Optional[Union[str, int]] = None,
-        is_inline: Optional[bool] = None,
-        role: Optional[MessageRole] = None,
-        _ctx: Optional[PromptContext] = None,
-    ):
-        """Initialize the Compositor object.
-
-        Args:
-            sep:
-                The separator string. Defaults to use the class default.
-            indexing:
-                The indexing mode. Defaults to use the class default.
-            indent:
-                The indentation string. Defaults to use the class default.
-            new_indent:
-                The new indentation string. Defaults to use the class default.
-            is_inline:
-                Flag indicating if the modifier is inline. Defaults to use the class default.
-            role:
-                The role of the modifier. Defaults to use the class default.
-            _ctx: The prompt context filled automatically by the APPL function.
-        """
-        super().__init__(_ctx)
-        if sep is not None:
-            self._sep = sep
-        if indexing is not None:
-            if isinstance(indexing, str):
-                indexing = Indexing(indexing)
-            self._indexing = indexing
-        else:
-            if self._indexing is None:
-                raise ValueError("Indexing must be provided.")
-            self._indexing = copy.copy(self._indexing)
-            # copy to avoid changing the class default
-        if indent is not None:
-            if isinstance(indent, int):
-                indent = " " * indent
-            self._inc_indent = indent
-        if new_indent is not None:
-            if isinstance(new_indent, int):
-                new_indent = " " * new_indent
-            self._new_indent = new_indent
-        if is_inline is not None:
-            self._is_inline = is_inline
-        if role is not None:
-            self._new_role = role
-
-    @override
-    @property
-    def push_args(self) -> PrinterPush:
-        return PrinterPush(
-            self._new_role,
-            self._sep,
-            self._indexing,
-            self._inc_indent,
-            self._new_indent,
-            self._is_inline,
-        )
-
-
-# Essential for compile
-class ApplStr(Compositor):
-    """A compositor that represents a string in the prompt.
-
-    Attributes:
-        _sep: The class default separator string is an empty string.
-        _new_indent: The class default new indentation string is an empty string.
-        _is_inline: The class default inline flag is True.
-
-    Examples:
-        ```py
-        >>> with ApplStr():
-        ...     "Hello, "
-        ...     "world!"
-        <<< The prompt will be:
-        Hello, world!
-        ```
-    """
-
-    _sep = ""
-    _new_indent = ""
-    _is_inline = True
+from __future__ import annotations
+
+import copy
+import traceback
+from abc import ABC, abstractmethod
+from contextlib import AbstractContextManager
+
+from .context import PromptContext
+from .printer import Indexing, PrinterPop, PrinterPush, PromptPrinter, PromptRecords
+from .types import *
+from .types import override
+
+
+class PrinterModifier(AbstractContextManager):
+    """The contextual compositor of the prompt printer.
+
+    Controls the behavior of the prompt printer within the context manager.
+    Should only be used within the APPL function.
+    """
+
+    __need_ctx__: bool = True
+
+    def __init__(self, _ctx: Optional[PromptContext] = None):
+        """Initialize the PrinterModifier object.
+
+        Args:
+            _ctx: The prompt context filled automatically by the APPL function.
+        """
+        self._ctx = _ctx
+
+    @property
+    def push_args(self) -> PrinterPush:
+        """The arguments to push to the printer."""
+        raise NotImplementedError
+
+    def _enter(self) -> None:
+        if self._ctx is None:
+            raise ValueError(
+                "Context is not provided, did you forget mark your function with @ppl?"
+            )
+        self._ctx.push_printer(self.push_args)
+
+    def _exit(
+        self,
+        _exc_type: Optional[type[BaseException]],
+        _exc_value: Optional[BaseException],
+        _traceback: Optional[TracebackType],
+    ) -> Optional[bool]:
+        if _exc_type:
+            # logger.debug(f"Exception occurred: {__exc_value}")
+            traceback.print_tb(_traceback)
+            return False
+        if self._ctx is not None:
+            self._ctx.pop_printer()
+        return None
+
+    def __enter__(self) -> "PrinterModifier":
+        self._enter()
+        return self
+
+    def __exit__(
+        self,
+        __exc_type: Optional[type[BaseException]],
+        __exc_value: Optional[BaseException],
+        __traceback: Optional[TracebackType],
+    ) -> Optional[bool]:
+        return self._exit(__exc_type, __exc_value, __traceback)
+
+
+class Compositor(PrinterModifier):
+    """The contextual compositor of the prompts.
+
+    This class represents a contextual compositor that modifies the behavior of the printer.
+    It provides various options for customizing the output format of the prompts within this context manager.
+
+    Attributes:
+        _sep: The class default separator string is None, indicating inherit from the parent.
+        _indexing: The class default indexing mode is empty indexing.
+        _inc_indent: The class default indentation string is empty string.
+        _new_indent: The class default new indentation string is None, indicating not overwrite the indent.
+        _is_inline: The class default inline flag is False.
+        _new_role: The class default role of the modifier is None, indicating not overwrite the role.
+    """
+
+    # The default value of the printer modifier
+    _sep: Optional[str] = None  # Default: inherit from the parent
+    _indexing: Indexing = Indexing()  # Default: empty indexing
+    _inc_indent: str = ""  # Default: no delta indent
+    _new_indent: Optional[str] = None  # Default: not overwrite the indent
+    _is_inline: bool = False  # Default: not inline
+    _new_role: Optional[MessageRole] = None  # Default: not overwrite the role
+
+    def __init__(
+        self,
+        sep: Optional[str] = None,
+        indexing: Union[Indexing, Optional[str]] = None,
+        indent: Optional[Union[str, int]] = None,
+        new_indent: Optional[Union[str, int]] = None,
+        is_inline: Optional[bool] = None,
+        role: Optional[MessageRole] = None,
+        _ctx: Optional[PromptContext] = None,
+    ):
+        """Initialize the Compositor object.
+
+        Args:
+            sep:
+                The separator string. Defaults to use the class default.
+            indexing:
+                The indexing mode. Defaults to use the class default.
+            indent:
+                The indentation string. Defaults to use the class default.
+            new_indent:
+                The new indentation string. Defaults to use the class default.
+            is_inline:
+                Flag indicating if the modifier is inline. Defaults to use the class default.
+            role:
+                The role of the modifier. Defaults to use the class default.
+            _ctx: The prompt context filled automatically by the APPL function.
+        """
+        super().__init__(_ctx)
+        if sep is not None:
+            self._sep = sep
+        if indexing is not None:
+            if isinstance(indexing, str):
+                indexing = Indexing(indexing)
+            self._indexing = indexing
+        else:
+            if self._indexing is None:
+                raise ValueError("Indexing must be provided.")
+            self._indexing = copy.copy(self._indexing)
+            # copy to avoid changing the class default
+        if indent is not None:
+            if isinstance(indent, int):
+                indent = " " * indent
+            self._inc_indent = indent
+        if new_indent is not None:
+            if isinstance(new_indent, int):
+                new_indent = " " * new_indent
+            self._new_indent = new_indent
+        if is_inline is not None:
+            self._is_inline = is_inline
+        if role is not None:
+            self._new_role = role
+
+    @override
+    @property
+    def push_args(self) -> PrinterPush:
+        return PrinterPush(
+            self._new_role,
+            self._sep,
+            self._indexing,
+            self._inc_indent,
+            self._new_indent,
+            self._is_inline,
+        )
+
+
+# Essential for compile
+class ApplStr(Compositor):
+    """A compositor that represents a string in the prompt.
+
+    Attributes:
+        _sep: The class default separator string is an empty string.
+        _new_indent: The class default new indentation string is an empty string.
+        _is_inline: The class default inline flag is True.
+
+    Examples:
+        ```py
+        >>> with ApplStr():
+        ...     "Hello, "
+        ...     "world!"
+        <<< The prompt will be:
+        Hello, world!
+        ```
+    """
+
+    _sep = ""
+    _new_indent = ""
+    _is_inline = True
```

### Comparing `applang-0.0.1a3/src/appl/core/printer.py` & `applang-0.0.1a4/src/appl/core/printer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,341 +1,341 @@
-from __future__ import annotations
-
-import copy
-from dataclasses import dataclass
-
-import roman
-
-from .message import BaseMessage, Conversation, as_message
-from .types import *
-
-
-class Indexing:
-    """The indexing method for the printer."""
-
-    def __init__(
-        self, method: Optional[str] = None, ind: int = 0, suffix: Optional[str] = None
-    ):
-        """Initialize the indexing method."""
-        self._method = method
-        self._ind = ind
-        self._suffix = suffix
-
-    def _get_index(self, ind: int) -> str:
-        if self._method is None:
-            return ""
-        default_suffix = ". "
-        if self._method == "number":
-            base = str(ind + 1)
-        elif self._method in ["lower", "upper", "letter", "Letter"]:
-            if ind >= 26:
-                raise ValueError("Letter-based indexing method only supports 26 items.")
-            base = chr(ord("A") + ind)
-            if self._method in ["lower", "letter"]:
-                base = base.lower()
-        elif self._method in ["roman", "Roman"]:
-            base = roman.toRoman(ind + 1)
-            if self._method == "roman":
-                base = base.lower()
-        else:
-            default_suffix = " "
-            if self._method == "star":
-                base = "*"
-            elif self._method == "dash":
-                base = "-"
-            elif self._method.startswith("sharp"):
-                base = "#" * int(self._method[5:])
-            else:
-                base = self._method
-
-        return base + (self._suffix or default_suffix)
-
-    def get_index(self, ind: Optional[int] = None) -> str:
-        """Get the index string for the current or given index."""
-        if ind is None:
-            ind = self._ind
-            self._ind += 1
-        if ind < 0:
-            raise ValueError("Indexing method does not support negative indexing.")
-        return self._get_index(ind)
-
-    def __repr__(self) -> str:
-        return f"Indexing(method={self._method!r}, ind={self._ind!r}, suffix={self._suffix!r})"
-
-
-@dataclass
-class PrinterState:
-    """A state of the printer."""
-
-    # settings
-    role: Optional[MessageRole] = None
-    """The role to be used for the message."""
-    separator: str = "\n"
-    """The separator to be used between texts."""
-    indexing: Indexing = Indexing(None, 0)
-    """The indexing method to be used."""
-    indent: str = ""
-    """The indent to be used in the beginning of each line."""
-    # inline means the first indent and indexing is inherited from the previous state
-    is_inline: bool = False
-    """Whether the state is inline. Inline means the first indent and
-    indexing is inherited from the previous non-inline state."""
-    # states
-    is_start: bool = True
-    """Whether the state is at the start of the scope."""
-    current_sep: str = ""
-    """The current separator to be used between texts."""
-
-
-@dataclass
-class PrinterPush:
-    """A record to push a new printer state to the stack."""
-
-    new_role: Optional[MessageRole] = None
-    """The new role to be used for the message."""
-    separator: Optional[str] = None
-    """The separator to be used between texts."""
-    indexing: Optional[Indexing] = None
-    """The indexing method to be used."""
-    inc_indent: str = ""
-    """The increment of the indent."""
-    new_indent: Optional[str] = None
-    """The new indent to be used."""
-    is_inline: Optional[bool] = False
-    """Whether the state is inline."""
-
-
-@dataclass
-class PrinterPop:
-    """A record to pop the last printer state from the stack."""
-
-
-RecordType = Union[BaseMessage, StringFuture, Image, PrinterPush, PrinterPop]
-"""Types allowed in the prompt records."""
-
-
-class PromptRecords:
-    """A class represents a list of prompt records."""
-
-    def __init__(self) -> None:
-        """Initialize the prompt records."""
-        self._records: List[RecordType] = []
-
-    @property
-    def records(self) -> List[RecordType]:
-        """The list of records."""
-        return self._records
-
-    def as_convo(self) -> Conversation:
-        """Convert the prompt records to a conversation."""
-        return PromptPrinter()(self)
-
-    def record(self, record: Union[str, RecordType]) -> None:
-        """Record a string, message, image, printer push or printer pop."""
-        if isinstance(record, str):  # compatible to str
-            record = StringFuture(record)
-        if (
-            isinstance(record, StringFuture)
-            or isinstance(record, Image)
-            or isinstance(record, BaseMessage)
-            or isinstance(record, PrinterPush)
-            or isinstance(record, PrinterPop)
-        ):
-            self._records.append(record)
-        else:
-            raise ValueError("Can only record Message, PrinterPush or PrinterPop")
-
-    def extend(self, record: "PromptRecords") -> None:
-        """Extend the prompt records with another prompt records."""
-        self._records.extend(record._records)
-
-    def copy(self) -> "PromptRecords":
-        """Copy the prompt records."""
-        return copy.deepcopy(self)
-
-    def __str__(self) -> str:
-        return str(self.as_convo())
-
-
-class PromptPrinter:
-    """A class to print prompt records as conversation.
-
-    The printer maintains a stack of printer states about the
-    current role, separator, indexing, and indentation.
-    """
-
-    def __init__(
-        self, states: Optional[List[PrinterState]] = None, is_newline: bool = True
-    ) -> None:
-        """Initialize the prompt printer."""
-        if states is None:
-            states = [PrinterState()]
-        self._states = states
-        self._is_newline = is_newline
-
-    @property
-    def states(self) -> List[PrinterState]:
-        """The stack of printer states."""
-        return self._states
-
-    def push(self, data: PrinterPush) -> None:
-        """Push a new printer state to the stack."""
-        self._push(**data.__dict__)
-
-    def pop(self) -> None:
-        """Pop the last printer state from the stack."""
-        if len(self._states) == 1:
-            raise ValueError("Cannot pop the first state.")
-        self._states.pop()
-
-    def _push(
-        self,
-        new_role: Optional[MessageRole] = None,
-        separator: Optional[str] = None,
-        indexing: Optional[Indexing] = None,
-        inc_indent: str = "",
-        new_indent: Optional[str] = None,
-        is_inline: bool = False,
-    ) -> None:
-        state = self.states[-1]
-        if new_role is None or new_role == state.role:
-            new_role = state.role
-            current_separator = state.current_sep
-            default_separator = state.separator  # Use the same separator as parent
-            default_indexing = state.indexing  # Use the same indexing as parent
-        else:  # a new role started
-            logger.debug(f"new role started {new_role}")
-            if len(self.states) > 1:
-                raise ValueError(
-                    "Cannot start a new role when there are states in the stack."
-                )
-            state.is_start = True  # reset the outmost state
-            state.current_sep = ""  # also reset the current separator
-            current_separator = ""
-            default_separator = "\n"
-            default_indexing = Indexing(None, 0)  # create a empty indexing
-            if new_indent is None:
-                new_indent = ""  # reset the indent
-                if inc_indent:
-                    raise ValueError(
-                        "Cannot specify inc_indent when new role started. "
-                        "Use new_indent instead."
-                    )
-
-        if separator is None:
-            separator = default_separator
-        if indexing is None:
-            indexing = default_indexing
-        else:
-            # Avoid changing the original indexing (could be a record)
-            indexing = copy.copy(indexing)
-        if new_indent is None:
-            new_indent = state.indent + inc_indent  # increment the indent
-        elif inc_indent:
-            raise ValueError("Cannot specify both inc_indent and new_indent.")
-
-        self._states.append(
-            PrinterState(
-                new_role,
-                separator,
-                indexing,
-                new_indent,
-                is_inline,
-                True,
-                # The current separator is inherited from the parent state
-                # it will change to its own separator after the first print.
-                current_sep=current_separator,
-            )
-        )
-
-    def _print_str(self, content: String) -> StringFuture:
-        state, previous = self._states[-1], self._states[:-1]
-        role = state.role
-        sep = state.current_sep
-        indent = state.indent
-        indexing = state.indexing
-        if state.is_start:  # is the first content in this scope
-            state.is_start = False
-            state.current_sep = state.separator
-            for st in previous[::-1]:
-                if st.role != role:
-                    break
-                if st.is_start:
-                    # after first print, change the separator to its own
-                    st.is_start = False
-                    st.current_sep = st.separator
-                else:
-                    break
-
-            if state.is_inline:
-                # inline means the first indent and indexing is
-                # inherited from the previous non-inline state
-                for st in previous[::-1]:
-                    if st.role != role:
-                        break
-                    if not st.is_inline:
-                        # Use the first non-inline's indent and indexing
-                        indent = st.indent
-                        indexing = st.indexing
-                        break
-        if sep.endswith("\n"):
-            self._is_newline = True
-
-        s = StringFuture(sep)
-        if self._is_newline:
-            if indent:
-                s += indent
-            self._is_newline = False
-        if cur_idx := indexing.get_index():
-            s += cur_idx
-        s += content
-
-        # TODO: maybe check whether `s` ends with newline
-        return s
-
-    def _print_message(self, content: String) -> BaseMessage:
-        """Print a string as message with the current printer state."""
-        role = self._states[-1].role  # the default role within the context
-        content = self._print_str(content)
-        return as_message(role, content)
-
-    def _print(
-        self, contents: Union[String, Image, BaseMessage, PromptRecords]
-    ) -> Conversation:
-        convo = Conversation(system_messages=[], messages=[])
-
-        def handle(rec: Union[RecordType, Image, str]) -> None:
-            if isinstance(rec, (str, StringFuture)):
-                convo.append(self._print_message(rec))
-            elif isinstance(rec, Image):
-                convo.append(as_message(self._states[-1].role, rec))
-                state = self._states[-1]
-                # reset current state after image, TODO: double check
-                state.is_start = True
-                state.current_sep = ""
-            elif isinstance(rec, BaseMessage):
-                convo.append(rec)
-                if rec.role is not None and len(self._states) == 1:
-                    # change role in the outmost state
-                    state = self._states[0]
-                    state.is_start = True  # reset the outmost state
-                    state.current_sep = ""  # also reset the current separator
-                # TODO: what should be the behavior if the role is changed
-                # in states other than the outmost one?
-                # should such behavior being allowed?
-
-            elif isinstance(rec, PrinterPush):
-                self.push(rec)
-            elif isinstance(rec, PrinterPop):
-                self.pop()
-            else:
-                raise ValueError(f"Unknown record type {type(rec)}")
-
-        if isinstance(contents, PromptRecords):
-            for rec in contents.records:
-                handle(rec)
-        else:
-            handle(contents)
-
-        return convo
-
-    __call__ = _print
+from __future__ import annotations
+
+import copy
+from dataclasses import dataclass
+
+import roman
+
+from .message import BaseMessage, Conversation, as_message
+from .types import *
+
+
+class Indexing:
+    """The indexing method for the printer."""
+
+    def __init__(
+        self, method: Optional[str] = None, ind: int = 0, suffix: Optional[str] = None
+    ):
+        """Initialize the indexing method."""
+        self._method = method
+        self._ind = ind
+        self._suffix = suffix
+
+    def _get_index(self, ind: int) -> str:
+        if self._method is None:
+            return ""
+        default_suffix = ". "
+        if self._method == "number":
+            base = str(ind + 1)
+        elif self._method in ["lower", "upper", "letter", "Letter"]:
+            if ind >= 26:
+                raise ValueError("Letter-based indexing method only supports 26 items.")
+            base = chr(ord("A") + ind)
+            if self._method in ["lower", "letter"]:
+                base = base.lower()
+        elif self._method in ["roman", "Roman"]:
+            base = roman.toRoman(ind + 1)
+            if self._method == "roman":
+                base = base.lower()
+        else:
+            default_suffix = " "
+            if self._method == "star":
+                base = "*"
+            elif self._method == "dash":
+                base = "-"
+            elif self._method.startswith("sharp"):
+                base = "#" * int(self._method[5:])
+            else:
+                base = self._method
+
+        return base + (self._suffix or default_suffix)
+
+    def get_index(self, ind: Optional[int] = None) -> str:
+        """Get the index string for the current or given index."""
+        if ind is None:
+            ind = self._ind
+            self._ind += 1
+        if ind < 0:
+            raise ValueError("Indexing method does not support negative indexing.")
+        return self._get_index(ind)
+
+    def __repr__(self) -> str:
+        return f"Indexing(method={self._method!r}, ind={self._ind!r}, suffix={self._suffix!r})"
+
+
+@dataclass
+class PrinterState:
+    """A state of the printer."""
+
+    # settings
+    role: Optional[MessageRole] = None
+    """The role to be used for the message."""
+    separator: str = "\n"
+    """The separator to be used between texts."""
+    indexing: Indexing = Indexing(None, 0)
+    """The indexing method to be used."""
+    indent: str = ""
+    """The indent to be used in the beginning of each line."""
+    # inline means the first indent and indexing is inherited from the previous state
+    is_inline: bool = False
+    """Whether the state is inline. Inline means the first indent and
+    indexing is inherited from the previous non-inline state."""
+    # states
+    is_start: bool = True
+    """Whether the state is at the start of the scope."""
+    current_sep: str = ""
+    """The current separator to be used between texts."""
+
+
+@dataclass
+class PrinterPush:
+    """A record to push a new printer state to the stack."""
+
+    new_role: Optional[MessageRole] = None
+    """The new role to be used for the message."""
+    separator: Optional[str] = None
+    """The separator to be used between texts."""
+    indexing: Optional[Indexing] = None
+    """The indexing method to be used."""
+    inc_indent: str = ""
+    """The increment of the indent."""
+    new_indent: Optional[str] = None
+    """The new indent to be used."""
+    is_inline: Optional[bool] = False
+    """Whether the state is inline."""
+
+
+@dataclass
+class PrinterPop:
+    """A record to pop the last printer state from the stack."""
+
+
+RecordType = Union[BaseMessage, StringFuture, Image, PrinterPush, PrinterPop]
+"""Types allowed in the prompt records."""
+
+
+class PromptRecords:
+    """A class represents a list of prompt records."""
+
+    def __init__(self) -> None:
+        """Initialize the prompt records."""
+        self._records: List[RecordType] = []
+
+    @property
+    def records(self) -> List[RecordType]:
+        """The list of records."""
+        return self._records
+
+    def as_convo(self) -> Conversation:
+        """Convert the prompt records to a conversation."""
+        return PromptPrinter()(self)
+
+    def record(self, record: Union[str, RecordType]) -> None:
+        """Record a string, message, image, printer push or printer pop."""
+        if isinstance(record, str):  # compatible to str
+            record = StringFuture(record)
+        if (
+            isinstance(record, StringFuture)
+            or isinstance(record, Image)
+            or isinstance(record, BaseMessage)
+            or isinstance(record, PrinterPush)
+            or isinstance(record, PrinterPop)
+        ):
+            self._records.append(record)
+        else:
+            raise ValueError("Can only record Message, PrinterPush or PrinterPop")
+
+    def extend(self, record: "PromptRecords") -> None:
+        """Extend the prompt records with another prompt records."""
+        self._records.extend(record._records)
+
+    def copy(self) -> "PromptRecords":
+        """Copy the prompt records."""
+        return copy.deepcopy(self)
+
+    def __str__(self) -> str:
+        return str(self.as_convo())
+
+
+class PromptPrinter:
+    """A class to print prompt records as conversation.
+
+    The printer maintains a stack of printer states about the
+    current role, separator, indexing, and indentation.
+    """
+
+    def __init__(
+        self, states: Optional[List[PrinterState]] = None, is_newline: bool = True
+    ) -> None:
+        """Initialize the prompt printer."""
+        if states is None:
+            states = [PrinterState()]
+        self._states = states
+        self._is_newline = is_newline
+
+    @property
+    def states(self) -> List[PrinterState]:
+        """The stack of printer states."""
+        return self._states
+
+    def push(self, data: PrinterPush) -> None:
+        """Push a new printer state to the stack."""
+        self._push(**data.__dict__)
+
+    def pop(self) -> None:
+        """Pop the last printer state from the stack."""
+        if len(self._states) == 1:
+            raise ValueError("Cannot pop the first state.")
+        self._states.pop()
+
+    def _push(
+        self,
+        new_role: Optional[MessageRole] = None,
+        separator: Optional[str] = None,
+        indexing: Optional[Indexing] = None,
+        inc_indent: str = "",
+        new_indent: Optional[str] = None,
+        is_inline: bool = False,
+    ) -> None:
+        state = self.states[-1]
+        if new_role is None or new_role == state.role:
+            new_role = state.role
+            current_separator = state.current_sep
+            default_separator = state.separator  # Use the same separator as parent
+            default_indexing = state.indexing  # Use the same indexing as parent
+        else:  # a new role started
+            logger.debug(f"new role started {new_role}")
+            if len(self.states) > 1:
+                raise ValueError(
+                    "Cannot start a new role when there are states in the stack."
+                )
+            state.is_start = True  # reset the outmost state
+            state.current_sep = ""  # also reset the current separator
+            current_separator = ""
+            default_separator = "\n"
+            default_indexing = Indexing(None, 0)  # create a empty indexing
+            if new_indent is None:
+                new_indent = ""  # reset the indent
+                if inc_indent:
+                    raise ValueError(
+                        "Cannot specify inc_indent when new role started. "
+                        "Use new_indent instead."
+                    )
+
+        if separator is None:
+            separator = default_separator
+        if indexing is None:
+            indexing = default_indexing
+        else:
+            # Avoid changing the original indexing (could be a record)
+            indexing = copy.copy(indexing)
+        if new_indent is None:
+            new_indent = state.indent + inc_indent  # increment the indent
+        elif inc_indent:
+            raise ValueError("Cannot specify both inc_indent and new_indent.")
+
+        self._states.append(
+            PrinterState(
+                new_role,
+                separator,
+                indexing,
+                new_indent,
+                is_inline,
+                True,
+                # The current separator is inherited from the parent state
+                # it will change to its own separator after the first print.
+                current_sep=current_separator,
+            )
+        )
+
+    def _print_str(self, content: String) -> StringFuture:
+        state, previous = self._states[-1], self._states[:-1]
+        role = state.role
+        sep = state.current_sep
+        indent = state.indent
+        indexing = state.indexing
+        if state.is_start:  # is the first content in this scope
+            state.is_start = False
+            state.current_sep = state.separator
+            for st in previous[::-1]:
+                if st.role != role:
+                    break
+                if st.is_start:
+                    # after first print, change the separator to its own
+                    st.is_start = False
+                    st.current_sep = st.separator
+                else:
+                    break
+
+            if state.is_inline:
+                # inline means the first indent and indexing is
+                # inherited from the previous non-inline state
+                for st in previous[::-1]:
+                    if st.role != role:
+                        break
+                    if not st.is_inline:
+                        # Use the first non-inline's indent and indexing
+                        indent = st.indent
+                        indexing = st.indexing
+                        break
+        if sep.endswith("\n"):
+            self._is_newline = True
+
+        s = StringFuture(sep)
+        if self._is_newline:
+            if indent:
+                s += indent
+            self._is_newline = False
+        if cur_idx := indexing.get_index():
+            s += cur_idx
+        s += content
+
+        # TODO: maybe check whether `s` ends with newline
+        return s
+
+    def _print_message(self, content: String) -> BaseMessage:
+        """Print a string as message with the current printer state."""
+        role = self._states[-1].role  # the default role within the context
+        content = self._print_str(content)
+        return as_message(role, content)
+
+    def _print(
+        self, contents: Union[String, Image, BaseMessage, PromptRecords]
+    ) -> Conversation:
+        convo = Conversation(system_messages=[], messages=[])
+
+        def handle(rec: Union[RecordType, Image, str]) -> None:
+            if isinstance(rec, (str, StringFuture)):
+                convo.append(self._print_message(rec))
+            elif isinstance(rec, Image):
+                convo.append(as_message(self._states[-1].role, rec))
+                state = self._states[-1]
+                # reset current state after image, TODO: double check
+                state.is_start = True
+                state.current_sep = ""
+            elif isinstance(rec, BaseMessage):
+                convo.append(rec)
+                if rec.role is not None and len(self._states) == 1:
+                    # change role in the outmost state
+                    state = self._states[0]
+                    state.is_start = True  # reset the outmost state
+                    state.current_sep = ""  # also reset the current separator
+                # TODO: what should be the behavior if the role is changed
+                # in states other than the outmost one?
+                # should such behavior being allowed?
+
+            elif isinstance(rec, PrinterPush):
+                self.push(rec)
+            elif isinstance(rec, PrinterPop):
+                self.pop()
+            else:
+                raise ValueError(f"Unknown record type {type(rec)}")
+
+        if isinstance(contents, PromptRecords):
+            for rec in contents.records:
+                handle(rec)
+        else:
+            handle(contents)
+
+        return convo
+
+    __call__ = _print
```

### Comparing `applang-0.0.1a3/src/appl/core/promptable/base.py` & `applang-0.0.1a4/src/appl/core/promptable/base.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from ..types import *
-
-
-class Promptable(ABC):
-    """Interface for objects that can be converted to a prompt string."""
-
-    @abstractmethod
-    def __prompt__(self) -> Any:
-        """Convert the object to a prompt object."""
-        raise NotImplementedError
-
-
-def promptify(obj: Any) -> Any:
-    """Convert an object to a prompt object if it is promptable."""
-    if isinstance(obj, Promptable):
-        s = obj.__prompt__()
-        if isinstance(s, str):
-            s = StringFuture(s)
-        return s
-
-    return StringFuture(str(obj))
+from ..types import *
+
+
+class Promptable(ABC):
+    """Interface for objects that can be converted to a prompt string."""
+
+    @abstractmethod
+    def __prompt__(self) -> Any:
+        """Convert the object to a prompt object."""
+        raise NotImplementedError
+
+
+def promptify(obj: Any) -> Any:
+    """Convert an object to a prompt object if it is promptable."""
+    if isinstance(obj, Promptable):
+        s = obj.__prompt__()
+        if isinstance(s, str):
+            s = StringFuture(s)
+        return s
+
+    return StringFuture(str(obj))
```

### Comparing `applang-0.0.1a3/src/appl/core/promptable/definition.py` & `applang-0.0.1a4/src/appl/core/promptable/definition.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from ..types import *
-from .base import Promptable
-from .formatter import Formattable, FormatterMeta
-
-
-class Definition(Promptable, Formattable):
-    """Represent a definition of a concept.
-
-    Attributes:
-        fstr: The format string for the definition.
-        name: The name of the definition.
-        desc: A description of the definition.
-        _forks: A list of all instances of this class.
-    """
-
-    fstr: str = "{}"
-    name: String = "Definition"
-    desc: String = ""
-    _forks: List["Definition"] = []
-
-    def __init__(
-        self,
-        name: Optional[String] = None,
-        desc: Optional[String] = None,
-        *,
-        sep: String = ": ",
-        details: Any = None,
-        fstr: Optional[str] = None,
-        var_name: Optional[str] = None,
-    ):
-        """Initialize the Definition with the given name and description.
-
-        Args:
-            name: The name of the definition.
-            desc: A description of the definition.
-            sep: The separator between the name and description.
-            details: Additional details about the definition.
-            fstr: The format string for the definition.
-            var_name: The name of the variable that the definition is stored in.
-        """
-        if name is not None:
-            self.name = name
-        if desc is not None:
-            self.desc = desc
-        self.sep = sep
-        self.details = details
-        if fstr is not None:
-            self.fstr = fstr
-        self.var_name = var_name or name
-
-        self._forks.append(self)
-
-    def __hash__(self) -> int:
-        return hash(self.var_name)
-
-    def __prompt__(self) -> List[Any]:
-        # Used when add the Definition to the prompt
-        desc = self.desc or ""
-        res = [f"{self.name}{self.sep}{desc}"]
-        if self.details is not None:
-            res.append(self.details)
-        return res
-
-    def __repr__(self):
-        # Used to display information
-        desc = self.desc or ""
-        s = f"{self.name}{self.sep}{desc}"
-        if self.details is not None:
-            s += f"\n{self.details}"
-        return s
-
-    def __str__(self):
-        # Used for reference in the prompt
-        return self.fstr.format(self.name)
-
-
-class BracketedDefinition(Definition):
-    """A Definition that is formatted with square brackets."""
-
-    fstr = "[{}]"
-
-
-def define(def_name: str, format_str: str = "{}") -> type:
-    """Create a new Definition subclass with the given name and format string."""
-
-    class CustomDef(Definition):
-        name = def_name
-        fstr = format_str
-
-    return CustomDef
-
-
-def define_bracketed(def_name: str) -> type:
-    """Create a new BracketedDefinition subclass with the given name."""
-
-    class CustomDef(BracketedDefinition):
-        name = def_name
-
-    return CustomDef
+from ..types import *
+from .base import Promptable
+from .formatter import Formattable, FormatterMeta
+
+
+class Definition(Promptable, Formattable):
+    """Represent a definition of a concept.
+
+    Attributes:
+        fstr: The format string for the definition.
+        name: The name of the definition.
+        desc: A description of the definition.
+        _forks: A list of all instances of this class.
+    """
+
+    fstr: str = "{}"
+    name: String = "Definition"
+    desc: String = ""
+    _forks: List["Definition"] = []
+
+    def __init__(
+        self,
+        name: Optional[String] = None,
+        desc: Optional[String] = None,
+        *,
+        sep: String = ": ",
+        details: Any = None,
+        fstr: Optional[str] = None,
+        var_name: Optional[str] = None,
+    ):
+        """Initialize the Definition with the given name and description.
+
+        Args:
+            name: The name of the definition.
+            desc: A description of the definition.
+            sep: The separator between the name and description.
+            details: Additional details about the definition.
+            fstr: The format string for the definition.
+            var_name: The name of the variable that the definition is stored in.
+        """
+        if name is not None:
+            self.name = name
+        if desc is not None:
+            self.desc = desc
+        self.sep = sep
+        self.details = details
+        if fstr is not None:
+            self.fstr = fstr
+        self.var_name = var_name or name
+
+        self._forks.append(self)
+
+    def __hash__(self) -> int:
+        return hash(self.var_name)
+
+    def __prompt__(self) -> List[Any]:
+        # Used when add the Definition to the prompt
+        desc = self.desc or ""
+        res = [f"{self.name}{self.sep}{desc}"]
+        if self.details is not None:
+            res.append(self.details)
+        return res
+
+    def __repr__(self):
+        # Used to display information
+        desc = self.desc or ""
+        s = f"{self.name}{self.sep}{desc}"
+        if self.details is not None:
+            s += f"\n{self.details}"
+        return s
+
+    def __str__(self):
+        # Used for reference in the prompt
+        return self.fstr.format(self.name)
+
+
+class BracketedDefinition(Definition):
+    """A Definition that is formatted with square brackets."""
+
+    fstr = "[{}]"
+
+
+def define(def_name: str, format_str: str = "{}") -> type:
+    """Create a new Definition subclass with the given name and format string."""
+
+    class CustomDef(Definition):
+        name = def_name
+        fstr = format_str
+
+    return CustomDef
+
+
+def define_bracketed(def_name: str) -> type:
+    """Create a new BracketedDefinition subclass with the given name."""
+
+    class CustomDef(BracketedDefinition):
+        name = def_name
+
+    return CustomDef
```

### Comparing `applang-0.0.1a3/src/appl/core/promptable/formatter.py` & `applang-0.0.1a4/src/appl/core/promptable/formatter.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from abc import ABCMeta
-
-from ..types import *
-
-
-# ABCMeta is required since Promptable is an abstract class
-class FormatterMeta(ABCMeta):
-    """Metaclass for classes that can be formatted."""
-
-    def _get_format_str(cls):
-        if fstr := getattr(cls, "fstr", None):
-            return fstr
-        return getattr(cls, "__format_str__", "{}")
-
-    def _get_format_name(cls):
-        if name := getattr(cls, "name", None):
-            return name
-        return getattr(cls, "__format_name__", cls.__name__)
-
-    def __format__(cls, format_spec: str) -> str:
-        fstr = cls._get_format_str()
-        name = cls._get_format_name()
-        return fstr.format(name, format_spec=format_spec)
-
-    def __repr__(cls):
-        return cls._get_format_name()
-
-
-class Formattable(metaclass=FormatterMeta):
-    """Base class for class objects that can be formatted.
-
-    Example:
-        ```py
-        >>> class Example(Formattable):
-        ...     fstr: str = "[{}]"
-        ...     name: str = "example"
-        >>> print(f"{Example}")
-        [example]
-        ```
-    """
-
-    fstr: str
-    name: String
+from abc import ABCMeta
+
+from ..types import *
+
+
+# ABCMeta is required since Promptable is an abstract class
+class FormatterMeta(ABCMeta):
+    """Metaclass for classes that can be formatted."""
+
+    def _get_format_str(cls):
+        if fstr := getattr(cls, "fstr", None):
+            return fstr
+        return getattr(cls, "__format_str__", "{}")
+
+    def _get_format_name(cls):
+        if name := getattr(cls, "name", None):
+            return name
+        return getattr(cls, "__format_name__", cls.__name__)
+
+    def __format__(cls, format_spec: str) -> str:
+        fstr = cls._get_format_str()
+        name = cls._get_format_name()
+        return fstr.format(name, format_spec=format_spec)
+
+    def __repr__(cls):
+        return cls._get_format_name()
+
+
+class Formattable(metaclass=FormatterMeta):
+    """Base class for class objects that can be formatted.
+
+    Example:
+        ```py
+        >>> class Example(Formattable):
+        ...     fstr: str = "[{}]"
+        ...     name: str = "example"
+        >>> print(f"{Example}")
+        [example]
+        ```
+    """
+
+    fstr: str
+    name: String
```

### Comparing `applang-0.0.1a3/src/appl/core/response.py` & `applang-0.0.1a4/src/appl/core/response.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-import time
-
-from litellm import (
-    CustomStreamWrapper,
-    ModelResponse,
-    completion_cost,
-    stream_chunk_builder,
-)
-from litellm.utils import Delta, Function
-from openai import Stream
-from openai.types.chat import (
-    ChatCompletion,
-    ChatCompletionChunk,
-    ChatCompletionMessageToolCall,
-)
-from openai.types.chat.chat_completion import Choice
-from openai.types.chat.chat_completion_chunk import (
-    ChoiceDelta,
-    ChoiceDeltaToolCallFunction,
-)
-from pydantic import model_validator
-from tqdm import tqdm
-
-from ..core.types import *
-from .config import configs
-from .tool import ToolCall
-from .types import *
-
-
-class CompletionResponse(BaseModel):
-    """A class wrapping the response from the LLM model.
-
-    For a streaming response, it tracks the chunks of the response and
-    builds the complete response when the streaming is finished.
-    """
-
-    raw_response: Any = Field(None, description="The raw response from the model")
-    """The raw response from the model."""
-    cost: Optional[float] = Field(None, description="The cost of the completion")
-    """The cost of the completion."""
-    chunks: List[Union[ModelResponse, ChatCompletionChunk]] = Field(
-        [], description="The chunks of the response when streaming"
-    )
-    """The chunks of the response when streaming."""
-    is_stream: bool = Field(False, description="Whether the response is a stream")
-    """Whether the response is a stream."""
-    is_finished: bool = Field(
-        False, description="Whether the response stream is finished"
-    )
-    """Whether the response stream is finished."""
-    post_finish_callbacks: List[Callable] = Field(
-        [], description="The post finish callbacks"
-    )
-    """The post finish callbacks."""
-    response_model: Any = Field(None, description="The given response model")
-    """The given response model."""
-    response_obj: Any = Field(
-        None, description="The response object of response model, could be a stream"
-    )
-    """The response object of response model, could be a stream."""
-    message: Optional[str] = Field(
-        None, description="The top-choice message from the completion"
-    )
-    """The top-choice message from the completion."""
-    tool_calls: List[ToolCall] = Field([], description="The tool calls")
-    """The tool calls."""
-
-    @model_validator(mode="after")
-    def _post_init(self) -> "CompletionResponse":
-        self._complete_response = None
-
-        if isinstance(self.raw_response, (CustomStreamWrapper, Stream)):
-            # ? supports for Async Steam?
-            self.is_stream = True
-        else:
-            self._finish(self.raw_response)  # type: ignore
-        return self
-
-    @property
-    def complete_response(self) -> Union[ModelResponse, ChatCompletion]:
-        """The complete response from the model. This will block until the response is finished."""
-        if self.is_finished:
-            return self._complete_response
-        self.streaming(display=False)
-        assert self.is_finished, "Response should be finished after streaming"
-        return self._complete_response  # type: ignore
-
-    @property
-    def results(self) -> Any:
-        """The results of the response.
-
-        Returns:
-            message (str):
-                The message if the response is a text completion.
-            tool_calls (List[ToolCall]):
-                The tool calls if the response is a list of tool calls.
-            response_obj (Any):
-                The object if the response is a response object.
-        """
-        if self.is_stream and not self.is_finished:
-            self.streaming()  # display the stream and finish the response
-        results: Any = self.message
-        if self.response_obj is not None:
-            results = self.response_obj
-        elif len(self.tool_calls):
-            results = self.tool_calls
-        return results
-
-    @property
-    def type(self) -> ResponseType:
-        """The type of the response."""
-        if not self.is_finished:
-            return ResponseType.UNFINISHED
-        if self.response_model is not None and self.response_obj is not None:
-            return ResponseType.OBJECT
-        if len(self.tool_calls):
-            return ResponseType.TOOL_CALL
-        return ResponseType.TEXT
-
-    def streaming(self, display: bool = True) -> "CompletionResponse":
-        """Stream the response object and finish the response."""
-        if not self.is_stream:
-            raise ValueError("Cannot iterate over non-streaming response")
-        if self.is_finished:
-            return self
-        if self.response_obj is not None:
-            if display:
-                interval = configs.getattrs("settings.logging.display.stream_interval")
-                pbar = tqdm(self.response_obj, desc="Streaming", dynamic_ncols=True)
-                current_time = time.time()
-                for chunk in pbar:
-                    if time.time() - current_time > interval:
-                        current_time = time.time()
-                        pbar.set_description(str(chunk.model_dump()))
-                logger.info(
-                    f"Response object streaming finished with:\n{chunk.model_dump()}"
-                )
-                pbar.close()
-            else:
-                for chunk in self.response_obj:
-                    pass
-            self.response_obj = chunk.model_dump()
-        else:
-            print("===== APPL BEGIN STREAMING =====", flush=True)
-            suffix = ""
-            for chunk in iter(self):
-                if not display:
-                    continue
-                suffix = self._print_chunk(chunk, suffix)
-            print(suffix, flush=True)
-            print("===== APPL END STREAMING =====", flush=True)
-        return self
-
-    def register_post_finish_callback(self, callback: Callable) -> None:
-        """Register a post finish callback.
-
-        The callback will be called after the response is finished.
-        """
-        if self.is_finished:
-            callback(self)
-        else:
-            self.post_finish_callbacks.append(callback)
-
-    def _print_chunk(
-        self, chunk: Union[ModelResponse, ChatCompletionChunk], suffix: str = ""
-    ) -> str:
-        delta: Union[Delta, ChoiceDelta] = chunk.choices[0].delta
-
-        def flush(content: str) -> None:
-            print(content, end="", flush=True)
-
-        if delta is not None:
-            if delta.content is not None:
-                flush(delta.content)
-            elif getattr(delta, "tool_calls", None):
-                f: Union[Function, ChoiceDeltaToolCallFunction] = delta.tool_calls[
-                    0
-                ].function  # type: ignore
-                if f.name is not None:
-                    if suffix:
-                        flush(f"{suffix}, ")
-                    flush(f"{f.name}(")
-                    suffix = ")"
-                if f.arguments is not None:
-                    flush(f.arguments)
-        return suffix
-
-    def _finish(self, response: Any) -> None:
-        if self.is_finished:
-            logger.warning("Response already finished. Ignoring finish call.")
-            return
-        self.is_finished = True
-        self._complete_response = response
-        # parse the message and tool calls
-        if isinstance(response, (ModelResponse, ChatCompletion)):
-            message = response.choices[0].message
-            if getattr(message, "tool_calls", None):
-                for call in message.tool_calls:
-                    self.tool_calls.append(ToolCall.from_openai_tool_call(call))
-            elif message.content is not None:
-                self.message = message.content
-            else:
-                raise ValueError(f"Invalid response: {response}")
-        # post finish hook
-        for callback in self.post_finish_callbacks:
-            callback(self)
-
-    def _finish_stream(self) -> None:
-        try:
-            response = stream_chunk_builder(self.chunks)
-        except Exception:
-            logger.error("Error when building the response from the stream")
-            raise
-        self._finish(response)
-
-    def __str__(self):
-        if self.is_stream and not self.is_finished:
-            return repr(self)
-        return str(self.results)
-
-    def __next__(self):
-        if not self.is_stream:
-            raise ValueError("Cannot iterate over non-streaming response")
-        try:
-            chunk = next(self.raw_response)
-            self.chunks.append(chunk)
-            return chunk
-        except StopIteration:
-            self._finish_stream()
-            raise StopIteration
-
-    def __iter__(self):
-        if not self.is_stream:
-            raise ValueError("Cannot iterate over non-streaming response")
-        return self
-
-    def __getattr__(self, name: str) -> Any:
-        return getattr(self.complete_response, name)
+import time
+
+from litellm import (
+    CustomStreamWrapper,
+    ModelResponse,
+    completion_cost,
+    stream_chunk_builder,
+)
+from litellm.utils import Delta, Function
+from openai import Stream
+from openai.types.chat import (
+    ChatCompletion,
+    ChatCompletionChunk,
+    ChatCompletionMessageToolCall,
+)
+from openai.types.chat.chat_completion import Choice
+from openai.types.chat.chat_completion_chunk import (
+    ChoiceDelta,
+    ChoiceDeltaToolCallFunction,
+)
+from pydantic import model_validator
+from tqdm import tqdm
+
+from ..core.types import *
+from .config import configs
+from .tool import ToolCall
+from .types import *
+
+
+class CompletionResponse(BaseModel):
+    """A class wrapping the response from the LLM model.
+
+    For a streaming response, it tracks the chunks of the response and
+    builds the complete response when the streaming is finished.
+    """
+
+    raw_response: Any = Field(None, description="The raw response from the model")
+    """The raw response from the model."""
+    cost: Optional[float] = Field(None, description="The cost of the completion")
+    """The cost of the completion."""
+    chunks: List[Union[ModelResponse, ChatCompletionChunk]] = Field(
+        [], description="The chunks of the response when streaming"
+    )
+    """The chunks of the response when streaming."""
+    is_stream: bool = Field(False, description="Whether the response is a stream")
+    """Whether the response is a stream."""
+    is_finished: bool = Field(
+        False, description="Whether the response stream is finished"
+    )
+    """Whether the response stream is finished."""
+    post_finish_callbacks: List[Callable] = Field(
+        [], description="The post finish callbacks"
+    )
+    """The post finish callbacks."""
+    response_model: Any = Field(None, description="The given response model")
+    """The given response model."""
+    response_obj: Any = Field(
+        None, description="The response object of response model, could be a stream"
+    )
+    """The response object of response model, could be a stream."""
+    message: Optional[str] = Field(
+        None, description="The top-choice message from the completion"
+    )
+    """The top-choice message from the completion."""
+    tool_calls: List[ToolCall] = Field([], description="The tool calls")
+    """The tool calls."""
+
+    @model_validator(mode="after")
+    def _post_init(self) -> "CompletionResponse":
+        self._complete_response = None
+
+        if isinstance(self.raw_response, (CustomStreamWrapper, Stream)):
+            # ? supports for Async Steam?
+            self.is_stream = True
+        else:
+            self._finish(self.raw_response)  # type: ignore
+        return self
+
+    @property
+    def complete_response(self) -> Union[ModelResponse, ChatCompletion]:
+        """The complete response from the model. This will block until the response is finished."""
+        if self.is_finished:
+            return self._complete_response
+        self.streaming(display=False)
+        assert self.is_finished, "Response should be finished after streaming"
+        return self._complete_response  # type: ignore
+
+    @property
+    def results(self) -> Any:
+        """The results of the response.
+
+        Returns:
+            message (str):
+                The message if the response is a text completion.
+            tool_calls (List[ToolCall]):
+                The tool calls if the response is a list of tool calls.
+            response_obj (Any):
+                The object if the response is a response object.
+        """
+        if self.is_stream and not self.is_finished:
+            self.streaming()  # display the stream and finish the response
+        results: Any = self.message
+        if self.response_obj is not None:
+            results = self.response_obj
+        elif len(self.tool_calls):
+            results = self.tool_calls
+        return results
+
+    @property
+    def type(self) -> ResponseType:
+        """The type of the response."""
+        if not self.is_finished:
+            return ResponseType.UNFINISHED
+        if self.response_model is not None and self.response_obj is not None:
+            return ResponseType.OBJECT
+        if len(self.tool_calls):
+            return ResponseType.TOOL_CALL
+        return ResponseType.TEXT
+
+    def streaming(self, display: bool = True) -> "CompletionResponse":
+        """Stream the response object and finish the response."""
+        if not self.is_stream:
+            raise ValueError("Cannot iterate over non-streaming response")
+        if self.is_finished:
+            return self
+        if self.response_obj is not None:
+            if display:
+                interval = configs.getattrs("settings.logging.display.stream_interval")
+                pbar = tqdm(self.response_obj, desc="Streaming", dynamic_ncols=True)
+                current_time = time.time()
+                for chunk in pbar:
+                    if time.time() - current_time > interval:
+                        current_time = time.time()
+                        pbar.set_description(str(chunk.model_dump()))
+                logger.info(
+                    f"Response object streaming finished with:\n{chunk.model_dump()}"
+                )
+                pbar.close()
+            else:
+                for chunk in self.response_obj:
+                    pass
+            self.response_obj = chunk.model_dump()
+        else:
+            print("===== APPL BEGIN STREAMING =====", flush=True)
+            suffix = ""
+            for chunk in iter(self):
+                if not display:
+                    continue
+                suffix = self._print_chunk(chunk, suffix)
+            print(suffix, flush=True)
+            print("===== APPL END STREAMING =====", flush=True)
+        return self
+
+    def register_post_finish_callback(self, callback: Callable) -> None:
+        """Register a post finish callback.
+
+        The callback will be called after the response is finished.
+        """
+        if self.is_finished:
+            callback(self)
+        else:
+            self.post_finish_callbacks.append(callback)
+
+    def _print_chunk(
+        self, chunk: Union[ModelResponse, ChatCompletionChunk], suffix: str = ""
+    ) -> str:
+        delta: Union[Delta, ChoiceDelta] = chunk.choices[0].delta
+
+        def flush(content: str) -> None:
+            print(content, end="", flush=True)
+
+        if delta is not None:
+            if delta.content is not None:
+                flush(delta.content)
+            elif getattr(delta, "tool_calls", None):
+                f: Union[Function, ChoiceDeltaToolCallFunction] = delta.tool_calls[
+                    0
+                ].function  # type: ignore
+                if f.name is not None:
+                    if suffix:
+                        flush(f"{suffix}, ")
+                    flush(f"{f.name}(")
+                    suffix = ")"
+                if f.arguments is not None:
+                    flush(f.arguments)
+        return suffix
+
+    def _finish(self, response: Any) -> None:
+        if self.is_finished:
+            logger.warning("Response already finished. Ignoring finish call.")
+            return
+        self.is_finished = True
+        self._complete_response = response
+        # parse the message and tool calls
+        if isinstance(response, (ModelResponse, ChatCompletion)):
+            message = response.choices[0].message
+            if getattr(message, "tool_calls", None):
+                for call in message.tool_calls:
+                    self.tool_calls.append(ToolCall.from_openai_tool_call(call))
+            elif message.content is not None:
+                self.message = message.content
+            else:
+                raise ValueError(f"Invalid response: {response}")
+        # post finish hook
+        for callback in self.post_finish_callbacks:
+            callback(self)
+
+    def _finish_stream(self) -> None:
+        try:
+            response = stream_chunk_builder(self.chunks)
+        except Exception:
+            logger.error("Error when building the response from the stream")
+            raise
+        self._finish(response)
+
+    def __str__(self):
+        if self.is_stream and not self.is_finished:
+            return repr(self)
+        return str(self.results)
+
+    def __next__(self):
+        if not self.is_stream:
+            raise ValueError("Cannot iterate over non-streaming response")
+        try:
+            chunk = next(self.raw_response)
+            self.chunks.append(chunk)
+            return chunk
+        except StopIteration:
+            self._finish_stream()
+            raise StopIteration
+
+    def __iter__(self):
+        if not self.is_stream:
+            raise ValueError("Cannot iterate over non-streaming response")
+        return self
+
+    def __getattr__(self, name: str) -> Any:
+        return getattr(self.complete_response, name)
```

### Comparing `applang-0.0.1a3/src/appl/core/runtime.py` & `applang-0.0.1a4/src/appl/core/runtime.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-"""helper functions for runtime execution within the compiled function."""
-
-from .context import PromptContext
-from .generation import Generation
-from .message import BaseMessage
-from .printer import PromptRecords
-from .promptable import Promptable, promptify
-from .types import *
-
-
-def appl_with_ctx(
-    *args: Any,
-    _func: Callable,
-    _ctx: PromptContext = PromptContext(),
-    _globals: Any = None,
-    _locals: Any = None,
-    **kwargs: Any,
-) -> Any:
-    """Forward context to prompt functions."""
-    if _func is globals:
-        # use the globals when calling the function
-        return _globals
-    if _func is locals:
-        # use the locals when calling the function
-        return _locals
-    if _func in (exec, eval):
-        # fix the globals and locals for exec and eval
-        if len(args) < 2 and "globals" not in kwargs:
-            args = args + (_globals,)
-        elif len(args) < 3 and "locals" not in kwargs:
-            args = args + (_locals,)
-    if getattr(_func, "__need_ctx__", False):
-        kwargs["_ctx"] = _ctx  # add the context to the kwargs
-    return _func(*args, **kwargs)
-
-
-def appl_execute(
-    s: Any,
-    _ctx: PromptContext = PromptContext(),
-) -> None:
-    """Interact with the prompt context using the given value."""
-    if s is None:
-        return
-    if isinstance(s, str):
-        if _ctx._exclude_first_str and _ctx._is_first_str:
-            logger.debug(f'The first string """{s}""" is excluded from prompt.')
-        else:
-            _ctx.add_string(StringFuture(s))
-        _ctx._is_first_str = False
-    elif isinstance(s, StringFuture):
-        _ctx.add_string(s)
-    elif isinstance(s, PromptRecords):
-        _ctx.add_records(s)
-    elif isinstance(s, BaseMessage):
-        _ctx.add_message(s)
-    elif isinstance(s, Image):
-        _ctx.add_image(s)
-    elif isinstance(s, Generation):
-        appl_execute(s.as_prompt(), _ctx)
-    elif isinstance(s, Promptable):
-        # recursively apply
-        appl_execute(promptify(s), _ctx)
-    elif isinstance(s, Sequence):
-        # sequence of items, recursively apply
-        for x in s:
-            appl_execute(x, _ctx)
-    elif isinstance(s, Namespace):  # for advanced usage only
-        logger.info(f"updating context variables using the namespace: {s}")
-        _ctx._set_vars(s)
-    else:
-        logger.warning(f"Cannot convert {s} of type {type(s)} to prompt, ignore.")
-
-
-def appl_format(
-    value: Any, format_spec: str = "", conversion: int = -1
-) -> StringFuture:
-    """Create a StringFuture object that represents the formatted string."""
-    if conversion >= 0:
-        conversion_func: Dict[str, Callable] = {"s": str, "r": repr, "a": ascii}
-        if (c := chr(conversion)) not in conversion_func:
-            raise ValueError(f"Invalid conversion character: {c}")
-        value = StringFuture(CallFuture(conversion_func[c], value))
-
-    return StringFuture(CallFuture(format, value, format_spec))
+"""helper functions for runtime execution within the compiled function."""
+
+from .context import PromptContext
+from .generation import Generation
+from .message import BaseMessage
+from .printer import PromptRecords
+from .promptable import Promptable, promptify
+from .types import *
+
+
+def appl_with_ctx(
+    *args: Any,
+    _func: Callable,
+    _ctx: PromptContext = PromptContext(),
+    _globals: Any = None,
+    _locals: Any = None,
+    **kwargs: Any,
+) -> Any:
+    """Forward context to prompt functions."""
+    if _func is globals:
+        # use the globals when calling the function
+        return _globals
+    if _func is locals:
+        # use the locals when calling the function
+        return _locals
+    if _func in (exec, eval):
+        # fix the globals and locals for exec and eval
+        if len(args) < 2 and "globals" not in kwargs:
+            args = args + (_globals,)
+        elif len(args) < 3 and "locals" not in kwargs:
+            args = args + (_locals,)
+    if getattr(_func, "__need_ctx__", False):
+        kwargs["_ctx"] = _ctx  # add the context to the kwargs
+    return _func(*args, **kwargs)
+
+
+def appl_execute(
+    s: Any,
+    _ctx: PromptContext = PromptContext(),
+) -> None:
+    """Interact with the prompt context using the given value."""
+    if s is None:
+        return
+    if isinstance(s, str):
+        if _ctx._exclude_first_str and _ctx._is_first_str:
+            logger.debug(f'The first string """{s}""" is excluded from prompt.')
+        else:
+            _ctx.add_string(StringFuture(s))
+        _ctx._is_first_str = False
+    elif isinstance(s, StringFuture):
+        _ctx.add_string(s)
+    elif isinstance(s, PromptRecords):
+        _ctx.add_records(s)
+    elif isinstance(s, BaseMessage):
+        _ctx.add_message(s)
+    elif isinstance(s, Image):
+        _ctx.add_image(s)
+    elif isinstance(s, Generation):
+        appl_execute(s.as_prompt(), _ctx)
+    elif isinstance(s, Promptable):
+        # recursively apply
+        appl_execute(promptify(s), _ctx)
+    elif isinstance(s, Sequence):
+        # sequence of items, recursively apply
+        for x in s:
+            appl_execute(x, _ctx)
+    elif isinstance(s, Namespace):  # for advanced usage only
+        logger.info(f"updating context variables using the namespace: {s}")
+        _ctx._set_vars(s)
+    else:
+        logger.warning(f"Cannot convert {s} of type {type(s)} to prompt, ignore.")
+
+
+def appl_format(
+    value: Any, format_spec: str = "", conversion: int = -1
+) -> StringFuture:
+    """Create a StringFuture object that represents the formatted string."""
+    if conversion >= 0:
+        conversion_func: Dict[str, Callable] = {"s": str, "r": repr, "a": ascii}
+        if (c := chr(conversion)) not in conversion_func:
+            raise ValueError(f"Invalid conversion character: {c}")
+        value = StringFuture(CallFuture(conversion_func[c], value))
+
+    return StringFuture(CallFuture(format, value, format_spec))
```

### Comparing `applang-0.0.1a3/src/appl/core/tool.py` & `applang-0.0.1a4/src/appl/core/tool.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-import inspect
-import json
-from abc import ABC, abstractmethod
-from inspect import Signature
-
-from docstring_parser import Docstring, parse
-from openai.types.chat import ChatCompletionMessageToolCall
-from pydantic import ConfigDict, create_model, field_serializer
-
-from .types import *
-
-# from pydantic._internal._model_construction import ModelMetaclass
-
-
-class BaseTool(BaseModel, ABC):
-    """The base class for a Tool."""
-
-    model_config = ConfigDict(arbitrary_types_allowed=True)
-
-    name: str = Field(..., description="The name of the Tool")
-    """The name of the Tool."""
-    short_desc: str = Field("", description="The short description of the Tool")
-    """The short description of the Tool."""
-    long_desc: str = Field("", description="The long description of the Tool")
-    """The long description of the Tool."""
-    params: type[BaseModel] = Field(..., description="The parameters of the Tool")
-    """The parameters of the Tool."""
-    returns: type[BaseModel] = Field(..., description="The return of the Tool")
-    """The return of the Tool."""
-    raises: List[Dict[str, Optional[str]]] = Field(
-        [], description="The exceptions raised by the Tool"
-    )
-    """The exceptions raised by the Tool."""
-    examples: List[str] = Field([], description="The examples of the Tool")
-    """The examples of the Tool."""
-    info: Dict = Field({}, description="Additional information of the Tool")
-    """Additional information of the Tool."""
-
-    # TODO: add toolkit option
-    def __init__(self, func: Callable, **predefined: Any):
-        """Create a tool from a function."""
-        name = func.__name__
-        sig = inspect.signature(func)
-        doc = func.__doc__
-        super().__init__(name=name, **self.parse_data(sig, doc, predefined))
-        self._predefined = predefined
-        self._func = func
-        self.__name__ = name
-        self.__signature__ = sig  # type: ignore
-        self.__doc__ = doc  # overwrite the doc string
-
-    @classmethod
-    def parse_data(
-        cls, sig: Signature, docstring: Optional[str], predefined: Dict[str, Any]
-    ) -> Dict[str, Any]:
-        """Parse data from the signature and docstring of a function."""
-        doc = parse(docstring or "")
-        data: Dict[str, Any] = {
-            "short_desc": doc.short_description or "",
-            "long_desc": doc.long_description or "",
-        }
-
-        # build params
-        params = {}
-        doc_param = {p.arg_name: p for p in doc.params}
-        for name, param in sig.parameters.items():
-            anno = param.annotation
-            default = param.default
-
-            if default is param.empty:
-                default = ...  # required
-            if name in doc_param:
-                # fill in desc for the param
-                default = Field(default, description=doc_param[name].description)
-                # fill in type annotation if not annotated in the function
-                if (anno is param.empty) and (doc_param[name].type_name is not None):
-                    # use type annotation from docstring
-                    anno = doc_param[name].type_name
-            # replace empty annotation with Any
-            if anno is param.empty:
-                anno = Any
-            if name not in predefined:
-                params[name] = (anno, default)
-        data["params"] = create_model("parameters", **params)  # type: ignore
-
-        # build returns
-        anno = sig.return_annotation
-        if anno is sig.empty:
-            if (doc.returns is not None) and (doc.returns.type_name is not None):
-                # use type annotation from docstring
-                anno = doc.returns.type_name
-            else:
-                anno = Any
-        default = ...  # required
-        if doc.returns is not None:
-            # fill in desc for the return
-            default = Field(..., description=doc.returns.description)
-        data["returns"] = create_model("returns", returns=(anno, default))
-
-        # build raises
-        data["raises"] = [
-            {"type": exc.type_name, "desc": exc.description} for exc in doc.raises
-        ]
-
-        # build examples
-        data["examples"] = doc.examples
-        return data
-
-    @property
-    def openai_schema(self) -> dict:
-        """Get the OpenAI schema of the tool."""
-        return {
-            "type": "function",
-            "function": {
-                "name": self.name,
-                "description": self._get_description(),
-                "parameters": self.params.model_json_schema(),
-            },
-        }
-
-    def to_str(self) -> str:
-        """Represent the tool as a string."""
-        s = f"def {self.name}{self.__signature__}:\n"
-        s += f'    """{self.__doc__}"""'
-        return s
-
-    @abstractmethod
-    def _get_description(self) -> str:
-        raise NotImplementedError
-
-    @field_serializer("params", when_used="json")
-    def _serialize_params(self, params: type[BaseModel]) -> dict:
-        return params.model_json_schema()
-
-    @field_serializer("returns", when_used="json")
-    def _serialize_returns(self, returns: type[BaseModel]) -> dict:
-        return returns.model_json_schema()
-
-    def __str__(self) -> str:
-        return self.to_str()
-
-    def _call(self, *args: Any, **kwargs: Any) -> Any:
-        kwargs.update(self._predefined)  # use predefined kwargs
-        return self._func(*args, **kwargs)
-
-    __call__ = _call
-
-
-class Tool(BaseTool):
-    """The Tool class that can be called by LLMs."""
-
-    def __init__(self, func: Callable, use_short_desc: bool = False, **kwargs: Any):
-        """Create a tool from a function.
-
-        Args:
-            func: The function to create the tool from.
-            use_short_desc:
-                Whether to use the short description instead of the full description.
-            kwargs: Additional arguments for the tool.
-        """
-        super().__init__(func=func, **kwargs)
-        self._use_short_desc = use_short_desc
-
-    def _get_description(self):
-        if not self.short_desc:
-            logger.warning(f"Tool {self.name} has no description.")
-            return self.name
-
-        if (not self.long_desc) or self._use_short_desc:
-            return self.short_desc
-
-        # use full desc
-        return self.short_desc + "\n\n" + self.long_desc
-
-
-class ToolCall(BaseModel):
-    """The class representing a tool call."""
-
-    id: str = Field(..., description="The ID of the tool call.")
-    """The ID of the tool call."""
-    name: str = Field(..., description="The name of the function to call.")
-    """The name of the function to call."""
-    args: str = Field(..., description="The arguments to call the function with.")
-    """The arguments to call the function with."""
-
-    def get_dict(self):
-        """Get the OpenAI format dictionary representation of the tool call."""
-        return {
-            "id": self.id,
-            "type": "function",
-            "function": {
-                "name": self.name,
-                "arguments": self.args,
-            },
-        }
-
-    @classmethod
-    def from_openai_tool_call(cls, call: ChatCompletionMessageToolCall) -> "ToolCall":
-        """Create a ToolCall from an OpenAI tool call."""
-        return cls(
-            id=call.id,
-            name=call.function.name,
-            args=call.function.arguments,
-        )
+import inspect
+import json
+from abc import ABC, abstractmethod
+from inspect import Signature
+
+from docstring_parser import Docstring, parse
+from openai.types.chat import ChatCompletionMessageToolCall
+from pydantic import ConfigDict, create_model, field_serializer
+
+from .types import *
+
+# from pydantic._internal._model_construction import ModelMetaclass
+
+
+class BaseTool(BaseModel, ABC):
+    """The base class for a Tool."""
+
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
+    name: str = Field(..., description="The name of the Tool")
+    """The name of the Tool."""
+    short_desc: str = Field("", description="The short description of the Tool")
+    """The short description of the Tool."""
+    long_desc: str = Field("", description="The long description of the Tool")
+    """The long description of the Tool."""
+    params: type[BaseModel] = Field(..., description="The parameters of the Tool")
+    """The parameters of the Tool."""
+    returns: type[BaseModel] = Field(..., description="The return of the Tool")
+    """The return of the Tool."""
+    raises: List[Dict[str, Optional[str]]] = Field(
+        [], description="The exceptions raised by the Tool"
+    )
+    """The exceptions raised by the Tool."""
+    examples: List[str] = Field([], description="The examples of the Tool")
+    """The examples of the Tool."""
+    info: Dict = Field({}, description="Additional information of the Tool")
+    """Additional information of the Tool."""
+
+    # TODO: add toolkit option
+    def __init__(self, func: Callable, **predefined: Any):
+        """Create a tool from a function."""
+        name = func.__name__
+        sig = inspect.signature(func)
+        doc = func.__doc__
+        super().__init__(name=name, **self.parse_data(sig, doc, predefined))
+        self._predefined = predefined
+        self._func = func
+        self.__name__ = name
+        self.__signature__ = sig  # type: ignore
+        self.__doc__ = doc  # overwrite the doc string
+
+    @classmethod
+    def parse_data(
+        cls, sig: Signature, docstring: Optional[str], predefined: Dict[str, Any]
+    ) -> Dict[str, Any]:
+        """Parse data from the signature and docstring of a function."""
+        doc = parse(docstring or "")
+        data: Dict[str, Any] = {
+            "short_desc": doc.short_description or "",
+            "long_desc": doc.long_description or "",
+        }
+
+        # build params
+        params = {}
+        doc_param = {p.arg_name: p for p in doc.params}
+        for name, param in sig.parameters.items():
+            anno = param.annotation
+            default = param.default
+
+            if default is param.empty:
+                default = ...  # required
+            if name in doc_param:
+                # fill in desc for the param
+                default = Field(default, description=doc_param[name].description)
+                # fill in type annotation if not annotated in the function
+                if (anno is param.empty) and (doc_param[name].type_name is not None):
+                    # use type annotation from docstring
+                    anno = doc_param[name].type_name
+            # replace empty annotation with Any
+            if anno is param.empty:
+                anno = Any
+            if name not in predefined:
+                params[name] = (anno, default)
+        data["params"] = create_model("parameters", **params)  # type: ignore
+
+        # build returns
+        anno = sig.return_annotation
+        if anno is sig.empty:
+            if (doc.returns is not None) and (doc.returns.type_name is not None):
+                # use type annotation from docstring
+                anno = doc.returns.type_name
+            else:
+                anno = Any
+        default = ...  # required
+        if doc.returns is not None:
+            # fill in desc for the return
+            default = Field(..., description=doc.returns.description)
+        data["returns"] = create_model("returns", returns=(anno, default))
+
+        # build raises
+        data["raises"] = [
+            {"type": exc.type_name, "desc": exc.description} for exc in doc.raises
+        ]
+
+        # build examples
+        data["examples"] = doc.examples
+        return data
+
+    @property
+    def openai_schema(self) -> dict:
+        """Get the OpenAI schema of the tool."""
+        return {
+            "type": "function",
+            "function": {
+                "name": self.name,
+                "description": self._get_description(),
+                "parameters": self.params.model_json_schema(),
+            },
+        }
+
+    def to_str(self) -> str:
+        """Represent the tool as a string."""
+        s = f"def {self.name}{self.__signature__}:\n"
+        s += f'    """{self.__doc__}"""'
+        return s
+
+    @abstractmethod
+    def _get_description(self) -> str:
+        raise NotImplementedError
+
+    @field_serializer("params", when_used="json")
+    def _serialize_params(self, params: type[BaseModel]) -> dict:
+        return params.model_json_schema()
+
+    @field_serializer("returns", when_used="json")
+    def _serialize_returns(self, returns: type[BaseModel]) -> dict:
+        return returns.model_json_schema()
+
+    def __str__(self) -> str:
+        return self.to_str()
+
+    def _call(self, *args: Any, **kwargs: Any) -> Any:
+        kwargs.update(self._predefined)  # use predefined kwargs
+        return self._func(*args, **kwargs)
+
+    __call__ = _call
+
+
+class Tool(BaseTool):
+    """The Tool class that can be called by LLMs."""
+
+    def __init__(self, func: Callable, use_short_desc: bool = False, **kwargs: Any):
+        """Create a tool from a function.
+
+        Args:
+            func: The function to create the tool from.
+            use_short_desc:
+                Whether to use the short description instead of the full description.
+            kwargs: Additional arguments for the tool.
+        """
+        super().__init__(func=func, **kwargs)
+        self._use_short_desc = use_short_desc
+
+    def _get_description(self):
+        if not self.short_desc:
+            logger.warning(f"Tool {self.name} has no description.")
+            return self.name
+
+        if (not self.long_desc) or self._use_short_desc:
+            return self.short_desc
+
+        # use full desc
+        return self.short_desc + "\n\n" + self.long_desc
+
+
+class ToolCall(BaseModel):
+    """The class representing a tool call."""
+
+    id: str = Field(..., description="The ID of the tool call.")
+    """The ID of the tool call."""
+    name: str = Field(..., description="The name of the function to call.")
+    """The name of the function to call."""
+    args: str = Field(..., description="The arguments to call the function with.")
+    """The arguments to call the function with."""
+
+    def get_dict(self):
+        """Get the OpenAI format dictionary representation of the tool call."""
+        return {
+            "id": self.id,
+            "type": "function",
+            "function": {
+                "name": self.name,
+                "arguments": self.args,
+            },
+        }
+
+    @classmethod
+    def from_openai_tool_call(cls, call: ChatCompletionMessageToolCall) -> "ToolCall":
+        """Create a ToolCall from an OpenAI tool call."""
+        return cls(
+            id=call.id,
+            name=call.function.name,
+            args=call.function.arguments,
+        )
```

### Comparing `applang-0.0.1a3/src/appl/core/types/content.py` & `applang-0.0.1a4/src/appl/core/types/content.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from typing import Optional
-
-from pydantic import BaseModel, Field
-
-from .basic import *
-from .futures import String, is_string
-
-
-class Image(BaseModel):
-    """Represent an image in the message."""
-
-    url: str = Field(..., description="The URL of the image")
-    detail: Optional[str] = Field(
-        None, description="Specifies the detail level of the image."
-    )
-
-    def __init__(self, url: str, detail: Optional[str] = None) -> None:
-        """Initialize the image with the URL and detail level.
-
-        See [the guide](https://platform.openai.com/docs/guides/vision/low-or-high-fidelity-image-understanding)
-        for more information about the detail level.
-        """
-        super().__init__(url=url, detail=detail)
-
-    def __repr__(self) -> str:
-        return f"Image(url={self.url})"
-
-    def __str__(self) -> str:
-        return f"[Image]{self.url}"
-
-
-StrOrImg = Union[String, Image]
-"""A type that can be either a string or an image."""
-
-
-class ContentList(BaseModel):
-    """Represent a list of contents containing text and images."""
-
-    contents: List[StrOrImg] = Field(..., description="The content of the message")
-
-    def __iadd__(
-        self, other: Union[StrOrImg, List[StrOrImg], "ContentList"]
-    ) -> "ContentList":
-        if isinstance(other, ContentList):
-            self.extend(other.contents)
-        elif isinstance(other, list):
-            self.extend(other)
-        else:
-            self.append(other)
-        return self
-
-    def append(self, content: StrOrImg) -> None:
-        """Append a content to the list.
-
-        If the last content is a string, it will be concatenated with the new content.
-        """
-        if is_string(content) and len(self.contents) and is_string(self.contents[-1]):
-            self.contents[-1] += content  # type: ignore
-        else:
-            self.contents.append(content)
-
-    def extend(self, contents: list[StrOrImg]) -> None:
-        """Extend the list with multiple contents."""
-        for content in contents:
-            self.append(content)
-
-    def get_contents(self) -> List[Dict[str, Any]]:
-        """Return the contents as a list of dictionaries."""
-
-        def get_dict(content):
-            if isinstance(content, Image):
-                image_args = {"url": content.url}
-                if content.detail:
-                    image_args["detail"] = content.detail
-                return {"type": "image_url", "image_url": image_args}
-            return {"type": "text", "text": str(content)}
-
-        return [get_dict(c) for c in self.contents]
-
-    def __str__(self) -> str:
-        return "\n".join([str(c) for c in self.contents])
+from typing import Optional
+
+from pydantic import BaseModel, Field
+
+from .basic import *
+from .futures import String, is_string
+
+
+class Image(BaseModel):
+    """Represent an image in the message."""
+
+    url: str = Field(..., description="The URL of the image")
+    detail: Optional[str] = Field(
+        None, description="Specifies the detail level of the image."
+    )
+
+    def __init__(self, url: str, detail: Optional[str] = None) -> None:
+        """Initialize the image with the URL and detail level.
+
+        See [the guide](https://platform.openai.com/docs/guides/vision/low-or-high-fidelity-image-understanding)
+        for more information about the detail level.
+        """
+        super().__init__(url=url, detail=detail)
+
+    def __repr__(self) -> str:
+        return f"Image(url={self.url})"
+
+    def __str__(self) -> str:
+        return f"[Image]{self.url}"
+
+
+StrOrImg = Union[String, Image]
+"""A type that can be either a string or an image."""
+
+
+class ContentList(BaseModel):
+    """Represent a list of contents containing text and images."""
+
+    contents: List[StrOrImg] = Field(..., description="The content of the message")
+
+    def __iadd__(
+        self, other: Union[StrOrImg, List[StrOrImg], "ContentList"]
+    ) -> "ContentList":
+        if isinstance(other, ContentList):
+            self.extend(other.contents)
+        elif isinstance(other, list):
+            self.extend(other)
+        else:
+            self.append(other)
+        return self
+
+    def append(self, content: StrOrImg) -> None:
+        """Append a content to the list.
+
+        If the last content is a string, it will be concatenated with the new content.
+        """
+        if is_string(content) and len(self.contents) and is_string(self.contents[-1]):
+            self.contents[-1] += content  # type: ignore
+        else:
+            self.contents.append(content)
+
+    def extend(self, contents: list[StrOrImg]) -> None:
+        """Extend the list with multiple contents."""
+        for content in contents:
+            self.append(content)
+
+    def get_contents(self) -> List[Dict[str, Any]]:
+        """Return the contents as a list of dictionaries."""
+
+        def get_dict(content):
+            if isinstance(content, Image):
+                image_args = {"url": content.url}
+                if content.detail:
+                    image_args["detail"] = content.detail
+                return {"type": "image_url", "image_url": image_args}
+            return {"type": "text", "text": str(content)}
+
+        return [get_dict(c) for c in self.contents]
+
+    def __str__(self) -> str:
+        return "\n".join([str(c) for c in self.contents])
```

### Comparing `applang-0.0.1a3/src/appl/core/types/futures.py` & `applang-0.0.1a4/src/appl/core/types/futures.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,234 +1,234 @@
-from .basic import *
-
-
-class FutureValue(ABC):
-    """Represents a value that may not be ready yet."""
-
-    @abstractmethod
-    def _get_val(self):
-        """Get the value of the future.
-
-        If the future is not ready, it will block until the value is ready.
-        """
-        raise NotImplementedError
-
-    @property
-    def val(self):
-        """The value of the future."""
-        return self._get_val()
-
-    def __call__(self):
-        """Use call to get the value of the future."""
-        return self.val
-
-
-class CallFuture(FutureValue):
-    """Represent a function call that may not be ready yet."""
-
-    def __init__(
-        self,
-        func: Callable,
-        *args: Any,
-        use_process: bool = False,
-        lazy_eval: bool = False,
-        **kwargs: Any,
-    ):
-        """Initialize the CallFuture.
-
-        Args:
-            func: The function to call.
-            *args: The arguments of the function.
-            use_process: Whether to use a process pool executor.
-            lazy_eval: Whether to delay the start of the call until needed.
-            **kwargs: The keyword arguments of the function.
-        """
-        # TODO: maybe use a global executor from the config
-        self._executor = (
-            ProcessPoolExecutor(max_workers=1)
-            if use_process
-            else ThreadPoolExecutor(max_workers=1)
-        )
-        self._submit_fn = lambda: self._executor.submit(func, *args, **kwargs)
-        self._submitted = False
-        self._info = func.__name__
-        # self._debug = False
-        # if self._debug:
-        #     # arg and kwargs might contains future objects
-        #     args_list = [f"{arg}" for arg in args] + [
-        #         f"{k}={v!r}" for k, v in kwargs.items()
-        #     ]
-        #     args_str = ", ".join(args_list)
-        #     self._info += f"({args_str})"
-        if not lazy_eval:
-            # delay the start of the call until needed
-            self._submit()
-
-    def _submit(self) -> None:
-        if not self._submitted:
-            self._future: Future = self._submit_fn()
-            self._submitted = True
-
-    @property
-    def future(self):
-        """The future object of the call."""
-        if not self._submitted:
-            self._submit()
-        return self._future
-
-    def result(self) -> Any:
-        """Get the result of the call."""
-        # This will block until the result is available
-        return self.future.result()
-
-    def cancel(self) -> bool:
-        """Cancel the call."""
-        # Attempt to cancel the call
-        return self.future.cancel()
-
-    def done(self) -> bool:
-        """Check if the call has completed."""
-        # Check if the future has completed
-        return self.future.done()
-
-    def _get_val(self):
-        return self.result()
-
-    def __str__(self):
-        return str(self.val)
-
-    def __repr__(self):
-        return repr(self.future)
-
-
-# TODO: boolean future
-class CmpStringFuture(FutureValue):
-    """Represent a comparison between a StringFuture and another value."""
-
-    def __init__(
-        self, a: "StringFuture", b: "StringFuture", op: Callable[[str, str], bool]
-    ):
-        """Initialize the CmpStringFuture."""
-        self._a = a
-        self._b = b
-        self._op = op
-
-    def __bool__(self):
-        return self._op(str(self._a), str(self._b))
-
-    def _get_val(self):
-        return self.__bool__()
-
-
-class StringFuture(FutureValue, BaseModel):
-    """StringFuture is a string that may not be ready yet."""
-
-    s: List[Any] = Field([], description="The string content")
-
-    def __init__(self, content: Any = "", set_value: bool = False):
-        """Initialize the StringFuture."""
-        if set_value:
-            if not isinstance(content, List):
-                raise ValueError("Cannot set value to non-list.")
-            s = content
-        else:
-            s = [content]
-        super().__init__(s=s)
-
-    @classmethod
-    def from_list(cls, content: List[Any]) -> "StringFuture":
-        """Create a StringFuture from a list of content."""
-        return cls(content, set_value=True)
-
-    def _collapse(self) -> str:
-        return "".join([str(x) for x in self.s])
-
-    def materialized(self) -> "StringFuture":
-        """Materialize the StringFuture."""
-        self.s = [self._collapse()]
-        return self
-
-    def serialize(self) -> str:
-        """Serialize the StringFuture."""
-        return str(self)
-
-    def _get_val(self):
-        return str(self)
-
-    def __str__(self) -> str:
-        return self.materialized().s[0]
-
-    def __hash__(self) -> int:
-        return hash(str(self))
-
-    def __contains__(self, item: str) -> bool:
-        return item in str(self)
-
-    def __getattr__(self, key):
-        if not hasattr(str, key):
-            raise AttributeError("str has no attribute " + key)
-        return getattr(str(self), key)
-
-    def __iadd__(self, other: "String") -> "StringFuture":
-        if isinstance(other, str):
-            self.s.append(other)
-            return self
-        elif isinstance(other, StringFuture):
-            self.s += other.s
-            return self
-        else:
-            raise RuntimeError("Cannot add StringFuture to non-string.")
-
-    def __radd__(self, other: "String") -> "StringFuture":
-        if isinstance(other, str):
-            return StringFuture.from_list([other] + self.s)
-        else:
-            raise RuntimeError("Cannot add StringFuture to non-string.")
-
-    def __add__(self, other: "String") -> "StringFuture":
-        if isinstance(other, str):
-            return StringFuture.from_list(self.s + [other])
-        elif isinstance(other, StringFuture):
-            return StringFuture.from_list(self.s + other.s)
-        else:
-            raise RuntimeError("Cannot add StringFuture to non-string.")
-
-    def __eq__(self, other: Any) -> CmpStringFuture:  # type: ignore
-        return CmpStringFuture(self, other, operator.eq)
-
-    def __ge__(self, other: Any) -> CmpStringFuture:
-        return CmpStringFuture(self, other, operator.ge)
-
-    def __gt__(self, other: Any) -> CmpStringFuture:
-        return CmpStringFuture(self, other, operator.gt)
-
-    def __le__(self, other: Any) -> CmpStringFuture:
-        return CmpStringFuture(self, other, operator.le)
-
-    def __lt__(self, other: Any) -> CmpStringFuture:
-        return CmpStringFuture(self, other, operator.lt)
-
-    def __ne__(self, other: Any) -> CmpStringFuture:  # type: ignore
-        return CmpStringFuture(self, other, operator.ne)
-
-    def __format__(self, __format_spec: str) -> str:
-        return str(self).__format__(__format_spec)
-
-    def __getitem__(self, key: Union[SupportsIndex, slice]) -> "StringFuture":
-        def func():
-            return str(self)[key]
-
-        return StringFuture(CallFuture(func))
-
-    def __deepcopy__(self, memo: Optional[Dict[int, Any]] = None) -> "StringFuture":
-        # materialize before copying, to avoid functions wrapped in StringFuture running twice.
-        return StringFuture(str(self))
-
-
-# Type aliases
-String = Union[StringFuture, str]
-"""String is a type alias for StringFuture or str."""
-
-
-def is_string(s: Any) -> bool:
-    """Check if the object is a StringFuture or str."""
-    return isinstance(s, StringFuture) or isinstance(s, str)
+from .basic import *
+
+
+class FutureValue(ABC):
+    """Represents a value that may not be ready yet."""
+
+    @abstractmethod
+    def _get_val(self):
+        """Get the value of the future.
+
+        If the future is not ready, it will block until the value is ready.
+        """
+        raise NotImplementedError
+
+    @property
+    def val(self):
+        """The value of the future."""
+        return self._get_val()
+
+    def __call__(self):
+        """Use call to get the value of the future."""
+        return self.val
+
+
+class CallFuture(FutureValue):
+    """Represent a function call that may not be ready yet."""
+
+    def __init__(
+        self,
+        func: Callable,
+        *args: Any,
+        use_process: bool = False,
+        lazy_eval: bool = False,
+        **kwargs: Any,
+    ):
+        """Initialize the CallFuture.
+
+        Args:
+            func: The function to call.
+            *args: The arguments of the function.
+            use_process: Whether to use a process pool executor.
+            lazy_eval: Whether to delay the start of the call until needed.
+            **kwargs: The keyword arguments of the function.
+        """
+        # TODO: maybe use a global executor from the config
+        self._executor = (
+            ProcessPoolExecutor(max_workers=1)
+            if use_process
+            else ThreadPoolExecutor(max_workers=1)
+        )
+        self._submit_fn = lambda: self._executor.submit(func, *args, **kwargs)
+        self._submitted = False
+        self._info = func.__name__
+        # self._debug = False
+        # if self._debug:
+        #     # arg and kwargs might contains future objects
+        #     args_list = [f"{arg}" for arg in args] + [
+        #         f"{k}={v!r}" for k, v in kwargs.items()
+        #     ]
+        #     args_str = ", ".join(args_list)
+        #     self._info += f"({args_str})"
+        if not lazy_eval:
+            # delay the start of the call until needed
+            self._submit()
+
+    def _submit(self) -> None:
+        if not self._submitted:
+            self._future: Future = self._submit_fn()
+            self._submitted = True
+
+    @property
+    def future(self):
+        """The future object of the call."""
+        if not self._submitted:
+            self._submit()
+        return self._future
+
+    def result(self) -> Any:
+        """Get the result of the call."""
+        # This will block until the result is available
+        return self.future.result()
+
+    def cancel(self) -> bool:
+        """Cancel the call."""
+        # Attempt to cancel the call
+        return self.future.cancel()
+
+    def done(self) -> bool:
+        """Check if the call has completed."""
+        # Check if the future has completed
+        return self.future.done()
+
+    def _get_val(self):
+        return self.result()
+
+    def __str__(self):
+        return str(self.val)
+
+    def __repr__(self):
+        return repr(self.future)
+
+
+# TODO: boolean future
+class CmpStringFuture(FutureValue):
+    """Represent a comparison between a StringFuture and another value."""
+
+    def __init__(
+        self, a: "StringFuture", b: "StringFuture", op: Callable[[str, str], bool]
+    ):
+        """Initialize the CmpStringFuture."""
+        self._a = a
+        self._b = b
+        self._op = op
+
+    def __bool__(self):
+        return self._op(str(self._a), str(self._b))
+
+    def _get_val(self):
+        return self.__bool__()
+
+
+class StringFuture(FutureValue, BaseModel):
+    """StringFuture is a string that may not be ready yet."""
+
+    s: List[Any] = Field([], description="The string content")
+
+    def __init__(self, content: Any = "", set_value: bool = False):
+        """Initialize the StringFuture."""
+        if set_value:
+            if not isinstance(content, List):
+                raise ValueError("Cannot set value to non-list.")
+            s = content
+        else:
+            s = [content]
+        super().__init__(s=s)
+
+    @classmethod
+    def from_list(cls, content: List[Any]) -> "StringFuture":
+        """Create a StringFuture from a list of content."""
+        return cls(content, set_value=True)
+
+    def _collapse(self) -> str:
+        return "".join([str(x) for x in self.s])
+
+    def materialized(self) -> "StringFuture":
+        """Materialize the StringFuture."""
+        self.s = [self._collapse()]
+        return self
+
+    def serialize(self) -> str:
+        """Serialize the StringFuture."""
+        return str(self)
+
+    def _get_val(self):
+        return str(self)
+
+    def __str__(self) -> str:
+        return self.materialized().s[0]
+
+    def __hash__(self) -> int:
+        return hash(str(self))
+
+    def __contains__(self, item: str) -> bool:
+        return item in str(self)
+
+    def __getattr__(self, key):
+        if not hasattr(str, key):
+            raise AttributeError("str has no attribute " + key)
+        return getattr(str(self), key)
+
+    def __iadd__(self, other: "String") -> "StringFuture":
+        if isinstance(other, str):
+            self.s.append(other)
+            return self
+        elif isinstance(other, StringFuture):
+            self.s += other.s
+            return self
+        else:
+            raise RuntimeError("Cannot add StringFuture to non-string.")
+
+    def __radd__(self, other: "String") -> "StringFuture":
+        if isinstance(other, str):
+            return StringFuture.from_list([other] + self.s)
+        else:
+            raise RuntimeError("Cannot add StringFuture to non-string.")
+
+    def __add__(self, other: "String") -> "StringFuture":
+        if isinstance(other, str):
+            return StringFuture.from_list(self.s + [other])
+        elif isinstance(other, StringFuture):
+            return StringFuture.from_list(self.s + other.s)
+        else:
+            raise RuntimeError("Cannot add StringFuture to non-string.")
+
+    def __eq__(self, other: Any) -> CmpStringFuture:  # type: ignore
+        return CmpStringFuture(self, other, operator.eq)
+
+    def __ge__(self, other: Any) -> CmpStringFuture:
+        return CmpStringFuture(self, other, operator.ge)
+
+    def __gt__(self, other: Any) -> CmpStringFuture:
+        return CmpStringFuture(self, other, operator.gt)
+
+    def __le__(self, other: Any) -> CmpStringFuture:
+        return CmpStringFuture(self, other, operator.le)
+
+    def __lt__(self, other: Any) -> CmpStringFuture:
+        return CmpStringFuture(self, other, operator.lt)
+
+    def __ne__(self, other: Any) -> CmpStringFuture:  # type: ignore
+        return CmpStringFuture(self, other, operator.ne)
+
+    def __format__(self, __format_spec: str) -> str:
+        return str(self).__format__(__format_spec)
+
+    def __getitem__(self, key: Union[SupportsIndex, slice]) -> "StringFuture":
+        def func():
+            return str(self)[key]
+
+        return StringFuture(CallFuture(func))
+
+    def __deepcopy__(self, memo: Optional[Dict[int, Any]] = None) -> "StringFuture":
+        # materialize before copying, to avoid functions wrapped in StringFuture running twice.
+        return StringFuture(str(self))
+
+
+# Type aliases
+String = Union[StringFuture, str]
+"""String is a type alias for StringFuture or str."""
+
+
+def is_string(s: Any) -> bool:
+    """Check if the object is a StringFuture or str."""
+    return isinstance(s, StringFuture) or isinstance(s, str)
```

### Comparing `applang-0.0.1a3/src/appl/core/types/role.py` & `applang-0.0.1a4/src/appl/core/types/role.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from .basic import *
-
-# Roles
-SYSTEM = "system"
-USER = "user"
-ASSISTANT = "assistant"
-TOOL = "tool"
-
-
-class MessageRole(BaseModel):
-    """The role of the message owner."""
-
-    type: Optional[str] = None
-    name: Optional[str] = None
-
-    def __init__(self, type: Optional[str] = None, name: Optional[str] = None):
-        """Initialize the MessageRole object.
-
-        Args:
-            type: The type of the role.
-            name: An optional name for the role, differentiate between roles of the same type."
-        """
-        super().__init__(type=type, name=name)
-
-    @property
-    def is_system(self) -> bool:
-        """Whether the role is a system role."""
-        return self.type == SYSTEM
-
-    @property
-    def is_user(self) -> bool:
-        """Whether the role is a user role."""
-        return self.type == USER
-
-    @property
-    def is_assistant(self) -> bool:
-        """Whether the role is an assistant role."""
-        return self.type == ASSISTANT
-
-    @property
-    def is_tool(self) -> bool:
-        """Whether the role is a tool role."""
-        return self.type == TOOL
-
-    def get_dict(self) -> Dict[str, Any]:
-        """Get the role as a dictionary."""
-        data = {"role": self.type}
-        if self.name:
-            data["name"] = self.name
-        return data
-
-    def __str__(self) -> str:
-        s = str(self.type)
-        if self.name:
-            s += f"({self.name})"
-        return s
-
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, MessageRole):
-            return self.type == other.type and self.name == other.name
-        return False
-
-
-SYSTEM_ROLE = MessageRole(SYSTEM)
-"""The system role with name not specified."""
-USER_ROLE = MessageRole(USER)
-"""The user role with name not specified."""
-ASSISTANT_ROLE = MessageRole(ASSISTANT)
-"""The assistant role with name not specified."""
-TOOL_ROLE = MessageRole(TOOL)
-"""The tool role with name not specified."""
+from .basic import *
+
+# Roles
+SYSTEM = "system"
+USER = "user"
+ASSISTANT = "assistant"
+TOOL = "tool"
+
+
+class MessageRole(BaseModel):
+    """The role of the message owner."""
+
+    type: Optional[str] = None
+    name: Optional[str] = None
+
+    def __init__(self, type: Optional[str] = None, name: Optional[str] = None):
+        """Initialize the MessageRole object.
+
+        Args:
+            type: The type of the role.
+            name: An optional name for the role, differentiate between roles of the same type."
+        """
+        super().__init__(type=type, name=name)
+
+    @property
+    def is_system(self) -> bool:
+        """Whether the role is a system role."""
+        return self.type == SYSTEM
+
+    @property
+    def is_user(self) -> bool:
+        """Whether the role is a user role."""
+        return self.type == USER
+
+    @property
+    def is_assistant(self) -> bool:
+        """Whether the role is an assistant role."""
+        return self.type == ASSISTANT
+
+    @property
+    def is_tool(self) -> bool:
+        """Whether the role is a tool role."""
+        return self.type == TOOL
+
+    def get_dict(self) -> Dict[str, Any]:
+        """Get the role as a dictionary."""
+        data = {"role": self.type}
+        if self.name:
+            data["name"] = self.name
+        return data
+
+    def __str__(self) -> str:
+        s = str(self.type)
+        if self.name:
+            s += f"({self.name})"
+        return s
+
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, MessageRole):
+            return self.type == other.type and self.name == other.name
+        return False
+
+
+SYSTEM_ROLE = MessageRole(SYSTEM)
+"""The system role with name not specified."""
+USER_ROLE = MessageRole(USER)
+"""The user role with name not specified."""
+ASSISTANT_ROLE = MessageRole(ASSISTANT)
+"""The assistant role with name not specified."""
+TOOL_ROLE = MessageRole(TOOL)
+"""The tool role with name not specified."""
```

### Comparing `applang-0.0.1a3/src/appl/default_configs.yaml` & `applang-0.0.1a4/src/appl/default_configs.yaml`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-metadata: {}
-
-settings:
-  logging:
-    format: >- # The format of the log message, change HH:mm:ss.SSS to HH:mm:ss for the default loguru format
-      <green>{time:YYYY-MM-DD HH:mm:ss}</green> |
-      <level>{level: <8}</level> |
-      <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> |
-      <level>{message}</level>
-    log_level: "INFO" # The level of the log messages
-    max_length: 800 # The maximum length of the log message in bash
-    suffix_length: 200 # The length of the suffix (when truncated)
-    log_file:
-      enabled: false # default to not log to a file
-      path_format: './logs/{basename}_{time:YYYY_MM_DD__HH_mm_ss}'
-      # The path to the log file, ext will be added automatically
-      log_level: null # default to use the same level as the log_level
-    display:
-      configs: false # Display the configurations
-      llm_raw_call_args: false # Display the raw args for the llm calls
-      llm_raw_response: false # Display the raw response of the llm calls
-      llm_call_args: true # Display the args for the llm calls
-      llm_response: true # Display the response of the llm calls
-      llm_cache: false # Display the cache info
-      llm_cost: true # Display the cost of the calls
-      tool_calls: true # Display the tool calls
-      tool_results: true # Display the results of the tool calls
-      stream_interval: 1.0 # The interval in second to log the stream info
-  tracing:
-    enabled: false # default to not trace the calls
-    path_format: './dumps/traces/{basename}_{time:YYYY_MM_DD__HH_mm_ss}'
-    # The path to the trace file, ext will be added automatically
-    strict_match: true # when saving and loading cache, whether need to match the generation id
-  messages:
-    colors:
-      system: red
-      user: green
-      assistant: blue
-      tool: magenta
-  misc:
-    suppress_litellm_debug_info: true
-
-# When using APIs through litellm,
-#   see the list of available models at https://docs.litellm.ai/docs/providers
-# When using SRT server,
-#   set model to "srt" and api_base to the address of the server.
-servers:
-  default: gpt35-turbo # should avoid using '.' in the name
-  gpt35-turbo: # the name of the server
-    model: gpt-3.5-turbo # the model name
-  gpt4-turbo:
-    model: gpt-4-turbo
-  _dummy:
-    model: _dummy
+metadata: {}
+
+settings:
+  logging:
+    format: >- # The format of the log message, change HH:mm:ss.SSS to HH:mm:ss for the default loguru format
+      <green>{time:YYYY-MM-DD HH:mm:ss}</green> |
+      <level>{level: <8}</level> |
+      <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> |
+      <level>{message}</level>
+    log_level: "INFO" # The level of the log messages
+    max_length: 800 # The maximum length of the log message in bash
+    suffix_length: 200 # The length of the suffix (when truncated)
+    log_file:
+      enabled: false # default to not log to a file
+      path_format: './logs/{basename}_{time:YYYY_MM_DD__HH_mm_ss}'
+      # The path to the log file, ext will be added automatically
+      log_level: null # default to use the same level as the log_level
+    display:
+      configs: false # Display the configurations
+      llm_raw_call_args: false # Display the raw args for the llm calls
+      llm_raw_response: false # Display the raw response of the llm calls
+      llm_call_args: true # Display the args for the llm calls
+      llm_response: true # Display the response of the llm calls
+      llm_cache: false # Display the cache info
+      llm_cost: true # Display the cost of the calls
+      tool_calls: true # Display the tool calls
+      tool_results: true # Display the results of the tool calls
+      stream_interval: 1.0 # The interval in second to log the stream info
+  tracing:
+    enabled: false # default to not trace the calls
+    path_format: './dumps/traces/{basename}_{time:YYYY_MM_DD__HH_mm_ss}'
+    # The path to the trace file, ext will be added automatically
+    strict_match: true # when saving and loading cache, whether need to match the generation id
+  messages:
+    colors:
+      system: red
+      user: green
+      assistant: blue
+      tool: magenta
+  misc:
+    suppress_litellm_debug_info: true
+
+# When using APIs through litellm,
+#   see the list of available models at https://docs.litellm.ai/docs/providers
+# When using SRT server,
+#   set model to "srt" and api_base to the address of the server.
+servers:
+  default: gpt35-turbo # should avoid using '.' in the name
+  gpt35-turbo: # the name of the server
+    model: gpt-3.5-turbo # the model name
+  gpt4-turbo:
+    model: gpt-4-turbo
+  _dummy:
+    model: _dummy
```

### Comparing `applang-0.0.1a3/src/appl/func.py` & `applang-0.0.1a4/src/appl/func.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,439 +1,439 @@
-import copy
-import functools
-import inspect
-import sys
-import threading
-from inspect import signature
-from typing import overload
-
-from langsmith import traceable
-
-from .core import (
-    BaseTool,
-    Compositor,
-    Conversation,
-    GenArgs,
-    Generation,
-    PromptContext,
-    PromptFunc,
-    PromptRecords,
-    Tool,
-)
-from .core.globals import global_vars
-from .core.trace import FunctionCallEvent, FunctionReturnEvent, add_to_trace
-from .servers import server_manager
-from .types import *
-
-# https://docs.python.org/3/library/typing.html#typing.ParamSpec
-# https://docs.python.org/3/library/typing.html#typing.Concatenate
-# https://peps.python.org/pep-0612/
-# Callable[P, T] is used for static type inference (Pylance)
-P = ParamSpec("P")
-T = TypeVar("T")
-F = TypeVar("F", bound=Callable)
-
-
-def need_ctx(func: Callable[P, T]) -> Callable[P, T]:
-    """Decorate a function to mark it as needing a prompt context."""
-    setattr(func, "__need_ctx__", True)
-    return func
-
-
-def partial(func: Callable, *args: Any, **kwargs: Any) -> Any:
-    """Create a new function with partial application of the given arguments and keywords."""
-    new_func = functools.partial(func, *args, **kwargs)
-    if getattr(func, "__need_ctx__", True):
-        new_func = need_ctx(new_func)  # type: ignore
-    return new_func
-
-
-def wraps(func: F) -> Callable[[F], F]:
-    """Replace the functools.wraps to take care of the type hint."""
-
-    def decorator(wrapper: F) -> F:
-        return functools.wraps(func)(wrapper)
-
-    return decorator
-
-
-def auto_prime_gen(gen_func):
-    """Decorate a generator to automatically prime the generator."""
-
-    def wrapper(*args, **kwargs):
-        gen = gen_func(*args, **kwargs)
-        next(gen)  # prime the generator
-        return gen
-
-    return wrapper
-
-
-@overload
-def ppl(ctx: F) -> F: ...
-
-
-@overload
-def ppl(
-    ctx: str = "new",
-    comp: Optional[Compositor] = None,
-    *,
-    default_return: Optional[Literal["prompt"]] = None,
-    exclude_first_str: bool = False,
-    auto_prime: bool = False,
-    num_extra_wrappers: int = 0,
-    new_ctx_func: Callable = PromptContext,
-) -> Callable[[F], F]: ...
-
-
-def ppl(
-    ctx: Union[str, F] = "new",
-    comp: Optional[Compositor] = None,
-    *,
-    default_return: Optional[Literal["prompt"]] = None,
-    exclude_first_str: bool = False,
-    auto_prime: bool = False,
-    num_extra_wrappers: int = 0,
-    new_ctx_func: Callable = PromptContext,
-) -> Union[Callable[[F], F], F]:
-    """Decorate a function to mark it as an APPL function.
-
-    The function contains a prompt context, which could be same as or
-    copied from its caller function, or created from scratch, or resumed
-    from the last run.
-
-    Args:
-        ctx (str):
-            the method to deal with the child context, available methods includes:
-
-            - (default) "new" or "new_ctx": create a brand new context.
-            - "copy" or "copy_ctx":
-                copy from the parent's context, the change will not
-                affect the parent's context.
-            - "same" or "same_ctx":
-                use the same context as the parent's, the change will
-                affect the parent's context.
-            - "resume" or "resume_ctx":
-                resume its own context from the last run.
-                For the first run, it will use the parent's context.
-
-        comp (Compositor, optional):
-            the default compositor to be used. Defaults to None.
-        default_return (str, optional):
-            The default return value, "prompt" means return the prompt within
-            the function. Defaults to None.
-        exclude_first_str (bool, optional):
-            set to True to exclude the first string (liekly the docstring)
-            from the prompt. Defaults to False.
-        auto_prime (bool, optional):
-            set to True to automatically prime the generator. Defaults to False.
-        num_extra_wrappers (int, optional):
-            the number of extra wrappers to go back to the caller frame.
-        new_ctx_func (Callable, optional):
-            the function to create a new context. Defaults to PromptContext.
-    """
-    # The same doc string as PromptFunc (excluding the func argument)
-
-    ctx_method: str = "new"
-
-    def decorator(func: F) -> F:
-        """Decorate a function as prompt function."""
-        _is_class_method = False
-        if "." in (qualname := func.__qualname__):
-            # NOTE: this is a workaround for class methods, may not cover all cases
-            qualnames = qualname.split(".")
-            if qualnames[-2] != "<locals>":
-                _is_class_method = True
-
-        # ? should disable such usage?
-        # if not _is_class_method and "<locals>" in qualname and ctx_method == "resume":
-        #     raise ValueError("Cannot use 'resume' with local functions.")
-        prompt_func = PromptFunc(
-            func, ctx_method, comp, default_return, exclude_first_str, new_ctx_func
-        )
-
-        @need_ctx
-        @traceable(name=func.__name__, metadata={"appl": "func"})
-        @functools.wraps(func)
-        def wrapper(
-            *args: Any,
-            _globals: Optional[Dict] = None,
-            _locals: Optional[Dict] = None,
-            **kwargs: Any,
-        ) -> Any:
-            # add to trace (function call)
-            func_name = f"{prompt_func._name}_{prompt_func._run_cnt}"
-            prompt_func._run_cnt += 1
-            add_to_trace(
-                FunctionCallEvent(
-                    name=func_name,
-                    args={"args": repr(args), "kwargs": repr(kwargs)},
-                )
-            )
-            # closure variables
-            freevars = prompt_func.compiled_func.freevars
-            if _locals is None:
-                # * Workaround for closure variables
-                # Default: use the locals from the caller
-                frame = inspect.currentframe()
-                num_wrappers = (3 if auto_prime else 2) + num_extra_wrappers
-                for _ in range(num_wrappers):
-                    if frame is None:
-                        raise RuntimeError("No caller frame found")
-                    # back to @traceable frame, and the caller frame
-                    frame = frame.f_back
-                if frame is None:
-                    raise RuntimeError("No caller frame found")
-                _locals = frame.f_locals
-
-                if len(freevars):
-                    vars = {var: _locals.get(var, "NotFound") for var in freevars}
-                    logger.debug(
-                        f"For freevars of function {func.__name__}, "
-                        f"automatically using locals from the caller: {vars}"
-                    )
-                    for var in freevars:
-                        if var not in _locals:
-                            logger.warning(
-                                f"could not find variable {var} automatically from the caller frame."
-                            )
-            results = prompt_func(
-                *args,
-                _globals=_globals,
-                _locals=_locals,
-                _is_class_method=_is_class_method,
-                **kwargs,
-            )
-            # add to trace (function return)
-            add_to_trace(FunctionReturnEvent(name=func_name))  # ret=results
-            return results
-
-        if auto_prime:
-            wrapper = auto_prime_gen(wrapper)
-        setattr(wrapper, "_prompt_func", prompt_func)
-        return wrapper  # type: ignore
-
-    if isinstance(ctx, str):
-        ctx_method = ctx
-        # used as a decorator with arguments (e.g., @ppl(ctx="copy"))
-        # returns a decorator that takes a function as input
-        return decorator
-    else:
-        # used as a single decorator (i.e., @ppl)
-        return decorator(func=ctx)  # returns a wrapper
-
-
-def as_func(
-    func: Callable[P, T],
-    _globals: Optional[Dict] = None,
-    _locals: Optional[Dict] = None,
-) -> Callable[P, T]:
-    """Fill the globals and locals for a ppl function.
-
-    When locals not provided, it will use the locals from the caller.
-    """
-    frame = inspect.currentframe()
-    if _locals is None and frame is not None and frame.f_back is not None:
-        _locals = frame.f_back.f_locals
-    return partial(func, _globals=_globals, _locals=_locals)
-
-
-def as_str(obj: Any) -> StringFuture:
-    """Convert an object to a StringFuture object."""
-    return StringFuture(obj)
-
-
-def as_tool(func: Callable, **kwargs: Any) -> Tool:
-    """Wrap a given function with additional predefined arguments into a Tool.
-
-    This function allows converting a standard function into a 'Tool' by
-    specifying the function and any additional arguments that should be
-    pre-defined for it. These additional arguments are passed as keyword
-    arguments and will be bound to the function within the Tool object,
-    so that these arguments are not required when using this tool.
-
-    Args:
-        func (Callable):
-            The function to be converted into a Tool.
-        **kwargs:
-            Keyword arguments that will be predefined for the function in
-            the Tool object.
-
-    Returns:
-        Tool:
-            An object encapsulating the given function and its predefined
-            arguments, ready to be utilized as a Tool.
-
-    Examples:
-        Given a function `move_disk` that requires an environment and two
-        pegs to move a disk from one peg to another in the Tower of Hanoi
-        puzzle, one can create a tool with a predefined environment by:
-
-        ```python
-        def move_disk(env: HanoiEnv, from_peg: int, to_peg: int) -> str:
-            pass
-
-        env = HanoiEnv()
-        tools = [as_tool(move_disk, env=env)]
-        ```
-
-        In this example, `move_disk` is encapsulated into a Tool with `env`
-        predefined, so only `from_peg` and `to_peg` are required.
-    """
-    return Tool(func=func, **kwargs)
-
-
-def as_tool_choice(obj: Union[str, Callable, BaseTool]) -> dict:
-    """Build a tool choice argument for the OpenAI API from an object."""
-    if isinstance(obj, BaseTool):
-        name = obj.name
-    else:
-        name = getattr(obj, "__name__", str(obj))
-    return dict(type="function", function=dict(name=name))
-
-
-def call(
-    func: Callable, *args: Any, use_process: bool = False, **kwargs: Any
-) -> CallFuture:
-    """Create a CallFuture object from a function and its arguments.
-
-    The CallFuture object will call the function in a separate thread or process,
-    therefore the function need to be thread-safe or process-safe.
-    """
-    return CallFuture(func, *args, use_process=use_process, **kwargs)
-
-
-def openai_tool_schema(func: Callable) -> dict:
-    """Build openai tool schema from a function."""
-    return as_tool(func).openai_schema
-
-
-@need_ctx
-def get_var(name: str, _ctx: PromptContext) -> Any:
-    """Get a variable by name from the prompt context."""
-    return getattr(_ctx, name)
-
-
-@need_ctx
-def records(_ctx: Optional[PromptContext] = None) -> PromptRecords:
-    """Return the prompt defined in the current function.
-
-    Similar to locals() in Python in some sense.
-    """
-    # add default value for _ctx to avoid the warning of type checker
-    if _ctx is None:
-        raise ValueError(
-            "PromptContext is required for records, "
-            "this function should be called within @ppl function."
-        )
-    return _ctx.records
-
-
-@need_ctx
-def convo(_ctx: Optional[PromptContext] = None) -> Conversation:
-    """Return the full conversation in the context.
-
-    Similar to globals() in Python in some sense.
-    """
-    # Added default value for _ctx to avoid the warning of type checker
-    if _ctx is None:
-        raise ValueError(
-            "PromptContext is required for convo, "
-            "this function should be called within @ppl function."
-        )
-    return _ctx.messages
-
-
-def build_tools(tools: OneOrMany[Union[BaseTool, Callable]]) -> Sequence[BaseTool]:
-    """Build a list of tools from the given tools or functions."""
-
-    def convert_to_tool(tool: Union[BaseTool, Callable]) -> BaseTool:
-        if isinstance(tool, BaseTool):
-            return tool
-        if callable(tool):
-            return as_tool(tool)
-        raise ValueError(f"Invalid tool: {tool}")
-
-    # process tools
-    if isinstance(tools, BaseTool) or callable(tools):
-        return [convert_to_tool(tools)]
-    if isinstance(tools, Sequence):
-        return [convert_to_tool(tool) for tool in tools]
-    raise ValueError(f"Invalid tools: {tools}")
-
-
-@need_ctx
-def gen(
-    server: Optional[str] = None,
-    *,
-    max_tokens: Optional[int] = None,
-    stop: MaybeOneOrMany[str] = None,
-    temperature: Optional[float] = None,
-    top_p: Optional[float] = None,
-    n: Optional[int] = None,
-    tools: OneOrMany[Union[BaseTool, Callable]] = [],
-    tool_format: str = "auto",
-    stream: Optional[bool] = None,
-    mock_response: Optional[Union[CompletionResponse, str]] = None,
-    _ctx: Optional[PromptContext] = None,
-    **kwargs: Any,
-) -> Generation:
-    """Send a generation request to the LLM backend.
-
-    Args:
-        server (str, optional):
-            name of the backend server. Defaults to the default server set in the configs.
-        max_tokens (int, optional): maximum number of tokens to generate. Defaults to None.
-        stop (str|Sequence[str], optional): stop sequence(s). Defaults to None.
-        temperature (float, optional): temperature for sampling. Defaults to None.
-        top_p (float, optional): nucleus sampling parameter. Defaults to None.
-        n (int, optional): number of choices to generate. Defaults to 1.
-        tools (BaseTool|Callable|Sequence[BaseTool|Callable], optional): tools can be used. Defaults to None.
-        tool_format (str, optional): format for the tools. Defaults to "auto".
-        stream (bool, optional): whether to stream the results. Defaults to False.
-        mock_response (Union[CompletionResponse, str], optional): mock response for testing. Defaults to None.
-        _ctx (PromptContext): prompt context, will be automatically filled.
-        kwargs (Any): extra arguments for the generation.
-
-    Returns:
-        Generation: a future object representing the generation result
-    """
-    backend_server = server_manager.get_server(server)
-    if _ctx is None:
-        raise ValueError(
-            "PromptContext is required for generation."
-            "Normally, it should be automatically filled."
-        )
-    messages = _ctx.messages
-    messages.materialize()  # materialize the messages
-    # TODO: double check the correctness
-    messages = copy.deepcopy(messages)  # freeze the prompt for the generation
-
-    create_args = GenArgs(
-        model=backend_server.model_name,
-        messages=messages,
-        max_tokens=max_tokens,
-        stop=stop,
-        temperature=temperature,
-        top_p=top_p,
-        n=n,
-        tools=build_tools(tools),
-        tool_format=tool_format,  # type: ignore
-        stream=stream,
-    )
-
-    generation = Generation(
-        backend_server, create_args, mock_response=mock_response, _ctx=_ctx, **kwargs
-    )
-
-    @traceable(name=generation.id, metadata={"appl": "gen"})
-    def langsmith_trace(*args: Any, **kwargs: Any) -> None:
-        pass
-
-    langsmith_trace(backend_server, create_args, _ctx=_ctx, **kwargs)
-    return generation
-
-
-# def serialize(obj: Any) -> Any:
-#     if hasattr(obj, "serialize"):
-#         return obj.serialize()
-#     else:
-#         raise TypeError("Object of type '%s' is not serializable" % type(obj).__name__)
+import copy
+import functools
+import inspect
+import sys
+import threading
+from inspect import signature
+from typing import overload
+
+from langsmith import traceable
+
+from .core import (
+    BaseTool,
+    Compositor,
+    Conversation,
+    GenArgs,
+    Generation,
+    PromptContext,
+    PromptFunc,
+    PromptRecords,
+    Tool,
+)
+from .core.globals import global_vars
+from .core.trace import FunctionCallEvent, FunctionReturnEvent, add_to_trace
+from .servers import server_manager
+from .types import *
+
+# https://docs.python.org/3/library/typing.html#typing.ParamSpec
+# https://docs.python.org/3/library/typing.html#typing.Concatenate
+# https://peps.python.org/pep-0612/
+# Callable[P, T] is used for static type inference (Pylance)
+P = ParamSpec("P")
+T = TypeVar("T")
+F = TypeVar("F", bound=Callable)
+
+
+def need_ctx(func: Callable[P, T]) -> Callable[P, T]:
+    """Decorate a function to mark it as needing a prompt context."""
+    setattr(func, "__need_ctx__", True)
+    return func
+
+
+def partial(func: Callable, *args: Any, **kwargs: Any) -> Any:
+    """Create a new function with partial application of the given arguments and keywords."""
+    new_func = functools.partial(func, *args, **kwargs)
+    if getattr(func, "__need_ctx__", True):
+        new_func = need_ctx(new_func)  # type: ignore
+    return new_func
+
+
+def wraps(func: F) -> Callable[[F], F]:
+    """Replace the functools.wraps to take care of the type hint."""
+
+    def decorator(wrapper: F) -> F:
+        return functools.wraps(func)(wrapper)
+
+    return decorator
+
+
+def auto_prime_gen(gen_func):
+    """Decorate a generator to automatically prime the generator."""
+
+    def wrapper(*args, **kwargs):
+        gen = gen_func(*args, **kwargs)
+        next(gen)  # prime the generator
+        return gen
+
+    return wrapper
+
+
+@overload
+def ppl(ctx: F) -> F: ...
+
+
+@overload
+def ppl(
+    ctx: str = "new",
+    comp: Optional[Compositor] = None,
+    *,
+    default_return: Optional[Literal["prompt"]] = None,
+    exclude_first_str: bool = False,
+    auto_prime: bool = False,
+    num_extra_wrappers: int = 0,
+    new_ctx_func: Callable = PromptContext,
+) -> Callable[[F], F]: ...
+
+
+def ppl(
+    ctx: Union[str, F] = "new",
+    comp: Optional[Compositor] = None,
+    *,
+    default_return: Optional[Literal["prompt"]] = None,
+    exclude_first_str: bool = False,
+    auto_prime: bool = False,
+    num_extra_wrappers: int = 0,
+    new_ctx_func: Callable = PromptContext,
+) -> Union[Callable[[F], F], F]:
+    """Decorate a function to mark it as an APPL function.
+
+    The function contains a prompt context, which could be same as or
+    copied from its caller function, or created from scratch, or resumed
+    from the last run.
+
+    Args:
+        ctx (str):
+            the method to deal with the child context, available methods includes:
+
+            - (default) "new" or "new_ctx": create a brand new context.
+            - "copy" or "copy_ctx":
+                copy from the parent's context, the change will not
+                affect the parent's context.
+            - "same" or "same_ctx":
+                use the same context as the parent's, the change will
+                affect the parent's context.
+            - "resume" or "resume_ctx":
+                resume its own context from the last run.
+                For the first run, it will use the parent's context.
+
+        comp (Compositor, optional):
+            the default compositor to be used. Defaults to None.
+        default_return (str, optional):
+            The default return value, "prompt" means return the prompt within
+            the function. Defaults to None.
+        exclude_first_str (bool, optional):
+            set to True to exclude the first string (liekly the docstring)
+            from the prompt. Defaults to False.
+        auto_prime (bool, optional):
+            set to True to automatically prime the generator. Defaults to False.
+        num_extra_wrappers (int, optional):
+            the number of extra wrappers to go back to the caller frame.
+        new_ctx_func (Callable, optional):
+            the function to create a new context. Defaults to PromptContext.
+    """
+    # The same doc string as PromptFunc (excluding the func argument)
+
+    ctx_method: str = "new"
+
+    def decorator(func: F) -> F:
+        """Decorate a function as prompt function."""
+        _is_class_method = False
+        if "." in (qualname := func.__qualname__):
+            # NOTE: this is a workaround for class methods, may not cover all cases
+            qualnames = qualname.split(".")
+            if qualnames[-2] != "<locals>":
+                _is_class_method = True
+
+        # ? should disable such usage?
+        # if not _is_class_method and "<locals>" in qualname and ctx_method == "resume":
+        #     raise ValueError("Cannot use 'resume' with local functions.")
+        prompt_func = PromptFunc(
+            func, ctx_method, comp, default_return, exclude_first_str, new_ctx_func
+        )
+
+        @need_ctx
+        @traceable(name=func.__name__, metadata={"appl": "func"})
+        @functools.wraps(func)
+        def wrapper(
+            *args: Any,
+            _globals: Optional[Dict] = None,
+            _locals: Optional[Dict] = None,
+            **kwargs: Any,
+        ) -> Any:
+            # add to trace (function call)
+            func_name = f"{prompt_func._name}_{prompt_func._run_cnt}"
+            prompt_func._run_cnt += 1
+            add_to_trace(
+                FunctionCallEvent(
+                    name=func_name,
+                    args={"args": repr(args), "kwargs": repr(kwargs)},
+                )
+            )
+            # closure variables
+            freevars = prompt_func.compiled_func.freevars
+            if _locals is None:
+                # * Workaround for closure variables
+                # Default: use the locals from the caller
+                frame = inspect.currentframe()
+                num_wrappers = (3 if auto_prime else 2) + num_extra_wrappers
+                for _ in range(num_wrappers):
+                    if frame is None:
+                        raise RuntimeError("No caller frame found")
+                    # back to @traceable frame, and the caller frame
+                    frame = frame.f_back
+                if frame is None:
+                    raise RuntimeError("No caller frame found")
+                _locals = frame.f_locals
+
+                if len(freevars):
+                    vars = {var: _locals.get(var, "NotFound") for var in freevars}
+                    logger.debug(
+                        f"For freevars of function {func.__name__}, "
+                        f"automatically using locals from the caller: {vars}"
+                    )
+                    for var in freevars:
+                        if var not in _locals:
+                            logger.warning(
+                                f"could not find variable {var} automatically from the caller frame."
+                            )
+            results = prompt_func(
+                *args,
+                _globals=_globals,
+                _locals=_locals,
+                _is_class_method=_is_class_method,
+                **kwargs,
+            )
+            # add to trace (function return)
+            add_to_trace(FunctionReturnEvent(name=func_name))  # ret=results
+            return results
+
+        if auto_prime:
+            wrapper = auto_prime_gen(wrapper)
+        setattr(wrapper, "_prompt_func", prompt_func)
+        return wrapper  # type: ignore
+
+    if isinstance(ctx, str):
+        ctx_method = ctx
+        # used as a decorator with arguments (e.g., @ppl(ctx="copy"))
+        # returns a decorator that takes a function as input
+        return decorator
+    else:
+        # used as a single decorator (i.e., @ppl)
+        return decorator(func=ctx)  # returns a wrapper
+
+
+def as_func(
+    func: Callable[P, T],
+    _globals: Optional[Dict] = None,
+    _locals: Optional[Dict] = None,
+) -> Callable[P, T]:
+    """Fill the globals and locals for a ppl function.
+
+    When locals not provided, it will use the locals from the caller.
+    """
+    frame = inspect.currentframe()
+    if _locals is None and frame is not None and frame.f_back is not None:
+        _locals = frame.f_back.f_locals
+    return partial(func, _globals=_globals, _locals=_locals)
+
+
+def as_str(obj: Any) -> StringFuture:
+    """Convert an object to a StringFuture object."""
+    return StringFuture(obj)
+
+
+def as_tool(func: Callable, **kwargs: Any) -> Tool:
+    """Wrap a given function with additional predefined arguments into a Tool.
+
+    This function allows converting a standard function into a 'Tool' by
+    specifying the function and any additional arguments that should be
+    pre-defined for it. These additional arguments are passed as keyword
+    arguments and will be bound to the function within the Tool object,
+    so that these arguments are not required when using this tool.
+
+    Args:
+        func (Callable):
+            The function to be converted into a Tool.
+        **kwargs:
+            Keyword arguments that will be predefined for the function in
+            the Tool object.
+
+    Returns:
+        Tool:
+            An object encapsulating the given function and its predefined
+            arguments, ready to be utilized as a Tool.
+
+    Examples:
+        Given a function `move_disk` that requires an environment and two
+        pegs to move a disk from one peg to another in the Tower of Hanoi
+        puzzle, one can create a tool with a predefined environment by:
+
+        ```python
+        def move_disk(env: HanoiEnv, from_peg: int, to_peg: int) -> str:
+            pass
+
+        env = HanoiEnv()
+        tools = [as_tool(move_disk, env=env)]
+        ```
+
+        In this example, `move_disk` is encapsulated into a Tool with `env`
+        predefined, so only `from_peg` and `to_peg` are required.
+    """
+    return Tool(func=func, **kwargs)
+
+
+def as_tool_choice(obj: Union[str, Callable, BaseTool]) -> dict:
+    """Build a tool choice argument for the OpenAI API from an object."""
+    if isinstance(obj, BaseTool):
+        name = obj.name
+    else:
+        name = getattr(obj, "__name__", str(obj))
+    return dict(type="function", function=dict(name=name))
+
+
+def call(
+    func: Callable, *args: Any, use_process: bool = False, **kwargs: Any
+) -> CallFuture:
+    """Create a CallFuture object from a function and its arguments.
+
+    The CallFuture object will call the function in a separate thread or process,
+    therefore the function need to be thread-safe or process-safe.
+    """
+    return CallFuture(func, *args, use_process=use_process, **kwargs)
+
+
+def openai_tool_schema(func: Callable) -> dict:
+    """Build openai tool schema from a function."""
+    return as_tool(func).openai_schema
+
+
+@need_ctx
+def get_var(name: str, _ctx: PromptContext) -> Any:
+    """Get a variable by name from the prompt context."""
+    return getattr(_ctx, name)
+
+
+@need_ctx
+def records(_ctx: Optional[PromptContext] = None) -> PromptRecords:
+    """Return the prompt defined in the current function.
+
+    Similar to locals() in Python in some sense.
+    """
+    # add default value for _ctx to avoid the warning of type checker
+    if _ctx is None:
+        raise ValueError(
+            "PromptContext is required for records, "
+            "this function should be called within @ppl function."
+        )
+    return _ctx.records
+
+
+@need_ctx
+def convo(_ctx: Optional[PromptContext] = None) -> Conversation:
+    """Return the full conversation in the context.
+
+    Similar to globals() in Python in some sense.
+    """
+    # Added default value for _ctx to avoid the warning of type checker
+    if _ctx is None:
+        raise ValueError(
+            "PromptContext is required for convo, "
+            "this function should be called within @ppl function."
+        )
+    return _ctx.messages
+
+
+def build_tools(tools: OneOrMany[Union[BaseTool, Callable]]) -> Sequence[BaseTool]:
+    """Build a list of tools from the given tools or functions."""
+
+    def convert_to_tool(tool: Union[BaseTool, Callable]) -> BaseTool:
+        if isinstance(tool, BaseTool):
+            return tool
+        if callable(tool):
+            return as_tool(tool)
+        raise ValueError(f"Invalid tool: {tool}")
+
+    # process tools
+    if isinstance(tools, BaseTool) or callable(tools):
+        return [convert_to_tool(tools)]
+    if isinstance(tools, Sequence):
+        return [convert_to_tool(tool) for tool in tools]
+    raise ValueError(f"Invalid tools: {tools}")
+
+
+@need_ctx
+def gen(
+    server: Optional[str] = None,
+    *,
+    max_tokens: Optional[int] = None,
+    stop: MaybeOneOrMany[str] = None,
+    temperature: Optional[float] = None,
+    top_p: Optional[float] = None,
+    n: Optional[int] = None,
+    tools: OneOrMany[Union[BaseTool, Callable]] = [],
+    tool_format: str = "auto",
+    stream: Optional[bool] = None,
+    mock_response: Optional[Union[CompletionResponse, str]] = None,
+    _ctx: Optional[PromptContext] = None,
+    **kwargs: Any,
+) -> Generation:
+    """Send a generation request to the LLM backend.
+
+    Args:
+        server (str, optional):
+            name of the backend server. Defaults to the default server set in the configs.
+        max_tokens (int, optional): maximum number of tokens to generate. Defaults to None.
+        stop (str|Sequence[str], optional): stop sequence(s). Defaults to None.
+        temperature (float, optional): temperature for sampling. Defaults to None.
+        top_p (float, optional): nucleus sampling parameter. Defaults to None.
+        n (int, optional): number of choices to generate. Defaults to 1.
+        tools (BaseTool|Callable|Sequence[BaseTool|Callable], optional): tools can be used. Defaults to None.
+        tool_format (str, optional): format for the tools. Defaults to "auto".
+        stream (bool, optional): whether to stream the results. Defaults to False.
+        mock_response (Union[CompletionResponse, str], optional): mock response for testing. Defaults to None.
+        _ctx (PromptContext): prompt context, will be automatically filled.
+        kwargs (Any): extra arguments for the generation.
+
+    Returns:
+        Generation: a future object representing the generation result
+    """
+    backend_server = server_manager.get_server(server)
+    if _ctx is None:
+        raise ValueError(
+            "PromptContext is required for generation."
+            "Normally, it should be automatically filled."
+        )
+    messages = _ctx.messages
+    messages.materialize()  # materialize the messages
+    # TODO: double check the correctness
+    messages = copy.deepcopy(messages)  # freeze the prompt for the generation
+
+    create_args = GenArgs(
+        model=backend_server.model_name,
+        messages=messages,
+        max_tokens=max_tokens,
+        stop=stop,
+        temperature=temperature,
+        top_p=top_p,
+        n=n,
+        tools=build_tools(tools),
+        tool_format=tool_format,  # type: ignore
+        stream=stream,
+    )
+
+    generation = Generation(
+        backend_server, create_args, mock_response=mock_response, _ctx=_ctx, **kwargs
+    )
+
+    @traceable(name=generation.id, metadata={"appl": "gen"})
+    def langsmith_trace(*args: Any, **kwargs: Any) -> None:
+        pass
+
+    langsmith_trace(backend_server, create_args, _ctx=_ctx, **kwargs)
+    return generation
+
+
+# def serialize(obj: Any) -> Any:
+#     if hasattr(obj, "serialize"):
+#         return obj.serialize()
+#     else:
+#         raise TypeError("Object of type '%s' is not serializable" % type(obj).__name__)
```

### Comparing `applang-0.0.1a3/src/appl/role_changer.py` & `applang-0.0.1a4/src/appl/role_changer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from .core import PromptContext
-from .core.modifiers import PrinterModifier, PrinterPush
-from .core.types import override
-from .types import *
-
-
-class RoleChanger(PrinterModifier):
-    """The contextual role changer of the prompts."""
-
-    _new_role: Optional[MessageRole] = None
-
-    def __init__(
-        self, role: Optional[MessageRole] = None, _ctx: Optional[PromptContext] = None
-    ):
-        """Initialize the RoleChanger object.
-
-        Args:
-            role: The new role of the prompts. Defaults to None.
-            _ctx: The prompt context filled automatically by the APPL function.
-        """
-        super().__init__(_ctx)
-        if role is not None:
-            self._new_role = role
-
-    @override
-    @property
-    def push_args(self) -> PrinterPush:
-        return PrinterPush(new_role=self._new_role)
-
-
-class SystemRole(RoleChanger):
-    """Change the role of the prompts to system."""
-
-    def __init__(self, name: Optional[str] = None, **kwargs: Any):
-        """Initialize the SystemRole object.
-
-        Args:
-            name: The name of the system role. Defaults to None.
-            **kwargs: The keyword arguments to pass to the RoleChanger constructor.
-        """
-        role = MessageRole(SYSTEM, name=name)
-        super().__init__(role=role, **kwargs)
-
-
-class UserRole(RoleChanger):
-    """Change the role of the prompts to user."""
-
-    def __init__(self, name: Optional[str] = None, **kwargs: Any):
-        """Initialize the UserRole object.
-
-        Args:
-            name: The name of the user role. Defaults to None.
-            **kwargs: The keyword arguments to pass to the RoleChanger constructor.
-        """
-        role = MessageRole(USER, name=name)
-        super().__init__(role=role, **kwargs)
-
-
-class AIRole(RoleChanger):
-    """Change the role of the prompts to assistant."""
-
-    def __init__(self, name: Optional[str] = None, **kwargs: Any):
-        """Initialize the AIRole object.
-
-        Args:
-            name: The name of the assistant role. Defaults to None.
-            **kwargs: The keyword arguments to pass to the Role
-        """
-        role = MessageRole(ASSISTANT, name=name)
-        super().__init__(role=role, **kwargs)
-
-
-class ToolRole(RoleChanger):
-    """Change the role of the prompts to tool."""
-
-    def __init__(self, name: Optional[str] = None, **kwargs: Any):
-        """Initialize the ToolRole object.
-
-        Args:
-            name: The name of the tool role. Defaults to None.
-            **kwargs: The keyword arguments to pass to the RoleChanger constructor.
-        """
-        role = MessageRole(TOOL, name=name)
-        super().__init__(role=role, **kwargs)
+from .core import PromptContext
+from .core.modifiers import PrinterModifier, PrinterPush
+from .core.types import override
+from .types import *
+
+
+class RoleChanger(PrinterModifier):
+    """The contextual role changer of the prompts."""
+
+    _new_role: Optional[MessageRole] = None
+
+    def __init__(
+        self, role: Optional[MessageRole] = None, _ctx: Optional[PromptContext] = None
+    ):
+        """Initialize the RoleChanger object.
+
+        Args:
+            role: The new role of the prompts. Defaults to None.
+            _ctx: The prompt context filled automatically by the APPL function.
+        """
+        super().__init__(_ctx)
+        if role is not None:
+            self._new_role = role
+
+    @override
+    @property
+    def push_args(self) -> PrinterPush:
+        return PrinterPush(new_role=self._new_role)
+
+
+class SystemRole(RoleChanger):
+    """Change the role of the prompts to system."""
+
+    def __init__(self, name: Optional[str] = None, **kwargs: Any):
+        """Initialize the SystemRole object.
+
+        Args:
+            name: The name of the system role. Defaults to None.
+            **kwargs: The keyword arguments to pass to the RoleChanger constructor.
+        """
+        role = MessageRole(SYSTEM, name=name)
+        super().__init__(role=role, **kwargs)
+
+
+class UserRole(RoleChanger):
+    """Change the role of the prompts to user."""
+
+    def __init__(self, name: Optional[str] = None, **kwargs: Any):
+        """Initialize the UserRole object.
+
+        Args:
+            name: The name of the user role. Defaults to None.
+            **kwargs: The keyword arguments to pass to the RoleChanger constructor.
+        """
+        role = MessageRole(USER, name=name)
+        super().__init__(role=role, **kwargs)
+
+
+class AIRole(RoleChanger):
+    """Change the role of the prompts to assistant."""
+
+    def __init__(self, name: Optional[str] = None, **kwargs: Any):
+        """Initialize the AIRole object.
+
+        Args:
+            name: The name of the assistant role. Defaults to None.
+            **kwargs: The keyword arguments to pass to the Role
+        """
+        role = MessageRole(ASSISTANT, name=name)
+        super().__init__(role=role, **kwargs)
+
+
+class ToolRole(RoleChanger):
+    """Change the role of the prompts to tool."""
+
+    def __init__(self, name: Optional[str] = None, **kwargs: Any):
+        """Initialize the ToolRole object.
+
+        Args:
+            name: The name of the tool role. Defaults to None.
+            **kwargs: The keyword arguments to pass to the RoleChanger constructor.
+        """
+        role = MessageRole(TOOL, name=name)
+        super().__init__(role=role, **kwargs)
```

### Comparing `applang-0.0.1a3/src/appl/servers/api.py` & `applang-0.0.1a4/src/appl/servers/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,199 +1,198 @@
-from __future__ import annotations
-
-import asyncio
-import time
-from functools import wraps
-from importlib.metadata import version
-
-from langsmith import traceable
-from openai import OpenAI, Stream
-from openai.types.chat import ChatCompletion, ChatCompletionChunk
-
-import litellm
-from instructor.patch import Mode
-from litellm import (
-    CustomStreamWrapper,
-    ModelResponse,
-    completion_cost,
-    stream_chunk_builder,
-)
-from litellm.exceptions import NotFoundError
-
-from ..core import trace
-from ..core.config import configs
-from ..core.message import Conversation
-from ..core.response import CompletionResponse
-from ..core.server import BaseServer, GenArgs
-from ..core.tool import ToolCall
-from ..core.trace import (
-    CompletionRequestEvent,
-    CompletionResponseEvent,
-    add_to_trace,
-    find_in_cache,
-)
-from ..core.types import *
-
-try:
-    # instructor<0.5.0
-    from instructor.patch import wrap_chatcompletion
-
-    def patch(create: Callable, mode: Mode) -> Callable:
-        """Patch the `create` method.
-
-        Enables the following features:
-        - `response_model` parameter to parse the response from OpenAI's API
-        - `max_retries` parameter to retry the function if the response is not valid
-        - `validation_context` parameter to validate the response using the pydantic model
-        - `strict` parameter to use strict json parsing
-        """
-        return wrap_chatcompletion(create, mode)
-
-except ImportError:
-    from instructor.patch import patch  # type: ignore
-
-if configs.getattrs("settings.misc.suppress_litellm_debug_info"):
-    litellm.suppress_debug_info = True
-
-appl_version = version("appl")
-
-
-# wrap the completion function # TODO: wrap the acompletion function?
-@wraps(litellm.completion)
-def chat_completion(**kwargs: Any) -> CompletionResponse:
-    """Wrap the litellm.completion function to add tracing and logging."""
-    if "gen_id" not in kwargs:
-        raise ValueError("gen_id is required for tracing completion generation.")
-    gen_id = kwargs.pop("gen_id")
-    add_to_trace(CompletionRequestEvent(name=gen_id))
-
-    log_llm_call_args = configs.getattrs("settings.logging.display.llm_raw_call_args")
-    log_llm_response = configs.getattrs("settings.logging.display.llm_raw_response")
-    log_llm_cache = configs.getattrs("settings.logging.display.llm_cache")
-    if log_llm_call_args:
-        logger.info(f"Call completion [{gen_id}] with args: {kwargs}")
-
-    @traceable(
-        name=f"ChatCompletion_{gen_id}",
-        run_type="llm",
-        metadata={"appl": "completion", "appl_version": appl_version},
-    )
-    def wrapped(**inner_kwargs: Any) -> Tuple[Any, bool]:
-        if cache_ret := find_in_cache(gen_id, inner_kwargs):
-            if log_llm_cache:
-                logger.info("Found in cache, using cached response...")
-            if inner_kwargs.get("stream", False):
-                raise ValueError("Not support stream using cache yet.")
-                # TODO: support rebuild the stream from cached response
-            raw_response = cache_ret
-        else:
-            if log_llm_cache:
-                logger.info("Not found in cache, creating response...")
-            raw_response = litellm.completion(**inner_kwargs)
-        return raw_response, cache_ret is not None
-
-    raw_response, use_cache = wrapped(**kwargs)
-
-    def post_completion(response: CompletionResponse) -> None:
-        raw_response = response.complete_response
-        cost = 0.0
-        if not use_cache:
-            try:
-                cost = completion_cost(raw_response)
-            except litellm.exceptions.NotFoundError:
-                pass
-        response.cost = cost  # update the cost
-        add_to_trace(
-            CompletionResponseEvent(
-                name=gen_id, args=kwargs, ret=raw_response, cost=cost
-            )
-        )
-        if log_llm_response:
-            logger.info(f"Completion [{gen_id}] response: {response}")
-
-    return CompletionResponse(
-        raw_response=raw_response, post_finish_callbacks=[post_completion]
-    )  # type: ignore
-
-
-# TODO: add default batch_size, to avoid too many requests
-class APIServer(BaseServer):
-    """The server for API models. It is a wrapper of litellm.completion."""
-
-    def __init__(
-        self,
-        model: str,
-        base_url: Optional[str] = None,
-        api_key: Optional[str] = None,
-        is_custom_llm: bool = False,
-        wrap_mode: Optional[Mode] = Mode.TOOLS,
-        cost_currency: str = "USD",
-        **kwargs: Any,
-    ) -> None:
-        """Initialize the API server.
-
-        See [LiteLLM](https://docs.litellm.ai/docs/providers)
-        for available models and providers.
-        See [completion](https://docs.litellm.ai/docs/completion/input#input-params-1)
-        for available options.
-        """
-        super().__init__()
-        self._wrap_mode = wrap_mode
-        self._model = model
-        self._base_url = base_url
-        self._api_key = api_key
-        self._is_custom_llm = is_custom_llm
-        self._cost_currency = cost_currency
-        self._default_args = kwargs
-
-    @property
-    def model_name(self):
-        """The model name."""
-        return self._model
-
-    def _get_create_args(self, args: GenArgs, **kwargs: Any) -> dict:
-        # supports custom postprocess create_args
-        create_args = self._default_args.copy()
-        postprocess = kwargs.pop("postprocess_args", None)
-        if self._base_url is not None:
-            create_args["base_url"] = self._base_url
-        if self._api_key is not None:
-            create_args["api_key"] = self._api_key
-        if self._is_custom_llm:
-            create_args["custom_llm_provider"] = "openai"
-        create_args.update(kwargs)  # update create_args with other kwargs
-
-        # add args to create_args
-        create_args.update(args.preprocess(self._convert, is_openai=True))
-        if postprocess is not None:
-            create_args = postprocess(create_args)
-
-        return create_args
-
-    def _create(self, **kwargs: Any) -> CompletionResponse:
-        response: CompletionResponse = None  # type: ignore
-
-        response_model = kwargs.get("response_model", None)
-        if self._wrap_mode is not None and response_model is not None:
-
-            def wrapper(**inner_kwargs: Any) -> CompletionResponse:
-                nonlocal response
-                response = chat_completion(**inner_kwargs)
-                return response
-
-            # Use instructor.patch to enable using a pydantic model as response model
-            # added arguments: response_model, validation_context, max_retries
-            patched = patch(create=wrapper, mode=self._wrap_mode)
-            results = patched(**kwargs)
-            # fill in the response_model and response_obj
-            response.response_model = response_model
-            response.response_obj = results
-        else:
-            response = chat_completion(**kwargs)
-        return response
-
-    def _convert(self, conversation: Conversation) -> List[Dict[str, str]]:
-        return conversation.as_list()
-
-    def close(self):
-        """Close the server."""
-        pass
+from __future__ import annotations
+
+import asyncio
+import time
+from functools import wraps
+from importlib.metadata import version
+
+from langsmith import traceable
+from openai import OpenAI, Stream
+from openai.types.chat import ChatCompletion, ChatCompletionChunk
+
+import litellm
+from appl import __version__
+from instructor.patch import Mode
+from litellm import (
+    CustomStreamWrapper,
+    ModelResponse,
+    completion_cost,
+    stream_chunk_builder,
+)
+from litellm.exceptions import NotFoundError
+
+from ..core import trace
+from ..core.config import configs
+from ..core.message import Conversation
+from ..core.response import CompletionResponse
+from ..core.server import BaseServer, GenArgs
+from ..core.tool import ToolCall
+from ..core.trace import (
+    CompletionRequestEvent,
+    CompletionResponseEvent,
+    add_to_trace,
+    find_in_cache,
+)
+from ..core.types import *
+
+try:
+    # instructor<0.5.0
+    from instructor.patch import wrap_chatcompletion
+
+    def patch(create: Callable, mode: Mode) -> Callable:
+        """Patch the `create` method.
+
+        Enables the following features:
+        - `response_model` parameter to parse the response from OpenAI's API
+        - `max_retries` parameter to retry the function if the response is not valid
+        - `validation_context` parameter to validate the response using the pydantic model
+        - `strict` parameter to use strict json parsing
+        """
+        return wrap_chatcompletion(create, mode)
+
+except ImportError:
+    from instructor.patch import patch  # type: ignore
+
+if configs.getattrs("settings.misc.suppress_litellm_debug_info"):
+    litellm.suppress_debug_info = True
+
+
+# wrap the completion function # TODO: wrap the acompletion function?
+@wraps(litellm.completion)
+def chat_completion(**kwargs: Any) -> CompletionResponse:
+    """Wrap the litellm.completion function to add tracing and logging."""
+    if "gen_id" not in kwargs:
+        raise ValueError("gen_id is required for tracing completion generation.")
+    gen_id = kwargs.pop("gen_id")
+    add_to_trace(CompletionRequestEvent(name=gen_id))
+
+    log_llm_call_args = configs.getattrs("settings.logging.display.llm_raw_call_args")
+    log_llm_response = configs.getattrs("settings.logging.display.llm_raw_response")
+    log_llm_cache = configs.getattrs("settings.logging.display.llm_cache")
+    if log_llm_call_args:
+        logger.info(f"Call completion [{gen_id}] with args: {kwargs}")
+
+    @traceable(
+        name=f"ChatCompletion_{gen_id}",
+        run_type="llm",
+        metadata={"appl": "completion", "appl_version": __version__},
+    )
+    def wrapped(**inner_kwargs: Any) -> Tuple[Any, bool]:
+        if cache_ret := find_in_cache(gen_id, inner_kwargs):
+            if log_llm_cache:
+                logger.info("Found in cache, using cached response...")
+            if inner_kwargs.get("stream", False):
+                raise ValueError("Not support stream using cache yet.")
+                # TODO: support rebuild the stream from cached response
+            raw_response = cache_ret
+        else:
+            if log_llm_cache:
+                logger.info("Not found in cache, creating response...")
+            raw_response = litellm.completion(**inner_kwargs)
+        return raw_response, cache_ret is not None
+
+    raw_response, use_cache = wrapped(**kwargs)
+
+    def post_completion(response: CompletionResponse) -> None:
+        raw_response = response.complete_response
+        cost = 0.0
+        if not use_cache:
+            try:
+                cost = completion_cost(raw_response)
+            except litellm.exceptions.NotFoundError:
+                pass
+        response.cost = cost  # update the cost
+        add_to_trace(
+            CompletionResponseEvent(
+                name=gen_id, args=kwargs, ret=raw_response, cost=cost
+            )
+        )
+        if log_llm_response:
+            logger.info(f"Completion [{gen_id}] response: {response}")
+
+    return CompletionResponse(
+        raw_response=raw_response, post_finish_callbacks=[post_completion]
+    )  # type: ignore
+
+
+# TODO: add default batch_size, to avoid too many requests
+class APIServer(BaseServer):
+    """The server for API models. It is a wrapper of litellm.completion."""
+
+    def __init__(
+        self,
+        model: str,
+        base_url: Optional[str] = None,
+        api_key: Optional[str] = None,
+        is_custom_llm: bool = False,
+        wrap_mode: Optional[Mode] = Mode.TOOLS,
+        cost_currency: str = "USD",
+        **kwargs: Any,
+    ) -> None:
+        """Initialize the API server.
+
+        See [LiteLLM](https://docs.litellm.ai/docs/providers)
+        for available models and providers.
+        See [completion](https://docs.litellm.ai/docs/completion/input#input-params-1)
+        for available options.
+        """
+        super().__init__()
+        self._wrap_mode = wrap_mode
+        self._model = model
+        self._base_url = base_url
+        self._api_key = api_key
+        self._is_custom_llm = is_custom_llm
+        self._cost_currency = cost_currency
+        self._default_args = kwargs
+
+    @property
+    def model_name(self):
+        """The model name."""
+        return self._model
+
+    def _get_create_args(self, args: GenArgs, **kwargs: Any) -> dict:
+        # supports custom postprocess create_args
+        create_args = self._default_args.copy()
+        postprocess = kwargs.pop("postprocess_args", None)
+        if self._base_url is not None:
+            create_args["base_url"] = self._base_url
+        if self._api_key is not None:
+            create_args["api_key"] = self._api_key
+        if self._is_custom_llm:
+            create_args["custom_llm_provider"] = "openai"
+        create_args.update(kwargs)  # update create_args with other kwargs
+
+        # add args to create_args
+        create_args.update(args.preprocess(self._convert, is_openai=True))
+        if postprocess is not None:
+            create_args = postprocess(create_args)
+
+        return create_args
+
+    def _create(self, **kwargs: Any) -> CompletionResponse:
+        response: CompletionResponse = None  # type: ignore
+
+        response_model = kwargs.get("response_model", None)
+        if self._wrap_mode is not None and response_model is not None:
+
+            def wrapper(**inner_kwargs: Any) -> CompletionResponse:
+                nonlocal response
+                response = chat_completion(**inner_kwargs)
+                return response
+
+            # Use instructor.patch to enable using a pydantic model as response model
+            # added arguments: response_model, validation_context, max_retries
+            patched = patch(create=wrapper, mode=self._wrap_mode)
+            results = patched(**kwargs)
+            # fill in the response_model and response_obj
+            response.response_model = response_model
+            response.response_obj = results
+        else:
+            response = chat_completion(**kwargs)
+        return response
+
+    def _convert(self, conversation: Conversation) -> List[Dict[str, str]]:
+        return conversation.as_list()
+
+    def close(self):
+        """Close the server."""
+        pass
```

### Comparing `applang-0.0.1a3/src/appl/servers/manager.py` & `applang-0.0.1a4/src/appl/servers/manager.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from litellm import model_list, provider_list
-
-from ..core.config import configs
-from ..core.server import BaseServer, DummyServer
-from ..core.types import *
-
-
-def _init_server(
-    model: str,
-    provider: Optional[str] = None,
-    base_url: Optional[str] = None,
-    api_key: Optional[str] = None,
-    is_custom_llm: bool = False,
-    **kwargs: Any,
-) -> BaseServer:
-    """Initialize a server based on the model, provider and other arguments."""
-    if provider is None:
-        provider = model.split("/")[0]
-
-    if model == "_dummy":
-        server: BaseServer = DummyServer()  # for testing purposes
-    elif provider == "api" or model in model_list or provider in provider_list:
-        from .api import APIServer
-
-        msg = f"Initializing APIserver for model {model}"
-        if base_url is not None:
-            msg += f" with address {base_url}"
-        logger.info(msg)
-        server = APIServer(
-            model,
-            base_url=base_url,
-            api_key=api_key,
-            is_custom_llm=is_custom_llm,
-            **kwargs,
-        )
-    else:
-        raise ValueError(f"Unknown model {model}")
-
-    return server
-
-
-class ServerManager:
-    """The manager for all servers."""
-
-    def __init__(self) -> None:
-        """Initialize the server manager."""
-        self._servers: Dict[str, BaseServer] = {}
-
-    def register_server(self, name: str, server: BaseServer) -> None:
-        """Register a server with a name."""
-        self._servers[name] = server
-
-    def close_server(self, name: str) -> None:
-        """Close a server by name."""
-        if name in self._servers:
-            self._servers[name].close()
-            del self._servers[name]
-
-    def get_server(self, name: Optional[str]) -> BaseServer:
-        """Get a server by name. If name is None, get the default server."""
-        if name is None:
-            name = configs.getattrs("servers.default")
-
-        if name not in self._servers:
-            if name in configs.get("servers", {}):
-                server_config: dict = configs.servers[name]
-                server = _init_server(**server_config)
-                self.register_server(name, server)
-            else:
-                raise ValueError(f"Server {name} not found")
-        return self._servers[name]
-
-    @property
-    def default_server(self) -> BaseServer:
-        """The default server."""
-        if "default" not in self._servers:
-            raise ValueError("Default server not found")
-        return self._servers["default"]
-
-
-# Singleton server manager
-server_manager = ServerManager()
+from litellm import model_list, provider_list
+
+from ..core.config import configs
+from ..core.server import BaseServer, DummyServer
+from ..core.types import *
+
+
+def _init_server(
+    model: str,
+    provider: Optional[str] = None,
+    base_url: Optional[str] = None,
+    api_key: Optional[str] = None,
+    is_custom_llm: bool = False,
+    **kwargs: Any,
+) -> BaseServer:
+    """Initialize a server based on the model, provider and other arguments."""
+    if provider is None:
+        provider = model.split("/")[0]
+
+    if model == "_dummy":
+        server: BaseServer = DummyServer()  # for testing purposes
+    elif provider == "api" or model in model_list or provider in provider_list:
+        from .api import APIServer
+
+        msg = f"Initializing APIserver for model {model}"
+        if base_url is not None:
+            msg += f" with address {base_url}"
+        logger.info(msg)
+        server = APIServer(
+            model,
+            base_url=base_url,
+            api_key=api_key,
+            is_custom_llm=is_custom_llm,
+            **kwargs,
+        )
+    else:
+        raise ValueError(f"Unknown model {model}")
+
+    return server
+
+
+class ServerManager:
+    """The manager for all servers."""
+
+    def __init__(self) -> None:
+        """Initialize the server manager."""
+        self._servers: Dict[str, BaseServer] = {}
+
+    def register_server(self, name: str, server: BaseServer) -> None:
+        """Register a server with a name."""
+        self._servers[name] = server
+
+    def close_server(self, name: str) -> None:
+        """Close a server by name."""
+        if name in self._servers:
+            self._servers[name].close()
+            del self._servers[name]
+
+    def get_server(self, name: Optional[str]) -> BaseServer:
+        """Get a server by name. If name is None, get the default server."""
+        if name is None:
+            name = configs.getattrs("servers.default")
+
+        if name not in self._servers:
+            if name in configs.get("servers", {}):
+                server_config: dict = configs.servers[name]
+                server = _init_server(**server_config)
+                self.register_server(name, server)
+            else:
+                raise ValueError(f"Server {name} not found")
+        return self._servers[name]
+
+    @property
+    def default_server(self) -> BaseServer:
+        """The default server."""
+        if "default" not in self._servers:
+            raise ValueError("Default server not found")
+        return self._servers["default"]
+
+
+# Singleton server manager
+server_manager = ServerManager()
```

### Comparing `applang-0.0.1a3/src/appl/tracing/header.html` & `applang-0.0.1a4/src/appl/tracing/header.html`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-<head>
-    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"
-        integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
-    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
-        integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz"
-        crossorigin="anonymous"></script>
-    <style>
-        body {
-            max-width: 800px;
-            margin: auto;
-            font-family: sans-serif;
-        }
-    </style>
+<head>
+    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"
+        integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
+    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
+        integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz"
+        crossorigin="anonymous"></script>
+    <style>
+        body {
+            max-width: 800px;
+            margin: auto;
+            font-family: sans-serif;
+        }
+    </style>
 </head>
```

### Comparing `applang-0.0.1a3/src/appl/tracing/printer.py` & `applang-0.0.1a4/src/appl/tracing/printer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,220 +1,220 @@
-import os
-
-import appl
-
-from ..compositor import Tagged
-from ..core.config import Configs
-from ..core.io import load_file
-from ..core.printer import PromptRecords
-from ..core.trace import (
-    CompletionRequestEvent,
-    CompletionResponseEvent,
-    FunctionCallEvent,
-    FunctionReturnEvent,
-    GenerationInitEvent,
-    GenerationResponseEvent,
-    TraceEngineBase,
-    TraceEventBase,
-    TraceNode,
-    TracePrinterBase,
-)
-from ..core.types import *
-from ..func import ppl, records
-
-folder = os.path.dirname(__file__)
-
-
-class TraceHTMLPrinter(TracePrinterBase):
-    """The printer used to print the trace in the format of HTML."""
-
-    def __init__(self):
-        """Initialize the printer."""
-        super().__init__()
-        self._generation_style = "text-success-emphasis bg-Success-subtle list-group-item d-flex justify-content-between align-items-center"
-        self._time_style = "position-absolute top-0 start-100 translate-middle badge rounded-pill bg-info"
-        self._cost_style = "position-absolute bottom-0 start-100 translate-middle badge rounded-pill bg-warning"
-        self._longest_shown_output = 70
-
-        self._head = load_file(os.path.join(folder, "header.html"))
-        self._color_map = {
-            "user": "text-bg-info",
-            "assistant": "text-bg-warning",
-            "system": "text-bg-success",
-        }
-
-    @ppl(exclude_first_str=True)
-    def print(self, trace: TraceEngineBase, meta_data: Optional[Configs] = None) -> str:
-        """Print the trace in the format of HTML."""
-        with Tagged("html"):
-            self._head
-            with Tagged("body"):
-                for node in trace.trace_nodes.values():
-                    if node.parent is None:
-                        self._print_node(node, trace.min_timestamp)
-        if meta_data:
-            with Tagged("table", attrs={"class": "table small"}):
-                if start_time := meta_data.getattrs("info.start_time"):
-                    self._make_line("Start Time", start_time)
-                self._make_line("Full Configs", f"<pre>{meta_data.to_yaml()}</pre>")
-        return str(records())
-
-    @ppl
-    def _print_messages(self, messages: List[Union[str, Dict]]) -> PromptRecords:
-        def display(message: Union[str, Dict]) -> str:
-            return f'<div style="white-space: pre-wrap;">{message}</div>'
-
-        with Tagged("ul", attrs={"class": "list-group small"}):
-            for message in messages:
-                with Tagged("li", attrs={"class": "list-group-item"}):
-                    if (
-                        isinstance(message, dict)
-                        and "role" in message
-                        and "content" in message
-                    ):
-                        color = self._color_map.get(message["role"], "text-bg-info")
-                        f"<span class='badge {color}'>{message['role']}</span>"
-                        display(message["content"])
-                    else:
-                        display(message)
-        return records()
-
-    @ppl
-    def _print_genargs(self, args: Dict, output: Optional[str] = None) -> PromptRecords:
-        with Tagged("table", attrs={"class": "table small"}):
-            for k, v in args.items():
-                with Tagged("tr"):
-                    with Tagged("th"):
-                        f"{k}"
-                    with Tagged("td"):
-                        if k == "messages":
-                            self._print_messages(v)
-                        elif k in ["response_model"]:
-                            f"<pre>{v}</pre>"
-                        elif k == "stop":
-                            repr(v)
-                        else:
-                            f"{v}"
-            if output is not None:
-                self._make_line("output", output)
-        return records()
-
-    @ppl
-    def _print_gen(self, node: TraceNode, min_timestamp: float = 0.0) -> PromptRecords:
-        name = node.name
-        if node.args is not None:
-            completion = node.children[0] if node.children else None
-            with Tagged("ul", attrs={"class": "list-group m-1"}):
-                li_attrs = {"class": self._generation_style}
-                li_attrs.update(self._toggle_attrs(name))
-                with Tagged("li", attrs=li_attrs):
-                    f"<div><b>{name}:</b> {node.ret}</div>"
-                    if completion and (runtime := completion.runtime) > 0:
-                        f"<span class='{self._time_style}'>{runtime/1000.0:.2e} s</span>"
-                    if completion and (cost := completion.info.get("cost")):
-                        f"<span class='{self._cost_style}'>$ {cost:.2e}</span>"
-                with Tagged(
-                    "li", attrs={"class": "list-group-item collapse", "id": name}
-                ):
-                    self._print_genargs(node.args, node.ret)
-        else:
-            li_attrs = {
-                "class": "list-group-item text-warning-emphasis bg-warning-subtle"
-            }
-            with Tagged("ul", attrs={"class": "list-group m-1"}):
-                with Tagged("li", attrs=li_attrs):
-                    "Unfinished Generation"
-        return records()
-
-    @ppl
-    def _print_func(self, node: TraceNode, min_timestamp: float = 0.0) -> PromptRecords:
-        name = node.name
-        with Tagged("ul", attrs={"class": "list-group m-2"}):
-            li_attrs = {"class": "text-center bg-light list-group-item"}
-            li_attrs.update(self._toggle_attrs(name, True))
-            with Tagged("li", attrs=li_attrs):
-                f"<b>{name}</b>"
-            with Tagged("li", attrs={"class": "list-group-item show", "id": name}):
-                # display details for the function
-                # ? display time, args and kwargs
-                # with Tagged("table", attrs={"class": "table small"}):
-                #     start = (node.start_time - min_timestamp) / 1000.0
-                #     end = (node.end_time - min_timestamp) / 1000.0
-                #     runtime = end - start
-                #     self._make_line(
-                #         "Time", f"{runtime:.2e} s (from {start:.2e} to {end:.2e})"
-                #     )
-                #     # if node.args:
-                #     #     func_args = node.args["args"]
-                #     #     self._make_line("args", func_args)
-                #     #     func_kwargs = node.args["kwargs"]
-                #     #     for k, v in func_kwargs.items():
-                #     #         self._make_line(k, v)
-                for child in node.children:
-                    self._print_node(child, min_timestamp)
-        return records()
-
-    def _print_node(self, node: TraceNode, min_timestamp: float = 0.0) -> Any:
-        if node.type == "func":
-            return self._print_func(node, min_timestamp)
-        else:
-            return self._print_gen(node, min_timestamp)
-
-    def _toggle_attrs(self, name: str, expanded: bool = False) -> Dict:
-        return {
-            "data-bs-toggle": "collapse",
-            "href": f"#{name}",
-            "role": "button",
-            "aria-controls": name,
-            "aria-expanded": "true" if expanded else "false",
-        }
-
-    def _make_line(self, k: str, v: Any) -> str:
-        return f"<tr><th>{k}</th><td>{v}</td></tr>"
-
-
-class TraceProfilePrinter(TracePrinterBase):
-    """The printer used to print the trace in the format of profile."""
-
-    def __init__(self, display_functions: bool = False):
-        """Initialize the printer.
-
-        Args:
-            display_functions: Whether to display the function calls.
-        """
-        self._display_functions = display_functions
-
-    def build_event(self, event: TraceEventBase, min_timestamp: float) -> Dict:
-        """Build the event for the trace."""
-        ts = str((event.time_stamp - min_timestamp) * 1e6)
-        data = {"pid": 0, "tid": 0, "name": event.name, "ts": ts}
-        # TODO: add args to the trace
-        if isinstance(event, CompletionRequestEvent):
-            data["cat"] = "gen"
-            data["ph"] = "b"
-            data["id"] = event.name
-        elif isinstance(event, CompletionResponseEvent):
-            data["cat"] = "gen"
-            data["ph"] = "e"
-            data["id"] = event.name
-            data["cost"] = event.cost
-            data["output"] = event.ret.dict()
-        elif self._display_functions:
-            if isinstance(event, FunctionCallEvent):
-                data["cat"] = "func"
-                data["ph"] = "B"
-                data["tid"] = "main"
-            elif isinstance(event, FunctionReturnEvent):
-                data["cat"] = "func"
-                data["ph"] = "E"
-                data["tid"] = "main"
-        return data
-
-    def print(
-        self, trace: TraceEngineBase, meta_data: Optional[Configs] = None
-    ) -> Dict:
-        """Print the trace in the format of Chrome tracing."""
-        events = []
-        for event in trace.events:
-            if data := self.build_event(event, trace.min_timestamp):
-                events.append(data)
-        return {"traceEvents": events}
+import os
+
+import appl
+
+from ..compositor import Tagged
+from ..core.config import Configs
+from ..core.io import load_file
+from ..core.printer import PromptRecords
+from ..core.trace import (
+    CompletionRequestEvent,
+    CompletionResponseEvent,
+    FunctionCallEvent,
+    FunctionReturnEvent,
+    GenerationInitEvent,
+    GenerationResponseEvent,
+    TraceEngineBase,
+    TraceEventBase,
+    TraceNode,
+    TracePrinterBase,
+)
+from ..core.types import *
+from ..func import ppl, records
+
+folder = os.path.dirname(__file__)
+
+
+class TraceHTMLPrinter(TracePrinterBase):
+    """The printer used to print the trace in the format of HTML."""
+
+    def __init__(self):
+        """Initialize the printer."""
+        super().__init__()
+        self._generation_style = "text-success-emphasis bg-Success-subtle list-group-item d-flex justify-content-between align-items-center"
+        self._time_style = "position-absolute top-0 start-100 translate-middle badge rounded-pill bg-info"
+        self._cost_style = "position-absolute bottom-0 start-100 translate-middle badge rounded-pill bg-warning"
+        self._longest_shown_output = 70
+
+        self._head = load_file(os.path.join(folder, "header.html"))
+        self._color_map = {
+            "user": "text-bg-info",
+            "assistant": "text-bg-warning",
+            "system": "text-bg-success",
+        }
+
+    @ppl(exclude_first_str=True)
+    def print(self, trace: TraceEngineBase, meta_data: Optional[Configs] = None) -> str:
+        """Print the trace in the format of HTML."""
+        with Tagged("html"):
+            self._head
+            with Tagged("body"):
+                for node in trace.trace_nodes.values():
+                    if node.parent is None:
+                        self._print_node(node, trace.min_timestamp)
+        if meta_data:
+            with Tagged("table", attrs={"class": "table small"}):
+                if start_time := meta_data.getattrs("info.start_time"):
+                    self._make_line("Start Time", start_time)
+                self._make_line("Full Configs", f"<pre>{meta_data.to_yaml()}</pre>")
+        return str(records())
+
+    @ppl
+    def _print_messages(self, messages: List[Union[str, Dict]]) -> PromptRecords:
+        def display(message: Union[str, Dict]) -> str:
+            return f'<div style="white-space: pre-wrap;">{message}</div>'
+
+        with Tagged("ul", attrs={"class": "list-group small"}):
+            for message in messages:
+                with Tagged("li", attrs={"class": "list-group-item"}):
+                    if (
+                        isinstance(message, dict)
+                        and "role" in message
+                        and "content" in message
+                    ):
+                        color = self._color_map.get(message["role"], "text-bg-info")
+                        f"<span class='badge {color}'>{message['role']}</span>"
+                        display(message["content"])
+                    else:
+                        display(message)
+        return records()
+
+    @ppl
+    def _print_genargs(self, args: Dict, output: Optional[str] = None) -> PromptRecords:
+        with Tagged("table", attrs={"class": "table small"}):
+            for k, v in args.items():
+                with Tagged("tr"):
+                    with Tagged("th"):
+                        f"{k}"
+                    with Tagged("td"):
+                        if k == "messages":
+                            self._print_messages(v)
+                        elif k in ["response_model"]:
+                            f"<pre>{v}</pre>"
+                        elif k == "stop":
+                            repr(v)
+                        else:
+                            f"{v}"
+            if output is not None:
+                self._make_line("output", output)
+        return records()
+
+    @ppl
+    def _print_gen(self, node: TraceNode, min_timestamp: float = 0.0) -> PromptRecords:
+        name = node.name
+        if node.args is not None:
+            completion = node.children[0] if node.children else None
+            with Tagged("ul", attrs={"class": "list-group m-1"}):
+                li_attrs = {"class": self._generation_style}
+                li_attrs.update(self._toggle_attrs(name))
+                with Tagged("li", attrs=li_attrs):
+                    f"<div><b>{name}:</b> {node.ret}</div>"
+                    if completion and (runtime := completion.runtime) > 0:
+                        f"<span class='{self._time_style}'>{runtime/1000.0:.2e} s</span>"
+                    if completion and (cost := completion.info.get("cost")):
+                        f"<span class='{self._cost_style}'>$ {cost:.2e}</span>"
+                with Tagged(
+                    "li", attrs={"class": "list-group-item collapse", "id": name}
+                ):
+                    self._print_genargs(node.args, node.ret)
+        else:
+            li_attrs = {
+                "class": "list-group-item text-warning-emphasis bg-warning-subtle"
+            }
+            with Tagged("ul", attrs={"class": "list-group m-1"}):
+                with Tagged("li", attrs=li_attrs):
+                    "Unfinished Generation"
+        return records()
+
+    @ppl
+    def _print_func(self, node: TraceNode, min_timestamp: float = 0.0) -> PromptRecords:
+        name = node.name
+        with Tagged("ul", attrs={"class": "list-group m-2"}):
+            li_attrs = {"class": "text-center bg-light list-group-item"}
+            li_attrs.update(self._toggle_attrs(name, True))
+            with Tagged("li", attrs=li_attrs):
+                f"<b>{name}</b>"
+            with Tagged("li", attrs={"class": "list-group-item show", "id": name}):
+                # display details for the function
+                # ? display time, args and kwargs
+                # with Tagged("table", attrs={"class": "table small"}):
+                #     start = (node.start_time - min_timestamp) / 1000.0
+                #     end = (node.end_time - min_timestamp) / 1000.0
+                #     runtime = end - start
+                #     self._make_line(
+                #         "Time", f"{runtime:.2e} s (from {start:.2e} to {end:.2e})"
+                #     )
+                #     # if node.args:
+                #     #     func_args = node.args["args"]
+                #     #     self._make_line("args", func_args)
+                #     #     func_kwargs = node.args["kwargs"]
+                #     #     for k, v in func_kwargs.items():
+                #     #         self._make_line(k, v)
+                for child in node.children:
+                    self._print_node(child, min_timestamp)
+        return records()
+
+    def _print_node(self, node: TraceNode, min_timestamp: float = 0.0) -> Any:
+        if node.type == "func":
+            return self._print_func(node, min_timestamp)
+        else:
+            return self._print_gen(node, min_timestamp)
+
+    def _toggle_attrs(self, name: str, expanded: bool = False) -> Dict:
+        return {
+            "data-bs-toggle": "collapse",
+            "href": f"#{name}",
+            "role": "button",
+            "aria-controls": name,
+            "aria-expanded": "true" if expanded else "false",
+        }
+
+    def _make_line(self, k: str, v: Any) -> str:
+        return f"<tr><th>{k}</th><td>{v}</td></tr>"
+
+
+class TraceProfilePrinter(TracePrinterBase):
+    """The printer used to print the trace in the format of profile."""
+
+    def __init__(self, display_functions: bool = False):
+        """Initialize the printer.
+
+        Args:
+            display_functions: Whether to display the function calls.
+        """
+        self._display_functions = display_functions
+
+    def build_event(self, event: TraceEventBase, min_timestamp: float) -> Dict:
+        """Build the event for the trace."""
+        ts = str((event.time_stamp - min_timestamp) * 1e6)
+        data = {"pid": 0, "tid": 0, "name": event.name, "ts": ts}
+        # TODO: add args to the trace
+        if isinstance(event, CompletionRequestEvent):
+            data["cat"] = "gen"
+            data["ph"] = "b"
+            data["id"] = event.name
+        elif isinstance(event, CompletionResponseEvent):
+            data["cat"] = "gen"
+            data["ph"] = "e"
+            data["id"] = event.name
+            data["cost"] = event.cost
+            data["output"] = event.ret.dict()
+        elif self._display_functions:
+            if isinstance(event, FunctionCallEvent):
+                data["cat"] = "func"
+                data["ph"] = "B"
+                data["tid"] = "main"
+            elif isinstance(event, FunctionReturnEvent):
+                data["cat"] = "func"
+                data["ph"] = "E"
+                data["tid"] = "main"
+        return data
+
+    def print(
+        self, trace: TraceEngineBase, meta_data: Optional[Configs] = None
+    ) -> Dict:
+        """Print the trace in the format of Chrome tracing."""
+        events = []
+        for event in trace.events:
+            if data := self.build_event(event, trace.min_timestamp):
+                events.append(data)
+        return {"traceEvents": events}
```

### Comparing `applang-0.0.1a3/src/appl/types.py` & `applang-0.0.1a4/src/appl/types.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from .core.context import PromptContext
-from .core.function import PromptFunc
-from .core.message import (
-    AIMessage,
-    BaseMessage,
-    Conversation,
-    SystemMessage,
-    ToolMessage,
-    UserMessage,
-)
-from .core.modifiers import Compositor
-from .core.printer import Indexing, PromptPrinter, PromptRecords
-from .core.promptable import BracketedDefinition, Definition, FormatterMeta, Promptable
-from .core.response import CompletionResponse
-from .core.server import BaseServer, GenArgs
-from .core.tool import BaseTool, Tool
-from .core.types import *
+from .core.context import PromptContext
+from .core.function import PromptFunc
+from .core.message import (
+    AIMessage,
+    BaseMessage,
+    Conversation,
+    SystemMessage,
+    ToolMessage,
+    UserMessage,
+)
+from .core.modifiers import Compositor
+from .core.printer import Indexing, PromptPrinter, PromptRecords
+from .core.promptable import BracketedDefinition, Definition, FormatterMeta, Promptable
+from .core.response import CompletionResponse
+from .core.server import BaseServer, GenArgs
+from .core.tool import BaseTool, Tool
+from .core.types import *
```

### Comparing `applang-0.0.1a3/src/appl/utils.py` & `applang-0.0.1a4/src/appl/utils.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-import os
-import sys
-
-import loguru
-import tiktoken
-from dotenv.main import _walk_to_root
-
-from .core.config import configs
-from .types import *
-
-
-def _is_interactive():
-    """Decide whether this is running in a REPL or IPython notebook."""
-    try:
-        main = __import__("__main__", None, None, fromlist=["__file__"])
-    except ModuleNotFoundError:
-        return False
-    return not hasattr(main, "__file__")
-
-
-def get_folder(
-    current_folder: Optional[str] = None,
-    usecwd: bool = False,
-) -> str:
-    """Get the the current working directory."""
-    if usecwd or _is_interactive() or getattr(sys, "frozen", False):
-        # Should work without __file__, e.g. in REPL or IPython notebook.
-        folder = os.getcwd()
-    elif current_folder is not None:  # [ADD] option to specify the folder
-        folder = current_folder
-    else:
-        # will work for .py files
-        frame = sys._getframe()
-        current_file = __file__
-
-        while frame.f_code.co_filename == current_file:
-            assert frame.f_back is not None
-            frame = frame.f_back
-        frame_filename = frame.f_code.co_filename
-        folder = os.path.dirname(os.path.abspath(frame_filename))
-
-    return folder
-
-
-def find_files(folder: str, filenames: list[str]) -> list[str]:
-    """Find files in the folder or its parent folders."""
-    results = []
-    for dirname in _walk_to_root(folder):
-        for filename in filenames:
-            check_path = os.path.join(dirname, filename)
-            if os.path.isfile(check_path):
-                results.append(check_path)
-                # return the first found file among the filenames
-                break
-    return results
-
-
-# rewrite find_dotenv, origin in https://github.com/theskumar/python-dotenv/blob/main/src/dotenv/main.py
-def find_dotenv(
-    filename: str = ".env",
-    raise_error_if_not_found: bool = False,
-    current_folder: Optional[str] = None,
-    usecwd: bool = False,
-) -> str:
-    """Search in increasingly higher folders for the given file.
-
-    Returns path to the file if found, or an empty string otherwise.
-    """
-    # Rewrited the original function to add the option to start with a custom folder
-    folder = get_folder(current_folder, usecwd)
-    results = find_files(folder, [filename])
-    if results:
-        return results[0]
-
-    if raise_error_if_not_found:
-        raise IOError("File not found")
-    return ""
-
-
-def get_num_tokens(prompt: str, encoding: str = "cl100k_base") -> int:
-    """Get the number of tokens in the prompt for the given encoding."""
-    return len(tiktoken.get_encoding(encoding).encode(prompt))
-
-
-def get_meta_file(trace_file: str) -> str:
-    """Get the meta file storing metadata of the trace file."""
-    # meta file derived from trace_file: *.pkl -> *_meta.json
-    return os.path.splitext(trace_file)[0] + "_meta.json"
-
-
-class LoguruFormatter:
-    """Custom formatter for loguru logger."""
-
-    def __init__(
-        self,
-        fmt: Optional[str] = None,
-        max_length: Optional[int] = None,
-        suffix_length: int = 0,
-    ):
-        """Initialize the formatter with the format string and max length of the message.
-
-        Args:
-            fmt: The format string for the log message.
-            max_length: The maximum length of the message, truncate if longer.
-            suffix_length: The length of the suffix to keep when truncating.
-        """
-        if fmt is None:
-            fmt = configs.getattrs("settings.logging.format")
-        self.fmt = fmt.rstrip()
-        self.max_length = max_length
-        self.suffix_length = suffix_length
-
-    def loguru_format(self, record: Dict) -> str:
-        """Format the log message with the record."""
-        msg = record["message"]
-        fmt = self.fmt
-        if self.max_length is not None and len(msg) > self.max_length:
-            suffix_len = min(self.max_length, self.suffix_length)
-            truncated = msg[: self.max_length - suffix_len]
-            truncated += f"...(snipped {len(msg) - self.max_length} chars)"
-            if suffix_len > 0:
-                truncated += "..." + msg[-suffix_len:]
-            record["trunc_message"] = truncated
-            fmt = fmt.replace("{message}", "{trunc_message}")
-        return fmt + "\n"
+import os
+import sys
+
+import loguru
+import tiktoken
+from dotenv.main import _walk_to_root
+
+from .core.config import configs
+from .types import *
+
+
+def _is_interactive():
+    """Decide whether this is running in a REPL or IPython notebook."""
+    try:
+        main = __import__("__main__", None, None, fromlist=["__file__"])
+    except ModuleNotFoundError:
+        return False
+    return not hasattr(main, "__file__")
+
+
+def get_folder(
+    current_folder: Optional[str] = None,
+    usecwd: bool = False,
+) -> str:
+    """Get the the current working directory."""
+    if usecwd or _is_interactive() or getattr(sys, "frozen", False):
+        # Should work without __file__, e.g. in REPL or IPython notebook.
+        folder = os.getcwd()
+    elif current_folder is not None:  # [ADD] option to specify the folder
+        folder = current_folder
+    else:
+        # will work for .py files
+        frame = sys._getframe()
+        current_file = __file__
+
+        while frame.f_code.co_filename == current_file:
+            assert frame.f_back is not None
+            frame = frame.f_back
+        frame_filename = frame.f_code.co_filename
+        folder = os.path.dirname(os.path.abspath(frame_filename))
+
+    return folder
+
+
+def find_files(folder: str, filenames: list[str]) -> list[str]:
+    """Find files in the folder or its parent folders."""
+    results = []
+    for dirname in _walk_to_root(folder):
+        for filename in filenames:
+            check_path = os.path.join(dirname, filename)
+            if os.path.isfile(check_path):
+                results.append(check_path)
+                # return the first found file among the filenames
+                break
+    return results
+
+
+# rewrite find_dotenv, origin in https://github.com/theskumar/python-dotenv/blob/main/src/dotenv/main.py
+def find_dotenv(
+    filename: str = ".env",
+    raise_error_if_not_found: bool = False,
+    current_folder: Optional[str] = None,
+    usecwd: bool = False,
+) -> str:
+    """Search in increasingly higher folders for the given file.
+
+    Returns path to the file if found, or an empty string otherwise.
+    """
+    # Rewrited the original function to add the option to start with a custom folder
+    folder = get_folder(current_folder, usecwd)
+    results = find_files(folder, [filename])
+    if results:
+        return results[0]
+
+    if raise_error_if_not_found:
+        raise IOError("File not found")
+    return ""
+
+
+def get_num_tokens(prompt: str, encoding: str = "cl100k_base") -> int:
+    """Get the number of tokens in the prompt for the given encoding."""
+    return len(tiktoken.get_encoding(encoding).encode(prompt))
+
+
+def get_meta_file(trace_file: str) -> str:
+    """Get the meta file storing metadata of the trace file."""
+    # meta file derived from trace_file: *.pkl -> *_meta.json
+    return os.path.splitext(trace_file)[0] + "_meta.json"
+
+
+class LoguruFormatter:
+    """Custom formatter for loguru logger."""
+
+    def __init__(
+        self,
+        fmt: Optional[str] = None,
+        max_length: Optional[int] = None,
+        suffix_length: int = 0,
+    ):
+        """Initialize the formatter with the format string and max length of the message.
+
+        Args:
+            fmt: The format string for the log message.
+            max_length: The maximum length of the message, truncate if longer.
+            suffix_length: The length of the suffix to keep when truncating.
+        """
+        if fmt is None:
+            fmt = configs.getattrs("settings.logging.format")
+        self.fmt = fmt.rstrip()
+        self.max_length = max_length
+        self.suffix_length = suffix_length
+
+    def loguru_format(self, record: Dict) -> str:
+        """Format the log message with the record."""
+        msg = record["message"]
+        fmt = self.fmt
+        if self.max_length is not None and len(msg) > self.max_length:
+            suffix_len = min(self.max_length, self.suffix_length)
+            truncated = msg[: self.max_length - suffix_len]
+            truncated += f"...(snipped {len(msg) - self.max_length} chars)"
+            if suffix_len > 0:
+                truncated += "..." + msg[-suffix_len:]
+            record["trunc_message"] = truncated
+            fmt = fmt.replace("{message}", "{trunc_message}")
+        return fmt + "\n"
```

### Comparing `applang-0.0.1a3/tests/test_message.py` & `applang-0.0.1a4/tests/test_message.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-import pytest
-
-import appl
-from appl import AIRole, SystemRole, UserRole, ppl, records
-from appl.core import (
-    AIMessage,
-    Conversation,
-    PromptRecords,
-    SystemMessage,
-    ToolCall,
-    UserMessage,
-)
-
-
-def test_message():
-    sys = SystemMessage("You are a helpful assistant.")
-    user = UserMessage("Hello, who are you")
-    ai = AIMessage("I am a helpful assistant.")
-    assert sys.is_system
-    assert user.is_user
-    assert ai.is_ai
-    assert sys.get_dict() == {
-        "role": "system",
-        "content": "You are a helpful assistant.",
-    }
-    assert user.get_dict() == {"role": "user", "content": "Hello, who are you"}
-    assert ai.get_dict() == {
-        "role": "assistant",
-        "content": "I am a helpful assistant.",
-    }
-
-
-def test_msg_role():
-    @ppl
-    def func() -> PromptRecords:
-        "Hello"
-        AIMessage("World")
-        return records()
-
-    assert func().as_convo().as_list() == [
-        {"role": "user", "content": "Hello"},
-        {"role": "assistant", "content": "World"},
-    ]
-
-
-def test_chat_example():
-    @ppl
-    def func() -> PromptRecords:
-        SystemMessage("You are a helpful assistant.")
-        for i in range(5):
-            UserMessage("Hello")
-            AIMessage("World")
-        return records()
-
-    expected = [{"role": "system", "content": "You are a helpful assistant."}]
-    for i in range(5):
-        expected.append({"role": "user", "content": "Hello"})
-        expected.append({"role": "assistant", "content": "World"})
-    assert func().as_convo().as_list() == expected
-
-
-def test_system_msg():
-    @ppl
-    def func() -> PromptRecords:
-        with SystemRole():
-            "You are a helpful Assistant."
-            "You should be helpful."
-        with UserRole():
-            "Hello"
-        return records()
-
-    assert func().as_convo().as_list() == [
-        {
-            "role": "system",
-            "content": "You are a helpful Assistant.\nYou should be helpful.",
-        },
-        {"role": "user", "content": "Hello"},
-    ]
-
-
-def test_message_merge():
-    @ppl
-    def func() -> PromptRecords:
-        SystemMessage("You are a helpful assistant.")
-        UserMessage("Hello, who are you")
-        AIMessage("I am ")
-        AIMessage("a helpful ")
-        AIMessage("assistant.")
-        UserMessage("H")
-        UserMessage("i")
-        SystemMessage(" Add something to system prompt.")
-        return records()
-
-    assert func().as_convo().as_list() == [
-        {
-            "role": "system",
-            "content": "You are a helpful assistant. Add something to system prompt.",
-        },
-        {"role": "user", "content": "Hello, who are you"},
-        {"role": "assistant", "content": "I am a helpful assistant."},
-        {"role": "user", "content": "Hi"},
-    ]
-
-
-def test_ai_tool_call():
-    @ppl
-    def func() -> PromptRecords:
-        AIMessage(tool_calls=[ToolCall(id="1", name="add", args='{"x": 1, "y": 2}')])
-        return records()
-
-    assert func().as_convo().as_list() == [
-        {
-            "role": "assistant",
-            "content": None,
-            "tool_calls": [
-                {
-                    "id": "1",
-                    "type": "function",
-                    "function": {"name": "add", "arguments": '{"x": 1, "y": 2}'},
-                }
-            ],
-        },
-    ]
-
-
-def test_role_wrap():
-    @ppl
-    def func() -> PromptRecords:
-        with AIRole():
-            UserMessage("Hello")
-            AIMessage("World")
-        return records()
-
-    assert func().as_convo().as_list() == [
-        {"role": "user", "content": "Hello"},
-        {"role": "assistant", "content": "World"},
-    ]
-
-
-def test_mix_role_usage():
-    @ppl
-    def func() -> PromptRecords:
-        with AIRole():
-            UserMessage("Hello")
-            AIMessage("World")
-            "Again"
-        return records()
-
-    assert func().as_convo().as_list() == [
-        {"role": "user", "content": "Hello"},
-        {"role": "assistant", "content": "WorldAgain"},
-    ]
-
-
-def test_multi_user():
-    @ppl
-    def func() -> PromptRecords:
-        with UserRole("A"):
-            "Hello"
-        with UserRole("B"):
-            "World"
-        return records()
-
-    assert func().as_convo().as_list() == [
-        {"role": "user", "name": "A", "content": "Hello"},
-        {"role": "user", "name": "B", "content": "World"},
-    ]
-
-
-def test_role_change():
-    @ppl
-    def func() -> PromptRecords:
-        "Hello"
-        with AIRole():
-            "World"
-        return records()
-
-    assert func().as_convo().as_list() == [
-        {"role": "user", "content": "Hello"},
-        {"role": "assistant", "content": "World"},
-    ]
-
-
-def test_role_change_loop1():
-    @ppl
-    def func() -> PromptRecords:
-        for i in range(5):
-            "Hello"
-            with AIRole():
-                "World"
-        return records()
-
-    assert (
-        func().as_convo().as_list()
-        == [
-            {"role": "user", "content": "Hello"},
-            {"role": "assistant", "content": "World"},
-        ]
-        * 5
-    )
-
-
-def test_role_change_loop2():
-    @ppl
-    def func() -> PromptRecords:
-        for i in range(3):
-            "Hello"
-            AIMessage("World")
-        return records()
-
-    assert (
-        func().as_convo().as_list()
-        == [
-            {"role": "user", "content": "Hello"},
-            {"role": "assistant", "content": "World"},
-        ]
-        * 3
-    )
-
-
-def test_role_change_loop3():
-    @ppl
-    def func() -> PromptRecords:
-        "Hello"
-        for i in range(5):
-            with AIRole():
-                "Foo"
-            with UserRole():
-                "Bar"
-        return records()
-
-    expected = [{"role": "user", "content": "Hello"}]
-    for i in range(5):
-        expected.append({"role": "assistant", "content": "Foo"})
-        expected.append({"role": "user", "content": "Bar"})
-
-    assert func().as_convo().as_list() == expected
-
-
-def test_nested_role_error():
-    with pytest.raises(ValueError) as excinfo:
-
-        @ppl
-        def func() -> PromptRecords:
-            "Hello"
-            for i in range(5):
-                with UserRole():
-                    "Foo"
-                    with AIRole():
-                        "Bar"
-            return records()
-
-        func()
-
-    assert "Cannot start a new role" in str(excinfo.value)
+import pytest
+
+import appl
+from appl import AIRole, SystemRole, UserRole, ppl, records
+from appl.core import (
+    AIMessage,
+    Conversation,
+    PromptRecords,
+    SystemMessage,
+    ToolCall,
+    UserMessage,
+)
+
+
+def test_message():
+    sys = SystemMessage("You are a helpful assistant.")
+    user = UserMessage("Hello, who are you")
+    ai = AIMessage("I am a helpful assistant.")
+    assert sys.is_system
+    assert user.is_user
+    assert ai.is_ai
+    assert sys.get_dict() == {
+        "role": "system",
+        "content": "You are a helpful assistant.",
+    }
+    assert user.get_dict() == {"role": "user", "content": "Hello, who are you"}
+    assert ai.get_dict() == {
+        "role": "assistant",
+        "content": "I am a helpful assistant.",
+    }
+
+
+def test_msg_role():
+    @ppl
+    def func() -> PromptRecords:
+        "Hello"
+        AIMessage("World")
+        return records()
+
+    assert func().as_convo().as_list() == [
+        {"role": "user", "content": "Hello"},
+        {"role": "assistant", "content": "World"},
+    ]
+
+
+def test_chat_example():
+    @ppl
+    def func() -> PromptRecords:
+        SystemMessage("You are a helpful assistant.")
+        for i in range(5):
+            UserMessage("Hello")
+            AIMessage("World")
+        return records()
+
+    expected = [{"role": "system", "content": "You are a helpful assistant."}]
+    for i in range(5):
+        expected.append({"role": "user", "content": "Hello"})
+        expected.append({"role": "assistant", "content": "World"})
+    assert func().as_convo().as_list() == expected
+
+
+def test_system_msg():
+    @ppl
+    def func() -> PromptRecords:
+        with SystemRole():
+            "You are a helpful Assistant."
+            "You should be helpful."
+        with UserRole():
+            "Hello"
+        return records()
+
+    assert func().as_convo().as_list() == [
+        {
+            "role": "system",
+            "content": "You are a helpful Assistant.\nYou should be helpful.",
+        },
+        {"role": "user", "content": "Hello"},
+    ]
+
+
+def test_message_merge():
+    @ppl
+    def func() -> PromptRecords:
+        SystemMessage("You are a helpful assistant.")
+        UserMessage("Hello, who are you")
+        AIMessage("I am ")
+        AIMessage("a helpful ")
+        AIMessage("assistant.")
+        UserMessage("H")
+        UserMessage("i")
+        SystemMessage(" Add something to system prompt.")
+        return records()
+
+    assert func().as_convo().as_list() == [
+        {
+            "role": "system",
+            "content": "You are a helpful assistant. Add something to system prompt.",
+        },
+        {"role": "user", "content": "Hello, who are you"},
+        {"role": "assistant", "content": "I am a helpful assistant."},
+        {"role": "user", "content": "Hi"},
+    ]
+
+
+def test_ai_tool_call():
+    @ppl
+    def func() -> PromptRecords:
+        AIMessage(tool_calls=[ToolCall(id="1", name="add", args='{"x": 1, "y": 2}')])
+        return records()
+
+    assert func().as_convo().as_list() == [
+        {
+            "role": "assistant",
+            "content": None,
+            "tool_calls": [
+                {
+                    "id": "1",
+                    "type": "function",
+                    "function": {"name": "add", "arguments": '{"x": 1, "y": 2}'},
+                }
+            ],
+        },
+    ]
+
+
+def test_role_wrap():
+    @ppl
+    def func() -> PromptRecords:
+        with AIRole():
+            UserMessage("Hello")
+            AIMessage("World")
+        return records()
+
+    assert func().as_convo().as_list() == [
+        {"role": "user", "content": "Hello"},
+        {"role": "assistant", "content": "World"},
+    ]
+
+
+def test_mix_role_usage():
+    @ppl
+    def func() -> PromptRecords:
+        with AIRole():
+            UserMessage("Hello")
+            AIMessage("World")
+            "Again"
+        return records()
+
+    assert func().as_convo().as_list() == [
+        {"role": "user", "content": "Hello"},
+        {"role": "assistant", "content": "WorldAgain"},
+    ]
+
+
+def test_multi_user():
+    @ppl
+    def func() -> PromptRecords:
+        with UserRole("A"):
+            "Hello"
+        with UserRole("B"):
+            "World"
+        return records()
+
+    assert func().as_convo().as_list() == [
+        {"role": "user", "name": "A", "content": "Hello"},
+        {"role": "user", "name": "B", "content": "World"},
+    ]
+
+
+def test_role_change():
+    @ppl
+    def func() -> PromptRecords:
+        "Hello"
+        with AIRole():
+            "World"
+        return records()
+
+    assert func().as_convo().as_list() == [
+        {"role": "user", "content": "Hello"},
+        {"role": "assistant", "content": "World"},
+    ]
+
+
+def test_role_change_loop1():
+    @ppl
+    def func() -> PromptRecords:
+        for i in range(5):
+            "Hello"
+            with AIRole():
+                "World"
+        return records()
+
+    assert (
+        func().as_convo().as_list()
+        == [
+            {"role": "user", "content": "Hello"},
+            {"role": "assistant", "content": "World"},
+        ]
+        * 5
+    )
+
+
+def test_role_change_loop2():
+    @ppl
+    def func() -> PromptRecords:
+        for i in range(3):
+            "Hello"
+            AIMessage("World")
+        return records()
+
+    assert (
+        func().as_convo().as_list()
+        == [
+            {"role": "user", "content": "Hello"},
+            {"role": "assistant", "content": "World"},
+        ]
+        * 3
+    )
+
+
+def test_role_change_loop3():
+    @ppl
+    def func() -> PromptRecords:
+        "Hello"
+        for i in range(5):
+            with AIRole():
+                "Foo"
+            with UserRole():
+                "Bar"
+        return records()
+
+    expected = [{"role": "user", "content": "Hello"}]
+    for i in range(5):
+        expected.append({"role": "assistant", "content": "Foo"})
+        expected.append({"role": "user", "content": "Bar"})
+
+    assert func().as_convo().as_list() == expected
+
+
+def test_nested_role_error():
+    with pytest.raises(ValueError) as excinfo:
+
+        @ppl
+        def func() -> PromptRecords:
+            "Hello"
+            for i in range(5):
+                with UserRole():
+                    "Foo"
+                    with AIRole():
+                        "Bar"
+            return records()
+
+        func()
+
+    assert "Cannot start a new role" in str(excinfo.value)
```

### Comparing `applang-0.0.1a3/tests/test_openai.py` & `applang-0.0.1a4/tests/test_openai.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-"""Testing openai API calls
-
-NOTE: The tests could cost money if you have an openai key set.
-NOTE: Some tests might fail due to randomness in the API.
-You can skip these tests by setting the environment variable SKIP_MODEL_CALL_TESTS=1
-"""
-
-import os
-import sys
-
-import pytest
-from loguru import logger
-
-import appl
-from appl import AIRole, Generation, Image, UserRole, as_tool, gen, ppl
-from appl.const import NEWLINE
-
-
-@ppl
-def add():
-    "1+1="
-    return str(gen(max_tokens=2)).strip()
-
-
-appl.init()
-# NOTE: init here could influence other tests in other files.
-
-try:
-    add()
-    reason = None
-    openai_api_callable = True
-except Exception as e:
-    reason = str(e)
-    openai_api_callable = False
-
-skip_tests = os.environ.get("SKIP_LLM_CALL_TESTS") == "1"
-pytestmark = [
-    pytest.mark.skipif(skip_tests, reason="Skipped due to setting"),
-    pytest.mark.skipif(
-        not openai_api_callable,
-        reason=f"Error encountered when calling openai API: {reason}",
-    ),
-]
-
-
-# @pytest.mark.skipif(skip_tests, reason="Skipped due to setting")
-def test_openai():
-    assert add() == "2"
-
-
-def test_tool_call():
-    def special_number(x: int) -> int:
-        """A function to calculate the special number of an integer."""
-        return x**2 + 1
-
-    tools = [as_tool(special_number)]
-
-    @ppl
-    def func(x: int):
-        f"What's the special number of {x}?"
-        res = gen(tools=tools)
-        return [x.get_content() for x in res.run_tool_calls()]
-
-    assert func(5) == [special_number(5)]
-
-
-IMAGE_URL = "https://maproom.wpenginepowered.com/wp-content/uploads/OpenAI_Logo.svg_-500x123.png"
-
-
-def test_image():
-    @ppl
-    def query():
-        "Look, it's a commercial logo."
-        Image(IMAGE_URL)
-        "What's the text on the image? "
-        "Your output should be in the format: The text on the image is: ..."
-        return gen("gpt4-turbo", stop=NEWLINE)
-
-    assert "OpenAI" in str(query())
+"""Testing openai API calls
+
+NOTE: The tests could cost money if you have an openai key set.
+NOTE: Some tests might fail due to randomness in the API.
+You can skip these tests by setting the environment variable SKIP_MODEL_CALL_TESTS=1
+"""
+
+import os
+import sys
+
+import pytest
+from loguru import logger
+
+import appl
+from appl import AIRole, Generation, Image, UserRole, as_tool, gen, ppl
+from appl.const import NEWLINE
+
+
+@ppl
+def add():
+    "1+1="
+    return str(gen(max_tokens=2)).strip()
+
+
+appl.init()
+# NOTE: init here could influence other tests in other files.
+
+try:
+    add()
+    reason = None
+    openai_api_callable = True
+except Exception as e:
+    reason = str(e)
+    openai_api_callable = False
+
+skip_tests = os.environ.get("SKIP_LLM_CALL_TESTS") == "1"
+pytestmark = [
+    pytest.mark.skipif(skip_tests, reason="Skipped due to setting"),
+    pytest.mark.skipif(
+        not openai_api_callable,
+        reason=f"Error encountered when calling openai API: {reason}",
+    ),
+]
+
+
+# @pytest.mark.skipif(skip_tests, reason="Skipped due to setting")
+def test_openai():
+    assert add() == "2"
+
+
+def test_tool_call():
+    def special_number(x: int) -> int:
+        """A function to calculate the special number of an integer."""
+        return x**2 + 1
+
+    tools = [as_tool(special_number)]
+
+    @ppl
+    def func(x: int):
+        f"What's the special number of {x}?"
+        res = gen(tools=tools)
+        return [x.get_content() for x in res.run_tool_calls()]
+
+    assert func(5) == [special_number(5)]
+
+
+IMAGE_URL = "https://maproom.wpenginepowered.com/wp-content/uploads/OpenAI_Logo.svg_-500x123.png"
+
+
+def test_image():
+    @ppl
+    def query():
+        "Look, it's a commercial logo."
+        Image(IMAGE_URL)
+        "What's the text on the image? "
+        "Your output should be in the format: The text on the image is: ..."
+        return gen("gpt4-turbo", stop=NEWLINE)
+
+    assert "OpenAI" in str(query())
```

### Comparing `applang-0.0.1a3/tests/test_prompt.py` & `applang-0.0.1a4/tests/test_prompt.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,237 +1,237 @@
-import pytest
-
-import appl
-from appl import Generation, convo, define, gen, need_ctx, ppl, records
-from appl.compositor import *
-
-
-def test_return():
-    @ppl
-    def func():
-        "Hello World"
-        return "answer"
-
-    assert func() == "answer"
-
-
-def test_prompt():
-    @ppl
-    def func(_ctx):
-        "Hello World"
-        return records()
-
-    assert str(func()) == "Hello World"
-
-
-def test_fstring():
-    @ppl
-    def f1():
-        f"a is {1!r}"
-        return records()
-
-    assert str(f1()) == f"a is {1!r}"
-
-    @ppl
-    def f2():
-        f"a is {3.1415:.2f}"
-        return records()
-
-    assert str(f2()) == f"a is {3.1415:.2f}"
-
-
-def test_prompts_change():
-    @ppl
-    def func():
-        "Hello"
-        ret1 = records()  # the reference
-        ret2 = records().copy()  # the copy of the current prompt
-        "World"
-        ret3 = records()
-        return ret1, ret2, ret3
-
-    ret1, ret2, ret3 = func()
-    assert str(ret1) == "Hello\nWorld"
-    assert str(ret2) == "Hello"
-    assert str(ret3) == "Hello\nWorld"
-
-
-def test_return_prompt():
-    @ppl(default_return="prompt")
-    def f1():
-        "Hello World"
-
-    assert str(f1()) == "Hello World"
-
-    @ppl(default_return="prompt")
-    def f2():
-        "Hello World"
-        return "answer"
-
-    # The return is unchanged.
-    assert str(f2()) == "answer"
-
-
-def test_record():
-    @ppl
-    def f2():
-        "Hello"
-        "World"
-        return records()
-
-    @ppl
-    def func():
-        with NumberedList():
-            "first line"
-            "second line"
-            f2()  # add the prompts from f2, following the current format.
-        return records()
-
-    assert str(func()) == f"1. first line\n2. second line\n3. Hello\n4. World"
-
-
-def test_inner_func():
-    @ppl
-    def func():
-        "Hello"
-
-        def func2():  # the inner function use the same context from the outer function.
-            "World"
-
-        func2()
-        return records()
-
-    assert str(func()) == "Hello\nWorld"
-
-
-def test_exclude_first_str():
-    @ppl(exclude_first_str=True)
-    def func():
-        "This is a docstring"
-        "Hello"
-        return records()
-
-    assert str(func()) == "Hello"
-
-
-def test_copy_ctx():
-    @ppl(ctx="copy")
-    def addon():
-        "World"
-        return str(convo())
-
-    @ppl
-    def func2():
-        "Hello"
-        first = addon()
-        second = addon()
-        return first, second, records()
-
-    first, second, origin = func2()
-    assert first == "Hello\nWorld"
-    assert second == "Hello\nWorld"
-    assert str(origin) == "Hello"
-
-
-def test_resume_ctx():
-    @ppl(ctx="resume")
-    def resume_ctx():
-        "Hello"
-        return convo()
-
-    target = []
-    for i in range(3):
-        res = resume_ctx()
-        target += ["Hello"]
-        assert str(res) == "\n".join(target)
-
-
-def test_class_resume_ctx():
-    class A:
-        @ppl(ctx="resume")
-        def append(self, msg: str):
-            msg
-            return convo()
-
-        @classmethod
-        @ppl(ctx="resume")
-        def append_cls(cls, msg: str):
-            msg
-            return convo()
-
-    a = A()
-    b = A()
-    target_a = []
-    target_b = []
-    target_cls = []
-    for i in range(3):
-        res = a.append("Hello")
-        target_a += ["Hello"]
-        assert str(res) == "\n".join(target_a)
-        res = b.append("World")
-        target_b += ["World"]
-        assert str(res) == "\n".join(target_b)
-        res = A.append_cls("Class")
-        target_cls += ["Class"]
-        assert str(res) == "\n".join(target_cls)
-
-
-def test_class_func():
-    class ComplexPrompt:
-        def __init__(self, condition: str):
-            self._condition = condition
-
-        @ppl(ctx="same")
-        def sub1(self):
-            if self._condition:
-                "sub1, condition is true"
-            else:
-                "sub1, condition is false"
-
-        @ppl(ctx="same")
-        def sub2(self):
-            if self._condition:
-                "sub2, condition is true"
-            else:
-                "sub2, condition is false"
-
-        @ppl
-        def func(self):
-            self.sub1()
-            self.sub2()
-            return records()
-
-    prompt1 = ComplexPrompt(False).func()
-    prompt2 = ComplexPrompt(True).func()
-    assert str(prompt1) == "sub1, condition is false\nsub2, condition is false"
-    assert str(prompt2) == "sub1, condition is true\nsub2, condition is true"
-
-
-def test_generation_message():
-    appl.init()
-
-    @ppl
-    def func():
-        "Hello World"
-        gen1 = gen(lazy_eval=True)
-        "Hi"
-        gen2 = gen(lazy_eval=True)
-        return gen1, gen2
-
-    gen1, gen2 = func()
-    assert str(gen1._args.messages) == "Hello World"
-    assert str(gen2._args.messages) == "Hello World\nHi"
-
-
-def test_generation_message2():
-    def fakegen():
-        return "24"
-
-    @ppl
-    def func():
-        f"Q: 1 + 2 = ?"
-        f"A: 3"
-        f"Q: 15 + 9 = ?"
-        f"A: {fakegen()}"
-        return convo()
-
-    assert str(func()) == "Q: 1 + 2 = ?\nA: 3\nQ: 15 + 9 = ?\nA: 24"
+import pytest
+
+import appl
+from appl import Generation, convo, define, gen, need_ctx, ppl, records
+from appl.compositor import *
+
+
+def test_return():
+    @ppl
+    def func():
+        "Hello World"
+        return "answer"
+
+    assert func() == "answer"
+
+
+def test_prompt():
+    @ppl
+    def func(_ctx):
+        "Hello World"
+        return records()
+
+    assert str(func()) == "Hello World"
+
+
+def test_fstring():
+    @ppl
+    def f1():
+        f"a is {1!r}"
+        return records()
+
+    assert str(f1()) == f"a is {1!r}"
+
+    @ppl
+    def f2():
+        f"a is {3.1415:.2f}"
+        return records()
+
+    assert str(f2()) == f"a is {3.1415:.2f}"
+
+
+def test_prompts_change():
+    @ppl
+    def func():
+        "Hello"
+        ret1 = records()  # the reference
+        ret2 = records().copy()  # the copy of the current prompt
+        "World"
+        ret3 = records()
+        return ret1, ret2, ret3
+
+    ret1, ret2, ret3 = func()
+    assert str(ret1) == "Hello\nWorld"
+    assert str(ret2) == "Hello"
+    assert str(ret3) == "Hello\nWorld"
+
+
+def test_return_prompt():
+    @ppl(default_return="prompt")
+    def f1():
+        "Hello World"
+
+    assert str(f1()) == "Hello World"
+
+    @ppl(default_return="prompt")
+    def f2():
+        "Hello World"
+        return "answer"
+
+    # The return is unchanged.
+    assert str(f2()) == "answer"
+
+
+def test_record():
+    @ppl
+    def f2():
+        "Hello"
+        "World"
+        return records()
+
+    @ppl
+    def func():
+        with NumberedList():
+            "first line"
+            "second line"
+            f2()  # add the prompts from f2, following the current format.
+        return records()
+
+    assert str(func()) == f"1. first line\n2. second line\n3. Hello\n4. World"
+
+
+def test_inner_func():
+    @ppl
+    def func():
+        "Hello"
+
+        def func2():  # the inner function use the same context from the outer function.
+            "World"
+
+        func2()
+        return records()
+
+    assert str(func()) == "Hello\nWorld"
+
+
+def test_exclude_first_str():
+    @ppl(exclude_first_str=True)
+    def func():
+        "This is a docstring"
+        "Hello"
+        return records()
+
+    assert str(func()) == "Hello"
+
+
+def test_copy_ctx():
+    @ppl(ctx="copy")
+    def addon():
+        "World"
+        return str(convo())
+
+    @ppl
+    def func2():
+        "Hello"
+        first = addon()
+        second = addon()
+        return first, second, records()
+
+    first, second, origin = func2()
+    assert first == "Hello\nWorld"
+    assert second == "Hello\nWorld"
+    assert str(origin) == "Hello"
+
+
+def test_resume_ctx():
+    @ppl(ctx="resume")
+    def resume_ctx():
+        "Hello"
+        return convo()
+
+    target = []
+    for i in range(3):
+        res = resume_ctx()
+        target += ["Hello"]
+        assert str(res) == "\n".join(target)
+
+
+def test_class_resume_ctx():
+    class A:
+        @ppl(ctx="resume")
+        def append(self, msg: str):
+            msg
+            return convo()
+
+        @classmethod
+        @ppl(ctx="resume")
+        def append_cls(cls, msg: str):
+            msg
+            return convo()
+
+    a = A()
+    b = A()
+    target_a = []
+    target_b = []
+    target_cls = []
+    for i in range(3):
+        res = a.append("Hello")
+        target_a += ["Hello"]
+        assert str(res) == "\n".join(target_a)
+        res = b.append("World")
+        target_b += ["World"]
+        assert str(res) == "\n".join(target_b)
+        res = A.append_cls("Class")
+        target_cls += ["Class"]
+        assert str(res) == "\n".join(target_cls)
+
+
+def test_class_func():
+    class ComplexPrompt:
+        def __init__(self, condition: str):
+            self._condition = condition
+
+        @ppl(ctx="same")
+        def sub1(self):
+            if self._condition:
+                "sub1, condition is true"
+            else:
+                "sub1, condition is false"
+
+        @ppl(ctx="same")
+        def sub2(self):
+            if self._condition:
+                "sub2, condition is true"
+            else:
+                "sub2, condition is false"
+
+        @ppl
+        def func(self):
+            self.sub1()
+            self.sub2()
+            return records()
+
+    prompt1 = ComplexPrompt(False).func()
+    prompt2 = ComplexPrompt(True).func()
+    assert str(prompt1) == "sub1, condition is false\nsub2, condition is false"
+    assert str(prompt2) == "sub1, condition is true\nsub2, condition is true"
+
+
+def test_generation_message():
+    appl.init()
+
+    @ppl
+    def func():
+        "Hello World"
+        gen1 = gen(lazy_eval=True)
+        "Hi"
+        gen2 = gen(lazy_eval=True)
+        return gen1, gen2
+
+    gen1, gen2 = func()
+    assert str(gen1._args.messages) == "Hello World"
+    assert str(gen2._args.messages) == "Hello World\nHi"
+
+
+def test_generation_message2():
+    def fakegen():
+        return "24"
+
+    @ppl
+    def func():
+        f"Q: 1 + 2 = ?"
+        f"A: 3"
+        f"Q: 15 + 9 = ?"
+        f"A: {fakegen()}"
+        return convo()
+
+    assert str(func()) == "Q: 1 + 2 = ?\nA: 3\nQ: 15 + 9 = ?\nA: 24"
```

### Comparing `applang-0.0.1a3/tests/test_stringfuture.py` & `applang-0.0.1a4/tests/test_stringfuture.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import time
-
-import appl
-from appl import CallFuture
-from appl import StringFuture as S
-
-
-def _check_str(s: S, target: str):
-    assert type(s) == S
-    assert str(s) == target
-
-
-def test_concat():
-    _check_str(S("ab") + S("cd"), "abcd")
-    _check_str(S("AP") + "PL", "APPL")
-    _check_str("AP" + S("PL"), "APPL")
-    s = ""
-    s += S("AP")
-    _check_str(s, "AP")
-    s += "PL"
-    _check_str(s, "APPL")
-    s += S("E")
-    _check_str(s, "APPLE")
-
-
-def test_cmp():
-    assert S("APPL") == "APPL"
-    assert "APPL" == S("APPL")
-    assert S("APPL") == S("APPL")
-
-    assert S("APPL") != "APPLE"
-    assert "APPL" != S("APPLE")
-    assert S("APPL") != S("APPLE")
-
-    assert "APPL" >= S("AAA")
-    assert S("APPL") >= S("AAA")
-    assert S("APPL") >= "AAA"
-    assert S("APPL") > "AAA"
-    assert S("APPL") <= "ZZZ"
-    assert S("APPL") < "ZZZ"
-
-
-def test_contains():
-    assert "AP" in S("APPL")
-    assert "AP" not in S("AAA")
-
-
-def test_getitem():
-    assert S("APPL")[1] == "P"
-    assert S("APPL")[1:] == "PPL"
-    assert S("A.P.P.L").split(".") == ["A", "P", "P", "L"]
-
-
-def test_format():
-    assert f"{S('A'):3}" == "A  "
-    assert appl.format(1.234, ".2f") == "1.23"
-    assert isinstance(appl.format(1.234, ".2f"), S)
-
-
-def test_as_key():
-    d = {}
-    d[S("APPL")] = 1
-    assert d[S("APPL")] == 1
-    assert d["APPL"] == 1
-
-
-def test_future():
-    def run(t):
-        time.sleep(t)
-        return "a"
-
-    t0 = time.time()
-    n = 3
-    s = ""
-    for i in range(n):
-        s += S(CallFuture(run, t=0.2))
-    assert time.time() - t0 < 0.15
-    assert str(s) == "a" * n
-    assert time.time() - t0 < 0.4
+import time
+
+import appl
+from appl import CallFuture
+from appl import StringFuture as S
+
+
+def _check_str(s: S, target: str):
+    assert type(s) == S
+    assert str(s) == target
+
+
+def test_concat():
+    _check_str(S("ab") + S("cd"), "abcd")
+    _check_str(S("AP") + "PL", "APPL")
+    _check_str("AP" + S("PL"), "APPL")
+    s = ""
+    s += S("AP")
+    _check_str(s, "AP")
+    s += "PL"
+    _check_str(s, "APPL")
+    s += S("E")
+    _check_str(s, "APPLE")
+
+
+def test_cmp():
+    assert S("APPL") == "APPL"
+    assert "APPL" == S("APPL")
+    assert S("APPL") == S("APPL")
+
+    assert S("APPL") != "APPLE"
+    assert "APPL" != S("APPLE")
+    assert S("APPL") != S("APPLE")
+
+    assert "APPL" >= S("AAA")
+    assert S("APPL") >= S("AAA")
+    assert S("APPL") >= "AAA"
+    assert S("APPL") > "AAA"
+    assert S("APPL") <= "ZZZ"
+    assert S("APPL") < "ZZZ"
+
+
+def test_contains():
+    assert "AP" in S("APPL")
+    assert "AP" not in S("AAA")
+
+
+def test_getitem():
+    assert S("APPL")[1] == "P"
+    assert S("APPL")[1:] == "PPL"
+    assert S("A.P.P.L").split(".") == ["A", "P", "P", "L"]
+
+
+def test_format():
+    assert f"{S('A'):3}" == "A  "
+    assert appl.format(1.234, ".2f") == "1.23"
+    assert isinstance(appl.format(1.234, ".2f"), S)
+
+
+def test_as_key():
+    d = {}
+    d[S("APPL")] = 1
+    assert d[S("APPL")] == 1
+    assert d["APPL"] == 1
+
+
+def test_future():
+    def run(t):
+        time.sleep(t)
+        return "a"
+
+    t0 = time.time()
+    n = 3
+    s = ""
+    for i in range(n):
+        s += S(CallFuture(run, t=0.2))
+    assert time.time() - t0 < 0.15
+    assert str(s) == "a" * n
+    assert time.time() - t0 < 0.4
```

### Comparing `applang-0.0.1a3/tests/test_tool.py` & `applang-0.0.1a4/tests/test_tool.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-import time
-from typing import Any
-
-from pydantic import BaseModel, Field, create_model
-
-import appl
-from appl import Generation, as_tool, gen, ppl
-from appl.core import CompletionResponse, ResponseType, ToolCall
-
-
-def removed_keyword(d: Any, key: str) -> Any:
-    if isinstance(d, list):
-        return [removed_keyword(x, key) for x in d]
-    if isinstance(d, dict):
-        return {k: removed_keyword(v, key) for k, v in d.items() if k != key}
-    return d
-
-
-def get_openai_schema(include_desc=True, add_default=False):
-    args_schema = {
-        "type": "object",
-        "properties": {
-            "x": {"type": "integer"},
-            "y": {"type": "integer"},
-        },
-        "required": ["x", "y"],
-    }
-    if include_desc:
-        args_schema["properties"]["x"]["description"] = "first number"
-        args_schema["properties"]["y"]["description"] = "second number"
-    if add_default:
-        args_schema["properties"]["y"]["default"] = 1
-        args_schema["required"].remove("y")
-    schema = {
-        "type": "function",
-        "function": {
-            "name": "add",
-            "description": "Add two numbers together",
-            "parameters": args_schema,
-        },
-    }
-    return schema
-
-
-def test_as_tool():
-    def add(x: int, y: int) -> int:
-        """Add two numbers together
-
-        Args:
-            x (int): first number
-            y (int): second number
-        Returns:
-            int: sum of x and y
-        Raises:
-            ValueError: if x or y is not an integer
-        """
-        if not isinstance(x, int) or not isinstance(y, int):
-            raise ValueError("x and y must be integers")
-        return x + y
-
-    tool = as_tool(add)
-    assert tool(1, 2) == 3
-    assert tool.__doc__ == add.__doc__
-    assert removed_keyword(tool.openai_schema, "title") == get_openai_schema()
-    assert removed_keyword(tool.returns.model_json_schema(), "title") == {
-        "properties": {
-            "returns": {"type": "integer", "description": "sum of x and y"},
-        },
-        "type": "object",
-        "required": ["returns"],
-    }
-    assert tool.raises == [
-        {"type": "ValueError", "desc": "if x or y is not an integer"}
-    ]
-
-    def add(x, y=1):
-        """Add two numbers together
-
-        Args:
-            x (int): first number
-            y (int): second number
-        """
-
-    tool = as_tool(add)
-    assert removed_keyword(tool.openai_schema, "title") == get_openai_schema(
-        add_default=True
-    )
-
-    def add(x: int, y: int):
-        """Add two numbers together"""
-
-    tool = as_tool(add)
-    assert removed_keyword(tool.openai_schema, "title") == get_openai_schema(
-        include_desc=False
-    )
-
-
-class AddArgs(BaseModel):
-    x: int = Field(..., description="first number")
-    y: int = Field(1, description="second number")
-
-
-def test_args_schema():
-    def add(args: AddArgs):
-        """Add two numbers together"""
-        return args.x + args.y
-
-    tool = as_tool(add)
-    params = {}
-    params["args"] = (AddArgs, ...)
-    assert (
-        tool.params.model_json_schema()
-        == create_model("parameters", **params).model_json_schema()
-    )
-
-    def add(args: AddArgs = AddArgs(x=1, y=2)):
-        """Add two numbers together
-
-        Args:
-            args (AddArgs): arguments
-        """
-        return args.x + args.y
-
-    tool = as_tool(add)
-    params = {}
-    params["args"] = (AddArgs, Field(AddArgs(x=1, y=2), description="arguments"))
-    assert (
-        tool.params.model_json_schema()
-        == create_model("parameters", **params).model_json_schema()
-    )
-
-
-def test_tool_call_sequential():
-    appl.init()
-    response = CompletionResponse(
-        tool_calls=[
-            ToolCall(id="1", name="add", args='{"x": 1, "y": 2, "t": 0.1}'),
-            ToolCall(id="2", name="mul", args='{"x": 2, "y": 3}'),
-            ToolCall(id="3", name="add", args='{"x": 3, "y": 4}'),
-            ToolCall(id="4", name="add", args='{"x": 5, "y": 6}'),
-        ],
-    )
-
-    call_args = []
-
-    def add(x: int, y: int, t: float = 0.0) -> int:
-        time.sleep(t)
-        call_args.append((x, y))
-        return x + y
-
-    tools = [as_tool(add)]
-
-    def filter_fn(tool_calls: list[ToolCall]) -> list[ToolCall]:
-        return [tc for tc in tool_calls if tc.name == "add"]
-
-    @ppl
-    def func():
-        res = gen("_dummy", tools=tools, mock_response=response)
-        return [x.get_content() for x in res.run_tool_calls(filter_fn=filter_fn)]
-
-    assert func() == [3, 7, 11]
-    assert call_args == [(1, 2), (3, 4), (5, 6)]
-
-
-def test_tool_call_parallel():
-    appl.init()
-    response = CompletionResponse(
-        tool_calls=[
-            ToolCall(id="1", name="add", args='{"x": 1, "y": 2}'),
-            ToolCall(id="3", name="add", args='{"x": 3, "y": 4}'),
-        ],
-    )
-
-    t = 0.2
-
-    def add(x: int, y: int) -> int:
-        time.sleep(t)
-        return x + y
-
-    tools = [as_tool(add)]
-
-    @ppl
-    def func():
-        res = gen(tools=tools, mock_response=response)
-        return [x.get_content() for x in res.run_tool_calls(parallel="thread")]
-
-    start_time = time.time()
-    assert func() == [3, 7]
-    assert time.time() - start_time < t + 0.1
+import time
+from typing import Any
+
+from pydantic import BaseModel, Field, create_model
+
+import appl
+from appl import Generation, as_tool, gen, ppl
+from appl.core import CompletionResponse, ResponseType, ToolCall
+
+
+def removed_keyword(d: Any, key: str) -> Any:
+    if isinstance(d, list):
+        return [removed_keyword(x, key) for x in d]
+    if isinstance(d, dict):
+        return {k: removed_keyword(v, key) for k, v in d.items() if k != key}
+    return d
+
+
+def get_openai_schema(include_desc=True, add_default=False):
+    args_schema = {
+        "type": "object",
+        "properties": {
+            "x": {"type": "integer"},
+            "y": {"type": "integer"},
+        },
+        "required": ["x", "y"],
+    }
+    if include_desc:
+        args_schema["properties"]["x"]["description"] = "first number"
+        args_schema["properties"]["y"]["description"] = "second number"
+    if add_default:
+        args_schema["properties"]["y"]["default"] = 1
+        args_schema["required"].remove("y")
+    schema = {
+        "type": "function",
+        "function": {
+            "name": "add",
+            "description": "Add two numbers together",
+            "parameters": args_schema,
+        },
+    }
+    return schema
+
+
+def test_as_tool():
+    def add(x: int, y: int) -> int:
+        """Add two numbers together
+
+        Args:
+            x (int): first number
+            y (int): second number
+        Returns:
+            int: sum of x and y
+        Raises:
+            ValueError: if x or y is not an integer
+        """
+        if not isinstance(x, int) or not isinstance(y, int):
+            raise ValueError("x and y must be integers")
+        return x + y
+
+    tool = as_tool(add)
+    assert tool(1, 2) == 3
+    assert tool.__doc__ == add.__doc__
+    assert removed_keyword(tool.openai_schema, "title") == get_openai_schema()
+    assert removed_keyword(tool.returns.model_json_schema(), "title") == {
+        "properties": {
+            "returns": {"type": "integer", "description": "sum of x and y"},
+        },
+        "type": "object",
+        "required": ["returns"],
+    }
+    assert tool.raises == [
+        {"type": "ValueError", "desc": "if x or y is not an integer"}
+    ]
+
+    def add(x, y=1):
+        """Add two numbers together
+
+        Args:
+            x (int): first number
+            y (int): second number
+        """
+
+    tool = as_tool(add)
+    assert removed_keyword(tool.openai_schema, "title") == get_openai_schema(
+        add_default=True
+    )
+
+    def add(x: int, y: int):
+        """Add two numbers together"""
+
+    tool = as_tool(add)
+    assert removed_keyword(tool.openai_schema, "title") == get_openai_schema(
+        include_desc=False
+    )
+
+
+class AddArgs(BaseModel):
+    x: int = Field(..., description="first number")
+    y: int = Field(1, description="second number")
+
+
+def test_args_schema():
+    def add(args: AddArgs):
+        """Add two numbers together"""
+        return args.x + args.y
+
+    tool = as_tool(add)
+    params = {}
+    params["args"] = (AddArgs, ...)
+    assert (
+        tool.params.model_json_schema()
+        == create_model("parameters", **params).model_json_schema()
+    )
+
+    def add(args: AddArgs = AddArgs(x=1, y=2)):
+        """Add two numbers together
+
+        Args:
+            args (AddArgs): arguments
+        """
+        return args.x + args.y
+
+    tool = as_tool(add)
+    params = {}
+    params["args"] = (AddArgs, Field(AddArgs(x=1, y=2), description="arguments"))
+    assert (
+        tool.params.model_json_schema()
+        == create_model("parameters", **params).model_json_schema()
+    )
+
+
+def test_tool_call_sequential():
+    appl.init()
+    response = CompletionResponse(
+        tool_calls=[
+            ToolCall(id="1", name="add", args='{"x": 1, "y": 2, "t": 0.1}'),
+            ToolCall(id="2", name="mul", args='{"x": 2, "y": 3}'),
+            ToolCall(id="3", name="add", args='{"x": 3, "y": 4}'),
+            ToolCall(id="4", name="add", args='{"x": 5, "y": 6}'),
+        ],
+    )
+
+    call_args = []
+
+    def add(x: int, y: int, t: float = 0.0) -> int:
+        time.sleep(t)
+        call_args.append((x, y))
+        return x + y
+
+    tools = [as_tool(add)]
+
+    def filter_fn(tool_calls: list[ToolCall]) -> list[ToolCall]:
+        return [tc for tc in tool_calls if tc.name == "add"]
+
+    @ppl
+    def func():
+        res = gen("_dummy", tools=tools, mock_response=response)
+        return [x.get_content() for x in res.run_tool_calls(filter_fn=filter_fn)]
+
+    assert func() == [3, 7, 11]
+    assert call_args == [(1, 2), (3, 4), (5, 6)]
+
+
+def test_tool_call_parallel():
+    appl.init()
+    response = CompletionResponse(
+        tool_calls=[
+            ToolCall(id="1", name="add", args='{"x": 1, "y": 2}'),
+            ToolCall(id="3", name="add", args='{"x": 3, "y": 4}'),
+        ],
+    )
+
+    t = 0.2
+
+    def add(x: int, y: int) -> int:
+        time.sleep(t)
+        return x + y
+
+    tools = [as_tool(add)]
+
+    @ppl
+    def func():
+        res = gen(tools=tools, mock_response=response)
+        return [x.get_content() for x in res.run_tool_calls(parallel="thread")]
+
+    start_time = time.time()
+    assert func() == [3, 7]
+    assert time.time() - start_time < t + 0.1
```

### Comparing `applang-0.0.1a3/PKG-INFO` & `applang-0.0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: applang
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A Prompt Programming Language
 Author-Email: Honghua Dong <dhh19951@gmail.com>, QiDong Su <soodoshll@gmail.com>, Jim Gao <ybgao@cs.toronto.edu>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -62,15 +62,15 @@
 <!-- TODO: RoadMap -->
 
 ## Quick Start
 
 ### Installation
 You can simply install APPL from PyPI using pip:
 ```bash
-pip install -U appl
+pip install -U applang
 ```
 More installation options can be found in the [installation guide](https://appl-team.github.io/appl/install).
 
 ### Setup
 You need to set up API keys or your own LLM backends to interact with LLMs.
 
 In this guide, we use OpenAI API as the default backend.
```

