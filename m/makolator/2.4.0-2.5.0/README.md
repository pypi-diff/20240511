# Comparing `tmp/makolator-2.4.0.tar.gz` & `tmp/makolator-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makolator-2.4.0.tar", max compression
+gzip compressed data, was "makolator-2.5.0.tar", max compression
```

## Comparing `makolator-2.4.0.tar` & `makolator-2.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2024-01-22 20:27:32.946080 makolator-2.4.0/LICENSE
--rw-r--r--   0        0        0     1210 2024-01-22 20:27:32.946080 makolator-2.4.0/README.md
--rw-r--r--   0        0        0     5563 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/__init__.py
--rw-r--r--   0        0        0     1182 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/__main__.py
--rw-r--r--   0        0        0     8731 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/_inplace.py
--rw-r--r--   0        0        0     5017 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/_staticcode.py
--rw-r--r--   0        0        0     2031 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/_util.py
--rw-r--r--   0        0        0     4384 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/cli.py
--rw-r--r--   0        0        0     3039 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/config.py
--rw-r--r--   0        0        0     2004 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/datamodel.py
--rw-r--r--   0        0        0     2006 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/escape.py
--rw-r--r--   0        0        0     1215 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/exceptions.py
--rw-r--r--   0        0        0     2519 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/helper.py
--rw-r--r--   0        0        0     1902 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/info.py
--rw-r--r--   0        0        0    10192 2024-01-22 20:27:32.946080 makolator-2.4.0/makolator/makolator.py
--rw-r--r--   0        0        0     2434 2024-01-22 20:27:32.946080 makolator-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 makolator-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-11 17:22:18.766346 makolator-2.5.0/LICENSE
+-rw-r--r--   0        0        0     1210 2024-05-11 17:22:18.766346 makolator-2.5.0/README.md
+-rw-r--r--   0        0        0     5563 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/__init__.py
+-rw-r--r--   0        0        0     1182 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/__main__.py
+-rw-r--r--   0        0        0     9425 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/_inplace.py
+-rw-r--r--   0        0        0     5451 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/_staticcode.py
+-rw-r--r--   0        0        0     2283 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/_util.py
+-rw-r--r--   0        0        0     4960 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/cli.py
+-rw-r--r--   0        0        0     3167 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/config.py
+-rw-r--r--   0        0        0     2004 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/datamodel.py
+-rw-r--r--   0        0        0     2006 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/escape.py
+-rw-r--r--   0        0        0     1215 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/exceptions.py
+-rw-r--r--   0        0        0     2519 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/helper.py
+-rw-r--r--   0        0        0     1902 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/info.py
+-rw-r--r--   0        0        0    10229 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/makolator.py
+-rw-r--r--   0        0        0     2434 2024-05-11 17:22:18.766346 makolator-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 makolator-2.5.0/PKG-INFO
```

### Comparing `makolator-2.4.0/LICENSE` & `makolator-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `makolator-2.4.0/README.md` & `makolator-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `makolator-2.4.0/makolator/__init__.py` & `makolator-2.5.0/makolator/__init__.py`

 * *Files identical despite different names*

### Comparing `makolator-2.4.0/makolator/__main__.py` & `makolator-2.5.0/makolator/__main__.py`

 * *Files identical despite different names*

### Comparing `makolator-2.4.0/makolator/_inplace.py` & `makolator-2.5.0/makolator/_inplace.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 from aligntext import Align
 from attrs import define, field
 from mako.exceptions import text_error_template
 from mako.lookup import TemplateLookup
 from mako.runtime import Context
 from mako.template import Template
 
-from ._util import LOGGER, check_indent
+from ._util import LOGGER, check_indent, fill_marker
+from .config import Config
 from .exceptions import MakolatorError
 
 # pylint: disable=too-many-arguments,too-few-public-methods
 
 
 @define
 class InplaceInfo:
