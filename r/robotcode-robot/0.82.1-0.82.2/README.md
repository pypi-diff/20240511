# Comparing `tmp/robotcode_robot-0.82.1.tar.gz` & `tmp/robotcode_robot-0.82.2.tar.gz`

## Comparing `robotcode_robot-0.82.1.tar` & `robotcode_robot-0.82.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    88642 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/__init__.py
--rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/document_cache_helper.py
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/entities.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/errors.py
--rw-r--r--   0        0        0    56251 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    97124 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/library_doc.py
--rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/model_helper.py
--rw-r--r--   0        0        0    89792 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/namespace.py
--rw-r--r--   0        0        0    50086 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/namespace_analyzer.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/workspace_config.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/__init__.py
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/ast.py
--rw-r--r--   0        0        0    11621 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/markdownformatter.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/match.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/robot_path.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/stubs.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/variables.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/visitor.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/LICENSE.txt
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/pyproject.toml
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    88642 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/__init__.py
+-rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/document_cache_helper.py
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/entities.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/errors.py
+-rw-r--r--   0        0        0    56251 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    97124 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    30232 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/model_helper.py
+-rw-r--r--   0        0        0    91315 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/namespace.py
+-rw-r--r--   0        0        0    50937 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/namespace_analyzer.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/workspace_config.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/__init__.py
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/ast.py
+-rw-r--r--   0        0        0    11621 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/markdownformatter.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/match.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/robot_path.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/stubs.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/variables.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/visitor.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/LICENSE.txt
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/pyproject.toml
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/PKG-INFO
```

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.82.2/src/robotcode/robot/config/loader.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/config/model.py` & `robotcode_robot-0.82.2/src/robotcode/robot/config/model.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.82.2/src/robotcode/robot/config/utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/document_cache_helper.py` & `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/document_cache_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/entities.py` & `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/errors.py` & `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/errors.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/imports_manager.py` & `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/imports_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/library_doc.py` & `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/library_doc.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/model_helper.py` & `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/model_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -254,26 +254,28 @@
     @staticmethod
     def iter_expression_variables_from_token(
         expression: Token,
         namespace: Namespace,
         nodes: Optional[List[ast.AST]],
         position: Optional[Position] = None,
         skip_commandline_variables: bool = False,
+        skip_local_variables: bool = False,
         return_not_found: bool = False,
     ) -> Iterator[Tuple[Token, VariableDefinition]]:
         variable_started = False
         try:
             for toknum, tokval, (_, tokcol), _, _ in generate_tokens(StringIO(expression.value).readline):
                 if variable_started:
                     if toknum == python_token.NAME:
                         var = namespace.find_variable(
                             f"${{{tokval}}}",
                             nodes,
                             position,
                             skip_commandline_variables=skip_commandline_variables,
+                            skip_local_variables=skip_local_variables,
                             ignore_error=True,
                         )
                         sub_token = Token(
                             expression.type,
                             tokval,
                             expression.lineno,
                             expression.col_offset + tokcol,
@@ -372,14 +374,15 @@
     def iter_variables_from_token(
         cls,
         token: Token,
         namespace: Namespace,
         nodes: Optional[List[ast.AST]],
         position: Optional[Position] = None,
         skip_commandline_variables: bool = False,
+        skip_local_variables: bool = False,
         return_not_found: bool = False,
     ) -> Iterator[Tuple[Token, VariableDefinition]]:
         def is_number(name: str) -> bool:
             if name.startswith("$"):
                 finder = NumberFinder()
                 return bool(finder.find(name) != NOT_FOUND)
             return False
@@ -401,14 +404,15 @@
                                 sub_token.col_offset + 3,
                                 sub_token.error,
                             ),
                             namespace,
                             nodes,
                             position,
                             skip_commandline_variables=skip_commandline_variables,
+                            skip_local_variables=skip_local_variables,
                             return_not_found=return_not_found,
                         ):
                             yield v
                     elif base == "" and return_not_found:
                         yield (
                             sub_token,
                             VariableNotFoundDefinition(
@@ -457,14 +461,15 @@
                 sub_token = token_or_var
                 name = sub_token.value
                 var = namespace.find_variable(
                     name,
                     nodes,
                     position,
                     skip_commandline_variables=skip_commandline_variables,
+                    skip_local_variables=skip_local_variables,
                     ignore_error=True,
                 )
                 if var is not None:
                     yield strip_variable_token(sub_token), var
                     continue
 
                 if is_number(sub_token.value):
@@ -481,14 +486,15 @@
                         base_name, _ = match.groups()
                         name = f"{name[0]}{{{base_name.strip()}}}"
                         var = namespace.find_variable(
                             name,
                             nodes,
                             position,
                             skip_commandline_variables=skip_commandline_variables,
+                            skip_local_variables=skip_local_variables,
                             ignore_error=True,
                         )
                         sub_sub_token = Token(
                             sub_token.type,
                             name,
                             sub_token.lineno,
                             sub_token.col_offset,
```

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/namespace.py` & `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,16 @@
     Union,
     cast,
 )
 
 from robot.errors import VariableError
 from robot.libraries import STDLIBS
 from robot.parsing.lexer.tokens import Token
