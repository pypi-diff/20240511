# Comparing `tmp/setuptools-gettext-0.1.8.tar.gz` & `tmp/setuptools-gettext-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-gettext-0.1.8.tar", last modified: Mon Dec  4 23:26:04 2023, max compression
+gzip compressed data, was "setuptools-gettext-0.1.9.tar", last modified: Sun Jan 28 00:34:11 2024, max compression
```

## Comparing `setuptools-gettext-0.1.8.tar` & `setuptools-gettext-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,29 @@
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-12-04 23:26:04.905951 setuptools-gettext-0.1.8/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-12-04 23:26:04.901951 setuptools-gettext-0.1.8/.github/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-12-04 23:26:04.905951 setuptools-gettext-0.1.8/.github/workflows/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      188 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/.github/workflows/disperse.yml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1068 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/.github/workflows/pythontest.yml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       54 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/.gitignore
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    18092 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/COPYING
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       15 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/MANIFEST.in
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1807 2023-12-04 23:26:04.905951 setuptools-gettext-0.1.8/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      775 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/README.md
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      250 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/disperse.conf
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-12-04 23:26:04.905951 setuptools-gettext-0.1.8/example/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       40 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/example/.gitignore
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      449 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/example/README.md
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-12-04 23:26:04.905951 setuptools-gettext-0.1.8/example/hallowereld/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1116 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/example/hallowereld/__init__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       76 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/example/hallowereld/__main__.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-12-04 23:26:04.905951 setuptools-gettext-0.1.8/example/po/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      643 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/example/po/hallowereld.pot
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      746 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/example/po/nl.po
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      334 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/example/pyproject.toml
--rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)       58 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/example/setup.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2036 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/pyproject.toml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       38 2023-12-04 23:26:04.905951 setuptools-gettext-0.1.8/setup.cfg
--rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)       58 2023-12-04 23:26:00.000000 setuptools-gettext-0.1.8/setup.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-12-04 23:26:04.905951 setuptools-gettext-0.1.8/setuptools_gettext/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    11488 2023-12-04 23:26:02.000000 setuptools-gettext-0.1.8/setuptools_gettext/__init__.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2023-12-04 23:26:04.905951 setuptools-gettext-0.1.8/setuptools_gettext.egg-info/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1807 2023-12-04 23:26:04.000000 setuptools-gettext-0.1.8/setuptools_gettext.egg-info/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      649 2023-12-04 23:26:04.000000 setuptools-gettext-0.1.8/setuptools_gettext.egg-info/SOURCES.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2023-12-04 23:26:04.000000 setuptools-gettext-0.1.8/setuptools_gettext.egg-info/dependency_links.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      290 2023-12-04 23:26:04.000000 setuptools-gettext-0.1.8/setuptools_gettext.egg-info/entry_points.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       58 2023-12-04 23:26:04.000000 setuptools-gettext-0.1.8/setuptools_gettext.egg-info/requires.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       19 2023-12-04 23:26:04.000000 setuptools-gettext-0.1.8/setuptools_gettext.egg-info/top_level.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2023-12-04 23:26:04.000000 setuptools-gettext-0.1.8/setuptools_gettext.egg-info/zip-safe
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2024-01-28 00:34:11.904052 setuptools-gettext-0.1.9/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    18092 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/COPYING
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       15 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/MANIFEST.in
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1807 2024-01-28 00:34:11.904052 setuptools-gettext-0.1.9/PKG-INFO
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      775 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/README.md
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2024-01-28 00:34:11.904052 setuptools-gettext-0.1.9/example/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       40 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/example/.gitignore
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      449 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/example/README.md
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2024-01-28 00:34:11.904052 setuptools-gettext-0.1.9/example/hallowereld/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1186 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/example/hallowereld/__init__.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       76 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/example/hallowereld/__main__.py
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2024-01-28 00:34:11.904052 setuptools-gettext-0.1.9/example/po/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      643 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/example/po/hallowereld.pot
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      746 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/example/po/nl.po
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      334 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/example/pyproject.toml
+-rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)       58 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/example/setup.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2036 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/pyproject.toml
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       38 2024-01-28 00:34:11.904052 setuptools-gettext-0.1.9/setup.cfg
+-rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)       58 2024-01-28 00:34:08.000000 setuptools-gettext-0.1.9/setup.py
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2024-01-28 00:34:11.904052 setuptools-gettext-0.1.9/setuptools_gettext/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    10883 2024-01-28 00:34:10.000000 setuptools-gettext-0.1.9/setuptools_gettext/__init__.py
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2024-01-28 00:34:11.904052 setuptools-gettext-0.1.9/setuptools_gettext.egg-info/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1807 2024-01-28 00:34:11.000000 setuptools-gettext-0.1.9/setuptools_gettext.egg-info/PKG-INFO
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      560 2024-01-28 00:34:11.000000 setuptools-gettext-0.1.9/setuptools_gettext.egg-info/SOURCES.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2024-01-28 00:34:11.000000 setuptools-gettext-0.1.9/setuptools_gettext.egg-info/dependency_links.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      290 2024-01-28 00:34:11.000000 setuptools-gettext-0.1.9/setuptools_gettext.egg-info/entry_points.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       58 2024-01-28 00:34:11.000000 setuptools-gettext-0.1.9/setuptools_gettext.egg-info/requires.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       19 2024-01-28 00:34:11.000000 setuptools-gettext-0.1.9/setuptools_gettext.egg-info/top_level.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2024-01-28 00:34:11.000000 setuptools-gettext-0.1.9/setuptools_gettext.egg-info/zip-safe
```

### Comparing `setuptools-gettext-0.1.8/COPYING` & `setuptools-gettext-0.1.9/COPYING`

 * *Files identical despite different names*

### Comparing `setuptools-gettext-0.1.8/PKG-INFO` & `setuptools-gettext-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-gettext
-Version: 0.1.8
+Version: 0.1.9
 Summary: Setuptools gettext extension plugin
 Maintainer-email: Breezy Developers <breezy-core@googlegroups.com>
 Project-URL: Homepage, https://github.com/breezy-team/setuptools-gettext
 Project-URL: repository, https://github.com/breezy-team/setuptools-gettext.git
 Keywords: distutils,setuptools,gettext
 Classifier: Topic :: Software Development :: Version Control
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `setuptools-gettext-0.1.8/README.md` & `setuptools-gettext-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `setuptools-gettext-0.1.8/example/hallowereld/__init__.py` & `setuptools-gettext-0.1.9/example/hallowereld/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,26 +8,32 @@
     return _("Hello World!")
 
 
 def load_translations():
     import gettext
     import os
 