@@ -64,30 +65,29 @@
 
 
 @define
 class InplaceRenderer:
 
     """Inplace Renderer."""
 
-    template_marker: str
-    inplace_marker: str
+    config: Config
     templates: Tuple[Template, ...]
     ignore_unknown: bool
     eol: str
 
     def render(self, lookup: TemplateLookup, filepath: Path, outputfile, context: dict):  # noqa: C901
         """Render."""
         # pylint: disable=too-many-locals,too-many-nested-blocks
-        inplace_marker = self.inplace_marker
-        ibegin = re.compile(rf"(?P<indent>\s*).*{inplace_marker}\s+BEGIN\s(?P<funcname>[a-z_]+)\((?P<args>.*)\).*")
+        inplace_marker = self.config.inplace_marker
+        ibegin = re.compile(rf"(?P<indent>\s*).*{inplace_marker}\s+BEGIN\s(?P<funcname>[a-z_]+)\((?P<args>.*)\)")
         iinfo = None
 
-        template_marker = self.template_marker
+        template_marker = self.config.template_marker
         tinfo = None
-        tbegin = re.compile(rf"(?P<pre>.*)\s*{template_marker}\s+BEGIN.*")
+        tbegin = re.compile(rf"(?P<pre>.*)\s*{template_marker}\s+BEGIN")
         templates = list(self.templates)
 
         with open(filepath, encoding="utf-8") as inputfile:
             inputiter = enumerate(inputfile.readlines(), 1)
             try:
                 while True:
                     if iinfo:
@@ -100,29 +100,31 @@
                         self._process_template(filepath, lookup, outputfile, templates, inputiter, tinfo, tbegin)
                         tinfo = None
 
                     else:
                         # normal lines
                         while True:
                             lineno, line = next(inputiter)
-                            outputfile.write(line)
                             if inplace_marker:
                                 # search for "INPLACE BEGIN <funcname>(<args>)"
                                 beginmatch = ibegin.match(line)
                                 if beginmatch:
+                                    outputfile.write(self._fill_marker(beginmatch))
                                     # consume INPLACE BEGIN
                                     iinfo = self._start_inplace(templates, filepath, lineno, **beginmatch.groupdict())
                                     break
                             if template_marker:
                                 # search for "TEMPLATE BEGIN"
                                 beginmatch = tbegin.match(line)
                                 if beginmatch:
+                                    outputfile.write(self._fill_marker(beginmatch))
                                     # consume TEMPLATE BEGIN
                                     tinfo = TplInfo(lineno, beginmatch.group("pre"))
                                     break
+                            outputfile.write(line)
 
             except StopIteration:
                 pass
         if iinfo:
             raise MakolatorError(f"'{filepath!s}:{iinfo.lineno}' BEGIN {iinfo.funcname}({iinfo.args}) without END.")
         if tinfo:
             raise MakolatorError(f"'{filepath!s}:{tinfo.lineno}' BEGIN without END.")
@@ -138,55 +140,58 @@
                 raise MakolatorError(msg)
 
             endmatch = iinfo.end.match(line)
             if endmatch:
                 # fill
                 self._fill_inplace(filepath, outputfile, iinfo, context)
                 # propagate INPLACE END tag
-                outputfile.write(line)
+                outputfile.write(self._fill_marker(endmatch))
                 check_indent(filepath, lineno, iinfo.indent, endmatch.group("indent"))
                 # consume INPLACE END
                 break
 
     def _process_template(
         self, filepath: Path, lookup: TemplateLookup, outputfile, templates, inputiter, tinfo, tbegin
     ):
         # capture TEMPLATE
         pre = tinfo.pre
         prelen = len(pre)
-        tend = re.compile(rf"(?P<pre>.*)\s*{self.template_marker}\s+END.*")
+        tend = re.compile(rf"(?P<pre>.*)\s*{self.config.template_marker}\s+END")
         while True:
             _, line = next(inputiter)
