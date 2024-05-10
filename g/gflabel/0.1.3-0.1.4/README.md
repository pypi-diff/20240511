# Comparing `tmp/gflabel-0.1.3.tar.gz` & `tmp/gflabel-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gflabel-0.1.3.tar", max compression
+gzip compressed data, was "gflabel-0.1.4.tar", max compression
```

## Comparing `gflabel-0.1.3.tar` & `gflabel-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1456 2024-05-03 20:18:13.278077 gflabel-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0    10015 2024-05-03 20:18:13.278077 gflabel-0.1.3/README.md
--rw-r--r--   0        0        0      813 2024-05-03 20:18:13.282077 gflabel-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 20:18:13.282077 gflabel-0.1.3/src/gflabel/__init__.py
--rw-r--r--   0        0        0      220 2024-05-03 20:18:13.282077 gflabel-0.1.3/src/gflabel/bases/__init__.py
--rw-r--r--   0        0        0     1369 2024-05-03 20:18:13.282077 gflabel-0.1.3/src/gflabel/bases/plain.py
--rw-r--r--   0        0        0     3265 2024-05-03 20:18:13.282077 gflabel-0.1.3/src/gflabel/bases/pred.py
--rw-r--r--   0        0        0     3726 2024-05-03 20:18:13.282077 gflabel-0.1.3/src/gflabel/bases/webb.py
--rwxr-xr-x   0        0        0     9625 2024-05-03 20:18:13.282077 gflabel-0.1.3/src/gflabel/cli.py
--rw-r--r--   0        0        0    31301 2024-05-03 20:18:13.286078 gflabel-0.1.3/src/gflabel/fragments.py
--rw-r--r--   0        0        0     8880 2024-05-03 20:18:13.286078 gflabel-0.1.3/src/gflabel/label.py
--rw-r--r--   0        0        0     1637 2024-05-03 20:18:13.286078 gflabel-0.1.3/src/gflabel/options.py
--rw-r--r--   0        0        0    10562 1970-01-01 00:00:00.000000 gflabel-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-05-10 23:40:34.108978 gflabel-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0    12949 2024-05-10 23:40:34.108978 gflabel-0.1.4/README.md
+-rw-r--r--   0        0        0      813 2024-05-10 23:40:34.116978 gflabel-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 23:40:34.116978 gflabel-0.1.4/src/gflabel/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-10 23:40:34.116978 gflabel-0.1.4/src/gflabel/bases/__init__.py
+-rw-r--r--   0        0        0     1369 2024-05-10 23:40:34.116978 gflabel-0.1.4/src/gflabel/bases/plain.py
+-rw-r--r--   0        0        0     3265 2024-05-10 23:40:34.116978 gflabel-0.1.4/src/gflabel/bases/pred.py
+-rw-r--r--   0        0        0     3726 2024-05-10 23:40:34.116978 gflabel-0.1.4/src/gflabel/bases/webb.py
+-rw-r--r--   0        0        0   110480 2024-05-10 23:40:34.116978 gflabel-0.1.4/src/gflabel/chris-pikul-symbols.zip
+-rwxr-xr-x   0        0        0    11728 2024-05-10 23:40:34.116978 gflabel-0.1.4/src/gflabel/cli.py
+-rw-r--r--   0        0        0    38251 2024-05-10 23:40:34.116978 gflabel-0.1.4/src/gflabel/fragments.py
+-rw-r--r--   0        0        0     9321 2024-05-10 23:40:34.116978 gflabel-0.1.4/src/gflabel/label.py
+-rw-r--r--   0        0        0     2148 2024-05-10 23:40:34.116978 gflabel-0.1.4/src/gflabel/options.py
+-rw-r--r--   0        0        0     1450 2024-05-10 23:40:34.116978 gflabel-0.1.4/src/gflabel/util.py
+-rw-r--r--   0        0        0    13496 1970-01-01 00:00:00.000000 gflabel-0.1.4/PKG-INFO
```

### Comparing `gflabel-0.1.3/LICENSE.txt` & `gflabel-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.3/README.md` & `gflabel-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -45,14 +45,22 @@
 
 Otherwise, you can check out this repository and `pip install` it directly, or
 install directly from the github repo:
 
 ```
 pip install git+https://github.com/ndevenish/gflabel.git
 ```
+### VSCode Preview
+
+If you are using VSCode with the [vscode-ocp-cad-viewer][ocp-vscode] extension,
+you can add the `--vscode` flag when running `gflabel`, and the label should
+show up as a preview. This saves opening the output CAD files in a slicer or
+other viewer, and is useful when prototyping labels.
+
+[ocp-vscode]: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 
 ### Basic Examples
 
 By default, labels are written to an output file "`label.step`". You can change
 this with `-o FILENAME`. `.step`, `.stl` and `.svg` are recognised
 
 A simple, single label generation on a pred-style base:
@@ -173,14 +181,15 @@
 | &lt;number&gt;    | A gap of specific width, in mm.                                   |
 | bolt              | Variable length bolt, in the style of Printables pred-box labels.<br><br>If the requested bolt is longer than the available space, then the<br>bolt will be as large as possible with a broken thread. |
 | box               | Arbitrary width, height centered box. If height is not specified, will expand to row height. |
 | head              | Screw head with specifiable head-shape.                           |
 | hexhead           | Hexagonal screw head. Will accept drives, but not compulsory.     |
 | hexnut, nut       | Hexagonal outer profile nut with circular cutout.                 |
 | lockwasher        | Circular washer with a locking cutout.                            |
