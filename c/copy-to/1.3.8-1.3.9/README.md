# Comparing `tmp/copy-to-1.3.8.tar.gz` & `tmp/copy-to-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copy-to-1.3.8.tar", last modified: Tue Mar  5 21:13:13 2024, max compression
+gzip compressed data, was "copy-to-1.3.9.tar", last modified: Tue Mar  5 21:53:55 2024, max compression
```

## Comparing `copy-to-1.3.8.tar` & `copy-to-1.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2024-03-05 21:13:13.819361 copy-to-1.3.8/
--rw-r--r--   0 burp      (1000) burp      (1001)     1071 2024-01-04 01:45:52.000000 copy-to-1.3.8/LICENSE
--rw-r--r--   0 burp      (1000) burp      (1001)     8914 2024-03-05 21:13:13.819361 copy-to-1.3.8/PKG-INFO
--rw-r--r--   0 burp      (1000) burp      (1001)     8219 2024-03-05 21:12:50.000000 copy-to-1.3.8/README.md
-drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2024-03-05 21:13:13.819361 copy-to-1.3.8/copy_to.egg-info/
--rw-r--r--   0 burp      (1000) burp      (1001)     8914 2024-03-05 21:13:13.000000 copy-to-1.3.8/copy_to.egg-info/PKG-INFO
--rw-r--r--   0 burp      (1000) burp      (1001)      231 2024-03-05 21:13:13.000000 copy-to-1.3.8/copy_to.egg-info/SOURCES.txt
--rw-r--r--   0 burp      (1000) burp      (1001)        1 2024-03-05 21:13:13.000000 copy-to-1.3.8/copy_to.egg-info/dependency_links.txt
--rw-r--r--   0 burp      (1000) burp      (1001)       41 2024-03-05 21:13:13.000000 copy-to-1.3.8/copy_to.egg-info/entry_points.txt
--rw-r--r--   0 burp      (1000) burp      (1001)       60 2024-03-05 21:13:13.000000 copy-to-1.3.8/copy_to.egg-info/requires.txt
--rw-r--r--   0 burp      (1000) burp      (1001)        7 2024-03-05 21:13:13.000000 copy-to-1.3.8/copy_to.egg-info/top_level.txt
--rwxr-xr-x   0 burp      (1000) burp      (1001)    42114 2024-03-05 21:07:40.000000 copy-to-1.3.8/copy_to.py
--rw-r--r--   0 burp      (1000) burp      (1001)      842 2024-03-05 21:13:01.000000 copy-to-1.3.8/pyproject.toml
--rw-r--r--   0 burp      (1000) burp      (1001)       38 2024-03-05 21:13:13.822695 copy-to-1.3.8/setup.cfg
+drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2024-03-05 21:53:55.429813 copy-to-1.3.9/
+-rw-r--r--   0 burp      (1000) burp      (1001)     1071 2024-01-04 01:45:52.000000 copy-to-1.3.9/LICENSE
+-rw-r--r--   0 burp      (1000) burp      (1001)     8949 2024-03-05 21:53:55.429813 copy-to-1.3.9/PKG-INFO
+-rw-r--r--   0 burp      (1000) burp      (1001)     8254 2024-03-05 21:53:30.000000 copy-to-1.3.9/README.md
+drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2024-03-05 21:53:55.429813 copy-to-1.3.9/copy_to.egg-info/
+-rw-r--r--   0 burp      (1000) burp      (1001)     8949 2024-03-05 21:53:55.000000 copy-to-1.3.9/copy_to.egg-info/PKG-INFO
+-rw-r--r--   0 burp      (1000) burp      (1001)      231 2024-03-05 21:53:55.000000 copy-to-1.3.9/copy_to.egg-info/SOURCES.txt
+-rw-r--r--   0 burp      (1000) burp      (1001)        1 2024-03-05 21:53:55.000000 copy-to-1.3.9/copy_to.egg-info/dependency_links.txt
+-rw-r--r--   0 burp      (1000) burp      (1001)       41 2024-03-05 21:53:55.000000 copy-to-1.3.9/copy_to.egg-info/entry_points.txt
+-rw-r--r--   0 burp      (1000) burp      (1001)       60 2024-03-05 21:53:55.000000 copy-to-1.3.9/copy_to.egg-info/requires.txt
+-rw-r--r--   0 burp      (1000) burp      (1001)        7 2024-03-05 21:53:55.000000 copy-to-1.3.9/copy_to.egg-info/top_level.txt
+-rwxr-xr-x   0 burp      (1000) burp      (1001)    42114 2024-03-05 21:07:40.000000 copy-to-1.3.9/copy_to.py
+-rw-r--r--   0 burp      (1000) burp      (1001)      842 2024-03-05 21:53:41.000000 copy-to-1.3.9/pyproject.toml
+-rw-r--r--   0 burp      (1000) burp      (1001)       38 2024-03-05 21:53:55.429813 copy-to-1.3.9/setup.cfg
```

### Comparing `copy-to-1.3.8/LICENSE` & `copy-to-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `copy-to-1.3.8/PKG-INFO` & `copy-to-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-to
-Version: 1.3.8
+Version: 1.3.9
 Summary: A little commandline tool to copy and paste multiple files and directories to single directory with use of configuration
 Author-email: Stan Nys <stan96@duck.com>
 Project-URL: Homepage, https://github.com/excited-bore/copy-to
 Project-URL: Bug Tracker, https://github.com/excited-bore/copy-to/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,32 +37,31 @@
 python -m pip install --user pipx
 python -m pipx ensurepath
 python -m pipx install copy-to
 ```  
 
 Then, restart you shell.  
 