-    if os.path.exists('setup.py'):
+    if os.path.exists("setup.py"):
         # We are running from source, so we need to install the translations
         locale_dir = os.path.join(os.path.dirname(__file__), "locale")
     else:
         # Otherwise, we assume the translations are installed in the relevant
         # system directory that shares our prefix
 
         # Note that we can't just use sys.prefix, since while Python might be
         # installed in /usr, our package (and thus the translations) might be
         # in /usr/local
         locale_dir = os.path.join(
             os.path.dirname(__file__),
-            "..", "..", "..", "..", "share", "locale")
+            "..",
+            "..",
+            "..",
+            "..",
+            "share",
+            "locale",
+        )
     gettext.bindtextdomain("hallowereld", localedir=locale_dir)
     print("Loading translations from", locale_dir)
 
     # Set the default domain, so we can use gettext (or _()) instead of
     # dgettext
     gettext.textdomain("hallowereld")
```

### Comparing `setuptools-gettext-0.1.8/example/po/hallowereld.pot` & `setuptools-gettext-0.1.9/example/po/hallowereld.pot`

 * *Files identical despite different names*

### Comparing `setuptools-gettext-0.1.8/example/po/nl.po` & `setuptools-gettext-0.1.9/example/po/nl.po`

 * *Files identical despite different names*

### Comparing `setuptools-gettext-0.1.8/pyproject.toml` & `setuptools-gettext-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-gettext-0.1.8/setuptools_gettext/__init__.py` & `setuptools-gettext-0.1.9/setuptools_gettext/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,275 +20,265 @@
 
 """build_mo command for setup.py."""
 
 import logging
 import os
 import re
 import sys