+| sym, symbol       | Render an electronic symbol.                                      |
 | threaded_insert   | Representation of a threaded insert.                              |
 | variable_resistor | Electrical symbol of a variable resistor.                         |
 | washer            | Circular washer with a circular hole.                             |
 | webbolt           | Alternate bolt representation incorporating screw drive, with fixed length. |
 
 A basic set of examples showing the usage of some of these:
 
@@ -217,8 +226,59 @@
 both can be pointed backwards by adding the `flipped` feature.
 
 Examples showing some differences between the two bolts:
 
 ![](images/bolts.svg)
 
 
+### Electronic Symbols
+
+Electronic symbols can be generated using the `{symbol(...)}` fragment.
+GFLabel is using the [Chris Pikul Electronic Symbols ][pikul] library kindly
+released under MIT Licence.
+
+[pikul]: https://github.com/chris-pikul/electronic-symbols
+
+There are currently three main approaches to selecting the symbol that you
+want:
+
+- Exact [ID][ID], or exact [Filename][files], as defined the original source.
+- Component name, as listed on the symbol source [README][pikul] (and in the
+  table below). In cases where multiple symbols have the same name, they can
+  be differentiated by standard e.g. `{symbol(capacitor,iec)}`. If standard is
+  not specified, and there are multiple matches, then the first of [`common`,
+  `iec`, `ieee`] will be chosen (if doing so makes it unambiguous).
+- Fuzzy matching. You can pass in words or parts of words. Symbols with
+  category, name or ID that match these (in any order) will be selected. If
+  more than one candidate symbols matches, then the table of possible matches
+  will be returned so that you can refine it further.
+
+You can list all of the symbols available with `gflabel --list-symbols`.
+
+For an example of this fuzzy matching, the fragment `{symbol(ground)}` isn't
+enough to disambiguate between the possible options, so the table of matches
+is printed to help you refine the definition:
+
+```
+$ gflabel '{symbol(ground)}'
+...
+Could not decide on symbol from fuzzy specification "ground". Possible options:
+    ID                 Category Name                  Standard Filename
+    ground-com-signal  GROUND   Digital/Signal Ground COMMON   Ground-COM-Signal
+    ground-com-general GROUND   Common/Earth Ground   COMMON   Ground-COM-General
+    ground-com-chassis GROUND   Chassis Ground        COMMON   Ground-COM-Chassis
+
+Could not proceed: Please specify symbol more precisely.
+```
+
+Given this, you could disambiguate by refining the fuzzy specification e.g.
+`{symbol(signal ground)}`, matching the exact name `{symbol(Common/Earth Ground)}`,
+or specifying the ID/Filename exactly: `{symbol(Ground-COM-Signal)}`.
+
+[ID]: https://github.com/chris-pikul/electronic-symbols/blob/main/manifest.json
+[files]: https://github.com/chris-pikul/electronic-symbols/tree/main/SVG
+
+Here is a table of all symbols, rendered by GFLabel, with their name as per the
+source symbol library. Note that for some of the symbols, they are rendered
+incorrectly. This is an unresolved bug in GFLabel.
 
+![](images/symbols.svg)
```

### Comparing `gflabel-0.1.3/pyproject.toml` & `gflabel-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gflabel"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Nicholas Devenish <ndevenish@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -24,15 +24,15 @@
 [tool.ruff.lint.isort]
 required-imports = ["from __future__ import annotations"]
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpversion]
-current_version = "0.1.3"
+current_version = "0.1.4"
 tag = true
 tag_name = "v{new_version}"
 commit = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
```

### Comparing `gflabel-0.1.3/src/gflabel/bases/plain.py` & `gflabel-0.1.4/src/gflabel/bases/plain.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.3/src/gflabel/bases/pred.py` & `gflabel-0.1.4/src/gflabel/bases/pred.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.3/src/gflabel/bases/webb.py` & `gflabel-0.1.4/src/gflabel/bases/webb.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.3/src/gflabel/cli.py` & `gflabel-0.1.4/src/gflabel/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,42 +4,43 @@
 from __future__ import annotations
 
 import argparse
 import logging
 import sys
 from argparse import ArgumentParser
 from itertools import islice
+from typing import Any, Sequence
 
 import build123d as bd
 import rich
 import rich.table
 
 # from build123d import *
 from build123d import (
     BuildPart,
+    BuildSketch,
     ColorIndex,
-    Compound,
     ExportSVG,
     FontStyle,
     Keep,
     Location,
     Locations,
     Mode,
     Plane,
     Vector,
     add,
     export_step,
     extrude,
-    section,
 )
 
 from . import fragments
 from .bases import plain, pred, webb
 from .label import render_divided_label
 from .options import LabelStyle, RenderOptions
+from .util import IndentingRichHandler
 
 logger = logging.getLogger(__name__)
 
 if "--vscode" in sys.argv:
     from ocp_vscode import Camera, set_defaults, show
 
     set_defaults(reset_camera=Camera.CENTER)