-            # propagate
-            outputfile.write(line)
 
             beginmatch = tbegin.match(line)
             if beginmatch:
                 msg = f"missing END tag for '{filepath!s}:{tinfo.lineno}'"
                 raise MakolatorError(msg)
 
             # search for "INPLACE END"
             endmatch = tend.match(line)
             if endmatch:
+                outputfile.write(self._fill_marker(endmatch))
                 LOGGER.info("Template '%s:%d'", str(outputfile), tinfo.lineno)
                 templates.append(Template("".join(tinfo.lines), lookup=lookup))
                 break
+            else:
+                # propagate
+                outputfile.write(line)
+
             if line.startswith(pre):
                 line = line[prelen:]
             tinfo.lines.append(line)
 
     def _start_inplace(
         self, templates: List[Template], filepath: Path, lineno: int, indent: str, funcname: str, args: str
     ) -> Optional[InplaceInfo]:
         for template in templates:
             try:
                 func = template.get_def(funcname)
             except AttributeError:
                 continue
-            end = re.compile(rf"(?P<indent>\s*).*{self.inplace_marker}\s+END\s{funcname}.*")
+            end = re.compile(rf"(?P<indent>\s*).*{self.config.inplace_marker}\s+END\s{funcname}")
             return InplaceInfo(lineno, indent, funcname, args, func, end)
         if not self.ignore_unknown:
             raise MakolatorError(f"{filepath!s}:{lineno} Function '{funcname}' is not found in templates.")
         return None
 
     def _fill_inplace(self, filepath: Path, outputfile, inplace: InplaceInfo, context: dict):
         # pylint: disable=too-many-locals
@@ -225,10 +230,19 @@
                 if line:
                     outputfile.write(f"{indent}{line}\n")
                 else:
                     outputfile.write("\n")
 
         buffer.close()
 
+    def _fill_marker(self, mat: re.Match) -> str:
+        marker_fill = self.config.marker_fill
+        marker_linelength = self.config.marker_linelength
+        if marker_fill and marker_linelength:
+            line = mat.string[mat.start() : mat.end()]  # noqa
+            return fill_marker(line, marker_fill, marker_linelength) + "\n"
+        else:
+            return mat.string
+
 
 def _extract(*args, **kwargs):
     return (args, kwargs)
```

### Comparing `makolator-2.4.0/makolator/_staticcode.py` & `makolator-2.5.0/makolator/_staticcode.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 import re
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Dict, Iterator, List, Optional
 
 from attrs import define, field
 
-from ._util import LOGGER, check_indent, humanify
+from ._util import LOGGER, check_indent, fill_marker, humanify
+from .config import Config
 from .exceptions import MakolatorError
 
 StaticCodeMap = Dict[str, str]
 
 # pylint: disable=too-few-public-methods
 
 
@@ -49,39 +50,47 @@
 
 @define
 class StaticCode:
 
     """Static Code Manager."""
 
     comment_sep: str
-    marker: str
     staticcodemap: StaticCodeMap
+    marker: str
+    marker_fill: str = ""
+    marker_linelength: int = 0
 
     _names: List[str] = field(factory=list)
 
     def __call__(self, name, default=None, comment_sep=None):
         if name in self._names:
             raise MakolatorError(f"duplicate static code {name!r}")
         self._names.append(name)
         if comment_sep is None:
             comment_sep = self.comment_sep or ""
         code = self.staticcodemap.pop(name, default) or ""
         cpre = f"{comment_sep} " if comment_sep else ""
-        lines = [f"{cpre}{self.marker} BEGIN {name}"]
+        begin = f"{cpre}{self.marker} BEGIN {name}"
+        end = f"{cpre}{self.marker} END {name}"
+        if self.marker_fill and self.marker_linelength:
+            begin = fill_marker(begin, self.marker_fill, self.marker_linelength)
+            end = fill_marker(end, self.marker_fill, self.marker_linelength)
+        lines = [begin]
         lines.extend(code.splitlines())