+from distutils.command.install_data import install_data
 from typing import List, Optional, Tuple
 
 from setuptools import Command
 from setuptools.dist import Distribution
 
-__version__ = (0, 1, 8)
-DEFAULT_SOURCE_DIR = 'po'
-DEFAULT_BUILD_DIR = 'locale'
+__version__ = (0, 1, 9)
+DEFAULT_SOURCE_DIR = "po"
+DEFAULT_BUILD_DIR = "locale"
 
 
 def lang_from_dir(source_dir: os.PathLike) -> List[str]:
-    re_po = re.compile(r'^([a-zA-Z_]+)\.po$')
+    re_po = re.compile(r"^([a-zA-Z_]+)\.po$")
     lang = []
     for i in os.listdir(source_dir):
         mo = re_po.match(i)
         if mo:
             lang.append(mo.group(1))
     return lang
 
 
 def parse_lang(lang: str) -> List[str]:
-    return [i.strip() for i in lang.split(',') if i.strip()]
+    return [i.strip() for i in lang.split(",") if i.strip()]
 
 
 class build_mo(Command):
     """Subcommand of build command: build_mo."""
 
-    description = 'compile po files to mo files'
+    description = "compile po files to mo files"
 
     # List of options:
     #   - long name,
     #   - short name (None if no short name),
     #   - help string.
-    user_options = [('build-dir=', 'd', 'Directory to build locale files'),
-                    ('output-base=', 'o', 'mo-files base name'),
-                    ('force', 'f', 'Force creation of mo files'),
-                    ('lang=', None, 'Comma-separated list of languages '
-                                    'to process'),
-                    ]
+    user_options = [
+        ("build-dir=", "d", "Directory to build locale files"),
+        ("output-base=", "o", "mo-files base name"),
+        ("force", "f", "Force creation of mo files"),
+        ("lang=", None, "Comma-separated list of languages " "to process"),
+    ]
 
-    boolean_options = ['force']
+    boolean_options = ["force"]
 
     def initialize_options(self):
         self.build_dir = None
         self.output_base = None
         self.force = None
         self.lang = None
         self.outfiles = []
 
     def finalize_options(self):
-        self.set_undefined_options('build', ('force', 'force'))
+        self.set_undefined_options("build", ("force", "force"))
         self.prj_name = self.distribution.get_name()
         if not self.output_base:
-            self.output_base = self.prj_name or 'messages'
+            self.output_base = self.prj_name or "messages"
         self.source_dir = self.distribution.gettext_source_dir
         if self.build_dir is None:
             self.build_dir = (
-                getattr(self.distribution, 'gettext_build_dir', None)
-                or DEFAULT_BUILD_DIR)
+                getattr(self.distribution, "gettext_build_dir", None)
+                or DEFAULT_BUILD_DIR
+            )
         if self.lang is None:
             self.lang = lang_from_dir(self.source_dir)
         else:
             self.lang = parse_lang(self.lang)
 
     def get_inputs(self):
         inputs = []
         for lang in self.lang:
-            po = os.path.join(self.source_dir, lang + '.po')
+            po = os.path.join(self.source_dir, lang + ".po")
             if not os.path.isfile(po):
-                po = os.path.join(self.source_dir, lang + '.po')
+                po = os.path.join(self.source_dir, lang + ".po")
             inputs.append(po)
         return inputs
 
     def run(self):
         """Run msgfmt for each language."""
         if not self.lang:
             return
 