@@ -61,28 +62,52 @@
     def __init__(self, option_strings, dest, nargs=None, **kwargs):
         if nargs is not None:
             raise ValueError("nargs not allowed")
         super().__init__(option_strings, dest, nargs=0, **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
         table = rich.table.Table("NAMES", "DESCRIPTION")
-        table.add_row
 
         frags = fragments.fragment_description_table()
         multiline = [x for x in frags if len(x.description.splitlines()) > 1]
 
         for frag in multiline:
             table.add_row(", ".join(frag.names), frag.description, end_section=True)
         for frag in [x for x in frags if x not in multiline]:
             table.add_row(", ".join(frag.names), frag.description)
 
         rich.print(table)
         sys.exit(0)
 
 
+class ListSymbolsAction(argparse.Action):
+    def __init__(self, option_strings, dest, nargs=None, **kwargs):
+        if nargs is not None:
+            raise ValueError("nargs not allowed")
+        super().__init__(option_strings, dest, nargs=0, **kwargs)
+
+    def __call__(
+        self,
+        parser: ArgumentParser,
+        namespace: argparse.Namespace,
+        values: str | Sequence[Any] | None,
+        option_string: str | None = None,
+    ) -> None:
+        manifest = fragments.electronic_symbols_manifest()
+        cols = ["ID", "Category", "Name", "Standard", "Filename"]
+        table = rich.table.Table(*cols)
+        for symbol in manifest:
+            table.add_row(*[symbol[x.lower()] for x in cols])  # type: ignore
+        rich.print(table)
+        rich.print(
+            "\nSymbol Library © Chris Pikul with MIT License https://github.com/chris-pikul/electronic-symbols"
+        )
+        sys.exit(0)
+
+
 def run(argv: list[str] | None = None):
     parser = ArgumentParser(description="Generate gridfinity bin labels")
     parser.add_argument(
         "--base",
         choices=["pred", "plain", "none", "webb"],
         default="pred",
         help="Label base to generate onto. [Default: %(default)s]",
@@ -131,19 +156,27 @@
 
     parser.add_argument(
         "--font",
         help="The font to use for rendering. [Default: %(default)s]",
         type=str,
         default="Futura",
     )
-    parser.add_argument(
+
+    font_size = parser.add_mutually_exclusive_group()
+    font_size.add_argument(
+        "--font-size-maximum",
+        help="Specify a maximum font size (in mm) to use for rendering. The text may end up smaller than this if it needs to fit in the area.",
+        type=float,
+    )
+    font_size.add_argument(
         "--font-size",
         help="The font size (in mm) to use for rendering. If unset, then the font will use as much vertical space as needed (that also fits within the horizontal area).",
         type=float,
     )
+
     parser.add_argument(
         "--font-style",
         help="The font style use for rendering. [Default: %(default)s]",
         choices=[x.name.lower() for x in FontStyle],
         default="regular",
         type=str,
     )
@@ -151,39 +184,67 @@
         "--margin",
         help="The margin area (in mm) to leave around the label contents. Default is per-base.",
         type=float,
     )
     parser.add_argument(
         "-o",
         "--output",
-        help="Output filename. [Default: %(default)s]",
-        default="label.step",
+        help="Output filename(s). [Default: %(default)s]",
+        default=["label.step"],
+        nargs="*",
     )
     parser.add_argument(
         "--style",
         help="How the label contents are formed.",
         choices=LabelStyle,
         default=LabelStyle.EMBOSSED,
         type=LabelStyle,
     )
     parser.add_argument(
         "--list-fragments",
         help="List all available fragments.",
         action=ListFragmentsAction,
     )
+    parser.add_argument(
+        "--list-symbols",
+        help="List all available electronic symbols",
+        action=ListSymbolsAction,
+    )
+    parser.add_argument(
+        "--gap",
+        help="Vertical gap (in mm) between physical labels. Default: %(default)s mm",
+        default=2,
+        type=float,
+    )
+    parser.add_argument("-v", "--verbose", help="Verbose output", action="store_true")
     args = parser.parse_args(argv)
 
     logging.basicConfig(
-        level=logging.DEBUG,
+        level=logging.DEBUG if args.verbose else logging.INFO,
+        handlers=[
+            IndentingRichHandler(
+                show_time=args.verbose,
+                show_level=args.verbose,
+                show_path=args.verbose,
+                log_time_format="[%Y-%m-%d %H:%M:%S]",
+            )
+        ],
+        format="%(message)s",
     )
     logging.getLogger("websockets").setLevel(logging.WARNING)
     logging.getLogger("build123d").setLevel(logging.WARNING)
 
+    logger.debug(f"Args: {args}")
+
+    # We cannot have debossed labels with no label
     assert not (args.base == "none" and args.style == LabelStyle.DEBOSSED)
 
+    # We don't need to generate 3D shapes if we are only doing SVG
+    is_2d = all([x.endswith(".svg") for x in args.output])
+
     # If running in VSCode mode, then we can hardcode a label here
     if not args.labels:
         args.labels = ["{webbolt(pozi)}{...}M3×20"]
 
     if not args.width:
         if args.base in {"pred", "webb"}:
             args.width = "1"
@@ -196,91 +257,88 @@
         else:
             args.margin = 0.2
     args.width = int(args.width.rstrip("u"))
     args.divisions = args.divisions or len(args.labels)
     args.labels = [x.replace("\\n", "\n") for x in args.labels]
 
     options = RenderOptions.from_args(args)
-    print(options)
+    logger.debug("Got render options: %s", options)
     with BuildPart() as part:
         y = 0
-        for labels in batched(args.labels, args.divisions):
-            with Locations([Location([0, y])]):
-                if args.base == "pred":
-                    body = pred.body(
-                        args.width, recessed=args.style == LabelStyle.EMBOSSED
-                    )
-                elif args.base == "plain":
-                    if args.width < 10:
-                        logger.warning(
-                            f"Warning: Small width ({args.width}) for plain base. Did you specify in mm?"
-                        )
-                    body = plain.body(args.width, args.height)
-                elif args.base == "webb":
-                    body = webb.body()
-                else:
-                    body = None
-
-                if body:
-                    y -= body.part.bounding_box().size.Y + 2
-                    add(body.part)
-                    label_area = body.area
-                else:
-                    y -= args.height + 2
-                    label_area = Vector(X=args.width, Y=args.height)
-
-                add(
-                    render_divided_label(
-                        labels, label_area, divisions=args.divisions, options=options
-                    )
-                )
-                extrude(
-                    amount=args.depth,
-                    mode=(
-                        Mode.ADD if args.style == LabelStyle.EMBOSSED else Mode.SUBTRACT
-                    ),
+        if args.base == "pred":
+            body = pred.body(args.width, recessed=args.style == LabelStyle.EMBOSSED)
+        elif args.base == "plain":
+            if args.width < 10:
+                logger.warning(
+                    f"Warning: Small width ({args.width}) for plain base. Did you specify in mm?"
                 )
+            body = plain.body(args.width, args.height)
+        elif args.base == "webb":
+            body = webb.body()
+        else:
+            body = None
 
-    if args.output.endswith(".stl"):
-        bd.export_stl(part.part, args.output)
-    elif args.output.endswith(".step"):
-        export_step(part.part, args.output)
-    elif args.output.endswith(".svg"):
-        visible, hidden = part.part.project_to_viewport(
-            (0, 0, 50), viewport_up=(0, 1, 0)
-        )
-        max_dimension = max(*Compound(children=visible + hidden).bounding_box().size)
+        if body:
+            y_offset_each_label = body.part.bounding_box().size.Y + args.gap
+            label_area = body.area
+        else:
+            y_offset_each_label = args.height + args.gap
+            label_area = Vector(X=args.width, Y=args.height)
+
+        body_locations = []
+        with BuildSketch() as label_sketch:
+            all_labels = []
+            for labels in batched(args.labels, args.divisions):
+                body_locations.append((0, y))
+                try:
+                    all_labels.append(
+                        render_divided_label(
+                            labels,
+                            label_area,
+                            divisions=args.divisions,
+                            options=options,
+                        ).locate(Location([0, y]))
+                    )
+                except fragments.InvalidFragmentSpecification as e:
+                    rich.print(f"\n[y][b]Could not proceed: {e}[/b][/y]\n")
+                    sys.exit(1)
+                y -= y_offset_each_label
+            logger.debug("Combining all labels")
+            add(all_labels)
+
+        if not is_2d:
+            # Create all of the bases
+            if body:
+                logger.debug("Creating label bodies")
+                with Locations(body_locations):
+                    add(body.part)
 
-        if args.base == "none":
-            print("Rendering from section")
-            lines = section(part.part, Plane.XY, height=args.depth / 2)
-            e = ExportSVG(scale=100 / max_dimension)
-            # max_dimension = max(*Compound(children=visible + _hidden).bounding_box().size)
-            e.add_layer(
-                "Visible",
-                fill_color=ColorIndex.BLACK,
-                # line_color=ColorIndex.BLACK,
-                line_weight=0.1,
+            logger.debug("Extruding labels")
+            extrude(
+                amount=args.depth,
+                mode=(Mode.ADD if args.style == LabelStyle.EMBOSSED else Mode.SUBTRACT),
             )
-            e.add_shape(lines, layer="Visible")
-            e.write(args.output)
-        else:
-            exporter = ExportSVG(scale=100 / max_dimension)
-            exporter.add_layer("Visible", fill_color=ColorIndex.YELLOW)
-            # exporter.add_layer(
-            #     "Hidden", line_color=(99, 99, 99), line_type=LineType.ISO_DOT
-            # )
-            exporter.add_shape(visible, layer="Visible")
-            # exporter.add_shape(hidden, layer="Hidden")
-            exporter.write(args.output)
 
-    else:
-        print(f"Error: Do not understand output format '{args.output}'")
+    for output in args.output:
+        if output.endswith(".stl"):
+            bd.export_stl(part.part, output)
+        elif output.endswith(".step"):
+            export_step(part.part, output)
+        elif output.endswith(".svg"):
+            max_dimension = max(label_sketch.sketch.bounding_box().size)
+            exporter = ExportSVG(scale=100 / max_dimension)
+            exporter.add_layer("Shapes", fill_color=ColorIndex.BLACK, line_weight=0)
+            logger.info(f"Writing SVG {output}")
+            exporter.add_shape(label_sketch.sketch, layer="Shapes")
+            exporter.write(output)
+        else:
+            logger.error(f"Error: Do not understand output format '{args.output}'")
 
     if args.vscode:
+        # Export both step and stl in vscode_ocp mode
         bd.export_stl(part.part, "label.stl")
         export_step(part.part, "label.step")
         # Split the base for display as two colours
         show_parts = []
         show_cols: list[str | tuple[float, float, float] | None] = []
         top = part.part.split(Plane.XY, keep=Keep.TOP)
         if top:
```

### Comparing `gflabel-0.1.3/src/gflabel/fragments.py` & `gflabel-0.1.4/src/gflabel/fragments.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from __future__ import annotations
 
 import functools
+import importlib.resources
+import io
+import itertools
+import json
 import logging
 import re
 import textwrap
+import zipfile
 from abc import ABCMeta, abstractmethod
 from collections.abc import Callable
 from math import cos, radians, sin
-from typing import Any, Iterable, NamedTuple, Type
+from typing import Any, Iterable, NamedTuple, Type, TypedDict
 
 from build123d import (
     Align,
     Axis,
     BuildLine,
     BuildSketch,
     CenterArc,
@@ -30,20 +35,22 @@
     Sketch,
     SlotCenterToCenter,
     Text,
     Triangle,
     Vector,
     add,
     fillet,
+    import_svg,
     make_face,
     mirror,
     offset,
 )
 
 from .options import RenderOptions
+from .util import format_table
 
 logger = logging.getLogger(__name__)
 RE_FRAGMENT = re.compile(r"(.+?)(?:\((.*)\))?$")
 
 FRAGMENTS: dict[str, Type[Fragment] | Callable[..., Fragment]] = {}
 
 # Alias names for drive. These should be remapped before rendering
@@ -65,14 +72,18 @@
     "triangle",
     "torx",
     "security",
     "phillipsslot",
 }
 
 
+class InvalidFragmentSpecification(RuntimeError):
+    pass
+
+
 def fragment_from_spec(spec: str) -> Fragment:
     # If the fragment is just a number, this is distance to space out
     try:
         value = float(spec)
     except ValueError:
         pass
     else:
@@ -217,39 +228,39 @@
     def __init__(self, text: str):
         self.text = text
 
     def render(self, height: float, maxsize: float, options: RenderOptions) -> Sketch:
         with BuildSketch() as sketch:
             Text(
                 self.text,
-                font_size=options.font.font_height_mm or height,
+                font_size=options.font.get_allowed_height(height),
                 font=options.font.font,
                 font_style=options.font.font_style,
             )
         return sketch.sketch
 
 
 @functools.lru_cache
 def _whitespace_width(spacechar: str, height: float, options: RenderOptions) -> float:
     """Calculate the width of a space at a specific text height"""
     w2 = (
         Text(
             f"a{spacechar}a",
-            font_size=options.font.font_height_mm or height,
+            font_size=options.font.get_allowed_height(height),
             font=options.font.font,
             font_style=options.font.font_style,
             mode=Mode.PRIVATE,
         )
         .bounding_box()
         .size.X
     )
     wn = (
         Text(
             "aa",
-            font_size=options.font.font_height_mm or height,
+            font_size=options.font.get_allowed_height(height),
             font=options.font.font,
             font_style=options.font.font_style,
             mode=Mode.PRIVATE,
         )
         .bounding_box()
         .size.X
     )
@@ -896,25 +907,215 @@
             description="A gap of specific width, in mm.",
             examples=["]{12.5}["],
         )
     )
     return sorted(descriptions, key=lambda x: x.names[0])
 
 
+class ManifestItem(TypedDict):
+    id: str
+    name: str
+    category: str
+    standard: str
+    filename: str
+
+
+@functools.cache
+def electronic_symbols_manifest() -> list[ManifestItem]:
+    with importlib.resources.files("gflabel").joinpath("chris-pikul-symbols.zip").open(
+        "rb"
+    ) as f:
+        zip = zipfile.ZipFile(f)
+        return json.loads(zip.read("manifest.json"))
+
+
+def _get_standard_requested(selectors: Iterable[str]) -> str | None:
+    """Given a list of selectors, did we ask for a standard?"""
+    aliases = {
+        "com": "common",
+        "ansi": "ieee",
+        "euro": "iec",
+        "europe": "iec",
+    }
+    # Convert this to a set and resolve aliases
+    requested = set(aliases.get(x.lower(), x.lower()) for x in selectors)
+    # Work out if a specific standard was requested
+    standards = {x.upper() for x in requested & {"iec", "ieee", "common"}}
+    if len(standards) > 1:
+        raise ValueError(
+            f"Got more than one symbol standard selected: '{', '.join(standards)}'"
+        )
+    return next(iter(standards), None)
+
+
+def _match_electronic_symbol_from_standard(
+    preferred_standards: list[str],
+    matches: list[ManifestItem],
+) -> list[ManifestItem]:
+    # IF all matches are in the same category, then choose based on standard.
+    def _get_standard(x):
+        return x["standard"].lower()
+
+    grouped_match = itertools.groupby(
+        sorted(matches, key=lambda x: preferred_standards.index(_get_standard(x))),
+        key=_get_standard,
+    )
+    return list(next(iter(grouped_match), [[]])[1])
+
+
+def _match_electronic_symbol_with_selectors(selectors: Iterable[str]) -> ManifestItem:
+    """
+    Match a symbol in the electronics manifest.
+
+    Returns:
+        The manifest entry. If no result, a ValueError will be raised.
+    """
+    # Convert this to a set and resolve aliases
+    aliases: dict[str, str] = {}
+    requested = set(
+        aliases.get(x.lower(), x.lower())
+        .removesuffix(".svg")
+        .removesuffix(".png")
+        .removesuffix(".jpg")
+        for x in selectors
+    )
+
+    # Work out if we requested a standard
+    standard_req = _get_standard_requested(requested)
+    # Make a standard order to discriminate otherwise matches
+    standards_order = ["common", "iec", "ieee"]
+    if standard_req:
+        standards_order.remove(standard_req.lower())
+        standards_order.insert(0, standard_req.lower())
+        requested.remove(standard_req.lower())
+
+    manifest = electronic_symbols_manifest()
+
+    # Firstly, have we been given an exact ID, name or filename
+    matches = [
+        x
+        for x in manifest
+        if {
+            x["name"].lower(),
+            x["id"].lower(),
+            x["filename"].lower(),
+            # We handle standard separately, but accept exact name
+            # with/without it - some of the source components have it
+            x["name"]
+            .lower()
+            .replace(" (IEEE/ANSI)", "")
+            .replace(" (Common Style)", ""),
+        }
+        & requested
+    ]
+    if len(matches) == 1:
+        logger.debug("Found exact electronic symbol match: %s", repr(matches[0]["id"]))
+        return matches[0]
+
+    if not matches:
+        # We don't have any exact matches, so do fuzzy matching instead
+        logger.debug("No exact matches, using fuzzy matches instead")
+        # Split the request into a pool of matching tokens
+        match_tokens = set(itertools.chain(*[x.split() for x in requested]))
+        logger.debug(f"Using match soup: {match_tokens!r}")
+        for symbol in manifest:
+            # Create a soup for this symbol
+            soup = set(
+                itertools.chain(
+                    *[
+                        x.lower().split()
+                        for x in {symbol["category"], symbol["name"], symbol["id"]}
+                    ]
+                )
+            )
+            if "logic" in soup:
+                soup.add("gate")
+            # Use this symbol if all of our tokens are in any of the soup
+            if all(any(cand in s for s in soup) for cand in match_tokens):
+                logger.debug(f"    {symbol['id']} was a complete match!")
+                matches.append(symbol)
+
+    if len(matches) == 1:
+        logger.debug("Found fuzzy symbol match: %s", repr(matches[0]["id"]))
+        return matches[0]
+
+    if not matches:
+        raise InvalidFragmentSpecification(
+            f"Could find no matches for definition '{','.join(requested)}'"
+        )
+
+    # We have multiple matches. Try
+    logger.debug(f"Got {len(matches)} matches. Attempting to refine.")
+
+    if len({x["category"] for x in matches}) == 1:
+        matches = _match_electronic_symbol_from_standard(standards_order, matches)
+        if len(matches) == 1:
+            logger.debug(
+                f"Using symbol \"{matches[0]['id']}\" because standard [b]{matches[0]['standard']}[/b] is preferred.",
+                extra={"markup": True},
+            )
+            return matches[0]
+        else:
+            logger.debug(
+                f"Preferred standard was not enough to discriminate, {len(matches)} equivalent matches"
+            )
+    if matches:
+        cols = ["ID", "Category", "Name", "Standard", "Filename"]
+        logger.error(
+            f"Could not decide on symbol from fuzzy specification \"{','.join(requested)}\". Possible options:"
+            + "\n"
+            + "\n".join(
+                format_table(cols, matches, lambda x: x.lower(), prefix="    ")
+            ),  # type: ignore
+            extra={"markup": "True"},
+        )
+    else:
+        logger.error(
+            f"No electronic symbols matched the specification \"{','.join(requested)}\""
+        )
+    raise InvalidFragmentSpecification("Please specify symbol more precisely.")
+
+
+@fragment("symbol", "sym")
+class _electrical_symbol_fragment(Fragment):
+    """Render an electronic symbol."""
+
+    def __init__(self, *selectors: str):
+        self.symbol = _match_electronic_symbol_with_selectors(selectors)
+
+        with importlib.resources.files("gflabel").joinpath(
+            "chris-pikul-symbols.zip"
+        ).open("rb") as f:
+            zip = zipfile.ZipFile(f)
+            svg_data = io.StringIO(
+                zip.read("SVG/" + self.symbol["filename"] + ".svg").decode()
+            )
+            self.shapes = import_svg(svg_data, flip_y=False)
+
+    def render(self, height: float, maxsize: float, options: RenderOptions) -> Sketch:
+        with BuildSketch() as _sketch:
+            add(self.shapes)
+        bb = _sketch.sketch.bounding_box()
+        # Resize this to match the requested height, and to be centered
+        return _sketch.sketch.translate(-bb.center()).scale(height / bb.size.Y)
+
+
 if __name__ == "__main__":
     # Generate a markdown table of fragment definitions
     frags = fragment_description_table()
     maxname = max(len(", ".join(frag.names)) for frag in frags)
 
     # os.geten
     desc_len = 82 - maxname
     print(f"| {'Names':{maxname}} | {'Description':{desc_len}} |")
     print("|" + "-" * (maxname + 2) + "|" + "-" * (desc_len + 2) + "|")
 
     for frag in frags:
 
         def _clean(s):
+            if s is None:
+                return ""
             return s.replace("<", "&lt;").replace(">", "&gt;").replace("\n", "<br>")
 
         desc = _clean(frag.description)
         names = _clean(", ".join(frag.names))
         print(f"| {names:{maxname}} | {desc:{desc_len}} |")
```

### Comparing `gflabel-0.1.3/src/gflabel/label.py` & `gflabel-0.1.4/src/gflabel/label.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Vector,
     add,
 )
 from rich import print
 
 from . import fragments
 from .options import RenderOptions