-from robot.parsing.model.blocks import (
-    Keyword,
-    SettingSection,
-    TestCase,
-    VariableSection,
-)
-from robot.parsing.model.statements import Arguments, Statement
+from robot.parsing.model.blocks import Keyword, SettingSection, TestCase, VariableSection
+from robot.parsing.model.statements import Arguments, Fixture, Statement, Timeout
 from robot.parsing.model.statements import LibraryImport as RobotLibraryImport
 from robot.parsing.model.statements import ResourceImport as RobotResourceImport
 from robot.parsing.model.statements import (
     VariablesImport as RobotVariablesImport,
 )
 from robot.variables.search import (
     is_scalar_assign,
@@ -178,15 +173,15 @@
                     has_value=has_value,
                     resolvable=True,
                     value=value,
                 )
             )
 
 
-class BlockVariableVisitor(Visitor):
+class VariableVisitorBase(Visitor):
     def __init__(
         self,
         namespace: "Namespace",
         nodes: Optional[List[ast.AST]] = None,
         position: Optional[Position] = None,
         in_args: bool = True,
     ) -> None:
@@ -194,30 +189,104 @@
         self.namespace = namespace
         self.nodes = nodes
         self.position = position
         self.in_args = in_args
 
         self._results: Dict[str, VariableDefinition] = {}
         self.current_kw_doc: Optional[KeywordDoc] = None
+        self.current_kw: Optional[Keyword] = None
+
+    def get_variable_token(self, token: Token) -> Optional[Token]:
+        return next(
+            (
+                v
+                for v in itertools.dropwhile(
+                    lambda t: t.type in Token.NON_DATA_TOKENS,
+                    tokenize_variables(token, ignore_errors=True, extra_types={Token.VARIABLE}),
+                )
+                if v.type == Token.VARIABLE
+            ),
+            None,
+        )
+
+
+class ArgumentVisitor(VariableVisitorBase):
+    def __init__(
+        self,
+        namespace: "Namespace",
+        nodes: Optional[List[ast.AST]],
+        position: Optional[Position],
+        in_args: bool,
+        current_kw_doc: Optional[KeywordDoc],
+    ) -> None:
+        super().__init__(namespace, nodes, position, in_args)
+
+        self.current_kw_doc: Optional[KeywordDoc] = current_kw_doc
+
+    def get(self, model: ast.AST) -> Dict[str, VariableDefinition]:
+        self._results = {}
+
+        self.visit(model)
+
+        return self._results
+
+    def visit_Arguments(self, node: Statement) -> None:  # noqa: N802
+        args: List[str] = []
+
+        arguments = node.get_tokens(Token.ARGUMENT)
+
+        for argument_token in arguments:
+            try:
+                argument = self.get_variable_token(argument_token)
+
+                if argument is not None and argument.value != "@{}":
+                    if (
+                        self.in_args
+                        and self.position is not None
+                        and self.position in range_from_token(argument_token)
+                        and self.position > range_from_token(argument).end
+                    ):
+                        break
+
+                    if argument.value not in args:
+                        args.append(argument.value)
+                        arg_def = ArgumentDefinition(
+                            name=argument.value,
+                            name_token=strip_variable_token(argument),
+                            line_no=argument.lineno,
+                            col_offset=argument.col_offset,
+                            end_line_no=argument.lineno,
+                            end_col_offset=argument.end_col_offset,
+                            source=self.namespace.source,
+                            keyword_doc=self.current_kw_doc,
+                        )
+                        self._results[argument.value] = arg_def
+
+            except VariableError:
+                pass
 