-        if find_executable('msgfmt') is None:
+        if find_executable("msgfmt") is None:
             logging.warn("GNU gettext msgfmt utility not found!")
             logging.warn("Skip compiling po files.")
             return
 
-        if 'en' in self.lang:
-            if find_executable('msginit') is None:
+        if "en" in self.lang:
+            if find_executable("msginit") is None:
                 logging.warn("GNU gettext msginit utility not found!")
                 logging.warn("Skip creating English PO file.")
             else:
-                logging.info('Creating English PO file...')
-                pot = (self.prj_name or 'messages') + '.pot'
-                en_po = 'en.po'
-                self.spawn(['msginit',
-                            '--no-translator',
-                            '-l', 'en',
-                            '-i', os.path.join(self.source_dir, pot),
-                            '-o', os.path.join(self.source_dir, en_po),
-                            ])
+                logging.info("Creating English PO file...")
+                pot = (self.prj_name or "messages") + ".pot"
+                en_po = "en.po"
+                self.spawn(
+                    [
+                        "msginit",
+                        "--no-translator",
+                        "-l",
+                        "en",
+                        "-i",
+                        os.path.join(self.source_dir, pot),
+                        "-o",
+                        os.path.join(self.source_dir, en_po),
+                    ]
+                )
 
         basename = self.output_base
-        if not basename.endswith('.mo'):
-            basename += '.mo'
+        if not basename.endswith(".mo"):
+            basename += ".mo"
 
         for lang in self.lang:
-            po = os.path.join(self.source_dir, lang + '.po')
+            po = os.path.join(self.source_dir, lang + ".po")
             if not os.path.isfile(po):
-                po = os.path.join(self.source_dir, lang + '.po')
-            dir_ = os.path.join(self.build_dir, lang, 'LC_MESSAGES')
+                po = os.path.join(self.source_dir, lang + ".po")
+            dir_ = os.path.join(self.build_dir, lang, "LC_MESSAGES")
             self.mkpath(dir_)
             mo = os.path.join(dir_, basename)
             if self.force or newer(po, mo):
-                logging.info(f'Compile: {po} -> {mo}')
-                self.spawn(['msgfmt', '-o', mo, po])
+                logging.info(f"Compile: {po} -> {mo}")
+                self.spawn(["msgfmt", "-o", mo, po])
                 self.outfiles.append(mo)
 
     def get_outputs(self):
         return self.outfiles
 
 
 class clean_mo(Command):
-    description = 'clean .mo files'
+    description = "clean .mo files"
 
-    user_options = [('build-dir=', 'd', 'Directory to build locale files')]
+    user_options = [("build-dir=", "d", "Directory to build locale files")]
 
     def initialize_options(self):
         self.build_dir = None
 
     def finalize_options(self):
         if self.build_dir is None:
             self.build_dir = (
-                getattr(self.distribution, 'gettext_build_dir', None)
-                or DEFAULT_BUILD_DIR)
+                getattr(self.distribution, "gettext_build_dir", None)
+                or DEFAULT_BUILD_DIR
+            )
 
     def run(self):
         if not os.path.isdir(self.build_dir):
             return
         for root, dirs, files in os.walk(self.build_dir):
             for file_ in files:
-                if file_.endswith('.mo'):
+                if file_.endswith(".mo"):
                     os.unlink(os.path.join(root, file_))
 
 
-class install_mo(Command):
-
+class install_mo(install_data):
     description: str = "install .mo files"
 
-    user_options = [
-        (
-            'install-dir=',
-            'd',
-            "base directory for installing data files "
-            "(default: installation base dir)",
-        ),
-        ('root=', None,
-         "install everything relative to this alternate root directory"),
-        ('force', 'f', "force installation (overwrite existing files)"),
-    ]
-
-    boolean_options: List[str] = ['force']
     build_dir: Optional[str]
-    install_dir: Optional[str]
-    root: Optional[str]
 
     def initialize_options(self) -> None:
