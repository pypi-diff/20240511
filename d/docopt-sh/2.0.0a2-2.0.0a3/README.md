# Comparing `tmp/docopt_sh-2.0.0a2.tar.gz` & `tmp/docopt_sh-2.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docopt_sh-2.0.0a2.tar", max compression
+gzip compressed data, was "docopt_sh-2.0.0a3.tar", max compression
```

## Comparing `docopt_sh-2.0.0a2.tar` & `docopt_sh-2.0.0a3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1059 2024-05-10 10:16:59.772494 docopt_sh-2.0.0a2/LICENSE
--rw-r--r--   0        0        0      602 2024-05-10 10:16:59.772494 docopt_sh-2.0.0a2/docopt_sh/__init__.py
--rw-r--r--   0        0        0     3590 2024-05-10 10:16:59.772494 docopt_sh-2.0.0a2/docopt_sh/__main__.py
--rw-r--r--   0        0        0     4011 2024-05-10 10:16:59.772494 docopt_sh-2.0.0a2/docopt_sh/bash.py
--rw-r--r--   0        0        0    17437 2024-05-10 10:16:59.772494 docopt_sh-2.0.0a2/docopt_sh/docopt.sh
--rw-r--r--   0        0        0    10211 2024-05-10 10:16:59.772494 docopt_sh-2.0.0a2/docopt_sh/parser.py
--rw-r--r--   0        0        0     9063 2024-05-10 10:16:59.772494 docopt_sh-2.0.0a2/docopt_sh/script.py
--rw-r--r--   0        0        0      221 2024-05-10 10:16:59.772494 docopt_sh-2.0.0a2/docs/README.pypi.md
--rw-r--r--   0        0        0     1218 2024-05-10 10:17:10.332499 docopt_sh-2.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 docopt_sh-2.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/LICENSE
+-rw-r--r--   0        0        0      602 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/__init__.py
+-rw-r--r--   0        0        0     3590 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/__main__.py
+-rw-r--r--   0        0        0     4011 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/bash.py
+-rw-r--r--   0        0        0    17767 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/docopt.sh
+-rw-r--r--   0        0        0    10651 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/parser.py
+-rw-r--r--   0        0        0     9063 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/script.py
+-rw-r--r--   0        0        0      221 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docs/README.pypi.md
+-rw-r--r--   0        0        0     1218 2024-05-11 07:07:42.586063 docopt_sh-2.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 docopt_sh-2.0.0a3/PKG-INFO
```

### Comparing `docopt_sh-2.0.0a2/LICENSE` & `docopt_sh-2.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a2/docopt_sh/__init__.py` & `docopt_sh-2.0.0a3/docopt_sh/__init__.py`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a2/docopt_sh/__main__.py` & `docopt_sh-2.0.0a3/docopt_sh/__main__.py`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a2/docopt_sh/bash.py` & `docopt_sh-2.0.0a3/docopt_sh/bash.py`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a2/docopt_sh/docopt.sh` & `docopt_sh-2.0.0a3/docopt_sh/docopt.sh`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,22 @@
   digest="DOC DIGEST"
   # Options array. Each entry consists of:
   # * short name
   # * long name
   # * argcount (0 or 1)
   # The items are space separated. The order matches the AST node numbering
   options=("OPTIONS")
-  # This is the AST representing the parsed doc.
+  # This is the AST representing the parsed doc. The last node is the root.
+  # Options are first, as mentioned above. The comments above each node is
+  # shows what part of the DOC it is parsing (with line numbers).
+
   "NODES"
 
+  # Exit function that is callable from the parent shell. It outputs an
+  # optional error message and then prints the usage part of the doc
   # shellcheck disable=2016
   cat <<<' docopt_exit() {
   [[ -n $1 ]] && printf "%s\n" "$1" >&2
   printf "%s\n" ""DOC USAGE"" >&2
   exit 1
 }'
 