-        lines.append(f"{cpre}{self.marker} END {name}")
+        lines.append(end)
         return "\n".join(lines)
 
 
 @contextmanager
-def read(filepath: Optional[Path], comment_sep: str, marker: str) -> Iterator[StaticCode]:
+def read(filepath: Optional[Path], comment_sep: str, config: Config) -> Iterator[StaticCode]:
     """Read from ``filepath``."""
     staticcodemap: StaticCodeMap = {}
+    marker = config.static_marker
     _read(filepath, marker, staticcodemap)
-    yield StaticCode(comment_sep, marker, staticcodemap)
+    yield StaticCode(comment_sep, staticcodemap, marker, config.marker_fill, config.marker_linelength)
     if staticcodemap:
         names = humanify(staticcodemap)
         raise MakolatorError(f"'{filepath!s}': unknown static code {names}")
 
 
 def _read(filepath: Optional[Path], marker: str, staticcodemap: StaticCodeMap):
     if filepath and marker:
```

### Comparing `makolator-2.4.0/makolator/_util.py` & `makolator-2.5.0/makolator/_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,7 +53,17 @@
 
 
 def humanify(iterable):
     """Just join names from `iterable`."""
     if iterable:
         return ", ".join(repr(str(item)) for item in iterable)
     return "''"
+
+
+def fill_marker(line: str, fill: str, length: int):
+    filllen = len(fill)
+    linelen = len(line) + 1
+    if linelen >= length:
+        return line
+    count = (length - linelen) // filllen
+    filling = fill * count
+    return f"{line} {filling}"
```

### Comparing `makolator-2.4.0/makolator/cli.py` & `makolator-2.5.0/makolator/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,22 +98,37 @@
             "--template-path",
             "-T",
             type=Path,
             default=[],
             action="append",
             help="Directories with templates referred by include/inherit/...",
         )
+        sub.add_argument(
+            "--marker-fill",
+            type=str,
+            help=(
+                "Static Code, Inplace and Template Marker are filled with "
+                "this given value until reaching line length of --marker-linelength."
+            ),
+        )
+        sub.add_argument(
+            "--marker-linelength",
+            type=int,
+            help=("Static Code, Inplace and Template Marker are filled until " "--marker-linelength."),
+        )
 
     args = parser.parse_args(args=args)
     if args.cmd:
         config = Config(
             verbose=args.verbose,
             diffout=print if args.show_diff else None,
             existing=args.existing,
             template_paths=args.template_path + [Path(".")],
+            marker_fill=args.marker_fill,
+            marker_linelength=args.marker_linelength,
         )
         info = Info(cli=get_cli())
         mklt = Makolator(config=config, info=info)
         if args.cmd == "gen":
             mklt.gen(args.templates, args.output)
         else:
             mklt.config.inplace_eol_comment = args.eol