-On Linux / MacOs, try running it once if autocompletions aren't working  
-
-You can also run:  
-```
-sudo activate-global-python-argcomplete
-```  
-
 For autocompletion on Windows Powershell v5.1, first run:  
 ```
 Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted
 ```  
 
 Then, for Powershell autocompletion in general, run:  
 ```
 python ((where.exe register-python-argcomplete).Split([Environment]::NewLine) | Select -First 1) --shell powershell copy-to.exe > $env:temp/copy-to.psm1
 Import-Module $env:temp/copy-to.psm1
 ```  
-Then run it once and autocompletion should work.  
+
+For Linux / MacOs, try running it once if autocompletions aren't working  
+
+You can also run:  
+```
+sudo activate-global-python-argcomplete
+```  
 
 ## How to use it:  
 
 Add a pairset of destination folder - source files and/or directories with  
 ```
 copy-to add myname destination_folder sourcefile1 (sourcefolder1 sourcefile2 sourcefile3 sourcefolder2/*) ...
 ```  
@@ -77,19 +76,20 @@
 copy-to run-reverse myname1 (myname2)
 ```  
 
 When the destination is missing, a prompt will ask you if you want to create the destination folder.  
 
 Run and run-reverse can also run without arguments when git is installed and present in a git local repository that has configured copy-to. This is so it can be hooked to a git macro more easily, f.ex. with an alias/function  
 
-Windows Powershell:  
+Windows Powershell: (put in your profile - `notepad $profile`)  
 ```
 function git-status { copy-to.exe run && git.exe status }
 ```  
-Linux bash:  
+
+Linux bash (put in your .bashrc - `nano ~/.bashrc`):  
 ```
 alias git-status="copy-to run && git status"
 ```  
 
 or for those who use it, on startup of [Lazygit](https://github.com/jesseduffield/lazygit):  
 
 Windows Powershell:
```

