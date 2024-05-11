# Comparing `tmp/mkdoxy-1.2.3.tar.gz` & `tmp/mkdoxy-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdoxy-1.2.3.tar", last modified: Wed May  1 09:18:55 2024, max compression
+gzip compressed data, was "mkdoxy-1.2.4.tar", last modified: Sat May 11 14:55:02 2024, max compression
```

## Comparing `mkdoxy-1.2.3.tar` & `mkdoxy-1.2.4.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-01 09:18:55.291480 mkdoxy-1.2.3/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.2.3/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     5843 2024-05-01 09:18:55.291229 mkdoxy-1.2.3/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     4473 2024-04-18 23:45:18.000000 mkdoxy-1.2.3/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-01 09:18:55.285937 mkdoxy-1.2.3/mkdoxy/
--rw-r--r--   0 kuba       (501) staff       (20)     2935 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/DoxyTagParser.py
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.2.3/mkdoxy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      303 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/cache.py
--rw-r--r--   0 kuba       (501) staff       (20)     3585 2024-04-19 08:51:39.000000 mkdoxy-1.2.3/mkdoxy/constants.py
--rw-r--r--   0 kuba       (501) staff       (20)     5619 2024-04-18 23:46:38.000000 mkdoxy-1.2.3/mkdoxy/doxygen.py
--rw-r--r--   0 kuba       (501) staff       (20)     9806 2024-05-01 08:49:31.000000 mkdoxy-1.2.3/mkdoxy/doxyrun.py
--rw-r--r--   0 kuba       (501) staff       (20)      603 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/mkdoxy/filters.py
--rw-r--r--   0 kuba       (501) staff       (20)     2414 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/finder.py
--rw-r--r--   0 kuba       (501) staff       (20)    13298 2024-04-18 23:45:14.000000 mkdoxy-1.2.3/mkdoxy/generatorAuto.py
--rw-r--r--   0 kuba       (501) staff       (20)    20151 2024-05-01 09:14:08.000000 mkdoxy-1.2.3/mkdoxy/generatorBase.py
--rw-r--r--   0 kuba       (501) staff       (20)    15506 2024-05-01 09:11:13.000000 mkdoxy-1.2.3/mkdoxy/generatorSnippets.py
--rw-r--r--   0 kuba       (501) staff       (20)     5320 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/mkdoxy/markdown.py
--rw-r--r--   0 kuba       (501) staff       (20)    26618 2024-04-18 23:46:44.000000 mkdoxy-1.2.3/mkdoxy/node.py
--rw-r--r--   0 kuba       (501) staff       (20)     8941 2024-05-01 08:49:31.000000 mkdoxy-1.2.3/mkdoxy/plugin.py
--rw-r--r--   0 kuba       (501) staff       (20)    11689 2024-04-18 23:46:45.000000 mkdoxy-1.2.3/mkdoxy/property.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-01 09:18:55.289900 mkdoxy-1.2.3/mkdoxy/templates/
--rw-r--r--   0 kuba       (501) staff       (20)      517 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/annotated.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      380 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/classes.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      544 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/code.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      614 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/error.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      214 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/mkdoxy/templates/example.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      582 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/examples.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      408 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/files.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      499 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/hierarchy.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      438 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/index.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      797 2024-04-18 23:45:18.000000 mkdoxy-1.2.3/mkdoxy/templates/memDef.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     1698 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/memTab.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     4673 2024-04-18 23:45:14.000000 mkdoxy-1.2.3/mkdoxy/templates/member.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      426 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/modules.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      414 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/namespaces.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      272 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/mkdoxy/templates/page.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      465 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/mkdoxy/templates/programlisting.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      233 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/relatedPages.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     3534 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/utils.py
--rw-r--r--   0 kuba       (501) staff       (20)     9999 2024-04-18 23:46:47.000000 mkdoxy-1.2.3/mkdoxy/xml_parser.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-01 09:18:55.290388 mkdoxy-1.2.3/mkdoxy.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     5843 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/PKG-INFO
--rwxr-xr-x   0 kuba       (501) staff       (20)     1127 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/SOURCES.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        1 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/dependency_links.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       47 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/entry_points.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)      143 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/requires.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        7 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       62 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/pyproject.toml
--rw-r--r--   0 kuba       (501) staff       (20)       38 2024-05-01 09:18:55.291518 mkdoxy-1.2.3/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1841 2024-05-01 09:15:31.000000 mkdoxy-1.2.3/setup.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-01 09:18:55.290115 mkdoxy-1.2.3/tests/
--rw-r--r--   0 kuba       (501) staff       (20)     2390 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/tests/test_doxyrun.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-11 14:55:02.752738 mkdoxy-1.2.4/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.2.4/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     5843 2024-05-11 14:55:02.752259 mkdoxy-1.2.4/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     4473 2024-04-18 23:45:18.000000 mkdoxy-1.2.4/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-11 14:55:02.743158 mkdoxy-1.2.4/mkdoxy/
+-rw-r--r--   0 kuba       (501) staff       (20)     2935 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/DoxyTagParser.py
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.2.4/mkdoxy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      303 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/cache.py
+-rw-r--r--   0 kuba       (501) staff       (20)     3585 2024-04-19 08:51:39.000000 mkdoxy-1.2.4/mkdoxy/constants.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5655 2024-05-11 14:49:57.000000 mkdoxy-1.2.4/mkdoxy/doxygen.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9806 2024-05-01 08:49:31.000000 mkdoxy-1.2.4/mkdoxy/doxyrun.py
+-rw-r--r--   0 kuba       (501) staff       (20)      603 2024-04-03 00:10:24.000000 mkdoxy-1.2.4/mkdoxy/filters.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2414 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/finder.py
+-rw-r--r--   0 kuba       (501) staff       (20)    13298 2024-04-18 23:45:14.000000 mkdoxy-1.2.4/mkdoxy/generatorAuto.py
+-rw-r--r--   0 kuba       (501) staff       (20)    20151 2024-05-01 09:14:08.000000 mkdoxy-1.2.4/mkdoxy/generatorBase.py
+-rw-r--r--   0 kuba       (501) staff       (20)    15318 2024-05-11 14:49:57.000000 mkdoxy-1.2.4/mkdoxy/generatorSnippets.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5320 2024-04-03 00:10:24.000000 mkdoxy-1.2.4/mkdoxy/markdown.py
+-rw-r--r--   0 kuba       (501) staff       (20)    26606 2024-05-11 14:49:57.000000 mkdoxy-1.2.4/mkdoxy/node.py
+-rw-r--r--   0 kuba       (501) staff       (20)     8941 2024-05-01 08:49:31.000000 mkdoxy-1.2.4/mkdoxy/plugin.py
+-rw-r--r--   0 kuba       (501) staff       (20)      162 2024-05-11 14:49:57.000000 mkdoxy-1.2.4/mkdoxy/project.py
+-rw-r--r--   0 kuba       (501) staff       (20)    11689 2024-04-18 23:46:45.000000 mkdoxy-1.2.4/mkdoxy/property.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-11 14:55:02.749840 mkdoxy-1.2.4/mkdoxy/templates/
+-rw-r--r--   0 kuba       (501) staff       (20)      517 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/templates/annotated.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      380 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/templates/classes.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      544 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/templates/code.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      614 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/templates/error.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      214 2024-04-03 00:10:24.000000 mkdoxy-1.2.4/mkdoxy/templates/example.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      582 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/templates/examples.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      408 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/templates/files.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      499 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/templates/hierarchy.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      438 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/templates/index.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      797 2024-04-18 23:45:18.000000 mkdoxy-1.2.4/mkdoxy/templates/memDef.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     1753 2024-05-11 14:49:57.000000 mkdoxy-1.2.4/mkdoxy/templates/memTab.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     4673 2024-04-18 23:45:14.000000 mkdoxy-1.2.4/mkdoxy/templates/member.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      426 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/templates/modules.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      414 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/templates/namespaces.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      272 2024-04-03 00:10:24.000000 mkdoxy-1.2.4/mkdoxy/templates/page.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      465 2024-04-03 00:10:24.000000 mkdoxy-1.2.4/mkdoxy/templates/programlisting.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      233 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/templates/relatedPages.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     3534 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/mkdoxy/utils.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9999 2024-04-18 23:46:47.000000 mkdoxy-1.2.4/mkdoxy/xml_parser.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-11 14:55:02.750695 mkdoxy-1.2.4/mkdoxy.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     5843 2024-05-11 14:55:02.000000 mkdoxy-1.2.4/mkdoxy.egg-info/PKG-INFO
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1145 2024-05-11 14:55:02.000000 mkdoxy-1.2.4/mkdoxy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        1 2024-05-11 14:55:02.000000 mkdoxy-1.2.4/mkdoxy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)       47 2024-05-11 14:55:02.000000 mkdoxy-1.2.4/mkdoxy.egg-info/entry_points.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)      143 2024-05-11 14:55:02.000000 mkdoxy-1.2.4/mkdoxy.egg-info/requires.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        7 2024-05-11 14:55:02.000000 mkdoxy-1.2.4/mkdoxy.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       62 2024-04-02 23:57:40.000000 mkdoxy-1.2.4/pyproject.toml
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2024-05-11 14:55:02.752844 mkdoxy-1.2.4/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1841 2024-05-11 14:53:51.000000 mkdoxy-1.2.4/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-11 14:55:02.750216 mkdoxy-1.2.4/tests/
+-rw-r--r--   0 kuba       (501) staff       (20)     2390 2024-04-03 00:10:24.000000 mkdoxy-1.2.4/tests/test_doxyrun.py
```

### Comparing `mkdoxy-1.2.3/LICENSE` & `mkdoxy-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/PKG-INFO` & `mkdoxy-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.2.3
+Version: 1.2.4
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.3 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.4 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
```

### Comparing `mkdoxy-1.2.3/README.md` & `mkdoxy-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/DoxyTagParser.py` & `mkdoxy-1.2.4/mkdoxy/DoxyTagParser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/constants.py` & `mkdoxy-1.2.4/mkdoxy/constants.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/doxygen.py` & `mkdoxy-1.2.4/mkdoxy/doxygen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,85 @@
 import logging
 import os
 from xml.etree import ElementTree
 
 from mkdoxy.cache import Cache
 from mkdoxy.constants import Kind, Visibility
 from mkdoxy.node import Node