+from .util import IndentingRichHandler
 
 logger = logging.getLogger(__name__)
 
 RE_FRAGMENT = re.compile(r"((?<!{){[^{}]+})")
 
 
 def _spec_to_fragments(spec: str) -> list[fragments.Fragment]:
@@ -86,56 +87,65 @@
             for n, line in enumerate(lines):
                 # Calculate the y of the line center
                 render_y = (
                     area.Y / 2
                     - (row_height + self.opts.line_spacing_mm) * n
                     - row_height / 2
                 )
-                print(f"Rendering line {n} ({line}) at {render_y})")
+                logger.info(f'Rendering line {n+1} ("{line}")')
+                IndentingRichHandler.indent()
                 with Locations([(0, render_y)]):
                     add(
                         self._render_single_line(
                             line,
                             Vector(X=area.X, Y=row_height),
                             self.opts.allow_overheight,
                         )
                     )
+                IndentingRichHandler.dedent()
 
         scale_to_maxwidth = area.X / sketch.sketch.bounding_box().size.X
         scale_to_maxheight = area.Y / sketch.sketch.bounding_box().size.Y
-        if scale_to_maxheight < 1:
+
+        if scale_to_maxheight < 1 - 1e3:
             print(
                 f"Vertical scale is too high for area ({scale_to_maxheight}); downscaling"
             )
         to_scale = min(scale_to_maxheight, scale_to_maxwidth, 1)
         print(f"Got scale: {to_scale}")
         if to_scale < 0.99 and not is_rescaling:
             print(f"Rescaling as {scale_to_maxwidth}")
             # We need to scale this down. Resort to adjusting the height and re-requesting.
             # second = make_text_label(
             #     spec,
             #     maxwidth,
             #     maxheight=maxheight * scale_to_maxwidth * 0.95,
             #     _rescaling=True,
             # )
