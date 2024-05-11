# Comparing `tmp/autotrash-0.4.6.tar.gz` & `tmp/autotrash-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrash-0.4.6.tar", max compression
+gzip compressed data, was "autotrash-0.4.7.tar", max compression
```

## Comparing `autotrash-0.4.6.tar` & `autotrash-0.4.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35068 2023-09-08 20:47:31.174012 autotrash-0.4.6/LICENSE.txt
--rw-r--r--   0        0        0     4276 2023-09-08 20:47:31.174012 autotrash-0.4.6/README.md
--rw-r--r--   0        0        0      818 2023-09-08 20:47:47.785844 autotrash-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      160 2023-09-08 20:47:31.174012 autotrash-0.4.6/src/autotrash/__init__.py
--rw-r--r--   0        0        0    17456 2023-09-08 20:47:31.174012 autotrash-0.4.6/src/autotrash/app.py
--rw-r--r--   0        0        0     5266 2023-09-08 20:47:31.174012 autotrash-0.4.6/src/autotrash/options.py
--rw-r--r--   0        0        0     4963 1970-01-01 00:00:00.000000 autotrash-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0    35068 2024-05-11 19:38:35.698828 autotrash-0.4.7/LICENSE.txt
+-rw-r--r--   0        0        0     4308 2024-05-11 19:38:35.698828 autotrash-0.4.7/README.md
+-rw-r--r--   0        0        0      779 2024-05-11 19:38:52.634758 autotrash-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      160 2024-05-11 19:38:35.702828 autotrash-0.4.7/src/autotrash/__init__.py
+-rw-r--r--   0        0        0    17512 2024-05-11 19:38:35.702828 autotrash-0.4.7/src/autotrash/app.py
+-rw-r--r--   0        0        0     5266 2024-05-11 19:38:35.702828 autotrash-0.4.7/src/autotrash/options.py
+-rw-r--r--   0        0        0     4995 1970-01-01 00:00:00.000000 autotrash-0.4.7/PKG-INFO
```

### Comparing `autotrash-0.4.6/LICENSE.txt` & `autotrash-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autotrash-0.4.6/README.md` & `autotrash-0.4.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,22 @@
 trash information file.
 
 Installation
 ============
 
 There are mulitple ways to install the software. Either using your Linux distribution package manager (if a package is available) or using the Python package directly.
 
-Using a distribution package is preferred as it will also ensure that autotrash is updated during your regular updates, however not all distributions have autotrash available as a package, so you may need ot use python directly anyway.
+Using a distribution package is preferred as it will also ensure that autotrash is updated during your regular updates, however not all distributions have autotrash available as a package, so you may need to use python directly anyway.
 
 - Using the a package manager:
-    - On Fedora consider using `yum install autotrash`
+    - On Fedora, using `pipx`:
+        ```
+        sudo dnf install pipx
+        pipx install autotrash
+        ```
     - On Ubuntu and Debian, using `pipx`:
         ```
         sudo apt-get install pipx
         pipx install autotrash
         ```
     - On ArchLinux, there is an [AUR package available](https://aur.archlinux.org/packages/autotrash/)
 
@@ -104,8 +108,8 @@
     poetry run autotrash
 
 Or by using the shell:
 
     poetry shell
     autotrash --help
 
-All pull requests and master builds are tested using github actions and require [`black`](https://github.com/psf/black) formatting.
+All pull requests and master builds are tested using github actions and require pre-commit to succeed.
```

### Comparing `autotrash-0.4.6/src/autotrash/app.py` & `autotrash-0.4.7/src/autotrash/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,19 +414,18 @@
 [Unit]
 Description=Empty trash
 Documentation=https://github.com/bneijt/autotrash
 
 [Service]
 Type=oneshot
 ExecStart="{}" {}
-""".format(
-        executable_path, args
-    )
+""".format(executable_path, args)
 
-    systemd_dir = os.path.expanduser("~/.config/systemd/user")
+    config_dir = os.environ.get("XDG_CONFIG_HOME") or os.path.expanduser("~/.config")
+    systemd_dir = f"{config_dir}/systemd/user"
     os.makedirs(systemd_dir, exist_ok=True)
 
     with open(os.path.join(systemd_dir, "autotrash.timer"), "w") as f:
         f.write(timer_file)
 
     with open(os.path.join(systemd_dir, "autotrash.service"), "w") as f:
         f.write(service_file)
```

### Comparing `autotrash-0.4.6/src/autotrash/options.py` & `autotrash-0.4.7/src/autotrash/options.py`

 * *Files identical despite different names*

### Comparing `autotrash-0.4.6/PKG-INFO` & `autotrash-0.4.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrash
-Version: 0.4.6
+Version: 0.4.7
 Summary: Script to automatically purge old trash
 Home-page: https://github.com/bneijt/autotrash
 Author: Bram Neijt
 Author-email: bram@neijt.nl
 Requires-Python: >=3.8,<4
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,18 +27,22 @@
 trash information file.
 
 Installation
 ============
 
 There are mulitple ways to install the software. Either using your Linux distribution package manager (if a package is available) or using the Python package directly.
 
-Using a distribution package is preferred as it will also ensure that autotrash is updated during your regular updates, however not all distributions have autotrash available as a package, so you may need ot use python directly anyway.
+Using a distribution package is preferred as it will also ensure that autotrash is updated during your regular updates, however not all distributions have autotrash available as a package, so you may need to use python directly anyway.
 
 - Using the a package manager:
-    - On Fedora consider using `yum install autotrash`
+    - On Fedora, using `pipx`:
+        ```
+        sudo dnf install pipx
+        pipx install autotrash
+        ```
     - On Ubuntu and Debian, using `pipx`:
         ```
         sudo apt-get install pipx
         pipx install autotrash
         ```
     - On ArchLinux, there is an [AUR package available](https://aur.archlinux.org/packages/autotrash/)
 
@@ -122,9 +126,9 @@
     poetry run autotrash
 
 Or by using the shell:
 
     poetry shell
     autotrash --help
 
-All pull requests and master builds are tested using github actions and require [`black`](https://github.com/psf/black) formatting.
+All pull requests and master builds are tested using github actions and require pre-commit to succeed.
```

