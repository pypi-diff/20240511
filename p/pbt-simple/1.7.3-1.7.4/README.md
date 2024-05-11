# Comparing `tmp/pbt_simple-1.7.3.tar.gz` & `tmp/pbt_simple-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbt_simple-1.7.3.tar", max compression
+gzip compressed data, was "pbt_simple-1.7.4.tar", max compression
```

## Comparing `pbt_simple-1.7.3.tar` & `pbt_simple-1.7.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/LICENSE
--rw-r--r--   0        0        0      178 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/README.md
--rw-r--r--   0        0        0      952 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/__init__.py
--rw-r--r--   0        0        0     1224 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/__main__.py
--rw-r--r--   0        0        0        0 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/commands/__init__.py
--rw-r--r--   0        0        0     2684 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/commands/build.py
--rw-r--r--   0        0        0     1550 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/commands/git.py
--rw-r--r--   0        0        0    16053 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/commands/install.py
--rw-r--r--   0        0        0     1209 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/commands/list.py
--rw-r--r--   0        0        0     6874 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/config.py
--rw-r--r--   0        0        0     5611 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/misc.py
--rw-r--r--   0        0        0        0 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/package/__init__.py
--rw-r--r--   0        0        0    12017 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/package/discovery.py
--rw-r--r--   0        0        0     3452 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/package/graph.py
--rw-r--r--   0        0        0     6853 2024-04-07 21:33:41.736920 pbt_simple-1.7.3/sbt/package/package.py
--rw-r--r--   0        0        0        0 2024-04-07 21:33:41.740920 pbt_simple-1.7.3/sbt/registry/__init__.py
--rw-r--r--   0        0        0     2834 2024-04-07 21:33:41.740920 pbt_simple-1.7.3/sbt/registry/pypi.py
--rw-r--r--   0        0        0      434 2024-04-07 21:33:41.740920 pbt_simple-1.7.3/sbt/registry/registry.py
--rw-r--r--   0        0        0        0 2024-04-07 21:33:41.740920 pbt_simple-1.7.3/sbt/vcs/__init__.py
--rw-r--r--   0        0        0    10514 2024-04-07 21:33:41.740920 pbt_simple-1.7.3/sbt/vcs/git.py
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 pbt_simple-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/LICENSE
+-rw-r--r--   0        0        0      178 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/README.md
+-rw-r--r--   0        0        0      952 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/__init__.py
+-rw-r--r--   0        0        0     1224 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/commands/__init__.py
+-rw-r--r--   0        0        0     2693 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/commands/build.py
+-rw-r--r--   0        0        0     1550 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/commands/git.py
+-rw-r--r--   0        0        0    16253 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/commands/install.py
+-rw-r--r--   0        0        0     1209 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/commands/list.py
+-rw-r--r--   0        0        0     6874 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/config.py
+-rw-r--r--   0        0        0     5611 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/misc.py
+-rw-r--r--   0        0        0        0 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/package/__init__.py
+-rw-r--r--   0        0        0    12169 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/package/discovery.py
+-rw-r--r--   0        0        0     3452 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/package/graph.py
+-rw-r--r--   0        0        0     7100 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/package/package.py
+-rw-r--r--   0        0        0        0 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/registry/__init__.py
+-rw-r--r--   0        0        0     2834 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/registry/pypi.py
+-rw-r--r--   0        0        0      434 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/registry/registry.py
+-rw-r--r--   0        0        0        0 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/vcs/__init__.py
+-rw-r--r--   0        0        0    10514 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/vcs/git.py
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 pbt_simple-1.7.4/PKG-INFO
```

### Comparing `pbt_simple-1.7.3/LICENSE` & `pbt_simple-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.3/pyproject.toml` & `pbt_simple-1.7.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbt-simple"
-version = "1.7.3"
+version = "1.7.4"
 description = "A simpler version of [PBT](https://github.com/binh-vu/pbt) for installing a package (and its local dependencies in editable mode) and build extension modules written in PYO3."
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "sbt" }]
 homepage = "https://github.com/binh-vu/pbt-simple"
 repository = "https://github.com/binh-vu/pbt-simple"
```

### Comparing `pbt_simple-1.7.3/sbt/__main__.py` & `pbt_simple-1.7.4/sbt/__main__.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.3/sbt/commands/build.py` & `pbt_simple-1.7.4/sbt/commands/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     (whl_file,) = [x for x in outdir.glob("*.whl")]
     with zipfile.ZipFile(whl_file, "r") as zip_ref:
         zip_ref.extractall(outdir)
 
     pkg_name = pkg.name.replace("-", "_")
     pkg_dir = outdir / pkg_name
     if not pkg_dir.exists():
-        for name in pkg.include:
+        for name in pkg.include_packages:
             pkg_name = name.replace("-", "_")
             pkg_dir = outdir / pkg_name
             if pkg_dir.exists():
                 break
         else:
             raise RuntimeError(f"Cannot find the package directory in {outdir}")
```

### Comparing `pbt_simple-1.7.3/sbt/commands/git.py` & `pbt_simple-1.7.4/sbt/commands/git.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.3/sbt/commands/install.py` & `pbt_simple-1.7.4/sbt/commands/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,16 +288,19 @@
             doc = document()
 
             tbl = table()
             tbl.add("name", pkg.name)
             tbl.add("version", pkg.version)
             tbl.add("description", "")
             tbl.add("authors", [])