```

### Comparing `makolator-2.4.0/makolator/config.py` & `makolator-2.5.0/makolator/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,7 +104,13 @@
     Line Comment Symbols.
 
     File Suffix dependent comment starter.
     """
 
     inplace_eol_comment: Optional[str] = None
     """End-Of-Line Comment Added On Every Inplace Generated Line """
+
+    marker_fill: str = "="
+    """Marker Filling."""
+
+    marker_linelength: int = 0
+    """Marker Line Length for Filling."""
```

### Comparing `makolator-2.4.0/makolator/datamodel.py` & `makolator-2.5.0/makolator/datamodel.py`

 * *Files identical despite different names*

### Comparing `makolator-2.4.0/makolator/escape.py` & `makolator-2.5.0/makolator/escape.py`

 * *Files identical despite different names*

### Comparing `makolator-2.4.0/makolator/exceptions.py` & `makolator-2.5.0/makolator/exceptions.py`

 * *Files identical despite different names*

### Comparing `makolator-2.4.0/makolator/helper.py` & `makolator-2.5.0/makolator/helper.py`

 * *Files identical despite different names*

### Comparing `makolator-2.4.0/makolator/info.py` & `makolator-2.5.0/makolator/info.py`

 * *Files identical despite different names*

### Comparing `makolator-2.4.0/makolator/makolator.py` & `makolator-2.5.0/makolator/makolator.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,21 +138,21 @@
         tplfilepaths, lookup = self._create_template_lookup(
             template_filepaths, self.config.template_paths, required=True
         )
         templates = self._create_templates(tplfilepaths, lookup)
         context = context or {}
         comment_sep = self._get_comment_sep(dest)
         if dest is None:
-            with read(dest, comment_sep, self.config.static_marker) as staticcode:
+            with read(dest, comment_sep, self.config) as staticcode:
                 self._render(next(templates), sys.stdout, None, context, staticcode)
         else:
             # Mako takes care about proper newline handling. Therefore we deactivate
             # the universal newline mode, by setting newline="".
             with self.open_outputfile(dest, newline="") as output:
-                with read(dest, comment_sep, self.config.static_marker) as staticcode:
+                with read(dest, comment_sep, self.config) as staticcode:
                     template = next(templates)  # Load template
                     LOGGER.info("Generate '%s'", dest)
                     self._render(template, output, dest, context, staticcode)
 
     def _render(self, template: Template, output, dest: Optional[Path], context: dict, staticcode: StaticCode):
         # pylint: disable=too-many-arguments
         context = Context(output, **self._get_render_context(dest, context, staticcode))
@@ -180,17 +180,17 @@
         LOGGER.debug("inplace(%r, %s)", [str(filepath) for filepath in template_filepaths], filepath)
         tplfilepaths, lookup = self._create_template_lookup(template_filepaths, self.config.template_paths)
         templates = tuple(self._create_templates(tplfilepaths, lookup))
         config = self.config
         context = context or {}
         comment_sep = self._get_comment_sep(filepath)
         eol = self._get_eol(filepath, config.inplace_eol_comment)
-        inplace = InplaceRenderer(config.template_marker, config.inplace_marker, templates, ignore_unknown, eol)
+        inplace = InplaceRenderer(config, templates, ignore_unknown, eol)
         with self.open_outputfile(filepath, existing=Existing.KEEP_TIMESTAMP, newline="") as outputfile:
-            with read(filepath, comment_sep, config.static_marker) as staticcode:
+            with read(filepath, comment_sep, config) as staticcode:
                 context = self._get_render_context(filepath, context, staticcode)
                 inplace.render(lookup, filepath, outputfile, context)
 
     def _create_templates(self, tplfilepaths: List[Path], lookup: TemplateLookup) -> Generator[Template, None, None]:
         for tplfilepath in tplfilepaths:
             LOGGER.info("Template '%s'", tplfilepath)
             yield lookup.get_template(tplfilepath.name)
@@ -241,14 +241,16 @@
                 # relative
                 for searchpath in searchpaths:
                     joined = searchpath / filepath
                     if joined.exists():
                         yield joined
                         found = True
         if not found and required:
+            if not searchpaths:
+                raise MakolatorError(f"None of the templates {humanify(filepaths)}.")
             raise MakolatorError(f"None of the templates {humanify(filepaths)} found at {humanify(searchpaths)}.")
 
     def _get_render_context(self, output_filepath: Optional[Path], context: dict, staticcode: StaticCode) -> dict:
         result = dict(context)
         result.update(HELPER)
         result["datamodel"] = self.datamodel
         result["makolator"] = self
```

### Comparing `makolator-2.4.0/pyproject.toml` & `makolator-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makolator"
-version = "2.4.0"
+version = "2.5.0"
 description = "Extended Mako Templates for Python"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `makolator-2.4.0/PKG-INFO` & `makolator-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makolator
-Version: 2.4.0
+Version: 2.5.0
 Summary: Extended Mako Templates for Python
 License: MIT
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