+
+            # If we had an area that didn't fill the whole height, then we need
+            # to scale down THAT height, instead of the "total available" height
+            height_to_scale = min(area.Y, sketch.sketch.bounding_box().size.Y)
+
             second_try = self._do_multiline_render(
                 spec,
-                Vector(X=area.X, Y=area.Y * to_scale * 0.95),
+                Vector(X=area.X, Y=height_to_scale * to_scale * 0.95),
                 is_rescaling=True,
             )
             # If this didn't help, then error
             if (bbox_w := second_try.bounding_box().size.X) > area.X:
                 logger.warning(
                     'Warning: Could not fit label "%s" in box of width %.2f, got %.1f',
                     spec,
                     area.X,
                     bbox_w,
                 )
+            print_spec = spec.replace("\n", "\\n")
             print(
-                f'Entry "{spec}" calculated width = {sketch.sketch.bounding_box().size.X:.1f} (max {area.X})'
+                f'Entry "{print_spec}" calculated width = {sketch.sketch.bounding_box().size.X:.1f} (max {area.X})'
             )
             return second_try
         print(
             f'Entry "{spec}" calculated width = {sketch.sketch.bounding_box().size.X:.1f} (max {area.X})'
         )
 
         return sketch.sketch
```

### Comparing `gflabel-0.1.3/src/gflabel/options.py` & `gflabel-0.1.4/src/gflabel/options.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,14 +25,23 @@
     font: str = "Futura"
     font_style: FontStyle = FontStyle.BOLD
     # The font height, in mm. If this is unspecified, then the font will
     # be scaled to maximum area height, and then scaled down accordingly.
     # Setting this can explicitly cause overflow, as the text will be
     # unable to scale down if required.
     font_height_mm: float | None = None
