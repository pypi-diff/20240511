# Comparing `tmp/thztools-0.3.6.tar.gz` & `tmp/thztools-0.4.0.tar.gz`

## Comparing `thztools-0.3.6.tar` & `thztools-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 thztools-0.3.6/.gitattributes
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 thztools-0.3.6/CHANGELOG.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.3.6/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 thztools-0.3.6/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.3.6/.idea/modules.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.3.6/.idea/other.xml
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 thztools-0.3.6/.idea/thztools.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.3.6/.idea/vcs.xml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.3.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 thztools-0.3.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 thztools-0.3.6/.vscode/settings.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 thztools-0.3.6/logo/make_logo.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 thztools-0.3.6/src/thztools/__about__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 thztools-0.3.6/src/thztools/__init__.py
--rw-r--r--   0        0        0    44430 2020-02-02 00:00:00.000000 thztools-0.3.6/src/thztools/thztools.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 thztools-0.3.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.3.6/LICENSE
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 thztools-0.3.6/README.md
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 thztools-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 thztools-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 thztools-0.4.0/.gitattributes
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 thztools-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 thztools-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/modules.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/other.xml
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/thztools.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 thztools-0.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 thztools-0.4.0/logo/make_logo.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 thztools-0.4.0/paper/paper.bib
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 thztools-0.4.0/paper/paper.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 thztools-0.4.0/src/thztools/__about__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 thztools-0.4.0/src/thztools/__init__.py
+-rw-r--r--   0        0        0    64696 2020-02-02 00:00:00.000000 thztools-0.4.0/src/thztools/thztools.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 thztools-0.4.0/README.md
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 thztools-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 thztools-0.4.0/PKG-INFO
```

### Comparing `thztools-0.3.6/.idea/thztools.iml` & `thztools-0.4.0/.idea/thztools.iml`

 * *Files 14% similar despite different names*

#### Comparing `thztools-0.3.6/.idea/thztools.iml` & `thztools-0.4.0/.idea/thztools.iml`

```diff
@@ -3,20 +3,22 @@
   <component name="NewModuleRootManager">
     <content url="file://$MODULE_DIR$">
       <sourceFolder url="file://$MODULE_DIR$" isTestSource="false"/>
       <sourceFolder url="file://$MODULE_DIR$/src" isTestSource="false"/>
       <excludeFolder url="file://$MODULE_DIR$/.pytest_cache"/>
       <excludeFolder url="file://$MODULE_DIR$/dist"/>
       <excludeFolder url="file://$MODULE_DIR$/docs/build"/>
-      <excludeFolder url="file://$MODULE_DIR$/examples/.ipynb_checkpoints"/>
       <excludeFolder url="file://$MODULE_DIR$/thztools.egg-info"/>
       <excludeFolder url="file://$MODULE_DIR$/.idea/dictionaries"/>
       <excludeFolder url="file://$MODULE_DIR$/.mypy_cache/3.11"/>
       <excludeFolder url="file://$MODULE_DIR$/.ruff_cache/content"/>
       <excludeFolder url="file://$MODULE_DIR$/htmlcov"/>
+      <excludeFolder url="file://$MODULE_DIR$/docs/doctest/.doctrees"/>
+      <excludeFolder url="file://$MODULE_DIR$/docs/doctest/plot_directive"/>
+      <excludeFolder url="file://$MODULE_DIR$/docs/source/examples/.ipynb_checkpoints"/>
     </content>
     <orderEntry type="jdk" jdkName="thztools" jdkType="Python SDK"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
   <component name="PyDocumentationSettings">
     <option name="format" value="NUMPY"/>
     <option name="myDocStringFormat" value="NumPy"/>
```

### Comparing `thztools-0.3.6/.idea/inspectionProfiles/Project_Default.xml` & `thztools-0.4.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `thztools-0.3.6/logo/make_logo.py` & `thztools-0.4.0/logo/make_logo.py`

 * *Files identical despite different names*

