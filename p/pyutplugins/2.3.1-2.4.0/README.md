# Comparing `tmp/pyutplugins-2.3.1.tar.gz` & `tmp/pyutplugins-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutplugins-2.3.1.tar", last modified: Wed Mar 13 00:10:54 2024, max compression
+gzip compressed data, was "pyutplugins-2.4.0.tar", last modified: Sat May 11 20:27:17 2024, max compression
```

## Comparing `pyutplugins-2.3.1.tar` & `pyutplugins-2.4.0.tar`

### file list

```diff
@@ -1,159 +1,171 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.146901 pyutplugins-2.3.1/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-01-04 04:11:16.000000 pyutplugins-2.3.1/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2702 2024-03-13 00:10:54.146682 pyutplugins-2.3.1/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1856 2023-09-21 21:54:41.000000 pyutplugins-2.3.1/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1060 2024-03-12 23:56:04.000000 pyutplugins-2.3.1/pyproject.toml
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-03-13 00:10:54.146944 pyutplugins-2.3.1/setup.cfg
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.120137 pyutplugins-2.3.1/src/
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.123672 pyutplugins-2.3.1/src/pyutplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6617 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ExternalTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/IPluginAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7962 2024-03-08 21:53:24.000000 pyutplugins-2.3.1/src/pyutplugins/PluginManager.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-03-12 23:58:47.000000 pyutplugins-2.3.1/src/pyutplugins/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.125271 pyutplugins-2.3.1/src/pyutplugins/common/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1133 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/common/ElementTreeData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2744 2024-02-05 21:04:27.000000 pyutplugins-2.3.1/src/pyutplugins/common/LinkMakerMixin.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      471 2024-01-27 20:56:43.000000 pyutplugins-2.3.1/src/pyutplugins/common/PluginTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/common/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/common/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.125753 pyutplugins-2.3.1/src/pyutplugins/common/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/common/ui/BaseEditDialog.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/common/ui/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.126224 pyutplugins-2.3.1/src/pyutplugins/common/ui/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5182 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/common/ui/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/common/ui/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/common/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.127042 pyutplugins-2.3.1/src/pyutplugins/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/exceptions/InvalidPluginExtensionException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/exceptions/InvalidPluginNameException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/exceptions/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/exceptions/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.129108 pyutplugins-2.3.1/src/pyutplugins/ioplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4236 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOAscii.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/IODTD.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOGML.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOJava.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3245 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOMermaid.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6403 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOPdf.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9664 2024-02-05 02:43:00.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOWxImage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8278 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOXml.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.130136 pyutplugins-2.3.1/src/pyutplugins/ioplugins/dtd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/dtd/DTDAttribute.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/dtd/DTDElementTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10417 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/dtd/DTDParser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/dtd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/dtd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.130859 pyutplugins-2.3.1/src/pyutplugins/ioplugins/gml/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8649 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/gml/GMLExporter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/gml/UnsupportedOperation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/gml/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/gml/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.131723 pyutplugins-2.3.1/src/pyutplugins/ioplugins/java/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28064 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/java/JavaReader.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11176 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/java/JavaWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/java/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/java/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.132433 pyutplugins-2.3.1/src/pyutplugins/ioplugins/mermaid/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/mermaid/MermaidDirection.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12586 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/mermaid/MermaidWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/mermaid/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/mermaid/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.133244 pyutplugins-2.3.1/src/pyutplugins/ioplugins/pdf/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/pdf/ImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/pdf/ImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12933 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/pdf/PyUmlDefinitionAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/pdf/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/pdf/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.134404 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6135 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/PythonParseException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12478 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/PyutToPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10232 2024-02-05 02:43:00.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/ReverseEngineerPythonV3.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.136561 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/pythonpegparser/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    54703 2024-02-05 14:09:02.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexer.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    17041 2024-02-05 02:43:00.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexerBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   541896 2024-02-05 14:09:03.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2024-02-05 02:43:00.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParserBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    35740 2024-02-05 02:43:00.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonPegParserVisitor.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.137669 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2892 2024-02-05 02:43:00.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/ParentsDictionaryHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1592 2024-02-05 02:43:00.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/ParserTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3974 2024-02-05 02:43:00.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/PyutBaseVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5181 2024-02-05 02:43:00.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegClassVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20411 2024-02-05 02:43:00.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-02-05 02:43:00.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.138334 pyutplugins-2.3.1/src/pyutplugins/ioplugins/wximage/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4853 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/wximage/WxImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/wximage/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/ioplugins/wximage/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.139251 pyutplugins-2.3.1/src/pyutplugins/plugininterfaces/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11800 2024-03-07 18:41:20.000000 pyutplugins-2.3.1/src/pyutplugins/plugininterfaces/BasePluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugininterfaces/IOPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1364 2024-03-08 21:53:51.000000 pyutplugins-2.3.1/src/pyutplugins/plugininterfaces/ToolPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugininterfaces/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugininterfaces/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.140845 pyutplugins-2.3.1/src/pyutplugins/plugintypes/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugintypes/BaseFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugintypes/BaseRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugintypes/ExportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugintypes/ImportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugintypes/InputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugintypes/MultipleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugintypes/OutputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugintypes/PluginDataTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugintypes/SingleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugintypes/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/plugintypes/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.141261 pyutplugins-2.3.1/src/pyutplugins/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7286 2024-01-17 21:40:45.000000 pyutplugins-2.3.1/src/pyutplugins/preferences/PluginPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.142495 pyutplugins-2.3.1/src/pyutplugins/toolplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1729 2024-03-07 18:37:20.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/ToolArrangeLinks.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5225 2024-03-11 01:31:01.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/ToolForceDirectedLayout.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2024-03-08 05:03:28.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/ToolSugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/ToolTransforms.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.143463 pyutplugins-2.3.1/src/pyutplugins/toolplugins/forcedirectedlayout/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8287 2024-03-09 15:59:30.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/forcedirectedlayout/ConfigurationPanel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2069 2024-03-08 21:45:45.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/forcedirectedlayout/DlgConfiguration.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1245 2024-03-09 19:18:23.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/forcedirectedlayout/OglNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-07 17:58:31.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/forcedirectedlayout/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/forcedirectedlayout/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.144346 pyutplugins-2.3.1/src/pyutplugins/toolplugins/orthogonal/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2001 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/orthogonal/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/orthogonal/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.146250 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3560 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28457 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/Sugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-13 00:10:54.146410 pyutplugins-2.3.1/src/pyutplugins.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2702 2024-03-13 00:10:54.000000 pyutplugins-2.3.1/src/pyutplugins.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6227 2024-03-13 00:10:54.000000 pyutplugins-2.3.1/src/pyutplugins.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-03-13 00:10:54.000000 pyutplugins-2.3.1/src/pyutplugins.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      240 2024-03-13 00:10:54.000000 pyutplugins-2.3.1/src/pyutplugins.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2024-03-13 00:10:54.000000 pyutplugins-2.3.1/src/pyutplugins.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.758022 pyutplugins-2.4.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2024-04-26 20:44:48.000000 pyutplugins-2.4.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2744 2024-05-11 20:27:17.757816 pyutplugins-2.4.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1856 2023-09-21 21:54:41.000000 pyutplugins-2.4.0/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1092 2024-05-10 18:22:45.000000 pyutplugins-2.4.0/pyproject.toml
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-05-11 20:27:17.758064 pyutplugins-2.4.0/setup.cfg
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.730224 pyutplugins-2.4.0/src/
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.733845 pyutplugins-2.4.0/src/pyutplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8405 2024-05-09 19:12:08.000000 pyutplugins-2.4.0/src/pyutplugins/ExternalTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3913 2024-05-09 18:28:12.000000 pyutplugins-2.4.0/src/pyutplugins/IPluginAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9462 2024-05-11 19:54:18.000000 pyutplugins-2.4.0/src/pyutplugins/PluginManager.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-05-11 20:27:12.000000 pyutplugins-2.4.0/src/pyutplugins/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.735502 pyutplugins-2.4.0/src/pyutplugins/common/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1133 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ElementTreeData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2373 2024-04-28 17:55:59.000000 pyutplugins-2.4.0/src/pyutplugins/common/LinkMakerMixin.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      471 2024-01-27 20:56:43.000000 pyutplugins-2.4.0/src/pyutplugins/common/PluginTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.735922 pyutplugins-2.4.0/src/pyutplugins/common/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/BaseEditDialog.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.736409 pyutplugins-2.4.0/src/pyutplugins/common/ui/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5182 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.737331 pyutplugins-2.4.0/src/pyutplugins/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/exceptions/InvalidPluginExtensionException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/exceptions/InvalidPluginNameException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/exceptions/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/exceptions/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.739409 pyutplugins-2.4.0/src/pyutplugins/ioplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4236 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOAscii.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IODTD.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOGML.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOJava.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3260 2024-05-11 19:29:41.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOMermaid.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6403 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOPdf.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9664 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOWxImage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8278 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOXml.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.740157 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/DTDAttribute.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/DTDElementTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10417 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/DTDParser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.740630 pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8649 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/GMLExporter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/UnsupportedOperation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.741357 pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28064 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/JavaReader.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11176 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/JavaWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.741946 pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/MermaidDirection.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13434 2024-05-11 19:55:08.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/MermaidWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.742652 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/ImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/ImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12933 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/PyUmlDefinitionAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.743641 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6135 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/PythonParseException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12478 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/PyutToPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10232 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/ReverseEngineerPythonV3.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.745333 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    54703 2024-02-05 14:09:02.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexer.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    17041 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexerBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   541896 2024-02-05 14:09:03.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParserBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    35740 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonPegParserVisitor.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.746447 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2892 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/ParentsDictionaryHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1592 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/ParserTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3974 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutBaseVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5181 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegClassVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20411 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.747112 pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4852 2024-05-01 01:58:53.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/WxImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.748074 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11800 2024-03-07 18:41:20.000000 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/BasePluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/IOPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1364 2024-03-08 21:53:51.000000 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/ToolPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.749715 pyutplugins-2.4.0/src/pyutplugins/plugintypes/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/BaseFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/BaseRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/ExportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/ImportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/InputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/MultipleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/OutputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/PluginDataTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/SingleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.750158 pyutplugins-2.4.0/src/pyutplugins/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7286 2024-01-17 21:40:45.000000 pyutplugins-2.4.0/src/pyutplugins/preferences/PluginPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.752332 pyutplugins-2.4.0/src/pyutplugins/toolplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1729 2024-04-25 17:28:09.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolArrangeLinks.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5225 2024-03-11 01:31:01.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolForceDirectedLayout.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4534 2024-04-28 19:32:22.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolLoadLayout.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2024-03-08 05:03:28.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2427 2024-05-06 22:41:41.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolOrthogonalRouting.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4012 2024-04-28 17:19:08.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolSaveLayout.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2024-05-02 19:47:25.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolSugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolTransforms.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.753363 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8287 2024-03-09 15:59:30.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/ConfigurationPanel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2069 2024-03-08 21:45:45.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/DlgConfiguration.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1245 2024-03-09 19:18:23.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/OglNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-07 17:58:31.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.754240 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2001 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.755154 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9817 2024-05-10 19:24:31.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/DlgConfiguration.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3467 2024-05-10 19:47:03.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/LabelledSlider.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6852 2024-05-10 19:05:00.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/OrthogonalConnectorAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 21:22:45.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.755458 pyutplugins-2.4.0/src/pyutplugins/toolplugins/savelayout/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      903 2024-04-28 17:19:08.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/savelayout/Layout.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 17:19:08.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/savelayout/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.757383 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3560 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28457 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/Sugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.757514 pyutplugins-2.4.0/src/pyutplugins.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2744 2024-05-11 20:27:17.000000 pyutplugins-2.4.0/src/pyutplugins.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6791 2024-05-11 20:27:17.000000 pyutplugins-2.4.0/src/pyutplugins.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-05-11 20:27:17.000000 pyutplugins-2.4.0/src/pyutplugins.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      267 2024-05-11 20:27:17.000000 pyutplugins-2.4.0/src/pyutplugins.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2024-05-11 20:27:17.000000 pyutplugins-2.4.0/src/pyutplugins.egg-info/top_level.txt
```

### Comparing `pyutplugins-2.3.1/LICENSE` & `pyutplugins-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/PKG-INFO` & `pyutplugins-2.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: pyutplugins
-Version: 2.3.1
+Version: 2.4.0
 Summary: Pyut Plugins
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/pyutplugins
 Keywords: pyut,python,plugin
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: codeallybasic>=1.3.1
 Requires-Dist: codeallyadvanced>=1.3.1
 Requires-Dist: pyutmodelv2>=2.1.5