@@ -319,34 +324,34 @@
     done
   fi
   return 0
 }
 
 choice() {
   local initial_params=("${params[@]}") best_match_idx match_count node_idx
-  # Increase testdepth, so that we can test all subtrees without setting variables
+  # Increase testdepth so that we can test all subtrees without setting variables
   : $((testdepth++))
   # Determine the best subtree match
   for node_idx in "$@"; do
     if "node_$node_idx"; then
       # Subtree matches
       if [[ -z $match_count || ${#params[@]} -lt $match_count ]]; then
         # More params consumed than last iteration, best match so far
         best_match_idx=$node_idx
         match_count=${#params[@]}
       fi
     fi
     params=("${initial_params[@]}")
   done
+  # Done checking, decrease the testdepth again
+  : $((testdepth--))
   # Check if any subtree matched
   if [[ -n $best_match_idx ]]; then
-    # Decrease testdepth and let the best-matching subtree set the variables
-    if [[ $((--testdepth)) -eq 0 ]]; then
-      "node_$best_match_idx"
-    fi
+    # Let the best-matching subtree set the variables
+    [[ $testdepth -eq 0 ]] && "node_$best_match_idx"
     return 0
   fi
   # No subtree matched, reset the remaining params
   params=("${initial_params[@]}")
   return 1
 }
```

### Comparing `docopt_sh-2.0.0a2/docopt_sh/parser.py` & `docopt_sh-2.0.0a3/docopt_sh/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,17 @@
       ),
       '"DOC USAGE"': '${{DOC:{start}:{length}}}'.format(
         start=script.doc.trimmed_value_start + usage_start,
         length=usage_end - usage_start,
       ),
       '"DOC DIGEST"': hashlib.sha256(script.doc.untrimmed_value.encode('utf-8')).hexdigest()[0:5],
       '"OPTIONS"': generate_options_array(leaf_nodes),
-      '  "NODES"': indent('\n'.join(map(str, map(lambda n: ast_cmd(n, nodes), nodes))), level=1),
+      '  "NODES"': indent('\n'.join(
+        map(str, map(lambda n: ast_cmd(n, nodes, script.doc.trimmed_value), nodes))), level=1
+      ),
       '"VARNAMES"': ' '.join([bash_ifs_value(var_name(node)) for node in leaf_nodes]),
       '  "OUTPUT VARNAMES ASSIGNMENTS"': generate_default_assignments(leaf_nodes),
       '  "EARLY RETURN"\n': '' if leaf_nodes else '  return 0\n',
       '"ROOT NODE IDX"': len(nodes) - 1,
     }
     main = self.library.functions['docopt'].replace_literal(replacements)
     if self.parameters.minify:
@@ -216,27 +218,32 @@
     }[type(node)]  # type: ignore
   elif type(node) is P.Argument or type(node.default) not in [bool, int]:
     return 'value'
   else:
     return 'switch'
 
 
-def ast_cmd(node, sorted_nodes):
+def ast_cmd(node, sorted_nodes, doc):
   idx = sorted_nodes.index(node)
   if isinstance(node, P.Group):
+    if len(sorted_nodes) == 1 and isinstance(node, P.Sequence):
+      # noop program. Avoid a shellcheck error by calling `sequence` without params
+      return Code(f'# parsing is a no-op\nnode_{idx}(){{\n  return 0\n}}\n')
     args = ' '.join([str(sorted_nodes.index(item)) for item in node.items])
   else:
     args = var_name(node)
     if type(node) is P.Argument:
       args += ' ' + bash_ifs_value('a')
     else:
       args += ' ' + bash_ifs_value(idx if type(node) is P.Option else f'a:{node.ident}')
     if type(node.default) in [list, int]:
       args += ' true'
-  return Code(f'node_{idx}(){{\n  {helper_name(node)} {args}\n}}\n')
+  # Show where in the DOC the parsing node originates from
+  marked_source = '\n'.join(map(lambda line: f'# {line}', node.mark.show(doc).split('\n')))
+  return Code(f'{marked_source}\nnode_{idx}(){{\n  {helper_name(node)} {args}\n}}\n')
 
 
 def var_name(node):
   return bash_variable_name(
     node.definition.ident if isinstance(node, P.Option) else node.ident
   )
```

### Comparing `docopt_sh-2.0.0a2/docopt_sh/script.py` & `docopt_sh-2.0.0a3/docopt_sh/script.py`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a2/pyproject.toml` & `docopt_sh-2.0.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "docopt-sh"
 description = "Command-line argument parser for bash 3.2, 4+, and 5+."
-version = "2.0.0-alpha2"
+version = "2.0.0-alpha3"
 authors = ["Anders Ingemann <anders@ingemann.de>"]
 license = "MIT"
 readme = "docs/README.pypi.md"
 homepage = "https://github.com/andsens/docopt.sh"
 repository = "https://github.com/andsens/docopt.sh"
 classifiers = [
   "Topic :: Utilities",
```

### Comparing `docopt_sh-2.0.0a2/PKG-INFO` & `docopt_sh-2.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docopt-sh
-Version: 2.0.0a2
+Version: 2.0.0a3
 Summary: Command-line argument parser for bash 3.2, 4+, and 5+.
 Home-page: https://github.com/andsens/docopt.sh
 License: MIT
 Author: Anders Ingemann
 Author-email: anders@ingemann.de
 Requires-Python: >=3.11.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

