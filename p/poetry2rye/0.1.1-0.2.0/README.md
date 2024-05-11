# Comparing `tmp/poetry2rye-0.1.1.tar.gz` & `tmp/poetry2rye-0.2.0.tar.gz`

## Comparing `poetry2rye-0.1.1.tar` & `poetry2rye-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.python-version
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/requirements-dev.lock
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/requirements.lock
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/poetry2rye.iml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/workspace.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/src/poetry2rye/__init__.py
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/src/poetry2rye/convert.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/src/poetry2rye/main.py
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/src/poetry2rye/project.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/src/poetry2rye/utils.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/LICENSE
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/README.md
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/.python-version
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/requirements.lock
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/.idea/.gitignore
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/.idea/modules.xml
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/.idea/poetry2rye.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/src/poetry2rye/__init__.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/src/poetry2rye/convert.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/src/poetry2rye/main.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/src/poetry2rye/project.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/src/poetry2rye/utils.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/README.md
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 poetry2rye-0.2.0/PKG-INFO
```

### Comparing `poetry2rye-0.1.1/.idea/workspace.xml` & `poetry2rye-0.2.0/.idea/workspace.xml`

 * *Files 16% similar despite different names*

#### Comparing `poetry2rye-0.1.1/.idea/workspace.xml` & `poetry2rye-0.2.0/.idea/workspace.xml`

```diff
@@ -1,22 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="fd34f470-3de9-4a99-986d-899ced410e33" name="変更" comment="created">
-      <change afterPath="$PROJECT_DIR$/src/poetry2rye/convert.py" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/src/poetry2rye/main.py" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/src/poetry2rye/project.py" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/src/poetry2rye/utils.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/requirements-dev.lock" beforeDir="false" afterPath="$PROJECT_DIR$/requirements-dev.lock" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/requirements.lock" beforeDir="false" afterPath="$PROJECT_DIR$/requirements.lock" afterDir="false"/>
+    <list default="true" id="fd34f470-3de9-4a99-986d-899ced410e33" name="変更" comment="fix: update dependency">
+      <change beforePath="$PROJECT_DIR$/src/poetry2rye/convert.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/poetry2rye/convert.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/poetry2rye/project.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/poetry2rye/project.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -25,43 +19,66 @@
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
+  <component name="GitHubPullRequestSearchHistory">{
+  &quot;lastFilter&quot;: {
+    &quot;state&quot;: &quot;OPEN&quot;,
+    &quot;assignee&quot;: &quot;nahco314&quot;
+  }
+}</component>
+  <component name="GithubPullRequestsUISettings">{
+  &quot;selectedUrlAndAccountId&quot;: {
+    &quot;url&quot;: &quot;https://github.com/nahco314/poetry2rye.git&quot;,
+    &quot;accountId&quot;: &quot;c4a9a7e8-1074-44e5-b265-027e9c401369&quot;
+  }
+}</component>
   <component name="MacroExpansionManager">
     <option name="directoryName" value="mllplg75"/>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
+  <component name="ProjectColorInfo">{
+  &quot;customColor&quot;: &quot;&quot;,
+  &quot;associatedIndex&quot;: 6
+}</component>
   <component name="ProjectId" id="2QTohsvwjiNyrwveUyq5ET5svjk"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "WebServerToolWindowFactoryState": "false",
-    "last_opened_file_path": "/home/nahco314/PycharmProjects/__test_0",
+    "git-widget-placeholder": "master",
+    "last_opened_file_path": "/home/nahco314/PycharmProjects/cp",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
-    "settings.editor.selected.configurable": "preferences.lookFeel",
+    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
+  <component name="RecentsManager">
+    <key name="CopyFile.RECENT_KEYS">
+      <recent name="$PROJECT_DIR$"/>
+    </key>
+  </component>
   <component name="RunManager" selected="Python.convert">
     <configuration name="convert" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="poetry2rye"/>
+      <option name="ENV_FILES" value=""/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/src/poetry2rye"/>
@@ -76,14 +93,15 @@
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
     <configuration name="project" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="poetry2rye"/>
+      <option name="ENV_FILES" value=""/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/src/poetry2rye"/>
@@ -103,26 +121,59 @@
     <recent_temporary>
       <list>
         <item itemvalue="Python.convert"/>
         <item itemvalue="Python.project"/>
       </list>
     </recent_temporary>
   </component>