### Comparing `copy-to-1.3.8/README.md` & `copy-to-1.3.9/copy_to.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: copy-to
+Version: 1.3.9
+Summary: A little commandline tool to copy and paste multiple files and directories to single directory with use of configuration
+Author-email: Stan Nys <stan96@duck.com>
+Project-URL: Homepage, https://github.com/excited-bore/copy-to
+Project-URL: Bug Tracker, https://github.com/excited-bore/copy-to/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: argcomplete>=3.2.1
+Requires-Dist: GitPython>=3.1.14
+Requires-Dist: prompt_toolkit>=3.0.20
+
 ## Copy-to
 
 A little python script I use in conjunction with git so you can easily copy (config) files located outside of a git repository to one (or to wherever you want to). Useful for dotfiles and such.  
 
 Available on with pip/pipx: https://pypi.org/project/copy-to/  
 
 Depends on [argcomplete](https://pypi.org/project/argcomplete/), [GitPython](https://pypi.org/project/GitPython/), [prompt_toolkit](https://pypi.org/project/prompt_toolkit/)  
@@ -20,32 +37,31 @@
 python -m pip install --user pipx
 python -m pipx ensurepath
 python -m pipx install copy-to
 ```  
 
 Then, restart you shell.  
 
-On Linux / MacOs, try running it once if autocompletions aren't working  
-
-You can also run:  
-```
-sudo activate-global-python-argcomplete
-```  
-
 For autocompletion on Windows Powershell v5.1, first run:  
 ```
 Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted
 ```  
 
 Then, for Powershell autocompletion in general, run:  
 ```
 python ((where.exe register-python-argcomplete).Split([Environment]::NewLine) | Select -First 1) --shell powershell copy-to.exe > $env:temp/copy-to.psm1
 Import-Module $env:temp/copy-to.psm1
 ```  
-Then run it once and autocompletion should work.  
+
+For Linux / MacOs, try running it once if autocompletions aren't working  
+
+You can also run:  
+```
+sudo activate-global-python-argcomplete
+```  
 
 ## How to use it:  
 
 Add a pairset of destination folder - source files and/or directories with  
 ```
 copy-to add myname destination_folder sourcefile1 (sourcefolder1 sourcefile2 sourcefile3 sourcefolder2/*) ...
 ```  
@@ -60,19 +76,20 @@
 copy-to run-reverse myname1 (myname2)
 ```  
 
 When the destination is missing, a prompt will ask you if you want to create the destination folder.  
 
 Run and run-reverse can also run without arguments when git is installed and present in a git local repository that has configured copy-to. This is so it can be hooked to a git macro more easily, f.ex. with an alias/function  
 
-Windows Powershell:  
+Windows Powershell: (put in your profile - `notepad $profile`)  
 ```
 function git-status { copy-to.exe run && git.exe status }
 ```  
-Linux bash:  
+
+Linux bash (put in your .bashrc - `nano ~/.bashrc`):  
 ```
 alias git-status="copy-to run && git status"
 ```  
 
 or for those who use it, on startup of [Lazygit](https://github.com/jesseduffield/lazygit):  
 
 Windows Powershell:
```

### Comparing `copy-to-1.3.8/copy_to.egg-info/PKG-INFO` & `copy-to-1.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: copy-to
-Version: 1.3.8
-Summary: A little commandline tool to copy and paste multiple files and directories to single directory with use of configuration
-Author-email: Stan Nys <stan96@duck.com>
-Project-URL: Homepage, https://github.com/excited-bore/copy-to
-Project-URL: Bug Tracker, https://github.com/excited-bore/copy-to/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: argcomplete>=3.2.1
-Requires-Dist: GitPython>=3.1.14
-Requires-Dist: prompt_toolkit>=3.0.20
-
 ## Copy-to
 
 A little python script I use in conjunction with git so you can easily copy (config) files located outside of a git repository to one (or to wherever you want to). Useful for dotfiles and such.  
 
 Available on with pip/pipx: https://pypi.org/project/copy-to/  
 
 Depends on [argcomplete](https://pypi.org/project/argcomplete/), [GitPython](https://pypi.org/project/GitPython/), [prompt_toolkit](https://pypi.org/project/prompt_toolkit/)  
@@ -37,32 +20,31 @@
 python -m pip install --user pipx
 python -m pipx ensurepath
 python -m pipx install copy-to
 ```  
 
 Then, restart you shell.  
 
-On Linux / MacOs, try running it once if autocompletions aren't working  
-
-You can also run:  
-```
-sudo activate-global-python-argcomplete
-```  
-
 For autocompletion on Windows Powershell v5.1, first run:  
 ```
 Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted
 ```  
 
 Then, for Powershell autocompletion in general, run:  
 ```
 python ((where.exe register-python-argcomplete).Split([Environment]::NewLine) | Select -First 1) --shell powershell copy-to.exe > $env:temp/copy-to.psm1
 Import-Module $env:temp/copy-to.psm1
 ```  
-Then run it once and autocompletion should work.  
+
+For Linux / MacOs, try running it once if autocompletions aren't working  
+
+You can also run:  
+```
+sudo activate-global-python-argcomplete
+```  
 
 ## How to use it:  
 
 Add a pairset of destination folder - source files and/or directories with  
 ```
 copy-to add myname destination_folder sourcefile1 (sourcefolder1 sourcefile2 sourcefile3 sourcefolder2/*) ...
 ```  
@@ -77,19 +59,20 @@
 copy-to run-reverse myname1 (myname2)
 ```  
 
 When the destination is missing, a prompt will ask you if you want to create the destination folder.  
 
 Run and run-reverse can also run without arguments when git is installed and present in a git local repository that has configured copy-to. This is so it can be hooked to a git macro more easily, f.ex. with an alias/function  
 
-Windows Powershell:  
+Windows Powershell: (put in your profile - `notepad $profile`)  
 ```
 function git-status { copy-to.exe run && git.exe status }
 ```  
-Linux bash:  
+
+Linux bash (put in your .bashrc - `nano ~/.bashrc`):  
 ```
 alias git-status="copy-to run && git status"
 ```  
 
 or for those who use it, on startup of [Lazygit](https://github.com/jesseduffield/lazygit):  
 
 Windows Powershell:
```

### Comparing `copy-to-1.3.8/copy_to.py` & `copy-to-1.3.9/copy_to.py`

 * *Files identical despite different names*

### Comparing `copy-to-1.3.8/pyproject.toml` & `copy-to-1.3.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools","argcomplete", "GitPython", "prompt_toolkit"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "copy-to"
-version = "1.3.8"
+version = "1.3.9"
 authors = [
   { name="Stan Nys", email="stan96@duck.com" },
 ]
 
 description = "A little commandline tool to copy and paste multiple files and directories to single directory with use of configuration"
 readme = "README.md"
 requires-python = ">=3.7"
```