+
+class OnlyArgumentsVisitor(VariableVisitorBase):
     def get(self, model: ast.AST) -> List[VariableDefinition]:
         self._results = {}
 
         self.visit(model)
 
         return list(self._results.values())
 
     def visit(self, node: ast.AST) -> None:
         if self.position is None or self.position >= range_from_node(node).start:
             super().visit(node)
 
     def visit_Keyword(self, node: ast.AST) -> None:  # noqa: N802
+        self.current_kw = cast(Keyword, node)
         try:
             self.generic_visit(node)
         finally:
+            self.current_kw = None
             self.current_kw_doc = None
 
     def visit_KeywordName(self, node: Statement) -> None:  # noqa: N802
         from .model_helper import ModelHelper
 
         name_token = node.get_token(Token.KEYWORD_NAME)
 
@@ -244,61 +313,23 @@
                         col_offset=variable_token.col_offset,
                         end_line_no=variable_token.lineno,
                         end_col_offset=variable_token.end_col_offset,
                         source=self.namespace.source,
                         keyword_doc=self.current_kw_doc,
                     )
 
-    def get_variable_token(self, token: Token) -> Optional[Token]:
-        return next(
-            (
-                v
-                for v in itertools.dropwhile(
-                    lambda t: t.type in Token.NON_DATA_TOKENS,
-                    tokenize_variables(token, ignore_errors=True, extra_types={Token.VARIABLE}),
-                )
-                if v.type == Token.VARIABLE
-            ),
-            None,
-        )
-
-    def visit_Arguments(self, node: Statement) -> None:  # noqa: N802
-        args: List[str] = []
+            if self.current_kw is not None:
+                args = ArgumentVisitor(
+                    self.namespace, self.nodes, self.position, self.in_args, self.current_kw_doc
+                ).get(self.current_kw)
+                if args:
+                    self._results.update(args)
 
-        arguments = node.get_tokens(Token.ARGUMENT)
 
-        for argument_token in arguments:
-            try:
-                argument = self.get_variable_token(argument_token)
-
-                if argument is not None and argument.value != "@{}":
-                    if (
-                        self.in_args
-                        and self.position is not None
-                        and self.position in range_from_token(argument_token)
-                        and self.position > range_from_token(argument).end
-                    ):
-                        break
-
-                    if argument.value not in args:
-                        args.append(argument.value)
-                        arg_def = ArgumentDefinition(
-                            name=argument.value,
-                            name_token=strip_variable_token(argument),
-                            line_no=argument.lineno,
-                            col_offset=argument.col_offset,
-                            end_line_no=argument.lineno,
-                            end_col_offset=argument.end_col_offset,
-                            source=self.namespace.source,
-                            keyword_doc=self.current_kw_doc,
-                        )
-                        self._results[argument.value] = arg_def
-
-            except VariableError:
-                pass
+class BlockVariableVisitor(OnlyArgumentsVisitor):
 
     def visit_ExceptHeader(self, node: Statement) -> None:  # noqa: N802
         variables = node.get_tokens(Token.VARIABLE)[:1]
         if variables and is_scalar_assign(variables[0].value):
             try:
                 variable = self.get_variable_token(variables[0])
 
@@ -986,40 +1017,47 @@
             return self._global_variables
 
     def yield_variables(
         self,
         nodes: Optional[List[ast.AST]] = None,
         position: Optional[Position] = None,
         skip_commandline_variables: bool = False,
+        skip_local_variables: bool = False,
     ) -> Iterator[Tuple[VariableMatcher, VariableDefinition]]:
         yielded: Dict[VariableMatcher, VariableDefinition] = {}
 
         test_or_keyword = None
