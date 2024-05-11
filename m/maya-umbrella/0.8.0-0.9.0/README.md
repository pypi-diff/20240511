# Comparing `tmp/maya_umbrella-0.8.0.tar.gz` & `tmp/maya_umbrella-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maya_umbrella-0.8.0.tar", max compression
+gzip compressed data, was "maya_umbrella-0.9.0.tar", max compression
```

## Comparing `maya_umbrella-0.8.0.tar` & `maya_umbrella-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1060 2024-05-10 12:32:55.351753 maya_umbrella-0.8.0/LICENSE
--rw-r--r--   0        0        0     9945 2024-05-10 12:32:55.351753 maya_umbrella-0.8.0/README.md
--rw-r--r--   0        0        0      401 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/__init__.py
--rw-r--r--   0        0        0       22 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/__version__.py
--rw-r--r--   0        0        0     5044 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/cleaner.py
--rw-r--r--   0        0        0    13111 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/collector.py
--rw-r--r--   0        0        0      539 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/constants.py
--rw-r--r--   0        0        0     5601 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/defender.py
--rw-r--r--   0        0        0     8333 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/filesystem.py
--rw-r--r--   0        0        0        0 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/hooks/__init__.py
--rw-r--r--   0        0        0      761 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/hooks/delete_turtle.py
--rw-r--r--   0        0        0     1281 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/hooks/delete_unknown_plugin_node.py
--rw-r--r--   0        0        0      556 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/hooks/fix_model_panel.py
--rw-r--r--   0        0        0      484 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/hooks/fix_on_model_change_3dc.py
--rw-r--r--   0        0        0     2683 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/i18n.py
--rw-r--r--   0        0        0      962 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/locales/en_US.json
--rw-r--r--   0        0        0     1006 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/locales/zh_CN.json
--rw-r--r--   0        0        0     1338 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/log.py
--rw-r--r--   0        0        0     3645 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/maya_funs.py
--rw-r--r--   0        0        0     3921 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/scanner.py
--rw-r--r--   0        0        0      354 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/signatures.py
--rw-r--r--   0        0        0     1022 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/vaccine.py
--rw-r--r--   0        0        0        0 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/vaccines/__init__.py
--rw-r--r--   0        0        0      489 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/vaccines/vaccine1.py
--rw-r--r--   0        0        0     2123 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/vaccines/vaccine2.py
--rw-r--r--   0        0        0     3493 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/maya_umbrella/vaccines/vaccine3.py
--rw-r--r--   0        0        0     5285 2024-05-10 12:32:55.375753 maya_umbrella-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    10996 1970-01-01 00:00:00.000000 maya_umbrella-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-10 15:39:49.422952 maya_umbrella-0.9.0/LICENSE
+-rw-r--r--   0        0        0    10220 2024-05-10 15:39:49.422952 maya_umbrella-0.9.0/README.md
+-rw-r--r--   0        0        0      401 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/__version__.py
+-rw-r--r--   0        0        0     5044 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/cleaner.py
+-rw-r--r--   0        0        0    13111 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/collector.py
+-rw-r--r--   0        0        0      539 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/constants.py
+-rw-r--r--   0        0        0     5601 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/defender.py
+-rw-r--r--   0        0        0     9360 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/filesystem.py
+-rw-r--r--   0        0        0        0 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/hooks/__init__.py
+-rw-r--r--   0        0        0      761 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/hooks/delete_turtle.py
+-rw-r--r--   0        0        0     1281 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/hooks/delete_unknown_plugin_node.py
+-rw-r--r--   0        0        0      556 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/hooks/fix_model_panel.py
+-rw-r--r--   0        0        0      484 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/hooks/fix_on_model_change_3dc.py
+-rw-r--r--   0        0        0     2683 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/i18n.py
+-rw-r--r--   0        0        0      962 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/locales/en_US.json
+-rw-r--r--   0        0        0     1006 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/locales/zh_CN.json
+-rw-r--r--   0        0        0     1338 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/log.py
+-rw-r--r--   0        0        0     3645 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/maya_funs.py
+-rw-r--r--   0        0        0     3921 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/scanner.py
+-rw-r--r--   0        0        0      354 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/signatures.py
+-rw-r--r--   0        0        0     1022 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/vaccine.py
+-rw-r--r--   0        0        0        0 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/vaccines/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/vaccines/vaccine1.py
+-rw-r--r--   0        0        0     2123 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/vaccines/vaccine2.py
+-rw-r--r--   0        0        0     3493 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/maya_umbrella/vaccines/vaccine3.py
+-rw-r--r--   0        0        0     5285 2024-05-10 15:39:49.450952 maya_umbrella-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11271 1970-01-01 00:00:00.000000 maya_umbrella-0.9.0/PKG-INFO
```

### Comparing `maya_umbrella-0.8.0/LICENSE` & `maya_umbrella-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/README.md` & `maya_umbrella-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,23 @@
 This tool is designed to provide a robust solution for identifying and resolving any potential viruses within Autodesk
 Maya.
 It ensures a secure and seamless user experience by proactively scanning for threats and effectively neutralizing them.
 
 It can be provided as an API for seamless integration into your existing pipeline.
 
 # 安装