-            if sum(int(x != pkg.name) for x in pkg.include) > 0:
-                tbl.add("packages", [{"include": x} for x in pkg.include])
+            if sum(int(x != pkg.name) for x in pkg.include_packages) > 0:
+                tbl.add("packages", [{"include": x} for x in pkg.include_packages])
+
+            if len(pkg.include) > 0:
+                tbl.add("include", pkg.include)
 
             doc.add(SingleKey("tool.poetry", t=KeyType.Bare), tbl)
 
             tbl = table()
             tbl.add("requires", ["poetry-core>=1.0.0"])
             tbl.add("build-backend", "poetry.core.masonry.api")
             doc.add(nl())
@@ -319,16 +322,19 @@
 
         tbl = table()
         tbl.add("name", pkg.name)
         tbl.add("version", pkg.version)
         tbl.add("description", "")
         tbl.add("authors", [])
 
-        if sum(int(x != pkg.name) for x in pkg.include) > 0:
-            tbl.add("packages", [{"include": x} for x in pkg.include])
+        if sum(int(x != pkg.name) for x in pkg.include_packages) > 0:
+            tbl.add("packages", [{"include": x} for x in pkg.include_packages])
+
+        if len(pkg.include) > 0:
+            tbl.add("include", pkg.include)
 
         doc.add(SingleKey("tool.poetry", t=KeyType.Bare), tbl)
 
         tbl = table()
         if "python" not in deps:
             tbl.add("python", f"=={cfg.get_python_version()}")
         for dep, specs in deps.items():
```

### Comparing `pbt_simple-1.7.3/sbt/commands/list.py` & `pbt_simple-1.7.4/sbt/commands/list.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.3/sbt/config.py` & `pbt_simple-1.7.4/sbt/config.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.3/sbt/misc.py` & `pbt_simple-1.7.4/sbt/misc.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.3/sbt/package/discovery.py` & `pbt_simple-1.7.4/sbt/package/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     # not supported yet in pep-621
     # https://peps.python.org/pep-0621/#specify-files-to-include-when-building
     include = []
     if "tool" in cfg and "maturin" in cfg["tool"]:
         if "include" in cfg["tool"]["maturin"]:
             include = cfg["tool"]["maturin"]["include"]
 
-    return Package(name, version, loc, PackageType.Maturin, include, dependencies)
+    return Package(name=name, version=version, location=loc, type=PackageType.Maturin, include_packages=[], include=include, dependencies=dependencies)
 
 
 def parse_poetry_project(cfg: dict, loc: Path) -> Package:
     name = cfg["tool"]["poetry"]["name"]
     version = cfg["tool"]["poetry"]["version"]
 
     dependencies = {}
@@ -175,19 +175,19 @@
                 (parse_poetry_dep_spec(v) for v in vs),
                 key=attrgetter("constraint"),
             )
 
     # see https://python-poetry.org/docs/pyproject/#include-and-exclude
     # and https://python-poetry.org/docs/pyproject/#packages
     include = cfg["tool"]["poetry"].get("include", [])
+    include_packages = []
     for pkg_cfg in cfg["tool"]["poetry"].get("packages", []):
-        include.append(os.path.join(pkg_cfg.get("from", ""), pkg_cfg["include"]))
-    include = sorted(set(include))
+        include_packages.append(os.path.join(pkg_cfg.get("from", ""), pkg_cfg["include"]))
 
-    return Package(name, version, loc, PackageType.Poetry, include, dependencies)
+    return Package(name=name, version=version, location=loc, type=PackageType.Poetry, include_packages=include_packages, include=include, dependencies=dependencies)
 
 
 def parse_pep518_pkgname_with_extra(name: str) -> tuple[str, list[str]]:
     """Parse a spec containing extra dependencies: `<name>([(<extra>,)+])?"""
     m = re.match(r"([^\[]+)(?:\[(.+)\])?$", name)
     assert m is not None, name
```

### Comparing `pbt_simple-1.7.3/sbt/package/graph.py` & `pbt_simple-1.7.4/sbt/package/graph.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.3/sbt/package/package.py` & `pbt_simple-1.7.4/sbt/package/package.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 @dataclass
 class Package:
     name: str
     version: str
     location: Path
     type: PackageType
 
+    # equivalent to Poetry tool.poetry.packages -- for including packages that are located in different directories.
+    include_packages: list[str]
+    # equivalent to tool.poetry.include -- for files that will be included in the final package.
     include: list[str]
 
+
     dependencies: dict[str, DepConstraints]
 
     def find_manually_installed_dependencies(self, cache_dir: Path) -> list[Path]:
         """Find dependencies that were installed manually (via command line) into the package environment"""
         cache_file = self._get_manually_installed_dep_file(cache_dir)
         if not cache_file.exists():
             return []
```

### Comparing `pbt_simple-1.7.3/sbt/registry/pypi.py` & `pbt_simple-1.7.4/sbt/registry/pypi.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.3/sbt/vcs/git.py` & `pbt_simple-1.7.4/sbt/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.3/PKG-INFO` & `pbt_simple-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbt-simple
-Version: 1.7.3
+Version: 1.7.4
 Summary: A simpler version of [PBT](https://github.com/binh-vu/pbt) for installing a package (and its local dependencies in editable mode) and build extension modules written in PYO3.
 Home-page: https://github.com/binh-vu/pbt-simple
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