+from mkdoxy.project import ProjectContext
 from mkdoxy.xml_parser import XmlParser
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 
 class Doxygen:
     def __init__(self, index_path: str, parser: XmlParser, cache: Cache):
         self.debug = parser.debug
         path_xml = os.path.join(index_path, "index.xml")
         if self.debug:
             log.info(f"Loading XML from: {path_xml}")
         xml = ElementTree.parse(path_xml).getroot()
 
         self.parser = parser
-        self.cache = cache
+        self.ctx = ProjectContext(cache)
 
-        self.root = Node("root", None, self.cache, self.parser, None)
-        self.groups = Node("root", None, self.cache, self.parser, None)
-        self.files = Node("root", None, self.cache, self.parser, None)
-        self.pages = Node("root", None, self.cache, self.parser, None)
-        self.examples = Node("root", None, self.cache, self.parser, None)
+        self.root = Node("root", None, self.ctx, self.parser, None)
+        self.groups = Node("root", None, self.ctx, self.parser, None)
+        self.files = Node("root", None, self.ctx, self.parser, None)
+        self.pages = Node("root", None, self.ctx, self.parser, None)
+        self.examples = Node("root", None, self.ctx, self.parser, None)
 
         for compound in xml.findall("compound"):
             kind = Kind.from_str(compound.get("kind"))
             refid = compound.get("refid")
             if kind.is_language():
                 node = Node(
                     os.path.join(index_path, f"{refid}.xml"),
                     None,
-                    self.cache,
+                    self.ctx,
                     self.parser,
                     self.root,
                 )
                 node._visibility = Visibility.PUBLIC
                 self.root.add_child(node)
             if kind == Kind.GROUP:
                 node = Node(
                     os.path.join(index_path, f"{refid}.xml"),
                     None,
-                    self.cache,
+                    self.ctx,
                     self.parser,
                     self.root,
                 )
                 node._visibility = Visibility.PUBLIC
                 self.groups.add_child(node)
             if kind in [Kind.FILE, Kind.DIR]:
                 node = Node(
                     os.path.join(index_path, f"{refid}.xml"),
                     None,
-                    self.cache,
+                    self.ctx,
                     self.parser,
                     self.root,
                 )
                 node._visibility = Visibility.PUBLIC
                 self.files.add_child(node)
             if kind == Kind.PAGE:
                 node = Node(
                     os.path.join(index_path, f"{refid}.xml"),
                     None,
-                    self.cache,
+                    self.ctx,
                     self.parser,
                     self.root,
                 )
                 node._visibility = Visibility.PUBLIC
                 self.pages.add_child(node)
             if kind == Kind.EXAMPLE:
                 node = Node(
                     os.path.join(index_path, f"{refid}.xml"),
                     None,
-                    self.cache,
+                    self.ctx,
                     self.parser,
                     self.root,
                 )
                 node._visibility = Visibility.PUBLIC
                 self.examples.add_child(node)
 
         if self.debug:
```

### Comparing `mkdoxy-1.2.3/mkdoxy/doxyrun.py` & `mkdoxy-1.2.4/mkdoxy/doxyrun.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/filters.py` & `mkdoxy-1.2.4/mkdoxy/filters.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/finder.py` & `mkdoxy-1.2.4/mkdoxy/finder.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/generatorAuto.py` & `mkdoxy-1.2.4/mkdoxy/generatorAuto.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/generatorBase.py` & `mkdoxy-1.2.4/mkdoxy/generatorBase.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/generatorSnippets.py` & `mkdoxy-1.2.4/mkdoxy/generatorSnippets.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,32 +148,30 @@
         )
 
     def incorrect_argument(self, project: str, argument: str, config: dict, snippet: str) -> str:
         return self.doxyError(
             project,
             config,
             f"Incorrect argument: {argument}" if argument else f"Add argument to snippet: {project}",
-            f"Argument have to be based on this diagram → **:::doxy.{project}.<argument\>**",
+            f"Argument have to be based on this diagram → **:::doxy.{project}.<argument\\>**",
             "A list of available arguments:",
             "\n".join(self.doxy_arguments.keys()),
             "yaml",
             snippet,
         )
 
     def replace_markdown(self, start: int, end: int, replacement: str):
         self.markdown = self.markdown[:start] + replacement + "\n" + self.markdown[end:]
 