+    # Whether this is specifying exact font height
+    font_height_exact: bool = True
+
+    def get_allowed_height(self, requested_height: float) -> float:
+        """Calculate the font height, accounting for option specifications"""
+        if self.font_height_exact:
+            return self.font_height_mm or requested_height
+        else:
+            return min(self.font_height_mm or requested_height, requested_height)
 
 
 class RenderOptions(NamedTuple):
     line_spacing_mm: float = 0.1
     margin_mm: float = 0.4
     font: FontOptions = FontOptions()
     # Overheight fragments cause the entire line to be scaled down in
@@ -46,11 +55,12 @@
             x for x in FontStyle if x.name.lower() == args.font_style.lower()
         ][0]
         return cls(
             margin_mm=args.margin,
             font=FontOptions(
                 font=args.font,
                 font_style=font_style,
-                font_height_mm=args.font_size,
+                font_height_mm=args.font_size or args.font_size_maximum,
+                font_height_exact=not args.font_size_maximum,
             ),
             allow_overheight=not args.no_overheight,
         )
```

### Comparing `gflabel-0.1.3/PKG-INFO` & `gflabel-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gflabel
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: BSD-3-Clause
 Author: Nicholas Devenish
 Author-email: ndevenish@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -62,14 +62,22 @@
 
 Otherwise, you can check out this repository and `pip install` it directly, or
 install directly from the github repo:
 
 ```
 pip install git+https://github.com/ndevenish/gflabel.git
 ```
