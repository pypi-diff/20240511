# Comparing `tmp/package_auto_assembler-0.1.2.tar.gz` & `tmp/package_auto_assembler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "package_auto_assembler-0.1.2.tar", last modified: Wed May  8 22:15:05 2024, max compression
+gzip compressed data, was "package_auto_assembler-0.1.3.tar", last modified: Sat May 11 04:33:18 2024, max compression
```

## Comparing `package_auto_assembler-0.1.2.tar` & `package_auto_assembler-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:15:05.329915 package_auto_assembler-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 22:10:48.000000 package_auto_assembler-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26182 2024-05-08 22:15:05.329915 package_auto_assembler-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-08 22:10:48.000000 package_auto_assembler-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:15:05.329915 package_auto_assembler-0.1.2/package_auto_assembler/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:14:32.000000 package_auto_assembler-0.1.2/package_auto_assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61558 2024-05-08 22:14:32.000000 package_auto_assembler-0.1.2/package_auto_assembler/package_auto_assembler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-08 22:15:04.000000 package_auto_assembler-0.1.2/package_auto_assembler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:15:05.329915 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26182 2024-05-08 22:15:05.000000 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-08 22:15:05.000000 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:15:05.000000 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 22:15:05.000000 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 22:15:05.000000 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:15:05.329915 package_auto_assembler-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:33:18.227254 package_auto_assembler-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-11 04:28:27.000000 package_auto_assembler-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26375 2024-05-11 04:33:18.227254 package_auto_assembler-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-11 04:28:27.000000 package_auto_assembler-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:33:18.227254 package_auto_assembler-0.1.3/package_auto_assembler/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 04:32:33.000000 package_auto_assembler-0.1.3/package_auto_assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63143 2024-05-11 04:32:33.000000 package_auto_assembler-0.1.3/package_auto_assembler/package_auto_assembler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-11 04:33:17.000000 package_auto_assembler-0.1.3/package_auto_assembler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:33:18.227254 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26375 2024-05-11 04:33:18.000000 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-11 04:33:18.000000 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 04:33:18.000000 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-11 04:33:18.000000 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 04:33:18.000000 package_auto_assembler-0.1.3/package_auto_assembler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 04:33:18.227254 package_auto_assembler-0.1.3/setup.cfg
```

### Comparing `package_auto_assembler-0.1.2/LICENSE` & `package_auto_assembler-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `package_auto_assembler-0.1.2/PKG-INFO` & `package_auto_assembler-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package_auto_assembler
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -165,27 +165,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-05-08 22:14:33</td>
+      <td>2024-05-11 04:32:47</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-05-08 22:14:33</td>
+      <td>2024-05-11 04:32:47</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-05-08 22:14:33</td>
+      <td>2024-05-11 04:32:47</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -927,26 +927,31 @@
 
     No relevant commit messages found!
 
 
     No messages to clean were provided
 
 
-##### - overwritting commit messages fro example
+##### - overwritting commit messages from example
 
 
 ```python
 # commit messages from last merge
 rnh.commit_messages
 ```
 
 
 
 
-    ['Update README', 'Update requirements']
+    ['Update README',
+     'Update requirements',
+     '[package_auto_assembler] improved ReleaseNotesHandler with resistance to duplicate history',
+     'Update package version tracking files',
+     'Update README',
+     'Update requirements']
 
 
 
 
 ```python
 example_commit_messages = [
     '[example_module] usage example for initial release notes; bugfixes for RNH',
@@ -977,15 +982,15 @@
 ```
 
     Example filtered_messaged:
     ['[example_module] usage example for initial release notes; bugfixes for RNH', '[example_module] initial release notes handler']
     Example processed_messages:
     ['usage example for initial release notes', 'bugfixes for RNH', 'initial release notes handler']
     Example processed_note_entries:
-    ['# Release notes\n', '\n', '### 0.0.2\n\n    - usage example for initial release notes\n    - bugfixes for RNH\n    - initial release notes handler\n\n', '### 0.0.1\n', '\n', '    - initial version of example_module\n']
+    ['# Release notes\n', '\n', '### 0.0.2\n', '\n', '    - usage example for initial release notes\n', '    - bugfixes for RNH\n', '    - initial release notes handler\n', '\n', '### 0.0.1\n', '    - initial version of example_module\n']
 
 
 ##### - saving updated relese notes
 
 
 ```python
 rnh.existing_contents
@@ -993,15 +998,14 @@
 
 
 
 
     ['# Release notes\n',
      '\n',
      '### 0.0.1\n',
-     '\n',
      '    - initial version of example_module\n']
 
 
 
 
 ```python
 rnh.save_release_notes()
@@ -1021,11 +1025,10 @@
      '### 0.0.2\n',
      '\n',
      '    - usage example for initial release notes\n',
      '    - bugfixes for RNH\n',
      '    - initial release notes handler\n',
      '\n',
      '### 0.0.1\n',
-     '\n',
      '    - initial version of example_module\n']
```

### Comparing `package_auto_assembler-0.1.2/README.md` & `package_auto_assembler-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `package_auto_assembler-0.1.2/package_auto_assembler/package_auto_assembler.py` & `package_auto_assembler-0.1.3/package_auto_assembler/package_auto_assembler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1312,14 +1312,52 @@
         if self.logger is None:
             logging.basicConfig(level=self.loggerLvl, format=self.logger_format)
             logger = logging.getLogger(self.logger_name)
             logger.setLevel(self.loggerLvl)
 
             self.logger = logger
 
+    def _deduplicate_with_exceptions(self,
+                                     lst : list):
+
+        seen = set()
+        buffer = []
+        deduplicated = []
+        version_headers = []
+
+        for item in lst:
+
+            # start filling buffor after version is detected
+            if item.startswith("###"):
+
+                if item in version_headers:
+                    seen.add(item)
+                else:
+                    deduplicated += buffer
+
+                    if deduplicated[-1] != "\n":
+                        deduplicated.append("\n")
+
+                    version_headers.append(item)
+                if deduplicated[-1] != "\n":
+                    buffer.append("\n")
+
+            if item != lst[-1]:
+                # clean buffor when version is detected
+                if item.startswith("###"):
+                    buffer = []
+            else:
+                # in the end append buffor to deduplicated
+                buffer.append(item)
+                deduplicated += buffer
+
+            buffer.append(item)
+
+        return deduplicated
+
     def _get_commits_since_last_merge(self, n_last_messages : int = 1):
 
         # First, find the last merge commit
         find_merge_command = ["git", "log", "--merges", "--format=%H", "-n", str(n_last_messages)]
         merge_result = subprocess.run(find_merge_command, capture_output=True, text=True)
         if merge_result.returncode != 0:
             raise Exception("Failed to find last merge commit")
@@ -1408,32 +1446,47 @@
         if version is None:
             version = self.version
 
         if new_messages is None:
             new_messages = self.processed_messages
 
         # Prepare the new release note section
-        new_release_note = f"### {version}\n\n"
-        for msg in new_messages:
-            new_release_note += f"    - {msg}\n"
+        # new_release_note = f"### {version}\n\n"
+        # for msg in new_messages:
+        #     new_release_note += f"    - {msg}\n"
+
+        if new_messages:
+            new_release_notes = [f"### {version}\n"] + ["\n"]
+            for msg in new_messages:
+                new_release_notes += [f"    - {msg}\n"]
+        else:
+            new_release_notes = []
 
         # If there are existing contents, integrate the new entry
         if existing_contents:
             # Find the location of the first version heading to insert the new release note right after
             index = 0
             for line in existing_contents:
                 if line.strip().startswith('###'):
                     break
                 index += 1
 
             # Insert the new release note section into the contents
-            existing_contents.insert(index, new_release_note + "\n")
+            for new_release_note in new_release_notes:
+                existing_contents.insert(index, new_release_note)
+                index += 1
         else:
+
             # If no existing contents, start a new list of contents
-            existing_contents = ['# Release notes\n\n', new_release_note + "\n"]
+            existing_contents = ["# Release notes\n"] + ["\n"]
+            for new_release_note in new_release_notes:
+                existing_contents += new_release_note
+
+        existing_contents = self._deduplicate_with_exceptions(
+            lst=existing_contents)
 
         self.processed_note_entries = existing_contents
 
 
     def get_release_notes_content(self,
                                   filepath : str = None) -> str:
 
@@ -1469,14 +1522,17 @@
             note_entries = self.processed_note_entries
 
         if self.processed_messages != []:
             # Write the updated or new contents back to the file
             with open(filepath, 'w') as file:
                 file.writelines(note_entries)
 
+
+
+
 @attr.s
 class PackageAutoAssembler:
     # pylint: disable=too-many-instance-attributes
 
     ## inputs
     module_name = attr.ib(type=str)
```

### Comparing `package_auto_assembler-0.1.2/package_auto_assembler/setup.py` & `package_auto_assembler-0.1.3/package_auto_assembler/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="package_auto_assembler",
     packages=["package_auto_assembler"],
-    install_requires=['### package_auto_assembler.py', 'pandas', 'pyyaml', 'pip_audit==2.7.3', 'nbconvert', 'attrs>=22.2.0', 'stdlib-list', 'nbformat'],
+    install_requires=['### package_auto_assembler.py', 'nbconvert', 'attrs>=22.2.0', 'nbformat', 'pyyaml', 'pandas', 'stdlib-list', 'pip_audit==2.7.3'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.1.2"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.1.3"
 )
```

### Comparing `package_auto_assembler-0.1.2/package_auto_assembler.egg-info/PKG-INFO` & `package_auto_assembler-0.1.3/package_auto_assembler.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package-auto-assembler
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -165,27 +165,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-05-08 22:14:33</td>
+      <td>2024-05-11 04:32:47</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-05-08 22:14:33</td>
+      <td>2024-05-11 04:32:47</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-05-08 22:14:33</td>
+      <td>2024-05-11 04:32:47</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -927,26 +927,31 @@
 
     No relevant commit messages found!
 
 
     No messages to clean were provided
 
 
-##### - overwritting commit messages fro example
+##### - overwritting commit messages from example
 
 
 ```python
 # commit messages from last merge
 rnh.commit_messages
 ```
 
 
 
 
-    ['Update README', 'Update requirements']
+    ['Update README',
+     'Update requirements',
+     '[package_auto_assembler] improved ReleaseNotesHandler with resistance to duplicate history',
+     'Update package version tracking files',
+     'Update README',
+     'Update requirements']
 
 
 
 
 ```python
 example_commit_messages = [
     '[example_module] usage example for initial release notes; bugfixes for RNH',
@@ -977,15 +982,15 @@
 ```
 
     Example filtered_messaged:
     ['[example_module] usage example for initial release notes; bugfixes for RNH', '[example_module] initial release notes handler']
     Example processed_messages:
     ['usage example for initial release notes', 'bugfixes for RNH', 'initial release notes handler']
     Example processed_note_entries:
-    ['# Release notes\n', '\n', '### 0.0.2\n\n    - usage example for initial release notes\n    - bugfixes for RNH\n    - initial release notes handler\n\n', '### 0.0.1\n', '\n', '    - initial version of example_module\n']
+    ['# Release notes\n', '\n', '### 0.0.2\n', '\n', '    - usage example for initial release notes\n', '    - bugfixes for RNH\n', '    - initial release notes handler\n', '\n', '### 0.0.1\n', '    - initial version of example_module\n']
 
 
 ##### - saving updated relese notes
 
 
 ```python
 rnh.existing_contents
@@ -993,15 +998,14 @@
 
 
 
 
     ['# Release notes\n',
      '\n',
      '### 0.0.1\n',
-     '\n',
      '    - initial version of example_module\n']
 
 
 
 
 ```python
 rnh.save_release_notes()
@@ -1021,11 +1025,10 @@
      '### 0.0.2\n',
      '\n',
      '    - usage example for initial release notes\n',
      '    - bugfixes for RNH\n',
      '    - initial release notes handler\n',
      '\n',
      '### 0.0.1\n',
-     '\n',
      '    - initial version of example_module\n']
```