-    def _recurs_setLinkPrefixNode(self, node: Node, linkPrefix: str):
-        node.setLinkPrefix(linkPrefix)
-        if node.kind.is_parent():
-            self._recurs_setLinkPrefixNodes(node.children, linkPrefix)
-
-    def _recurs_setLinkPrefixNodes(self, nodes: [Node], linkPrefix: str):
-        for node in nodes:
-            self._recurs_setLinkPrefixNode(node, linkPrefix)
+    def _setLinkPrefixNode(self, node: Node, linkPrefix: str):
+        node.project.linkPrefix = linkPrefix
+
+    def _setLinkPrefixNodes(self, nodes: list[Node], linkPrefix: str):
+        if nodes:
+            nodes[0].project.linkPrefix = linkPrefix
 
     def is_project_exist(self, project: str):
         return project in self.projects
 
     def is_doxy_inactive(self, config: dict):
         return config.get("disable_doxy_snippets", False)
 
@@ -245,15 +243,15 @@
                 return self.doxyError(
                     project,
                     config,
                     f"Parameter start: {config.get('start')} is greater than end: {config.get('end')}",
                     f"{snippet}",
                     "yaml",
                 )
-            self._recurs_setLinkPrefixNode(node, self.pageUrlPrefix + project + "/")
+            self._setLinkPrefixNode(node, self.pageUrlPrefix + project + "/")
             return self.generatorBase[project].code(node, config, progCode)
         return self.doxyError(
             project,
             config,
             f"Did not find File: `{config.get('file')}`",
             "Check your file name",
             f"Available files in {project} project:",
@@ -277,15 +275,15 @@
             return errorMsg
 
         node = self.finder.doxyFunction(project, config.get("name"))
         if node is None:
             return self.doxyNodeIsNone(project, config, snippet)
 
         if isinstance(node, Node):
-            self._recurs_setLinkPrefixNode(node, self.pageUrlPrefix + project + "/")
+            self._setLinkPrefixNode(node, self.pageUrlPrefix + project + "/")
             return self.generatorBase[project].function(node, config)
         return self.doxyError(
             project,
             config,
             "Incorrect function configuration",
             f"Did not find Function with name: `{config.get('name')}`",
             "Available functions:",
@@ -300,15 +298,15 @@
             return errorMsg
 
         node = self.finder.doxyClass(project, config.get("name"))
         if node is None:
             return self.doxyNodeIsNone(project, config, snippet)
 
         if isinstance(node, Node):
-            self._recurs_setLinkPrefixNode(node, self.pageUrlPrefix + project + "/")
+            self._setLinkPrefixNode(node, self.pageUrlPrefix + project + "/")
             return self.generatorBase[project].member(node, config)
         return self.doxyError(
             project,
             config,
             "Incorrect class configuration",
             f"Did not find Class with name: `{config.get('name')}`",
             "Available classes:",
@@ -323,15 +321,15 @@
             return errorMsg
 
         node = self.finder.doxyClassMethod(project, config.get("name"), config.get("method"))
         if node is None:
             return self.doxyNodeIsNone(project, config, snippet)
 
         if isinstance(node, Node):
-            self._recurs_setLinkPrefixNode(node, self.pageUrlPrefix + project + "/")
+            self._setLinkPrefixNode(node, self.pageUrlPrefix + project + "/")
             return self.generatorBase[project].function(node, config)
         return self.doxyError(
             project,
             config,
             "Incorrect class method configuration",
             f"Did not find Class with name: `{config.get('name')}` and method: `{config.get('method')}`",
             "Available classes and methods:",
@@ -341,47 +339,47 @@
         )
 
     def doxyClassList(self, snippet, project: str, config):
         errorMsg = self.checkConfig(snippet, project, config, [])
         if errorMsg:
             return errorMsg
         nodes = self.doxygen[project].root.children
-        self._recurs_setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
+        self._setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
         return self.generatorBase[project].annotated(nodes, config)
 
     def doxyClassIndex(self, snippet, project: str, config):
         errorMsg = self.checkConfig(snippet, project, config, [])
         if errorMsg:
             return errorMsg
         nodes = self.doxygen[project].root.children
-        self._recurs_setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
+        self._setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
         return self.generatorBase[project].classes(nodes, config)
 
     def doxyClassHierarchy(self, snippet, project: str, config):
         errorMsg = self.checkConfig(snippet, project, config, [])
         if errorMsg:
             return errorMsg
         nodes = self.doxygen[project].root.children
-        self._recurs_setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
+        self._setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
         return self.generatorBase[project].hierarchy(nodes, config)
 
     def doxyNamespaceList(self, snippet, project: str, config):
         errorMsg = self.checkConfig(snippet, project, config, [])
         if errorMsg:
             return errorMsg
         nodes = self.doxygen[project].root.children
-        self._recurs_setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
+        self._setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
         return self.generatorBase[project].namespaces(nodes, config)
 
     def doxyFileList(self, snippet, project: str, config):
         errorMsg = self.checkConfig(snippet, project, config, [])
         if errorMsg:
             return errorMsg
         nodes = self.doxygen[project].files.children
-        self._recurs_setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
+        self._setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
         return self.generatorBase[project].fileindex(nodes, config)
 
     def doxyNodeIsNone(self, project: str, config: dict, snippet: str) -> str:
         return self.doxyError(
             project,
             config,
             f"Could not find coresponding snippet for project {project}",
```

### Comparing `mkdoxy-1.2.3/mkdoxy/markdown.py` & `mkdoxy-1.2.4/mkdoxy/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/node.py` & `mkdoxy-1.2.4/mkdoxy/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import logging
 import os
 from xml.etree import ElementTree
 from xml.etree.ElementTree import Element as Element
 
-from mkdoxy.cache import Cache
 from mkdoxy.constants import OVERLOAD_OPERATORS, Kind, Visibility
 from mkdoxy.markdown import escape
+from mkdoxy.project import ProjectContext
 from mkdoxy.property import Property
 from mkdoxy.utils import split_safe
 from mkdoxy.xml_parser import XmlParser
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 
 class Node:
     def __init__(
         self,
         xml_file: str,
         xml: Element,
-        cache: Cache,
+        project: ProjectContext,
         parser: XmlParser,
         parent: "Node",
         refid: str = None,
         debug: bool = False,
     ):
         self._children: ["Node"] = []
-        self._cache: Cache = cache
+        self._cache = project.cache
         self._parser: XmlParser = parser
         self._parent = parent
         self.debug = debug
-        self.linkPrefix = ""
+        self.project = project
 
         if xml_file == "root":
             self._refid = "root"
             self._kind = Kind.from_str("root")
             self._name = "root"
             self._xml = None
 
@@ -87,17 +87,14 @@
         self._initializer = Property.Initializer(self._xml, parser, self._kind)
         self._definition = Property.Definition(self._xml, parser, self._kind)
         self._programlisting = Property.Programlisting(self._xml, parser, self._kind)
 
     def __repr__(self):
         return f"Node: {self.name} refid: {self._refid}"
 
-    def setLinkPrefix(self, linkPrefix: str):
-        self.linkPrefix = linkPrefix
-
     def add_child(self, child: "Node"):
         self._children.append(child)
 
     def sort_children(self):
         self._children.sort(key=lambda x: x._name, reverse=False)
 
     def _check_for_children(self):
@@ -109,15 +106,15 @@
                     self.add_child(child)
                     continue
                 except Exception:
                     pass
             child = Node(
                 os.path.join(self._dirname, f"{refid}.xml"),
                 None,
-                self._cache,
+                self.project,
                 self._parser,
                 self,
             )
             child._visibility = Visibility.PUBLIC
             self.add_child(child)
 
         for innerclass in self._xml.findall("innerclass"):
@@ -134,23 +131,23 @@
                 except Exception:
                     pass
 
             try:
                 child = Node(
                     os.path.join(self._dirname, f"{refid}.xml"),
                     None,
-                    self._cache,
+                    self.project,
                     self._parser,
                     self,
                 )
             except FileNotFoundError:
                 child = Node(
                     os.path.join(self._dirname, f"{refid}.xml"),
                     Element("compounddef"),
-                    self._cache,
+                    self.project,
                     self._parser,
                     self,
                     refid=refid,
                 )
                 child._name = innerclass.text
             child._visibility = prot
             self.add_child(child)
@@ -164,15 +161,15 @@
                     continue
                 except Exception:
                     pass
 
             child = Node(
                 os.path.join(self._dirname, f"{refid}.xml"),
                 None,
-                self._cache,
+                self.project,
                 self._parser,
                 self,
             )
             child._visibility = Visibility.PUBLIC
             self.add_child(child)
 
         for innerdir in self._xml.findall("innerdir"):
@@ -184,15 +181,15 @@
                     continue
                 except Exception:
                     pass
 
             child = Node(
                 os.path.join(self._dirname, f"{refid}.xml"),
                 None,
-                self._cache,
+                self.project,
                 self._parser,
                 self,
             )
             child._visibility = Visibility.PUBLIC
             self.add_child(child)
 
         for innernamespace in self._xml.findall("innernamespace"):
@@ -205,15 +202,15 @@
                     continue
                 except Exception:
                     pass
 
             child = Node(
                 os.path.join(self._dirname, f"{refid}.xml"),
                 None,
-                self._cache,
+                self.project,
                 self._parser,
                 self,
             )
             child._visibility = Visibility.PUBLIC
             self.add_child(child)
 
         for sectiondef in self._xml.findall("sectiondef"):
@@ -224,15 +221,15 @@
                         refid = memberdef.get("id")
                         try:
                             child = self._cache.get(refid)
                             self.add_child(child)
                             continue
                         except Exception:
                             pass
-                    child = Node(None, memberdef, self._cache, self._parser, self)
+                    child = Node(None, memberdef, self.project, self._parser, self)
                     self.add_child(child)
 
         # for detaileddescription in self._xml.findall('detaileddescription'):
         # 	for para in detaileddescription.findall('para'):
         # 		for programlisting in para.findall('programlisting'):
         # 			pass
 
@@ -473,22 +470,22 @@
         if name.startswith("-"):
             name = name[1:]
         return f"{self._kind.value}-{name}"
 
     @property
     def url(self) -> str:
         if self.is_parent or self.is_group or self.is_file or self.is_dir or self.is_page:
-            return self.linkPrefix + self._refid + ".md"
+            return self.project.linkPrefix + self._refid + ".md"
         else:
             return f"{self._parent.url}#{self.anchor}"
 
     @property
     def base_url(self) -> str:
         def prefix(page: str):
-            return self.linkPrefix + page
+            return self.project.linkPrefix + page
 
         if self.is_group:
             return prefix("modules.md")
         elif self.is_file or self.is_dir:
             return prefix("files.md")
         elif self.is_namespace:
             return prefix("namespaces.md")
@@ -505,21 +502,21 @@
             return "Namespace List"
         else:
             return "ClassList"
 
     @property
     def url_source(self) -> str:
         if self.is_parent or self.is_group or self.is_file or self.is_dir:
-            return self.linkPrefix + self._refid + "_source.md"
+            return self.project.linkPrefix + self._refid + "_source.md"
         else:
-            return self.linkPrefix + self._refid + ".md"
+            return self.project.linkPrefix + self._refid + ".md"
 
     @property
     def filename(self) -> str:
-        return self.linkPrefix + self._refid + ".md"
+        return self.project.linkPrefix + self._refid + ".md"
 
     @property
     def root(self) -> "Node":
         return self if self._kind == Kind.ROOT else self._parent.root
 
     @property
     def name_tokens(self) -> [str]:
```

### Comparing `mkdoxy-1.2.3/mkdoxy/plugin.py` & `mkdoxy-1.2.4/mkdoxy/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/property.py` & `mkdoxy-1.2.4/mkdoxy/property.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/templates/annotated.jinja2` & `mkdoxy-1.2.4/mkdoxy/templates/annotated.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/templates/code.jinja2` & `mkdoxy-1.2.4/mkdoxy/templates/code.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/templates/error.jinja2` & `mkdoxy-1.2.4/mkdoxy/templates/error.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/templates/examples.jinja2` & `mkdoxy-1.2.4/mkdoxy/templates/examples.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/templates/memDef.jinja2` & `mkdoxy-1.2.4/mkdoxy/templates/memDef.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/templates/memTab.jinja2` & `mkdoxy-1.2.4/mkdoxy/templates/memTab.jinja2`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 {%- elif member.is_dir -%}
 | dir | [**{{member.name_short}}**]({{member.url}}) {{member.suffix}}<br>{{member.brief}} |
 {%- elif member.is_namespace -%}
 | {{member.kind.value}} | [**{{member.name_long if node.is_group else member.name_short}}**]({{member.url}}) {{member.suffix}}<br>{{member.brief}} |
 {%- elif member.is_class or member.is_interface or member.is_struct -%}
 | {{member.kind.value}} | [**{{member.name_long if node.is_group else member.name_short}}**]({{member.url}}) {{member.suffix}}<br>{{member.brief}} |
 {%- elif member.is_enum or member.is_function or member.is_variable or member.is_union or member.is_typedef -%}
-| {{member.prefix}} {{member.type}} | [**{{member.name_long if node.is_group else member.name_short}}**](#{{member.anchor}}) {{member.params}} {{member.suffix}}<br>{{member.brief}} |
+| {{member.prefix}} {{member.type}} | [**{{member.name_long if node.is_group else member.name_short}}**]({%- if parent %}{{member.url}}{%- else -%}#{{member.anchor}}{%- endif -%}) {{member.params}} {{member.suffix}}<br>{{member.brief}} |
 {%- else -%}
 | {{member.prefix}} {{member.type}} | [**{{member.name_long if node.is_group else member.name_short}}**]({{member.url}}) {{member.params}} {{member.suffix}}<br>{{member.brief}} |
 {%- endif %}
 {% endfor -%}
 
 {%- endif -%}
```

### Comparing `mkdoxy-1.2.3/mkdoxy/templates/member.jinja2` & `mkdoxy-1.2.4/mkdoxy/templates/member.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/utils.py` & `mkdoxy-1.2.4/mkdoxy/utils.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy/xml_parser.py` & `mkdoxy-1.2.4/mkdoxy/xml_parser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.3/mkdoxy.egg-info/PKG-INFO` & `mkdoxy-1.2.4/mkdoxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.2.3
+Version: 1.2.4
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.3 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.4 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
```

### Comparing `mkdoxy-1.2.3/mkdoxy.egg-info/SOURCES.txt` & `mkdoxy-1.2.4/mkdoxy.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 mkdoxy/finder.py
 mkdoxy/generatorAuto.py
 mkdoxy/generatorBase.py
 mkdoxy/generatorSnippets.py
 mkdoxy/markdown.py
 mkdoxy/node.py
 mkdoxy/plugin.py
+mkdoxy/project.py
 mkdoxy/property.py
 mkdoxy/utils.py
 mkdoxy/xml_parser.py
 mkdoxy.egg-info/PKG-INFO
 mkdoxy.egg-info/SOURCES.txt
 mkdoxy.egg-info/dependency_links.txt
 mkdoxy.egg-info/entry_points.txt
```

### Comparing `mkdoxy-1.2.3/setup.py` & `mkdoxy-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 # https://pypi.org/project/mkdoxy/
 setup(
     name="mkdoxy",
-    version="1.2.3",
+    version="1.2.4",
     description="MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords="mkdoxy, python, open-source, documentation, mkdocs, doxygen, multilanguage, code-snippets, code, snippets, documentation-generator",  # noqa: E501
     url="https://github.com/JakubAndrysek/MkDoxy",
     author="Jakub Andrýsek",
     author_email="email@kubaandrysek.cz",
```

### Comparing `mkdoxy-1.2.3/tests/test_doxyrun.py` & `mkdoxy-1.2.4/tests/test_doxyrun.py`

 * *Files identical despite different names*

