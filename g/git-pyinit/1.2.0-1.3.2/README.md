# Comparing `tmp/git_pyinit-1.2.0.tar.gz` & `tmp/git_pyinit-1.3.2.tar.gz`

## Comparing `git_pyinit-1.2.0.tar` & `git_pyinit-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/ruff.toml
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0    44936 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/_images/default_yaml.png
--rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/_images/directory_structure.png
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/src/git_pyinit/__about__.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/src/git_pyinit/__init__.py
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/src/git_pyinit/cli.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/src/git_pyinit/config.toml
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/src/git_pyinit/toml_reader.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/src/git_pyinit/utils.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/src/git_pyinit/exceptions/common.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/tests/unit_tests/test_directory_creation.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/README.md
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 git_pyinit-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/ruff.toml
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    44936 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/_images/default_yaml.png
+-rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/_images/directory_structure.png
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/src/git_pyinit/__about__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/src/git_pyinit/__init__.py
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/src/git_pyinit/cli.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/src/git_pyinit/config.toml
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/src/git_pyinit/toml_reader.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/src/git_pyinit/utils.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/src/git_pyinit/exceptions/common.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/tests/unit_tests/test_directory_creation.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/README.md
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 git_pyinit-1.3.2/PKG-INFO
```

### Comparing `git_pyinit-1.2.0/.github/workflows/lint.yml` & `git_pyinit-1.3.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `git_pyinit-1.2.0/.github/workflows/pytest.yml` & `git_pyinit-1.3.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `git_pyinit-1.2.0/_images/default_yaml.png` & `git_pyinit-1.3.2/_images/default_yaml.png`

 * *Files identical despite different names*

### Comparing `git_pyinit-1.2.0/_images/directory_structure.png` & `git_pyinit-1.3.2/_images/directory_structure.png`

 * *Files identical despite different names*

### Comparing `git_pyinit-1.2.0/src/git_pyinit/cli.py` & `git_pyinit-1.3.2/src/git_pyinit/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,18 @@
 import argparse
 import os
 import subprocess
 import sys
 from pathlib import Path
 
 from .exceptions.common import GitNotInstalled, HatchNotInstalled
-from .toml_reader import get_tool_list
+from .toml_reader import get_yaml_list
 from .utils import format_template
 
 