+  <component name="SharedIndexes">
+    <attachedChunks>
+      <set>
+        <option value="bundled-js-predefined-1d06a55b98c1-91d5c284f522-JavaScript-PY-241.15989.155"/>
+        <option value="bundled-python-sdk-babbdf50b680-7c6932dee5e4-com.jetbrains.pycharm.pro.sharedIndexes.bundled-PY-241.15989.155"/>
+      </set>
+    </attachedChunks>
+  </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="アプリケーションレベル" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="デフォルトタスク">
       <changelist id="fd34f470-3de9-4a99-986d-899ced410e33" name="変更" comment=""/>
       <created>1685387054971</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1685387054971</updated>
       <workItem from="1685387055969" duration="10367000"/>
       <workItem from="1685464921251" duration="5970000"/>
-      <workItem from="1685473028177" duration="10864000"/>
+      <workItem from="1685473028177" duration="12565000"/>
+      <workItem from="1685687322538" duration="665000"/>
+      <workItem from="1685719123088" duration="13000"/>
+      <workItem from="1685743124949" duration="6000"/>
+      <workItem from="1685748170927" duration="1208000"/>
+      <workItem from="1685783418982" duration="601000"/>
+      <workItem from="1685836884222" duration="1290000"/>
+      <workItem from="1685932745454" duration="599000"/>
+      <workItem from="1686155908875" duration="599000"/>
+      <workItem from="1686297900217" duration="148000"/>
+      <workItem from="1686462528601" duration="54000"/>
+      <workItem from="1686651897982" duration="101000"/>
+      <workItem from="1686722581773" duration="602000"/>
+      <workItem from="1687002573892" duration="89000"/>
+      <workItem from="1687088881246" duration="603000"/>
+      <workItem from="1715234101892" duration="1903000"/>
+      <workItem from="1715441911554" duration="4657000"/>
+    </task>
+    <task id="LOCAL-00001" summary="fix: update dependency">
+      <option name="closed" value="true"/>
+      <created>1715443014516</created>
+      <option name="number" value="00001"/>
+      <option name="presentableId" value="LOCAL-00001"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715443014516</updated>
     </task>
+    <option name="localTasksCounter" value="2"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -131,12 +182,16 @@
           <value>
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
+  <component name="VcsManagerConfiguration">
+    <MESSAGE value="fix: update dependency"/>
+    <option name="LAST_COMMIT_MESSAGE" value="fix: update dependency"/>
+  </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/poetry2rye$project.coverage" NAME="project のカバレッジ結果" MODIFIED="1685392433129" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/poetry2rye"/>
     <SUITE FILE_PATH="coverage/poetry2rye$convert.coverage" NAME="convert のカバレッジ結果" MODIFIED="1685396908506" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/poetry2rye"/>
   </component>
 </project>
```

### Comparing `poetry2rye-0.1.1/src/poetry2rye/convert.py` & `poetry2rye-0.2.0/src/poetry2rye/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 from poetry.core.version.helpers import format_python_constraint
 
 from poetry2rye.project import BasicDependency
 from poetry2rye.project import PoetryProject
 from poetry2rye.utils import get_next_backup_path
 
 
+def read_name_email(string: str) -> dict[str, str]:
+    name, _, email = string.rpartition(" ")
+    return {"name": name, "email": email[1:-1]}
+
+
 def convert(project_path: Path) -> None:
     project_backup = get_next_backup_path(project_path)
     shutil.copytree(project_path, project_backup, dirs_exist_ok=True, symlinks=True)
     print(f"created backup: {project_backup}")
 
     poetry_project = PoetryProject(project_path)
 
@@ -30,28 +35,20 @@
     project_sec["description"] = poetry_project.poetry["description"]
 
     # license (not used due to different format)
     if poetry_project.poetry.get("license"):
         pass
 
     # authors / maintainers
-    authors = []
-    for author in poetry_project.poetry["authors"]:
-        seps = author.split()
-        assert len(seps) == 2
-        authors.append({"name": seps[0], "email": seps[1][1:-1]})
+    authors = list(map(read_name_email, poetry_project.poetry["authors"]))
     if authors:
         project_sec["authors"] = tomlkit.array()
         project_sec["authors"].extend(authors)
 