### Comparing `thztools-0.3.6/.gitignore` & `thztools-0.4.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # MacOS
 # General
 .DS_Store
 
 # Local .gitignore
 Untitled*.ipynb
-**/correspondence/
+**/doctest/**
+**/tmp/**
+
+# NumPy data files
+**/*.npz
 
 # Python .gitignore:
 #	https://github.com/github/gitignore/blob/main/Python.gitignore
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
```

### Comparing `thztools-0.3.6/LICENSE` & `thztools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thztools-0.3.6/README.md` & `thztools-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 electromagnetic waveforms that are acquired as a function of *time*, which users typically
 represent as a function of *frequency* for analysis. THzTools makes it easier for researchers
 to use statistically optimal methods for doing this analysis, as described in [L. Mohtashemi et al.,
  Opt. Express **29**, 4912 (2021)](https://doi.org/10.1364/OE.417724).
 
 This is *alpha* software that is currently under development.
 
-| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-|:------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Project**       | [![DOI](https://zenodo.org/badge/569133241.svg)](https://zenodo.org/doi/10.5281/zenodo.10100093) ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)                                                                                                          |
-| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/pytest-with-coverage.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools) |
-| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
-| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+|:------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| **Project**       | [![DOI](https://zenodo.org/badge/569133241.svg)](https://zenodo.org/doi/10.5281/zenodo.10100093) ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) |
+| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/pytest-with-coverage.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools)          |
+| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
 
 The original MATLAB code is available at [Zenodo](https://zenodo.org/record/4876388).
```

### Comparing `thztools-0.3.6/pyproject.toml` & `thztools-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thztools"
 dynamic = ["version"]
-description = "Tools for terahertz time-domain spectroscopy (THz-TDS)"
+description = """
+Data analysis software tools for terahertz time-domain spectroscopy (THz-TDS)
+"""
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["terahertz", "THz", "time-domain spectroscopy", "data analysis"]
 authors = [
-    { name="Steve Dodge", email="jsdodge@sfu.ca" },
-    { name="Santiago Higuera Quintero", email="s.higuera@uniandes.edu.co" },
-    { name="Jonathan Posada", email="jonathan.posada1@udea.edu.co" },
-    { name="Alireza Noori", email="alireza_noori@sfu.ca"}
+    { name="Jonathan Posada Loaiza", email="jonathan.posada1@udea.edu.co" },
+    { name="Santiago Higuera-Quintero", email="s.higuera@uniandes.edu.co" },
+    { name="Alireza Noori", email="alireza_noori@sfu.ca" },
+    { name="Laleh Mohtashemi", email="lalehmo@gmail.com" },
+    { name="R. P. Hall", email="rph4@sfu.ca" },
+    { name="Naod Ayalew Yimam", email="nayimam@gmail.com"},
+    { name="J. Steven Dodge", email="jsdodge@sfu.ca" },
 ]
 maintainers = [
     { name="Steve Dodge", email="jsdodge@sfu.ca" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
@@ -30,32 +35,33 @@
   	"Programming Language :: Python :: Implementation :: CPython",
   	"Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-    "numpy",
+    "numpy>=1.21",
     "scipy",
-    "numdifftools",
 ]
 
 [project.urls]
 Documentation = "https://dodge-research-group.github.io/thztools/"
 Issues = "https://github.com/dodge-research-group/thztools/issues"
+Discussion = "https://github.com/dodge-research-group/thztools/discussions"
 Source = "https://github.com/dodge-research-group/thztools"
 
 [tool.hatch.version]
 path = "src/thztools/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
     "coverage[toml]>=6.5",
     "jupyter",
     "matplotlib",
+    "numdifftools",
     "pytest",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
     "- coverage combine",
@@ -65,15 +71,15 @@
 cov = [
     "test-cov",
     "cov-report",
 ]
 make-logo = ["python logo/make_logo.py; mv thztools_logo.svg docs/source/_static/;mv thztools_logo_dark.svg docs/source/_static/"]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11"]
+python = ["3.8", "3.9", "3.10", "3.11", "3.12",]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
     "black>=23.1.0",
     "black[jupyter]",
     "mypy>=1.0.0",
@@ -184,22 +190,28 @@
 ## Show warnings as errors for debugging
 #filterwarnings = [
 #    "error",
 #]
 
 [tool.hatch.envs.docs]
 dependencies = [
+    "ipykernel",
+    "IPython",
     "matplotlib",
+    "nbsphinx",
     "numpydoc",
     "pydata-sphinx-theme",
     "sphinx",
+    "sphinx-design",
+    "sphinx-gallery",
     "tomli",
 ]
 [tool.hatch.envs.docs.scripts]
 build = "sphinx-build -v -b html docs/source docs/build/html"
+test = "sphinx-build -v -b doctest docs/source docs/doctest"
 
 [tool.mypy]
 plugins = "numpy.typing.mypy_plugin"
 
 [[tool.mypy.overrides]]
 module = [
     "pytest",
```

### Comparing `thztools-0.3.6/PKG-INFO` & `thztools-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: thztools
-Version: 0.3.6
-Summary: Tools for terahertz time-domain spectroscopy (THz-TDS)
+Version: 0.4.0
+Summary: Data analysis software tools for terahertz time-domain spectroscopy (THz-TDS)
 Project-URL: Documentation, https://dodge-research-group.github.io/thztools/
 Project-URL: Issues, https://github.com/dodge-research-group/thztools/issues
+Project-URL: Discussion, https://github.com/dodge-research-group/thztools/discussions
 Project-URL: Source, https://github.com/dodge-research-group/thztools
-Author-email: Steve Dodge <jsdodge@sfu.ca>, Santiago Higuera Quintero <s.higuera@uniandes.edu.co>, Jonathan Posada <jonathan.posada1@udea.edu.co>, Alireza Noori <alireza_noori@sfu.ca>
+Author-email: Jonathan Posada Loaiza <jonathan.posada1@udea.edu.co>, Santiago Higuera-Quintero <s.higuera@uniandes.edu.co>, Alireza Noori <alireza_noori@sfu.ca>, Laleh Mohtashemi <lalehmo@gmail.com>, "R. P. Hall" <rph4@sfu.ca>, Naod Ayalew Yimam <nayimam@gmail.com>, "J. Steven Dodge" <jsdodge@sfu.ca>
 Maintainer-email: Steve Dodge <jsdodge@sfu.ca>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: THz,data analysis,terahertz,time-domain spectroscopy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -19,16 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: numdifftools
-Requires-Dist: numpy
+Requires-Dist: numpy>=1.21
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
 <div style="text-align: center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/dodge-research-group/thztools/main/docs/source/_static/thztools_logo_dark.svg" width="600">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/dodge-research-group/thztools/main/docs/source/_static/thztools_logo.svg" width="600">
@@ -41,15 +41,15 @@
 electromagnetic waveforms that are acquired as a function of *time*, which users typically
 represent as a function of *frequency* for analysis. THzTools makes it easier for researchers
 to use statistically optimal methods for doing this analysis, as described in [L. Mohtashemi et al.,
  Opt. Express **29**, 4912 (2021)](https://doi.org/10.1364/OE.417724).
 
 This is *alpha* software that is currently under development.
 
-| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-|:------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Project**       | [![DOI](https://zenodo.org/badge/569133241.svg)](https://zenodo.org/doi/10.5281/zenodo.10100093) ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)                                                                                                          |
-| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/pytest-with-coverage.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools) |
-| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
-| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+|:------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| **Project**       | [![DOI](https://zenodo.org/badge/569133241.svg)](https://zenodo.org/doi/10.5281/zenodo.10100093) ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) |
+| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/pytest-with-coverage.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools)          |
+| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
 
 The original MATLAB code is available at [Zenodo](https://zenodo.org/record/4876388).
```