-def backup_template():
-    return """name: Linting Stage
-
-on: [push]
-
-jobs:
-  build:
-    runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python-version: ["3.8"]
-    steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
-      with:
-        python-version: ${{ matrix.python-version }}
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install isort black
-    - name: Analysing the code with isort
-      run: |
-        isort . --check-only --skip-gitignore
-    -name: Analysing the code with black
-      run: |
-      black . --check
-"""
-
-
 class PrintConfig(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
         print(Path(__file__).parent / "config.toml")
         sys.exit(0)
 
 
 class OpenConfig(argparse.Action):
@@ -72,51 +42,89 @@
     parser.add_argument(
         "-p", "--mkdir", help="Create all the parent directories if they don't exist", action="store_true"
     )
     # Assume that any other arg will be passed directly to git init
     return parser.parse_known_args(input)
 
 
-def main(_input=None):
+def test_dependencies():
     # Make sure that git is installed on the system
     if subprocess.run(["git", "--version"], stdout=subprocess.DEVNULL, check=False).returncode:
         raise GitNotInstalled("git is not installed on this system or is not along your path, cannot continue.")
         sys.exit(1)
     # we should never hit this, but just in case
     elif subprocess.run(["hatch", "--version"], stdout=subprocess.DEVNULL, check=False).returncode:
         raise HatchNotInstalled("hatch is not installed on this system or is not along your path, cannot continue.")
         sys.exit(1)
-    args, assumed_git_args = get_args(_input)
+
+
+def create_project_and_cd(args) -> int:
     if args.project_name:
         proj = Path(args.project_name).absolute()
         if args.mkdir:
             # Use the parent, and rely on hatch to create the project name directory
             proj.parent.mkdir(parents=True, exist_ok=True)
         os.chdir(proj.parent)
         x = subprocess.run(["hatch", "new", proj.name], stdout=subprocess.PIPE, check=False)
-        _str = x.stdout.decode("utf-8")
-        print(_str)
-        _created_dir = _str.split("\n")[0]
-        os.chdir(_created_dir)
+        if x.returncode:
+            # if it failed, it most likely wasn't empty
+            if proj.exists():
+                os.chdir(proj)
+            else:
+                print(x.stdout.decode("utf-8"))
+                return 1
+        else:
+            _str = x.stdout.decode("utf-8")
+            print(_str)
+            # Use this in case hatch changes what directory is output
+            _created_dir = _str.split("\n")[0]
+            os.chdir(_created_dir)
     # assume that they mean this directory
     else:
         current_dir = Path(os.getcwd()).absolute()
         os.chdir(current_dir.parent)
         subprocess.run(["hatch", "new", current_dir.name], check=False)
         os.chdir(current_dir.name)
+    return 0
+
+
+def write_workflow_yaml(path, tools):
+    path.write_text(format_template(tools))
+
+
+def get_workflow_file(name):
+    if not name.endswith(".yml"):
+        name += ".yml"
+    return Path(".github", "workflows", name)
+
+
+def main(_input=None, standalone=False):
+    here = os.getcwd()
+
+    args, assumed_git_args = get_args(_input)
+    if (result := create_project_and_cd(args)) != 0 and not standalone:
+        sys.exit(result)
     subprocess.run(["git", "init", *assumed_git_args], check=False)
-    workflows_file = Path(".github/workflows/lint.yml")
-    if not (parent := workflows_file.parent).exists():
-        parent.mkdir(parents=True, exist_ok=True)
+
     script_dir = Path(__file__).parent
     config = script_dir / "config.toml"
     if not config.exists():
-        print("Could not find config, defaulting to backup string")
-        workflow_string = backup_template()
+        print("Could not find config, no yamls will be generated")
+        if standalone:
+            return 1
+        else:
+            sys.exit(1)
     else:
-        workflow_string = format_template(get_tool_list(config))
-    workflows_file.write_text(workflow_string)
+        yamls = get_yaml_list(config)
+    for yaml in yamls:
+        workflows_file = get_workflow_file(name=yaml.name)
+        if not (parent := workflows_file.parent).exists():
+            parent.mkdir(parents=True, exist_ok=True)
+        write_workflow_yaml(workflows_file, yaml)
     print("Done.")
 
+    # in case it's not being ran as a subshell
+    os.chdir(here)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `git_pyinit-1.2.0/src/git_pyinit/toml_reader.py` & `git_pyinit-1.3.2/src/git_pyinit/toml_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import InitVar, dataclass, field
 
 import toml
 
 
 @dataclass
 class TomlResults:
+    name: str
     runs_on: list
     py_vers: list
     tools: list
 
 
 @dataclass
 class Tool:
@@ -29,27 +30,32 @@
 
 
 def read_toml(filepath):
     with open(filepath) as f:
         return toml.load(f)
 
 
-def get_tool_list(filepath):
+def get_yaml_list(filepath):
     _toml = read_toml(filepath)
     _py_vers = _toml.get("build", {}).get("python_version", ["3.8"])
-    _runs_on = _toml.get("build", {}).get("runs_on", ["ubuntu-latest"])
-    tools = _toml.get("tool", {})
-    active = tools.get("active", [])
-    default = tools.get("default", {})
-    _end = []
-    for tool in active:
-        tool_section = tools.get(tool, {})
-        _end.append(
-            Tool(
-                name=tool_section.get("name", tool),
-                command=tool_section.get("command", None),
-                flags=tool_section.get("flags", default.get("flags", [])),
-                file_command=tool_section.get("file_command", default.get("file_command", "$(git ls-files '*.py')")),
-                active=tool_section.get("active", True),
+    _runs_on = _toml.get("build", {}).get("runs_on", "ubuntu-latest")
+    yamls = _toml.get("yaml", {}).get("active", [])
+    for yaml in yamls:
+        tools = _toml.get(yaml, {})
+        active = tools.get("active", [])
+        default = tools.get("default", [{}])
+        default = {k: v for d in default for k, v in d.items()}
+        _end = []
+        for tool in active:
+            tool_section = tools.get(tool, {})
+            _end.append(
+                Tool(
+                    name=tool_section.get("name", tool),
+                    command=tool_section.get("command", None),
+                    flags=tool_section.get("flags", default.get("flags", [])),
+                    file_command=tool_section.get(
+                        "file_command", default.get("file_command", "$(git ls-files '*.py')")
+                    ),
+                    active=tool_section.get("active", True),
+                )
             )
-        )
-    return TomlResults(runs_on=_runs_on, py_vers=_py_vers, tools=_end)
+        yield TomlResults(name=yaml, runs_on=_runs_on, py_vers=_py_vers, tools=_end)
```

### Comparing `git_pyinit-1.2.0/src/git_pyinit/utils.py` & `git_pyinit-1.3.2/src/git_pyinit/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,34 +5,35 @@
     template = """
     name: Linting Stage
 
     on: [push]
 
     jobs:
         build:
-          runs-on: ubuntu-latest
+          runs-on: {runs_on}
           strategy:
             matrix:
               python-version: {py_vers}
           steps:
           - uses: actions/checkout@v3
           - name: Set Up Python ${{{{ matrix.python-version }}}}
             uses: actions/setup-python@v3
             with:
               python-version: ${{{{ matrix.python-version }}}}
           - name: Install Dependencies
             run: |
               python -m pip install --upgrade pip
               pip install {yaml_commands}
     """.format(
+        runs_on=results.runs_on,
         py_vers=str(results.py_vers),
         yaml_commands=" ".join([tool.yaml_command for tool in results.tools if tool.active]),
     )
     for tool in results.tools:
         if not tool.active:
             continue
         template += f"""
-              - name: Analyzing code with {tool.name}
-                run: |
-                  {tool}
+          - name: Analyzing code with {tool.name}
+            run: |
+              {tool}
         """
     return template
```

### Comparing `git_pyinit-1.2.0/tests/unit_tests/test_directory_creation.py` & `git_pyinit-1.3.2/tests/unit_tests/test_directory_creation.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "project1/.git/hooks/applypatch-msg.sample",
     "project1/.git/hooks/commit-msg.sample",
     "project1/.git/hooks/push-to-checkout.sample",
     "project1/.git/hooks/pre-commit.sample",
     "project1/.git/hooks/prepare-commit-msg.sample",
     "project1/.git/info/exclude",
     "project1/.github/workflows/lint.yml",
+    "project1/.github/workflows/tests.yml",
 ]
 
 
 @pytest.fixture(scope="function")
 def tempdir(tmp_path_factory):
     fn = tmp_path_factory.mktemp("tempdir") / "folder1" / proj_name
     yield fn
@@ -54,7 +55,9 @@
 def test_success(tempdir):
     main([str(tempdir), "--mkdir"])
     structure = get_file_structure(tempdir, relative_to=tempdir.parent)
     assert structure
     str_structure = [str(x) for x in structure]
     for file in expected_found_files:
         assert file in str_structure, f"{file} not found in {structure}"
+        str_structure.remove(file)
+    assert not str_structure, f"Temporary directory had unexpected files. Expected [], got {str_structure}"
```

### Comparing `git_pyinit-1.2.0/.gitignore` & `git_pyinit-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `git_pyinit-1.2.0/LICENSE.txt` & `git_pyinit-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git_pyinit-1.2.0/pyproject.toml` & `git_pyinit-1.3.2/pyproject.toml`

 * *Files identical despite different names*