+        test_or_keyword_nodes = None
 
         if nodes:
             test_or_keyword_nodes = list(
                 itertools.dropwhile(
                     lambda v: not isinstance(v, (TestCase, Keyword)),
                     nodes if nodes else [],
                 )
             )
             test_or_keyword = test_or_keyword_nodes[0] if test_or_keyword_nodes else None
 
+        in_args = isinstance(test_or_keyword_nodes[-1], Arguments) if test_or_keyword_nodes else False
+        only_args = (
+            isinstance(test_or_keyword_nodes[-1], (Arguments, Fixture, Timeout)) if test_or_keyword_nodes else False
+        )
+
         for var in chain(
             *[
                 (
                     (
-                        BlockVariableVisitor(
+                        (OnlyArgumentsVisitor if only_args else BlockVariableVisitor)(
                             self,
                             nodes,
                             position,
-                            isinstance(test_or_keyword_nodes[-1], Arguments) if nodes else False,
+                            in_args,
                         ).get(test_or_keyword)
                     )
-                    if test_or_keyword is not None
+                    if test_or_keyword is not None and not skip_local_variables
                     else []
                 )
             ],
             self.get_global_variables(),
         ):
             if var.matcher not in yielded:
                 if skip_commandline_variables and isinstance(var, CommandLineVariableDefinition):
@@ -1077,14 +1115,15 @@
     @_logger.call
     def find_variable(
         self,
         name: str,
         nodes: Optional[List[ast.AST]] = None,
         position: Optional[Position] = None,
         skip_commandline_variables: bool = False,
+        skip_local_variables: bool = False,
         ignore_error: bool = False,
     ) -> Optional[VariableDefinition]:
         self.ensure_initialized()
 
         if name[:2] == "%{" and name[-1] == "}":
             var_name, _, default_value = name[2:-1].partition("=")
             return EnvironmentVariableDefinition(
@@ -1101,14 +1140,15 @@
         try:
             matcher = VariableMatcher(name)
 
             for m, v in self.yield_variables(
                 nodes,
                 position,
                 skip_commandline_variables=skip_commandline_variables,
+                skip_local_variables=skip_local_variables,
             ):
                 if matcher == m:
                     return v
         except InvalidVariableError:
             if not ignore_error:
                 raise
```

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/namespace_analyzer.py` & `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/namespace_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Type, Union
 
 import robot.parsing.model.statements
 from robot.parsing.lexer.tokens import Token
 from robot.parsing.model.blocks import Keyword, TestCase
 from robot.parsing.model.statements import (
     Arguments,
+    DefaultTags,
     DocumentationOrMetadata,
     Fixture,
     KeywordCall,
     LibraryImport,
     ResourceImport,
     Statement,
+    Tags,
     Template,
     TemplateArguments,
     TestCaseName,
     TestTemplate,
     Variable,
     VariablesImport,
 )
@@ -66,17 +68,43 @@
     is_embedded_keyword,
 )
 from .model_helper import ModelHelper
 from .namespace import KeywordFinder, Namespace
 
 if get_robot_version() < (7, 0):
     from robot.variables.search import VariableIterator
+
+    VARIABLE_NOT_FOUND_HINT_TYPES: Tuple[Any, ...] = (
+        DocumentationOrMetadata,
+        TestCaseName,
+        Tags,
+        robot.parsing.model.statements.ForceTags,
+        DefaultTags,
+    )
+
+    IN_SETTING_TYPES: Tuple[Any, ...] = (
+        DocumentationOrMetadata,
+        Tags,
+        robot.parsing.model.statements.ForceTags,
+        DefaultTags,
+        Template,
+    )
 else:
     from robot.variables.search import VariableMatches
 
+    VARIABLE_NOT_FOUND_HINT_TYPES = (
+        DocumentationOrMetadata,
+        TestCaseName,
+        Tags,
+        robot.parsing.model.statements.TestTags,
+        DefaultTags,
+    )
+
+    IN_SETTING_TYPES = (DocumentationOrMetadata, Tags, robot.parsing.model.statements.TestTags, DefaultTags, Template)
+
 
 @dataclass
 class AnalyzerResult:
     diagnostics: List[Diagnostic]
     keyword_references: Dict[KeywordDoc, Set[Location]]
     variable_references: Dict[VariableDefinition, Set[Location]]
     local_variable_assignments: Dict[VariableDefinition, Set[Range]]
@@ -262,18 +290,18 @@
         variable_statements = (Variable, robot.parsing.model.statements.Var)
 
     def visit(self, node: ast.AST) -> None:
         check_current_task_canceled()
 
         self.node_stack.append(node)
         try:
+            in_setting = isinstance(node, IN_SETTING_TYPES)
+
             severity = (
-                DiagnosticSeverity.HINT
-                if isinstance(node, (DocumentationOrMetadata, TestCaseName))
-                else DiagnosticSeverity.ERROR
+                DiagnosticSeverity.HINT if isinstance(node, VARIABLE_NOT_FOUND_HINT_TYPES) else DiagnosticSeverity.ERROR
             )
 
             if isinstance(node, KeywordCall) and node.keyword:
                 kw_doc = self.finder.find_keyword(node.keyword, raise_keyword_error=False)
                 if kw_doc is not None and kw_doc.longname == "BuiltIn.Comment":
                     severity = DiagnosticSeverity.HINT
 
@@ -291,14 +319,15 @@
 
                         for var_token, var in self.iter_variables_from_token(
                             token,
                             self.namespace,
                             self.node_stack,
                             range_from_token(token).start,
                             skip_commandline_variables=False,
+                            skip_local_variables=in_setting,
                             return_not_found=True,
                         ):
                             if isinstance(var, VariableNotFoundDefinition):
                                 self.append_diagnostics(
                                     range=range_from_token(var_token),
                                     message=f"Variable '{var.name}' not found.",
                                     severity=severity,
@@ -376,14 +405,15 @@
             ):
                 for var_token, var in self.iter_expression_variables_from_token(
                     token,
                     self.namespace,
                     self.node_stack,
                     range_from_token(token).start,
                     skip_commandline_variables=False,
+                    skip_local_variables=in_setting,
                     return_not_found=True,
                 ):
                     if isinstance(var, VariableNotFoundDefinition):
                         self.append_diagnostics(
                             range=range_from_token(var_token),
                             message=f"Variable '{var.name}' not found.",
                             severity=DiagnosticSeverity.ERROR,
```

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/workspace_config.py` & `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/workspace_config.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/utils/ast.py` & `robotcode_robot-0.82.2/src/robotcode/robot/utils/ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/utils/markdownformatter.py` & `robotcode_robot-0.82.2/src/robotcode/robot/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/utils/match.py` & `robotcode_robot-0.82.2/src/robotcode/robot/utils/match.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/utils/robot_path.py` & `robotcode_robot-0.82.2/src/robotcode/robot/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/utils/stubs.py` & `robotcode_robot-0.82.2/src/robotcode/robot/utils/stubs.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/utils/variables.py` & `robotcode_robot-0.82.2/src/robotcode/robot/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/src/robotcode/robot/utils/visitor.py` & `robotcode_robot-0.82.2/src/robotcode/robot/utils/visitor.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/.gitignore` & `robotcode_robot-0.82.2/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/LICENSE.txt` & `robotcode_robot-0.82.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/README.md` & `robotcode_robot-0.82.2/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.1/pyproject.toml` & `robotcode_robot-0.82.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
   "platformdirs>=3.2.0,<4.2.0",
-  "robotcode-core==0.82.1",
+  "robotcode-core==0.82.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://opencollective.com/robotcode"
 Documentation = "https://github.com/robotcodedev/robotcode#readme"
```

### Comparing `robotcode_robot-0.82.1/PKG-INFO` & `robotcode_robot-0.82.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-robot
-Version: 0.82.1
+Version: 0.82.2
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: platformdirs<4.2.0,>=3.2.0
-Requires-Dist: robotcode-core==0.82.1
+Requires-Dist: robotcode-core==0.82.2
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```