+
+## pip 安装
 maya_umbrella是以标准pipy包去发布的，所以我们可以通过pip install去安装
 ```shell
 your/maya-root/mayapy -m pip install maya-umbrella
 ```
+## 一键安装
+在release里面下载对应版本的zip包，解压后双击`install.bat`即可安装
+
 更新版本
 ```shell
 your/maya-root/mayapy -m pip install maya-umbrella --upgrade
 ```
 卸载
 ```shell
 your/maya-root/mayapy -m pip uninstall  maya-umbrella
@@ -51,21 +56,23 @@
 ```shell
 pip install nox poetry
 ```
 
 # 开发调试
 
 ```shell
-nox -s maya-2020
+nox -s maya -- 2020 --test
 ```
 
 ## 在maya中测试
 
-通过`nox -s maya-xxx`, 启动maya.
-nox会动态根据你本地安装得maya去注册nox session, 比如你本地安装了`maya-2020`，那么通过`nox -s maya-2018`
+通过`nox -s maya -- <maya version>`, 启动maya.
+nox会动态根据你本地安装得maya去注册nox session, 比如你本地安装了`maya-2020`，
+
+那么通过`nox -s maya -- 2018`, **注意：maya 与 版本号之间有 俩个`-`**
 
 启动maya后在脚本编辑器中执行下面得代码，就会动态的从`<repo>/tests/virus/`里面去open ma文件去进行测试.
 
 ```python
 import manual_test_in_maya
 
 manual_test_in_maya.start()
@@ -83,15 +90,15 @@
 ```shell
 nox -s ruff_check
 ```
 
 # 生成安装包
 
 执行下面的命令可以在<repo>/.zip下面创建zip，参数 `--version` 当前工具的版本号
-
+ **注意：`make-zip` 与 `--version`之间有 俩个`-`**
 ```shell
 nox -s make-zip -- --version 0.5.0
 ```
 
 # 环境变量
 
 我们可以通过下列环境变量去修改maya_umbrella的一些设置，方便有pipeline的公司可以更好的集成