+### VSCode Preview
+
+If you are using VSCode with the [vscode-ocp-cad-viewer][ocp-vscode] extension,
+you can add the `--vscode` flag when running `gflabel`, and the label should
+show up as a preview. This saves opening the output CAD files in a slicer or
+other viewer, and is useful when prototyping labels.
+
+[ocp-vscode]: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 
 ### Basic Examples
 
 By default, labels are written to an output file "`label.step`". You can change
 this with `-o FILENAME`. `.step`, `.stl` and `.svg` are recognised
 
 A simple, single label generation on a pred-style base:
@@ -190,14 +198,15 @@
 | &lt;number&gt;    | A gap of specific width, in mm.                                   |
 | bolt              | Variable length bolt, in the style of Printables pred-box labels.<br><br>If the requested bolt is longer than the available space, then the<br>bolt will be as large as possible with a broken thread. |
 | box               | Arbitrary width, height centered box. If height is not specified, will expand to row height. |
 | head              | Screw head with specifiable head-shape.                           |
 | hexhead           | Hexagonal screw head. Will accept drives, but not compulsory.     |
 | hexnut, nut       | Hexagonal outer profile nut with circular cutout.                 |
 | lockwasher        | Circular washer with a locking cutout.                            |
+| sym, symbol       | Render an electronic symbol.                                      |
 | threaded_insert   | Representation of a threaded insert.                              |
 | variable_resistor | Electrical symbol of a variable resistor.                         |
 | washer            | Circular washer with a circular hole.                             |
 | webbolt           | Alternate bolt representation incorporating screw drive, with fixed length. |
 
 A basic set of examples showing the usage of some of these:
 