-        self.install_dir = None
-        self.outfiles: List[str] = []
-        self.root = None
-        self.force = 0
+        super().initialize_options()
+        self.data_files: List[str] = []
         self.build_dir = None
 
     def finalize_options(self) -> None:
-        self.set_undefined_options(
-            'install',
-            ('install_data', 'install_dir'),
-            ('root', 'root'),
-            ('force', 'force'),
-        )
+        super().finalize_options()
         if self.build_dir is None:
-            self.build_dir = (
-                self.distribution.gettext_build_dir)  # type: ignore
+            self.build_dir = self.distribution.gettext_build_dir  # type: ignore
 
     def run(self) -> None:
         assert self.install_dir is not None
         assert self.build_dir is not None
-        self.mkpath(self.install_dir)
         import glob
+
         for filepath in glob.glob(self.build_dir + "/*/LC_MESSAGES/*.mo"):
-            langfile = filepath[len(self.build_dir.rstrip('/')+'/'):]
-            targetpath = os.path.join(
-                self.install_dir,
-                os.path.dirname(os.path.join("share/locale", langfile)))
-            if self.root is not None:
-                targetpath = change_root(self.root, targetpath)
-            self.mkpath(targetpath)
-            (out, _) = self.copy_file(filepath, targetpath)
-            self.outfiles.append(out)
+            langfile = filepath[len(self.build_dir.rstrip("/") + "/") :]
+            install_dir = os.path.dirname(
+                os.path.join("share/locale", langfile)
+            )
+            self.data_files.append((install_dir, [filepath]))  # type: ignore
+        super().run()
 
     def get_inputs(self):
         import glob
+
         return glob.glob(self.build_dir + "/*/LC_MESSAGES/*.mo")
 
     def get_outputs(self):
         return self.outfiles
 
 
 class update_pot(Command):
-
     description: str = "update the .pot file"
 
     user_options: List[Tuple[str, str, str]] = []
 
     def initialize_options(self) -> None:
         pass
 
     def finalize_options(self) -> None:
         pass
 
     def run(self) -> None:
         # TODO(jelmer): Support pygettext3 as well
-        xgettext = find_executable('xgettext')
+        xgettext = find_executable("xgettext")
         if xgettext is None:
             logging.error("GNU gettext xgettext utility not found!")
             return
         args = [xgettext]
-        args.extend([
-            "--package-name", self.distribution.get_name(),
-            "--from-code", "UTF-8",
-            "--sort-by-file",
-            "--add-comments=i18n:",
-            "-d", self.distribution.get_name(),
-            "-p", self.distribution.gettext_source_dir,  # type: ignore
-            "-o", f"{self.distribution.get_name()}.pot",
-            ])
+        args.extend(
+            [
+                "--package-name",
+                self.distribution.get_name(),
+                "--from-code",
+                "UTF-8",
+                "--sort-by-file",
+                "--add-comments=i18n:",
+                "-d",
+                self.distribution.get_name(),
+                "-p",
+                self.distribution.gettext_source_dir,  # type: ignore
+                "-o",
+                f"{self.distribution.get_name()}.pot",
+            ]
+        )
 
         input_files = []
-        for root, _dirs, files in os.walk('.'):
+        for root, _dirs, files in os.walk("."):
             for file_ in files:
-                if file_.endswith('.py'):
+                if file_.endswith(".py"):
                     input_files.append(os.path.join(root, file_))
         args.extend(input_files)
 
         pot_path = os.path.join(
-            self.distribution.gettext_source_dir, self.distribution.get_name())  # type: ignore
+            self.distribution.gettext_source_dir, self.distribution.get_name()  # type: ignore
+        )
         if os.path.exists(pot_path):
             args.append("--join")
         if self.distribution.get_contact():
             args += ["--msgid-bugs-address", self.distribution.get_contact()]
 
         self.spawn(args)
 
 
 def has_gettext(_c) -> bool:
     return os.path.isdir(DEFAULT_SOURCE_DIR)
 
 
 def pyprojecttoml_config(dist: Distribution) -> None:
     build = dist.get_command_class("build")