@@ -158,16 +165,16 @@
 print(api.scan_files_from_pattern("your/path/*.m[ab]"))
 
 ```
 
 # 案例
 如果你想要快速通过maya standalone去批量清理maya文件，可以`下载`或者`git clone`当前`main`分支的工程，
 根据上面指引设置好开发环境
-通过`nox`命令去启动maya standalone环境，maya版本根据你当前本地安装的maya为准，比如你本地安装了`2018`,
-那么就是 `nox -s maya-2018-s`
+通过`nox`命令去启动maya `standalone`环境，maya版本根据你当前本地安装的maya为准，比如你本地安装了`2018`,
+那么就是 `nox -s maya -- 2018 --standalone`
 下面的语法是启动一个maya-2020的环境去动态从`c:/test`文件夹下去查杀病毒
 ```shell
 nox -s maya-2020-s -- c:/test/*.m[ab]
 ```
 
 ## Contributors ✨
```

### Comparing `maya_umbrella-0.8.0/maya_umbrella/cleaner.py` & `maya_umbrella-0.9.0/maya_umbrella/cleaner.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/collector.py` & `maya_umbrella-0.9.0/maya_umbrella/collector.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/constants.py` & `maya_umbrella-0.9.0/maya_umbrella/constants.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/defender.py` & `maya_umbrella-0.9.0/maya_umbrella/defender.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/filesystem.py` & `maya_umbrella-0.9.0/maya_umbrella/filesystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,14 @@
         yield f
     try:
         os.replace(temp_path, src)
     except AttributeError:
         shutil.move(temp_path, src)
 
 
-
 def id_generator(size=6, chars=string.ascii_uppercase + string.digits):
     """Generate a random string of the given size using the given characters."""
     return "".join(random.choice(chars) for _ in range(size))
 
 
 def rename(src):
     """Rename the file at the given path to a random name and return the new path."""
@@ -262,7 +261,35 @@
         _, base_path = os.path.splitdrive(root)
         backup_path = os.path.join(root_path, base_path.strip(os.sep))
     try:
         os.makedirs(backup_path)
     except (OSError, IOError):  # noqa: UP024
         pass
     return os.path.join(backup_path, filename)
+
+
+def get_maya_install_root(maya_version):
+    """Get the Maya install root path."""
+    maya_location = os.environ.get("MAYA_LOCATION")
+    try:
+        # Import built-in modules
+        import winreg
+    except ImportError:
+        return maya_location
+    try:
+        key = winreg.OpenKey(
+            winreg.HKEY_LOCAL_MACHINE,
+            "SOFTWARE\\Autodesk\\Maya\\{maya_version}\\Setup\\InstallPath".format(maya_version=maya_version),
+        )
+        root, _ = winreg.QueryValueEx(key, "MAYA_INSTALL_LOCATION")
+        if not os.path.isdir(root):
+            print("Failed to locate the appropriate Maya path in the registration list.")
+    except OSError:
+        return maya_location
+    maya_location = maya_location or root
+    if not maya_location:
+        print("maya not found.")
+        return
+    maya_exe = os.path.join(maya_location, "bin", "maya.exe")
+    if not os.path.exists(maya_exe):
+        print("maya.exe not found in {maya_location}.".format(maya_location=maya_location))
+    return maya_location
```

### Comparing `maya_umbrella-0.8.0/maya_umbrella/hooks/delete_turtle.py` & `maya_umbrella-0.9.0/maya_umbrella/hooks/delete_turtle.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/hooks/delete_unknown_plugin_node.py` & `maya_umbrella-0.9.0/maya_umbrella/hooks/delete_unknown_plugin_node.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/hooks/fix_model_panel.py` & `maya_umbrella-0.9.0/maya_umbrella/hooks/fix_model_panel.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/i18n.py` & `maya_umbrella-0.9.0/maya_umbrella/i18n.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/locales/en_US.json` & `maya_umbrella-0.9.0/maya_umbrella/locales/en_US.json`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/locales/zh_CN.json` & `maya_umbrella-0.9.0/maya_umbrella/locales/zh_CN.json`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/log.py` & `maya_umbrella-0.9.0/maya_umbrella/log.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/maya_funs.py` & `maya_umbrella-0.9.0/maya_umbrella/maya_funs.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/scanner.py` & `maya_umbrella-0.9.0/maya_umbrella/scanner.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/vaccine.py` & `maya_umbrella-0.9.0/maya_umbrella/vaccine.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/vaccines/vaccine2.py` & `maya_umbrella-0.9.0/maya_umbrella/vaccines/vaccine2.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/maya_umbrella/vaccines/vaccine3.py` & `maya_umbrella-0.9.0/maya_umbrella/vaccines/vaccine3.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.8.0/pyproject.toml` & `maya_umbrella-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maya_umbrella"
-version = "0.8.0"
+version = "0.9.0"
 description = "Check and fix maya virus."
 homepage = "https://github.com/loonghao/maya_umbrella"
 repository = "https://github.com/loonghao/maya_umbrella"
 documentation = "https://github.com/loonghao/maya_umbrella"
 keywords = ["notifiers", "python", "Maya", "dcc"]
 authors = ["longhao <hal.long@outlook.com>"]
 license = "MIT"
@@ -32,15 +32,15 @@
 python = ">=2.7,<2.8 || >=3.6.0"
 
 [tool.poetry.dev-dependencies]
 nox = { version = "^2024.3.2", python = ">=3.8.1,<3.11" }
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.8.0"
+version = "0.9.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version",
     "maya_umbrella/__version__.py"
 ]
 
 [build-system]
```

### Comparing `maya_umbrella-0.8.0/PKG-INFO` & `maya_umbrella-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya_umbrella
-Version: 0.8.0
+Version: 0.9.0
 Summary: Check and fix maya virus.
 Home-page: https://github.com/loonghao/maya_umbrella
 License: MIT
 Keywords: notifiers,python,Maya,dcc
 Author: longhao
 Author-email: hal.long@outlook.com
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
@@ -49,18 +49,23 @@
 This tool is designed to provide a robust solution for identifying and resolving any potential viruses within Autodesk
 Maya.
 It ensures a secure and seamless user experience by proactively scanning for threats and effectively neutralizing them.
 
 It can be provided as an API for seamless integration into your existing pipeline.
 
 # 安装
+
+## pip 安装
 maya_umbrella是以标准pipy包去发布的，所以我们可以通过pip install去安装
 ```shell
 your/maya-root/mayapy -m pip install maya-umbrella
 ```
+## 一键安装
+在release里面下载对应版本的zip包，解压后双击`install.bat`即可安装
+
 更新版本
 ```shell
 your/maya-root/mayapy -m pip install maya-umbrella --upgrade
 ```
 卸载
 ```shell
 your/maya-root/mayapy -m pip uninstall  maya-umbrella
@@ -76,21 +81,23 @@
 ```shell
 pip install nox poetry
 ```
 
 # 开发调试
 
 ```shell
-nox -s maya-2020
+nox -s maya -- 2020 --test
 ```
 
 ## 在maya中测试
 
-通过`nox -s maya-xxx`, 启动maya.
-nox会动态根据你本地安装得maya去注册nox session, 比如你本地安装了`maya-2020`，那么通过`nox -s maya-2018`
+通过`nox -s maya -- <maya version>`, 启动maya.
+nox会动态根据你本地安装得maya去注册nox session, 比如你本地安装了`maya-2020`，
+
+那么通过`nox -s maya -- 2018`, **注意：maya 与 版本号之间有 俩个`-`**
 
 启动maya后在脚本编辑器中执行下面得代码，就会动态的从`<repo>/tests/virus/`里面去open ma文件去进行测试.
 
 ```python
 import manual_test_in_maya
 
 manual_test_in_maya.start()
@@ -108,15 +115,15 @@
 ```shell
 nox -s ruff_check
 ```
 
 # 生成安装包
 
 执行下面的命令可以在<repo>/.zip下面创建zip，参数 `--version` 当前工具的版本号
-
+ **注意：`make-zip` 与 `--version`之间有 俩个`-`**
 ```shell
 nox -s make-zip -- --version 0.5.0
 ```
 
 # 环境变量
 
 我们可以通过下列环境变量去修改maya_umbrella的一些设置，方便有pipeline的公司可以更好的集成
@@ -183,16 +190,16 @@
 print(api.scan_files_from_pattern("your/path/*.m[ab]"))
 
 ```
 
 # 案例
 如果你想要快速通过maya standalone去批量清理maya文件，可以`下载`或者`git clone`当前`main`分支的工程，
 根据上面指引设置好开发环境
-通过`nox`命令去启动maya standalone环境，maya版本根据你当前本地安装的maya为准，比如你本地安装了`2018`,
-那么就是 `nox -s maya-2018-s`
+通过`nox`命令去启动maya `standalone`环境，maya版本根据你当前本地安装的maya为准，比如你本地安装了`2018`,
+那么就是 `nox -s maya -- 2018 --standalone`
 下面的语法是启动一个maya-2020的环境去动态从`c:/test`文件夹下去查杀病毒
 ```shell
 nox -s maya-2020-s -- c:/test/*.m[ab]
 ```
 
 ## Contributors ✨
```