@@ -234,9 +243,59 @@
 both can be pointed backwards by adding the `flipped` feature.
 
 Examples showing some differences between the two bolts:
 
 ![](images/bolts.svg)
 
 
+### Electronic Symbols
+
+Electronic symbols can be generated using the `{symbol(...)}` fragment.
+GFLabel is using the [Chris Pikul Electronic Symbols ][pikul] library kindly
+released under MIT Licence.
+
+[pikul]: https://github.com/chris-pikul/electronic-symbols
+
+There are currently three main approaches to selecting the symbol that you
+want:
+
+- Exact [ID][ID], or exact [Filename][files], as defined the original source.
+- Component name, as listed on the symbol source [README][pikul] (and in the
+  table below). In cases where multiple symbols have the same name, they can
+  be differentiated by standard e.g. `{symbol(capacitor,iec)}`. If standard is
+  not specified, and there are multiple matches, then the first of [`common`,
+  `iec`, `ieee`] will be chosen (if doing so makes it unambiguous).
+- Fuzzy matching. You can pass in words or parts of words. Symbols with
+  category, name or ID that match these (in any order) will be selected. If
+  more than one candidate symbols matches, then the table of possible matches
+  will be returned so that you can refine it further.
+
+You can list all of the symbols available with `gflabel --list-symbols`.
+
+For an example of this fuzzy matching, the fragment `{symbol(ground)}` isn't
+enough to disambiguate between the possible options, so the table of matches
+is printed to help you refine the definition:
+
+```
+$ gflabel '{symbol(ground)}'
+...
+Could not decide on symbol from fuzzy specification "ground". Possible options:
+    ID                 Category Name                  Standard Filename
+    ground-com-signal  GROUND   Digital/Signal Ground COMMON   Ground-COM-Signal
+    ground-com-general GROUND   Common/Earth Ground   COMMON   Ground-COM-General
+    ground-com-chassis GROUND   Chassis Ground        COMMON   Ground-COM-Chassis
+
+Could not proceed: Please specify symbol more precisely.
+```
+
+Given this, you could disambiguate by refining the fuzzy specification e.g.
+`{symbol(signal ground)}`, matching the exact name `{symbol(Common/Earth Ground)}`,
+or specifying the ID/Filename exactly: `{symbol(Ground-COM-Signal)}`.
+
+[ID]: https://github.com/chris-pikul/electronic-symbols/blob/main/manifest.json
+[files]: https://github.com/chris-pikul/electronic-symbols/tree/main/SVG
 
+Here is a table of all symbols, rendered by GFLabel, with their name as per the
+source symbol library. Note that for some of the symbols, they are rendered
+incorrectly. This is an unresolved bug in GFLabel.
 
+![](images/symbols.svg)
```