-Requires-Dist: ogl>=2.1.20
-Requires-Dist: untanglepyut>=2.1.7
+Requires-Dist: ogl>=2.1.32
+Requires-Dist: untanglepyut>=2.1.8
 Requires-Dist: oglio>=2.1.7
 Requires-Dist: pyumldiagrams>=3.1.10
 Requires-Dist: wxPython~=4.2.1
 Requires-Dist: antlr4-python3-runtime==4.13.1
 Requires-Dist: networkx==3.0
 Requires-Dist: orthogonal==1.2.0
 Requires-Dist: pyforcedirectedlayout>=0.80.2
+Requires-Dist: pyorthogonalrouting>=1.2.0
 
 ![](https://github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-2-256x48.png "AGPL")
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/pyutplugins/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/pyutplugins/tree/master)
 [![PyPI version](https://badge.fury.io/py/pyutplugins.svg)](https://badge.fury.io/py/pyutplugins)
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: pyutplugins Version: 2.3.1 Summary: Pyut Plugins
+Metadata-Version: 2.1 Name: pyutplugins Version: 2.4.0 Summary: Pyut Plugins
 Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/pyutplugins Keywords: pyut,python,plugin
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 codeallybasic>=1.3.1 Requires-Dist: codeallyadvanced>=1.3.1 Requires-Dist:
-pyutmodelv2>=2.1.5 Requires-Dist: ogl>=2.1.20 Requires-Dist:
-untanglepyut>=2.1.7 Requires-Dist: oglio>=2.1.7 Requires-Dist:
+pyutmodelv2>=2.1.5 Requires-Dist: ogl>=2.1.32 Requires-Dist:
+untanglepyut>=2.1.8 Requires-Dist: oglio>=2.1.7 Requires-Dist:
 pyumldiagrams>=3.1.10 Requires-Dist: wxPython~=4.2.1 Requires-Dist: antlr4-
 python3-runtime==4.13.1 Requires-Dist: networkx==3.0 Requires-Dist:
-orthogonal==1.2.0 Requires-Dist: pyforcedirectedlayout>=0.80.2 ![](https://
-github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-
-badge-version-2-256x48.png "AGPL") [![Maintenance](https://img.shields.io/
-badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/
-graphs/commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/
-gh/hasii2011/pyutplugins/tree/master.svg?style=shield)](https://
-dl.circleci.com/status-badge/redirect/gh/hasii2011/pyutplugins/tree/master) [!
-[PyPI version](https://badge.fury.io/py/pyutplugins.svg)](https://
-badge.fury.io/py/pyutplugins) [![CircleCI](https://dl.circleci.com/insights-
-snapshot/gh/hasii2011/pyutplugins/master/main/badge.svg?window=30d)](https://
-app.circleci.com/insights/github/hasii2011/pyutplugins/workflows/main/
-overview?branch=master&reporting-window=last-30-days&insights-snapshot=true) #
-Introduction **TBD** # Overview **TBD** ## Developer Notes This project uses
-[buildlackey](https://github.com/hasii2011/buildlackey) for day to day
-development builds ___ Written by _H_u_m_b_e_r_t_o_ _A_._ _S_a_n_c_h_e_z_ _I_I (C) 2023 ___ I am
-concerned about GitHub's Copilot project ![](https://github.com/hasii2011/code-
-ally-basic/blob/master/developer/SillyGitHub.png) I urge you to read about the
-[Give up GitHub](https://GiveUpGitHub.org) campaign from [the Software Freedom
-Conservancy](https://sfconservancy.org). While I do not advocate for all the
-issues listed there I do not like that a company like Microsoft may profit from
-open source projects. I continue to use GitHub because it offers the services I
-need for free. But, I continue to monitor their terms of service. Any use of
-this project's code by GitHub Copilot, past or present, is done without my
-permission. I do not consent to GitHub's use of this project's code in Copilot.
+orthogonal==1.2.0 Requires-Dist: pyforcedirectedlayout>=0.80.2 Requires-Dist:
+pyorthogonalrouting>=1.2.0 ![](https://github.com/hasii2011/code-ally-basic/
+blob/master/developer/agpl-license-web-badge-version-2-256x48.png "AGPL") [!
+[Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
+//GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
+dl.circleci.com/status-badge/img/gh/hasii2011/pyutplugins/tree/
+master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/
+hasii2011/pyutplugins/tree/master) [![PyPI version](https://badge.fury.io/py/
+pyutplugins.svg)](https://badge.fury.io/py/pyutplugins) [![CircleCI](https://
+dl.circleci.com/insights-snapshot/gh/hasii2011/pyutplugins/master/main/
+badge.svg?window=30d)](https://app.circleci.com/insights/github/hasii2011/
+pyutplugins/workflows/main/overview?branch=master&reporting-window=last-30-
+days&insights-snapshot=true) # Introduction **TBD** # Overview **TBD** ##
+Developer Notes This project uses [buildlackey](https://github.com/hasii2011/
+buildlackey) for day to day development builds ___ Written by _H_u_m_b_e_r_t_o_ _A_.
+_S_a_n_c_h_e_z_ _I_I (C) 2023 ___ I am concerned about GitHub's Copilot project ![]
+(https://github.com/hasii2011/code-ally-basic/blob/master/developer/
+SillyGitHub.png) I urge you to read about the [Give up GitHub](https://
+GiveUpGitHub.org) campaign from [the Software Freedom Conservancy](https://
+sfconservancy.org). While I do not advocate for all the issues listed there I
+do not like that a company like Microsoft may profit from open source projects.
+I continue to use GitHub because it offers the services I need for free. But, I
+continue to monitor their terms of service. Any use of this project's code by
+GitHub Copilot, past or present, is done without my permission. I do not
+consent to GitHub's use of this project's code in Copilot.
```

### Comparing `pyutplugins-2.3.1/README.md` & `pyutplugins-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/pyproject.toml` & `pyutplugins-2.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 maintainers = [{name = 'Humberto A. Sanchez II', email = 'Humbert.A.Sanchez.II@gmail.com'}]
 keywords    = ['pyut', 'python', 'plugin']
 
 dependencies = [
   'codeallybasic>=1.3.1',
   'codeallyadvanced>=1.3.1',
   'pyutmodelv2>=2.1.5',
-  'ogl>=2.1.20',
-  'untanglepyut>=2.1.7',
+  'ogl>=2.1.32',
+  'untanglepyut>=2.1.8',
   'oglio>=2.1.7',
   'pyumldiagrams>=3.1.10',
   'wxPython~=4.2.1',
   'antlr4-python3-runtime==4.13.1',
   'networkx==3.0',
   'orthogonal==1.2.0',
   'pyforcedirectedlayout>=0.80.2',
+  'pyorthogonalrouting>=1.2.0',
 ]
 [project.urls]
 Repository = 'https://github.com/hasii2011/pyutplugins'
 
 
 [tool.setuptools.packages.find]
 where = ['src']
```

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ExternalTypes.py` & `pyutplugins-2.4.0/src/pyutplugins/ExternalTypes.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 from dataclasses import dataclass
 from dataclasses import field
 
 from os import path as osPath
 
 from enum import Enum
 
+from pyutmodelv2.enumerations.PyutLinkType import PyutLinkType
 from wx import ClientDC
 
 from pyutmodelv2.PyutLink import PyutLink
 
 from ogl.OglClass import OglClass
 from ogl.OglLink import OglLink
 from ogl.OglInterface2 import OglInterface2
 from ogl.OglNote import OglNote
 from ogl.OglText import OglText
-
+from ogl.OglObject import OglObject
+from ogl.OglPosition import OglPositions
 from ogl.OglUseCase import OglUseCase
 from ogl.OglActor import OglActor
 
 from ogl.sd.OglSDInstance import OglSDInstance
 from ogl.sd.OglSDMessage import OglSDMessage
 
 HybridLinks = Union[OglLink, OglInterface2]
@@ -89,14 +91,62 @@
     frameSize:          FrameSize  = field(default_factory=createFrameSizeFactory)
     clientDC:           ClientDC   = cast(ClientDC, None)
 
 
 FrameInformationCallback = Callable[[FrameInformation], None]
 FrameSizeCallback        = Callable[[FrameSize], None]
 
+NO_INTEGER: int = cast(int, None)
+
+
+@dataclass
+class ObjectBoundaries:
+    minX: int = NO_INTEGER
+    minY: int = NO_INTEGER
+    maxX: int = NO_INTEGER
+    maxY: int = NO_INTEGER
+
+
+ObjectBoundaryCallback = Callable[[ObjectBoundaries], None]
+
+InterfaceName          = NewType('InterfaceName', str)
+AssociationName        = NewType('AssociationName', str)
+SourceCardinality      = NewType('SourceCardinality', str)
+DestinationCardinality = NewType('DestinationCardinality', str)
+
+
+def createOglPositionsFactory() -> OglPositions:
+    return OglPositions([])
+
+
+@dataclass
+class LinkInformation:
+    """
+    The field interfaceName is only valid when linkType is PyutLinkType.INTERFACE
+    The fields
+        associationName
+        sourceCardinality
+        destinationCardinality
+    are valid only when linkType is  one of
+        PyutLinkType.ASSOCIATION
+        PyutLinkType.COMPOSITION
+        PyutLinkType.AGGREGATION
+    """
+    linkType:               PyutLinkType            = cast(PyutLinkType, None)
+    path:                   OglPositions            = field(default_factory=createOglPositionsFactory)
+    sourceShape:            OglObject               = cast(OglObject, None)
+    destinationShape:       OglObject               = cast(OglObject, None)
+    interfaceName:          InterfaceName           = cast(InterfaceName, None)
+    associationName:        AssociationName         = cast(AssociationName, None)
+    sourceCardinality:      SourceCardinality       = cast(SourceCardinality, None)
+    destinationCardinality: DestinationCardinality  = cast(DestinationCardinality, None)
+
+
+CreatedLinkCallback = Callable[[OglLink], None]
+
 
 def createPluginClassesFactory() -> OglClasses:
     """
     Factory method to create  the OglClasses data structure;
 
     Returns:  A new data structure
     """
```

### Comparing `pyutplugins-2.3.1/src/pyutplugins/IPluginAdapter.py` & `pyutplugins-2.4.0/src/pyutplugins/IPluginAdapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 
 from abc import ABC
 from abc import abstractmethod
 
 from dataclasses import dataclass
 
+from ogl.OglLink import OglLink
+
+from pyutplugins.ExternalTypes import CreatedLinkCallback
 from pyutplugins.ExternalTypes import CurrentProjectCallback
+from pyutplugins.ExternalTypes import LinkInformation
+from pyutplugins.ExternalTypes import ObjectBoundaryCallback
 from pyutplugins.ExternalTypes import OglObjectType
 from pyutplugins.ExternalTypes import FrameInformationCallback
 from pyutplugins.ExternalTypes import FrameSizeCallback
 from pyutplugins.ExternalTypes import PluginProject
 from pyutplugins.ExternalTypes import SelectedOglObjectsCallback
 
 
@@ -71,14 +76,25 @@
 
         Args:
             callback:  This method is invoked with a list of all the selected OglObjects
         """
         pass
 
     @abstractmethod
+    def getObjectBoundaries(self, callback: ObjectBoundaryCallback):
+        """
+        Request the boundaries around all the UML objects
+        on the current frame
+
+        Args:
+            callback:  The callback that receives the boundaries
+        """
+        pass
+
+    @abstractmethod
     def refreshFrame(self):
         """
         Refresh the currently displayed frame
         """
         pass
 
     @abstractmethod
@@ -126,7 +142,15 @@
 
     @abstractmethod
     def indicatePluginModifiedProject(self):
         """
         Plugins always work on the current frame or project
         """
         pass
+
+    @abstractmethod
+    def deleteLink(self, oglLink: OglLink):
+        pass
+
+    @abstractmethod
+    def createLink(self, linkInformation: LinkInformation, callback: CreatedLinkCallback):
+        pass
```

### Comparing `pyutplugins-2.3.1/src/pyutplugins/PluginManager.py` & `pyutplugins-2.4.0/src/pyutplugins/PluginManager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 
 from typing import Callable
 from typing import cast
 
 from logging import Logger
 from logging import getLogger
 
+from os import linesep as osLineSep
+
+from sys import exc_info
+
+from traceback import extract_tb
+
 from wx import ICON_ERROR
 from wx import OK
 
 from wx import MessageDialog
 from wx import NewIdRef
 
 from wx import Yield as wxYield
@@ -36,15 +42,18 @@
 from pyutplugins.ioplugins.IOWxImage import IOWxImage
 from pyutplugins.ioplugins.IOXml import IOXml
 from pyutplugins.ioplugins.IOMermaid import IOMermaid
 from pyutplugins.ioplugins.IOAscii import IOAscii
 
 from pyutplugins.toolplugins.ToolForceDirectedLayout import ToolForceDirectedLayout
 from pyutplugins.toolplugins.ToolArrangeLinks import ToolArrangeLinks
+from pyutplugins.toolplugins.ToolLoadLayout import ToolLoadLayout
 from pyutplugins.toolplugins.ToolOrthogonalLayoutV2 import ToolOrthogonalLayoutV2
+from pyutplugins.toolplugins.ToolOrthogonalRouting import ToolOrthogonalRouting
+from pyutplugins.toolplugins.ToolSaveLayout import ToolSaveLayout
 from pyutplugins.toolplugins.ToolSugiyama import ToolSugiyama
 from pyutplugins.toolplugins.ToolTransforms import ToolTransforms
 
 
 TOOL_PLUGIN_NAME_PREFIX: str = 'Tool'
 IO_PLUGIN_NAME_PREFIX:   str = 'IO'
 
@@ -64,15 +73,20 @@
     IOPlugin=packageName.PluginModule
 
     By convention prefix the plugin tool module name with the characters 'Tool'
     By convention prefix the plugin I/O module with the characters 'IO'
 
     """
     IO_PLUGINS:   PluginList = PluginList([IOMermaid, IODTD, IOGML, IOJava, IOPdf, IOPython, IOWxImage, IOXml, IOAscii])
-    TOOL_PLUGINS: PluginList = PluginList([ToolForceDirectedLayout, ToolArrangeLinks, ToolOrthogonalLayoutV2, ToolSugiyama, ToolTransforms])
+    TOOL_PLUGINS: PluginList = PluginList(
+        [
+            ToolOrthogonalRouting, ToolForceDirectedLayout, ToolArrangeLinks, ToolOrthogonalLayoutV2, ToolSugiyama, ToolTransforms,
+            ToolSaveLayout, ToolLoadLayout
+        ]
+    )
 
     def __init__(self, **kwargs):
         """
         Expects a pluginAdapter parameter in kwargs
 
         Args:
             *args:
@@ -88,14 +102,39 @@
         self._outputPluginsMap: OutputPluginMap  = OutputPluginMap()
 
         self._inputPluginClasses:  PluginList = cast(PluginList, None)
         self._outputPluginClasses: PluginList = cast(PluginList, None)
 
         self._pluginAdapter: IPluginAdapter = kwargs['pluginAdapter']
 
+    @classmethod
+    def getErrorInfo(cls) -> str:
+        """
+        TODO:
+        This needs to be moved to code ally basic
+        This version uses f strings
+
+        Returns:
+            System exception information as a formatted string
+        """
+        errMsg: str = ''
+        if exc_info()[0] is not None:
+            errMsg = f'Error : {exc_info()[0]}{osLineSep}'
+
+        if exc_info()[1] is not None:
+            errMsg = f'{errMsg}Msg   : {exc_info()[1]}{osLineSep}'
+
+        if exc_info()[2] is not None:
+            errMsg = f'{errMsg}Trace :{osLineSep}'
+
+            for el in extract_tb(exc_info()[2]):
+                errMsg = f'{errMsg}{str(el)}{osLineSep}'
+
+        return errMsg
+
     @property
     def inputPlugins(self) -> PluginList:
         """
         Get the input pyutplugins.
 
         Returns:  A list of classes (the pyutplugins classes).
         """
@@ -166,16 +205,22 @@
         # Create a plugin instance
         pluginInstance: ToolPluginInterface = clazz(pluginAdapter=self._pluginAdapter)
 
         # Do plugin functionality
         try:
             pluginInstance.executeTool()
             self.logger.debug(f"After tool plugin do action")
-        except (ValueError, Exception) as e:
+        except (ValueError, Exception, ) as e:
             self.logger.error(f'{e}')
+            extendedMessage: str = PluginManager.getErrorInfo()
+            self.logger.error(f'{extendedMessage}')
+            booBoo: MessageDialog = MessageDialog(parent=None,
+                                                  message=f'{extendedMessage}',
+                                                  caption='Error!', style=OK | ICON_ERROR)
+            booBoo.ShowModal()
 
     def doImport(self, wxId: int):
         """
         Args:
             wxId:       The ID ref of the menu item
         """
         idMap:        PluginIDMap    = self.inputPluginsMap.pluginIdMap
```

### Comparing `pyutplugins-2.3.1/src/pyutplugins/common/ElementTreeData.py` & `pyutplugins-2.4.0/src/pyutplugins/common/ElementTreeData.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/common/LinkMakerMixin.py` & `pyutplugins-2.4.0/src/pyutplugins/common/LinkMakerMixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 from typing import cast
 
 from logging import Logger
 from logging import getLogger
 
-from ogl.OglAssociation import OglAssociation
 from ogl.OglClass import OglClass
 from ogl.OglInterface import OglInterface
 from ogl.OglLink import OglLink
 from ogl.OglLinkFactory import OglLinkFactory
 
 from pyutmodelv2.PyutClass import PyutClass
 from pyutmodelv2.PyutLink import PyutLink
@@ -42,21 +41,14 @@
         """
         sourceClass:      PyutClass = cast(PyutClass, src.pyutObject)
         destinationClass: PyutClass = cast(PyutClass, dst.pyutObject)
 
         pyutLink: PyutLink = PyutLink("", linkType=linkType, source=sourceClass, destination=destinationClass)
 
         oglLink = self._oglLinkFactory.getOglLink(src, pyutLink, dst, linkType)
-        #
-        # TODO: Is this a hack?  I think it is
-        # duplicate from Pyut;   This should be done by the OglLinkFactory
-        #
-        if isinstance(oglLink, OglAssociation):
-            oglAssociation: OglAssociation = cast(OglAssociation, oglLink)
-            oglAssociation.createDefaultAssociationLabels()
 
         src.addLink(oglLink)
         dst.addLink(oglLink)
 
         pyutClass: PyutClass = cast(PyutClass, src.pyutObject)
         pyutClass.addLink(pyutLink)
```

### Comparing `pyutplugins-2.3.1/src/pyutplugins/common/ui/BaseEditDialog.py` & `pyutplugins-2.4.0/src/pyutplugins/common/ui/BaseEditDialog.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/common/ui/preferences/PluginPreferencesPage.py` & `pyutplugins-2.4.0/src/pyutplugins/common/ui/preferences/PluginPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOAscii.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOAscii.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/IODTD.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IODTD.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOGML.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOGML.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOJava.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOJava.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOMermaid.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOMermaid.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.logger: Logger = getLogger(__name__)
 
         self._requireSelection = False      # Override base class
         self._autoSelectAll    = True
         # from super class
         self._name    = PluginName('Mermaid Writer')
         self._author  = 'Humberto A. Sanchez II'
-        self._version = '0.50'
+        self._version = MermaidWriter.VERSION
         self._inputFormat  = cast(InputFormat, None)
         self._outputFormat = OutputFormat(formatName=FORMAT_NAME, extension=PLUGIN_EXTENSION, description=PLUGIN_DESCRIPTION)
 
         self._exportResponse: SingleFileRequestResponse = cast(SingleFileRequestResponse, None)
         self._oglObjects:     OglObjects                = cast(OglObjects, None)
 
     def setImportOptions(self) -> bool:
```

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOPdf.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOPdf.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOPython.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOPython.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOWxImage.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOWxImage.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/IOXml.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOXml.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/dtd/DTDParser.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/DTDParser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/gml/GMLExporter.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/GMLExporter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/java/JavaReader.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/JavaReader.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/java/JavaWriter.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/JavaWriter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/mermaid/MermaidDirection.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/MermaidDirection.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/mermaid/MermaidWriter.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/MermaidWriter.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,38 +12,40 @@
 
 from datetime import datetime
 
 from pathlib import Path
 
 from pyutmodelv2.PyutField import PyutField
 from pyutmodelv2.PyutField import PyutFields
+from pyutmodelv2.PyutInterface import PyutInterface
 from pyutmodelv2.PyutLink import LinkDestination
 from pyutmodelv2.PyutLink import LinkSource
 from pyutmodelv2.PyutLink import PyutLink
 from pyutmodelv2.PyutNote import PyutNote
 from pyutmodelv2.PyutText import PyutText
 from pyutmodelv2.PyutType import PyutType
 from pyutmodelv2.PyutClass import PyutClass
 from pyutmodelv2.PyutMethod import PyutMethod
 from pyutmodelv2.PyutParameter import PyutParameter
+from pyutmodelv2.PyutModelTypes import Implementors
 
 from pyutmodelv2.enumerations.PyutStereotype import PyutStereotype
 from pyutmodelv2.enumerations.PyutVisibility import PyutVisibility
 
 from ogl.OglNote import OglNote
 from ogl.OglText import OglText
 from ogl.OglLink import OglLink
-from ogl.OglNoteLink import OglNoteLink
 from ogl.OglClass import OglClass
+from ogl.OglNoteLink import OglNoteLink
 from ogl.OglInterface2 import OglInterface2
+from ogl.OglInterface import OglInterface
 from ogl.OglAggregation import OglAggregation
 from ogl.OglInheritance import OglInheritance
 from ogl.OglComposition import OglComposition
 from ogl.OglAssociation import OglAssociation
-from ogl.OglInterface import OglInterface
 
 from pyutplugins.ExternalTypes import OglObjects
 from pyutplugins.ioplugins.mermaid.MermaidDirection import MermaidDirection
 from pyutplugins.preferences.PluginPreferences import PluginPreferences
 
 
 indent1: str = '    '
@@ -55,18 +57,19 @@
 
 class MermaidArrow(Enum):
     INHERITANCE_ARROW = '<|--'  # Points to parent class
     AGGREGATION_LINK  = 'o--'   #
     COMPOSITION_LINK  = '*--'   #
     INTERFACE_LINK    = '..|>'  #
     ASSOCIATION_LINK  = '--'
+    LOLLIPOP_LINK     = '()--'  # left side is interface, right is implementor
 
 
 class MermaidWriter:
-    VERSION: str = '0.5'
+    VERSION: str = '0.7'
 
     def __init__(self, fqFileName: Path, writeCredits: bool = True):
         """
 
         Args:
             fqFileName:     Fully qualified file name to write to
             writeCredits:   We will always write credits.  Unit tests turn this off
@@ -178,15 +181,16 @@
                 case OglNoteLink():
                     oglNoteLink: OglNoteLink = cast(OglNoteLink, oglObject)
                     linkRefrain = self._getNoteLinkRefrain(oglNoteLink)
                 case OglAssociation():      # Most general needs to be last
                     oglAssociation: OglAssociation = cast(OglAssociation, oglObject)
                     linkRefrain = self._getAssociationLinkRefrain(oglAssociation=oglAssociation, arrowType=MermaidArrow.ASSOCIATION_LINK)
                 case OglInterface2():
-                    self.logger.warning(f'OglInterface2 (lollipops) not supported in Mermaid')
+                    oglInterface2: OglInterface2 = cast(OglInterface2, oglObject)
+                    linkRefrain = self._generateLollipopRefrain(oglInterface2)
                 case _:
                     pass        # Ignore non links
             linksStanza += linkRefrain
 
         return linksStanza
 
     def _getInheritanceLinkRefrain(self, oglLink: OglLink) -> str:
@@ -272,14 +276,33 @@
         assert isinstance(pyutNote, PyutNote), 'Diagram error;  Source must be the note'
 
         linkRefrain: str = (
             f'{indent1}note for {destObject.name} "{pyutNote.content}"{eol}'
         )
         return linkRefrain
 
+    def _generateLollipopRefrain(self, oglInterface2: OglInterface2) -> str:
+        """
+        Interface1 ()-- Interface1Impl
+        Args:
+            oglInterface2:
+
+        Returns:
+        """
+
+        pyutInterface: PyutInterface = oglInterface2.pyutInterface
+        implementors:  Implementors = pyutInterface.implementors
+
+        linkRefrain: str = ''
+        for implementor in implementors:
+            lollipopRefrain: str = f'{indent1}{pyutInterface.name} {MermaidArrow.LOLLIPOP_LINK.value} {implementor} {eol}'
+            linkRefrain += lollipopRefrain
+
+        return linkRefrain
+
     def _getCardinalityStrings(self, pyutLink) -> Tuple[str, str]:
         """
 
         Args:
             pyutLink:
 
         Returns: A tuple of source, destination cardinality strings
```

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/pdf/ImageOptions.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/ImageOptions.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/pdf/PyUmlDefinitionAdapter.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/PyUmlDefinitionAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/PyutToPython.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/PyutToPython.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/ReverseEngineerPythonV3.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/ReverseEngineerPythonV3.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexer.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexer.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexerBase.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexerBase.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParser.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParserBase.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParserBase.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonPegParserVisitor.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonPegParserVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/ParentsDictionaryHandler.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/ParentsDictionaryHandler.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/ParserTypes.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/ParserTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/PyutBaseVisitor.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutBaseVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegClassVisitor.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegClassVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegVisitor.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         self.Bind(EVT_BUTTON, self._onFileSelectClick,   self._fileSelectBtn)
         self.Bind(EVT_CHOICE, self._onImageFormatChoice, self._imageFormatChoice)
         #
         self._selectedFile.Bind(EVT_MOTION, self._fileSelectionMotion, self._selectedFile)
         self.Bind(EVT_BUTTON, self._onOk, id=ID_OK)
         self.Bind(EVT_CLOSE, self._onClose, id=ID_CANCEL)
 
-
     def _fileSelectionMotion(self, event: MouseEvent):
 
         ctrl: TextCtrl = event.GetEventObject()
 
         tip = ctrl.GetToolTip()
         tip.SetTip(self._outputFileName)
```

### Comparing `pyutplugins-2.3.1/src/pyutplugins/ioplugins/wximage/WxImageFormat.py` & `pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/WxImageFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/plugininterfaces/BasePluginInterface.py` & `pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/BasePluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/plugininterfaces/IOPluginInterface.py` & `pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/IOPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/plugininterfaces/ToolPluginInterface.py` & `pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/ToolPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/plugintypes/BaseFormat.py` & `pyutplugins-2.4.0/src/pyutplugins/plugintypes/BaseFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/plugintypes/InputFormat.py` & `pyutplugins-2.4.0/src/pyutplugins/plugintypes/InputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/plugintypes/OutputFormat.py` & `pyutplugins-2.4.0/src/pyutplugins/plugintypes/OutputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/plugintypes/PluginDataTypes.py` & `pyutplugins-2.4.0/src/pyutplugins/plugintypes/PluginDataTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/preferences/PluginPreferences.py` & `pyutplugins-2.4.0/src/pyutplugins/preferences/PluginPreferences.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/ToolArrangeLinks.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolArrangeLinks.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/ToolForceDirectedLayout.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolForceDirectedLayout.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/ToolSugiyama.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolSugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/ToolTransforms.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolTransforms.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/forcedirectedlayout/ConfigurationPanel.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/ConfigurationPanel.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/forcedirectedlayout/DlgConfiguration.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/DlgConfiguration.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/forcedirectedlayout/OglNode.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/OglNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/ALayoutLink.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/ALayoutLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/ALayoutNode.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/ALayoutNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/Sugiyama.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/Sugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py` & `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.3.1/src/pyutplugins.egg-info/PKG-INFO` & `pyutplugins-2.4.0/src/pyutplugins.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: pyutplugins
-Version: 2.3.1
+Version: 2.4.0
 Summary: Pyut Plugins
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/pyutplugins
 Keywords: pyut,python,plugin
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: codeallybasic>=1.3.1
 Requires-Dist: codeallyadvanced>=1.3.1
 Requires-Dist: pyutmodelv2>=2.1.5
-Requires-Dist: ogl>=2.1.20
-Requires-Dist: untanglepyut>=2.1.7
+Requires-Dist: ogl>=2.1.32
+Requires-Dist: untanglepyut>=2.1.8
 Requires-Dist: oglio>=2.1.7
 Requires-Dist: pyumldiagrams>=3.1.10
 Requires-Dist: wxPython~=4.2.1
 Requires-Dist: antlr4-python3-runtime==4.13.1
 Requires-Dist: networkx==3.0
 Requires-Dist: orthogonal==1.2.0
 Requires-Dist: pyforcedirectedlayout>=0.80.2
+Requires-Dist: pyorthogonalrouting>=1.2.0
 
 ![](https://github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-2-256x48.png "AGPL")
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/pyutplugins/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/pyutplugins/tree/master)
 [![PyPI version](https://badge.fury.io/py/pyutplugins.svg)](https://badge.fury.io/py/pyutplugins)
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: pyutplugins Version: 2.3.1 Summary: Pyut Plugins
+Metadata-Version: 2.1 Name: pyutplugins Version: 2.4.0 Summary: Pyut Plugins
 Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/pyutplugins Keywords: pyut,python,plugin
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 codeallybasic>=1.3.1 Requires-Dist: codeallyadvanced>=1.3.1 Requires-Dist:
-pyutmodelv2>=2.1.5 Requires-Dist: ogl>=2.1.20 Requires-Dist:
-untanglepyut>=2.1.7 Requires-Dist: oglio>=2.1.7 Requires-Dist:
+pyutmodelv2>=2.1.5 Requires-Dist: ogl>=2.1.32 Requires-Dist:
+untanglepyut>=2.1.8 Requires-Dist: oglio>=2.1.7 Requires-Dist:
 pyumldiagrams>=3.1.10 Requires-Dist: wxPython~=4.2.1 Requires-Dist: antlr4-
 python3-runtime==4.13.1 Requires-Dist: networkx==3.0 Requires-Dist:
-orthogonal==1.2.0 Requires-Dist: pyforcedirectedlayout>=0.80.2 ![](https://
-github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-
-badge-version-2-256x48.png "AGPL") [![Maintenance](https://img.shields.io/
-badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/
-graphs/commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/
-gh/hasii2011/pyutplugins/tree/master.svg?style=shield)](https://
-dl.circleci.com/status-badge/redirect/gh/hasii2011/pyutplugins/tree/master) [!
-[PyPI version](https://badge.fury.io/py/pyutplugins.svg)](https://
-badge.fury.io/py/pyutplugins) [![CircleCI](https://dl.circleci.com/insights-
-snapshot/gh/hasii2011/pyutplugins/master/main/badge.svg?window=30d)](https://
-app.circleci.com/insights/github/hasii2011/pyutplugins/workflows/main/
-overview?branch=master&reporting-window=last-30-days&insights-snapshot=true) #
-Introduction **TBD** # Overview **TBD** ## Developer Notes This project uses
-[buildlackey](https://github.com/hasii2011/buildlackey) for day to day
-development builds ___ Written by _H_u_m_b_e_r_t_o_ _A_._ _S_a_n_c_h_e_z_ _I_I (C) 2023 ___ I am
-concerned about GitHub's Copilot project ![](https://github.com/hasii2011/code-
-ally-basic/blob/master/developer/SillyGitHub.png) I urge you to read about the
-[Give up GitHub](https://GiveUpGitHub.org) campaign from [the Software Freedom
-Conservancy](https://sfconservancy.org). While I do not advocate for all the
-issues listed there I do not like that a company like Microsoft may profit from
-open source projects. I continue to use GitHub because it offers the services I
-need for free. But, I continue to monitor their terms of service. Any use of
-this project's code by GitHub Copilot, past or present, is done without my
-permission. I do not consent to GitHub's use of this project's code in Copilot.
+orthogonal==1.2.0 Requires-Dist: pyforcedirectedlayout>=0.80.2 Requires-Dist:
+pyorthogonalrouting>=1.2.0 ![](https://github.com/hasii2011/code-ally-basic/
+blob/master/developer/agpl-license-web-badge-version-2-256x48.png "AGPL") [!
+[Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
+//GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
+dl.circleci.com/status-badge/img/gh/hasii2011/pyutplugins/tree/
+master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/
+hasii2011/pyutplugins/tree/master) [![PyPI version](https://badge.fury.io/py/
+pyutplugins.svg)](https://badge.fury.io/py/pyutplugins) [![CircleCI](https://
+dl.circleci.com/insights-snapshot/gh/hasii2011/pyutplugins/master/main/
+badge.svg?window=30d)](https://app.circleci.com/insights/github/hasii2011/
+pyutplugins/workflows/main/overview?branch=master&reporting-window=last-30-
+days&insights-snapshot=true) # Introduction **TBD** # Overview **TBD** ##
+Developer Notes This project uses [buildlackey](https://github.com/hasii2011/
+buildlackey) for day to day development builds ___ Written by _H_u_m_b_e_r_t_o_ _A_.
+_S_a_n_c_h_e_z_ _I_I (C) 2023 ___ I am concerned about GitHub's Copilot project ![]
+(https://github.com/hasii2011/code-ally-basic/blob/master/developer/
+SillyGitHub.png) I urge you to read about the [Give up GitHub](https://
+GiveUpGitHub.org) campaign from [the Software Freedom Conservancy](https://
+sfconservancy.org). While I do not advocate for all the issues listed there I
+do not like that a company like Microsoft may profit from open source projects.
+I continue to use GitHub because it offers the services I need for free. But, I
+continue to monitor their terms of service. Any use of this project's code by
+GitHub Copilot, past or present, is done without my permission. I do not
+consent to GitHub's use of this project's code in Copilot.
```

### Comparing `pyutplugins-2.3.1/src/pyutplugins.egg-info/SOURCES.txt` & `pyutplugins-2.4.0/src/pyutplugins.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -99,15 +99,18 @@
 src/pyutplugins/plugintypes/__init__.py
 src/pyutplugins/plugintypes/py.typed
 src/pyutplugins/preferences/PluginPreferences.py
 src/pyutplugins/preferences/__init__.py
 src/pyutplugins/preferences/py.typed
 src/pyutplugins/toolplugins/ToolArrangeLinks.py
 src/pyutplugins/toolplugins/ToolForceDirectedLayout.py
+src/pyutplugins/toolplugins/ToolLoadLayout.py
 src/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
+src/pyutplugins/toolplugins/ToolOrthogonalRouting.py
+src/pyutplugins/toolplugins/ToolSaveLayout.py
 src/pyutplugins/toolplugins/ToolSugiyama.py
 src/pyutplugins/toolplugins/ToolTransforms.py
 src/pyutplugins/toolplugins/__init__.py
 src/pyutplugins/toolplugins/py.typed
 src/pyutplugins/toolplugins/forcedirectedlayout/ConfigurationPanel.py
 src/pyutplugins/toolplugins/forcedirectedlayout/DlgConfiguration.py
 src/pyutplugins/toolplugins/forcedirectedlayout/OglNode.py
@@ -115,14 +118,21 @@
 src/pyutplugins/toolplugins/forcedirectedlayout/py.typed
 src/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
 src/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
 src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
 src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
 src/pyutplugins/toolplugins/orthogonal/__init__.py
 src/pyutplugins/toolplugins/orthogonal/py.typed
+src/pyutplugins/toolplugins/orthogonalrouting/DlgConfiguration.py
+src/pyutplugins/toolplugins/orthogonalrouting/LabelledSlider.py
+src/pyutplugins/toolplugins/orthogonalrouting/OrthogonalConnectorAdapter.py
+src/pyutplugins/toolplugins/orthogonalrouting/__init__.py
+src/pyutplugins/toolplugins/orthogonalrouting/py.typed
+src/pyutplugins/toolplugins/savelayout/Layout.py
+src/pyutplugins/toolplugins/savelayout/__init__.py
 src/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
 src/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
 src/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
 src/pyutplugins/toolplugins/sugiyama/Sugiyama.py
 src/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
 src/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
 src/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
```