-    build.sub_commands.append(('build_mo', has_gettext))
+    build.sub_commands.append(("build_mo", has_gettext))
     clean = dist.get_command_class("clean")
-    clean.sub_commands.append(('clean_mo', has_gettext))
+    clean.sub_commands.append(("clean_mo", has_gettext))
     install = dist.get_command_class("install")
-    install.sub_commands.append(('install_mo', has_gettext))
+    install.sub_commands.append(("install_mo", has_gettext))
 
     if sys.version_info[:2] >= (3, 11):
         from tomllib import load as toml_load
     else:
         from tomli import load as toml_load
     try:
         with open("pyproject.toml", "rb") as f:
@@ -300,28 +290,30 @@
             load_pyproject_config(dist, cfg)
         else:
             load_pyproject_config(dist, {})
 
 
 def load_pyproject_config(dist: Distribution, cfg) -> None:
     dist.gettext_source_dir = (  # type: ignore
-        cfg.get("source_dir") or DEFAULT_SOURCE_DIR)
+        cfg.get("source_dir") or DEFAULT_SOURCE_DIR
+    )
     dist.gettext_build_dir = (  # type: ignore
-        cfg.get("build_dir") or DEFAULT_BUILD_DIR)
+        cfg.get("build_dir") or DEFAULT_BUILD_DIR
+    )
 
 
 def find_executable(executable):
     _, ext = os.path.splitext(executable)
-    if sys.platform == 'win32' and ext != '.exe':
-        executable = executable + '.exe'
+    if sys.platform == "win32" and ext != ".exe":
+        executable = executable + ".exe"
 
     if os.path.isfile(executable):
         return executable
 
-    path = os.environ.get('PATH', os.defpath)
+    path = os.environ.get("PATH", os.defpath)
 
     # PATH='' doesn't match, whereas PATH=':' looks in the current directory
     if not path:
         return None
 
     paths = path.split(os.pathsep)
     for p in paths:
@@ -340,19 +332,19 @@
     mtime1 = os.stat(source)[ST_MTIME]
     mtime2 = os.stat(target)[ST_MTIME]
 
     return mtime1 > mtime2
 
 
 def change_root(new_root, pathname):
-    if os.name == 'posix':
+    if os.name == "posix":
         if not os.path.isabs(pathname):
             return os.path.join(new_root, pathname)
         else:
             return os.path.join(new_root, pathname[1:])
-    elif os.name == 'nt':
+    elif os.name == "nt":
         (drive, path) = os.path.splitdrive(pathname)
-        if path[0] == '\\':
+        if path[0] == "\\":
             path = path[1:]
         return os.path.join(new_root, path)
     else:
         raise AssertionError("Unsupported OS: %s" % os.name)
```

### Comparing `setuptools-gettext-0.1.8/setuptools_gettext.egg-info/PKG-INFO` & `setuptools-gettext-0.1.9/setuptools_gettext.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-gettext
-Version: 0.1.8
+Version: 0.1.9
 Summary: Setuptools gettext extension plugin
 Maintainer-email: Breezy Developers <breezy-core@googlegroups.com>
 Project-URL: Homepage, https://github.com/breezy-team/setuptools-gettext
 Project-URL: repository, https://github.com/breezy-team/setuptools-gettext.git
 Keywords: distutils,setuptools,gettext
 Classifier: Topic :: Software Development :: Version Control
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `setuptools-gettext-0.1.8/setuptools_gettext.egg-info/SOURCES.txt` & `setuptools-gettext-0.1.9/setuptools_gettext.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-.gitignore
 COPYING
 MANIFEST.in
 README.md
-disperse.conf
 pyproject.toml
 setup.py
-.github/workflows/disperse.yml
-.github/workflows/pythontest.yml
 example/.gitignore
 example/README.md
 example/pyproject.toml
 example/setup.py
 example/hallowereld/__init__.py
 example/hallowereld/__main__.py
 example/po/hallowereld.pot
```