-    maintainers = []
-    for maintainer in poetry_project.poetry.get("maintainers", []):
-        seps = maintainer.split()
-        assert len(seps) == 2
-        maintainers.append({"name": seps[0], "email": seps[1][1:-1]})
+    maintainers = list(map(read_name_email, poetry_project.poetry.get("maintainers", [])))
     if maintainers:
         project_sec["maintainers"] = tomlkit.array()
         project_sec["maintainers"].extend(maintainers)
 
     # readme
     if poetry_project.poetry.get("readme"):
         project_sec["readme"] = poetry_project.poetry["readme"]
@@ -112,25 +109,28 @@
                 )
             )
             result["build-system"]["requires"].append("hatchling")
             result["build-system"]["build-backend"] = "hatchling.build"
         else:
             result[name] = deepcopy(pyproject[name])
 
+    packages = [f"src/{poetry_project.module_name}"]
+
     result["tool"]["rye"] = tool_rye_sec
     result["tool"]["hatch"] = {"metadata": {"allow-direct-references": True}}
+    result["tool"]["hatch"]["build"] = {"targets": {"wheel": {"packages": packages}}}
 
     with open(project_path / "pyproject.toml", "w") as f:
         f.write(tomlkit.dumps(result))
 
     # find "poetry" in pyproject.toml and print it
     with open(project_path / "pyproject.toml") as f:
         for num, content in enumerate(f.readlines(), start=1):
             if "poetry" in content:
-                print(f"Found 'poetry' in line {num}: {content}")
+                print(f"Found 'poetry' in line {num}: {content.strip()}")
 
     if (project_path / "poetry.lock").exists():
         os.remove(project_path / "poetry.lock")
     if not (project_path / "src").exists():
         (project_path / "src").mkdir()
         shutil.move(
             poetry_project.module_path,
```

### Comparing `poetry2rye-0.1.1/src/poetry2rye/main.py` & `poetry2rye-0.2.0/src/poetry2rye/main.py`

 * *Files identical despite different names*

### Comparing `poetry2rye-0.1.1/src/poetry2rye/project.py` & `poetry2rye-0.2.0/src/poetry2rye/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,22 +80,29 @@
             "pyproject.toml written using "
             "tool.poetry. this may change in the "
             "future."
         )
         assert self.poetry is not None, "poetry section not found in pyproject.toml"
 
         self.src_path: Path
+        self.module_path: Path
         # this method is not exact, but tentatively we do this
         if (self.path / "src").exists():
             self.src_path = self.path / "src"
+            sub_lst = list(self.src_path.iterdir())
+            if len(sub_lst) == 1:
+                self.src_path = sub_lst[0]
+            elif len(sub_lst) == 0:
+                raise FileNotFoundError("no subdirectories found in src")
+            else:
+                raise FileNotFoundError("multiple subdirectories found in src")
         else:
             self.src_path = self.path
-
-        self.module_path = self.src_path / self.module_name
-        assert self.module_path.exists(), "module not found"
+            self.module_path = self.src_path / self.module_name
+            assert self.module_path.exists(), "module not found"
 
     def process_dependencies_dict(
         self, dct: dict[str, Any], is_dev: bool
     ) -> list[Dependency]:
         res = []
 
         for name, item in dct.items():
```

### Comparing `poetry2rye-0.1.1/src/poetry2rye/utils.py` & `poetry2rye-0.2.0/src/poetry2rye/utils.py`

 * *Files identical despite different names*

### Comparing `poetry2rye-0.1.1/LICENSE` & `poetry2rye-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry2rye-0.1.1/README.md` & `poetry2rye-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `poetry2rye-0.1.1/PKG-INFO` & `poetry2rye-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: poetry2rye
-Version: 0.1.1
+Version: 0.2.0
 Summary: A simple tool to migrate your Poetry project to rye
 Author-email: nahco314 <nahco3_ta@yahoo.co.jp>
 License-File: LICENSE
 Requires-Python: >=3.11
-Requires-Dist: poetry-core~=1.6.1
+Requires-Dist: poetry-core>=1.9.0
 Requires-Dist: pydantic~=1.10.8
 Requires-Dist: pyproject-parser~=0.9.0
 Requires-Dist: python-slugify~=8.0.1
 Requires-Dist: tomlkit~=0.11.8
+Requires-Dist: typing-extensions>=4.11.0
 Description-Content-Type: text/markdown
 
 # poetry2rye
 
 A simple tool to migrate your Poetry project to rye.
 
 # Install
```

