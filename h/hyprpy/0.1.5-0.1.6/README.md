# Comparing `tmp/hyprpy-0.1.5.tar.gz` & `tmp/hyprpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprpy-0.1.5.tar", last modified: Wed Sep 13 15:51:47 2023, max compression
+gzip compressed data, was "hyprpy-0.1.6.tar", last modified: Sat May 11 11:58:40 2024, max compression
```

## Comparing `hyprpy-0.1.5.tar` & `hyprpy-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2023-09-13 15:51:47.088339 hyprpy-0.1.5/
--rw-r--r--   0 ulinja    (1000) users      (100)     1064 2023-08-14 03:22:15.000000 hyprpy-0.1.5/LICENSE
--rw-r--r--   0 ulinja    (1000) users      (100)     3363 2023-09-13 15:51:47.088339 hyprpy-0.1.5/PKG-INFO
--rw-r--r--   0 ulinja    (1000) users      (100)     2176 2023-09-13 15:50:53.000000 hyprpy-0.1.5/README.md
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2023-09-13 15:51:47.084339 hyprpy-0.1.5/hyprpy/
--rw-r--r--   0 ulinja    (1000) users      (100)      194 2023-08-14 05:03:40.000000 hyprpy-0.1.5/hyprpy/__init__.py
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2023-09-13 15:51:47.086339 hyprpy-0.1.5/hyprpy/components/
--rw-r--r--   0 ulinja    (1000) users      (100)    10332 2023-09-13 15:23:33.000000 hyprpy-0.1.5/hyprpy/components/__init__.py
--rw-r--r--   0 ulinja    (1000) users      (100)      434 2023-08-14 05:03:40.000000 hyprpy-0.1.5/hyprpy/components/common.py
--rw-r--r--   0 ulinja    (1000) users      (100)    10848 2023-09-13 15:02:46.000000 hyprpy-0.1.5/hyprpy/components/instances.py
--rw-r--r--   0 ulinja    (1000) users      (100)     2594 2023-08-15 17:45:43.000000 hyprpy-0.1.5/hyprpy/components/monitors.py
--rw-r--r--   0 ulinja    (1000) users      (100)     3478 2023-08-15 17:45:43.000000 hyprpy-0.1.5/hyprpy/components/windows.py
--rw-r--r--   0 ulinja    (1000) users      (100)     2410 2023-08-15 17:45:43.000000 hyprpy-0.1.5/hyprpy/components/workspaces.py
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2023-09-13 15:51:47.087339 hyprpy-0.1.5/hyprpy/data/
--rw-r--r--   0 ulinja    (1000) users      (100)     3092 2023-08-14 05:03:40.000000 hyprpy-0.1.5/hyprpy/data/__init__.py
--rw-r--r--   0 ulinja    (1000) users      (100)     5230 2023-08-15 17:45:43.000000 hyprpy-0.1.5/hyprpy/data/models.py
--rw-r--r--   0 ulinja    (1000) users      (100)      647 2023-08-14 05:03:40.000000 hyprpy-0.1.5/hyprpy/data/validators.py
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2023-09-13 15:51:47.087339 hyprpy-0.1.5/hyprpy/utils/
--rw-r--r--   0 ulinja    (1000) users      (100)        0 2023-08-14 05:03:40.000000 hyprpy-0.1.5/hyprpy/utils/__init__.py
--rw-r--r--   0 ulinja    (1000) users      (100)     4411 2023-08-15 17:45:43.000000 hyprpy-0.1.5/hyprpy/utils/assertions.py
--rw-r--r--   0 ulinja    (1000) users      (100)     2868 2023-08-14 16:23:04.000000 hyprpy-0.1.5/hyprpy/utils/shell.py
--rw-r--r--   0 ulinja    (1000) users      (100)     4090 2023-08-14 05:03:40.000000 hyprpy-0.1.5/hyprpy/utils/signals.py
--rw-r--r--   0 ulinja    (1000) users      (100)     9202 2023-08-15 17:45:43.000000 hyprpy-0.1.5/hyprpy/utils/sockets.py
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2023-09-13 15:51:47.085339 hyprpy-0.1.5/hyprpy.egg-info/
--rw-r--r--   0 ulinja    (1000) users      (100)     3363 2023-09-13 15:51:47.000000 hyprpy-0.1.5/hyprpy.egg-info/PKG-INFO
--rw-r--r--   0 ulinja    (1000) users      (100)      584 2023-09-13 15:51:47.000000 hyprpy-0.1.5/hyprpy.egg-info/SOURCES.txt
--rw-r--r--   0 ulinja    (1000) users      (100)        1 2023-09-13 15:51:47.000000 hyprpy-0.1.5/hyprpy.egg-info/dependency_links.txt
--rw-r--r--   0 ulinja    (1000) users      (100)       16 2023-09-13 15:51:47.000000 hyprpy-0.1.5/hyprpy.egg-info/requires.txt
--rw-r--r--   0 ulinja    (1000) users      (100)        7 2023-09-13 15:51:47.000000 hyprpy-0.1.5/hyprpy.egg-info/top_level.txt
--rw-r--r--   0 ulinja    (1000) users      (100)       81 2023-08-14 05:03:40.000000 hyprpy-0.1.5/pyproject.toml
--rw-r--r--   0 ulinja    (1000) users      (100)     1177 2023-09-13 15:51:47.089339 hyprpy-0.1.5/setup.cfg
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.294684 hyprpy-0.1.6/
+-rw-r--r--   0 ulinja    (1000) users      (100)     1064 2023-08-14 03:22:15.000000 hyprpy-0.1.6/LICENSE
+-rw-r--r--   0 ulinja    (1000) users      (100)     3410 2024-05-11 11:58:40.294684 hyprpy-0.1.6/PKG-INFO
+-rw-r--r--   0 ulinja    (1000) users      (100)     2223 2024-05-11 11:55:20.000000 hyprpy-0.1.6/README.md
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.287684 hyprpy-0.1.6/hyprpy/
+-rw-r--r--   0 ulinja    (1000) users      (100)      194 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/__init__.py
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.290684 hyprpy-0.1.6/hyprpy/components/
+-rw-r--r--   0 ulinja    (1000) users      (100)    10332 2023-09-13 15:23:33.000000 hyprpy-0.1.6/hyprpy/components/__init__.py
+-rw-r--r--   0 ulinja    (1000) users      (100)      434 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/components/common.py
+-rw-r--r--   0 ulinja    (1000) users      (100)    11810 2024-05-11 11:35:10.000000 hyprpy-0.1.6/hyprpy/components/instances.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     2594 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/components/monitors.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     3478 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/components/windows.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     2410 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/components/workspaces.py
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.291684 hyprpy-0.1.6/hyprpy/data/
+-rw-r--r--   0 ulinja    (1000) users      (100)     3092 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/data/__init__.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     5230 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/data/models.py
+-rw-r--r--   0 ulinja    (1000) users      (100)      647 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/data/validators.py
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.293684 hyprpy-0.1.6/hyprpy/utils/
+-rw-r--r--   0 ulinja    (1000) users      (100)        0 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/utils/__init__.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     4411 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/utils/assertions.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     2868 2023-08-14 16:23:04.000000 hyprpy-0.1.6/hyprpy/utils/shell.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     4090 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/utils/signals.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     9202 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/utils/sockets.py
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.293684 hyprpy-0.1.6/hyprpy.egg-info/
+-rw-r--r--   0 ulinja    (1000) users      (100)     3410 2024-05-11 11:58:40.000000 hyprpy-0.1.6/hyprpy.egg-info/PKG-INFO
+-rw-r--r--   0 ulinja    (1000) users      (100)      584 2024-05-11 11:58:40.000000 hyprpy-0.1.6/hyprpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ulinja    (1000) users      (100)        1 2024-05-11 11:58:40.000000 hyprpy-0.1.6/hyprpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ulinja    (1000) users      (100)       16 2024-05-11 11:58:40.000000 hyprpy-0.1.6/hyprpy.egg-info/requires.txt
+-rw-r--r--   0 ulinja    (1000) users      (100)        7 2024-05-11 11:58:40.000000 hyprpy-0.1.6/hyprpy.egg-info/top_level.txt
+-rw-r--r--   0 ulinja    (1000) users      (100)       81 2023-08-14 05:03:40.000000 hyprpy-0.1.6/pyproject.toml
+-rw-r--r--   0 ulinja    (1000) users      (100)     1177 2024-05-11 11:58:40.295684 hyprpy-0.1.6/setup.cfg
```

### Comparing `hyprpy-0.1.5/LICENSE` & `hyprpy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/PKG-INFO` & `hyprpy-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python bindings for the Hyprland compositor.
 Author: Julian Lobbes
 Author-email: julian@lobbes.dev
 Project-URL: repo, https://github.com/ulinja/hyprpy
 Project-URL: docs, https://hyprpy.lobbes.dev/
 Keywords: hyprland,wayland,compositor,window manager
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -100,9 +100,8 @@
 
 Hyprpy is in active development! Please file an issue if you find any bugs or have a feature request.
 
 Your contributions are greatly appreciated.
 
 ### Roadmap
 
-- [ ] dispatchers for components
-- [ ] ???
+- [ ] include [dispatchers in components API](https://github.com/ulinja/hyprpy/issues/11)
```

### Comparing `hyprpy-0.1.5/README.md` & `hyprpy-0.1.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -71,9 +71,8 @@
 
 Hyprpy is in active development! Please file an issue if you find any bugs or have a feature request.
 
 Your contributions are greatly appreciated.
 
 ### Roadmap
 
-- [ ] dispatchers for components
-- [ ] ???
+- [ ] include [dispatchers in components API](https://github.com/ulinja/hyprpy/issues/11)
```

### Comparing `hyprpy-0.1.5/hyprpy/components/__init__.py` & `hyprpy-0.1.6/hyprpy/components/__init__.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/hyprpy/components/instances.py` & `hyprpy-0.1.6/hyprpy/components/instances.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,18 +55,43 @@
         #: Signal emitted when the focus changes to another window. Sends ``active_window_address``, the :attr:`~hyprpy.components.windows.Window.address` of the now active window, as signal data.
         self.signal_active_window_changed: Signal = Signal(self)
 
 
     def __repr__(self):
         return f"<Instance(signature={self.signature!r})>"
 
+    def dispatch(self, arguments: list[str]) -> Union[str, None]:
+        """Runs a generic dispatcher command with the given arguments and returns ``None`` on success or a string indicating errors.
+
+        See the `Hyprland Wiki <https://wiki.hyprland.org/Configuring/Dispatchers/>`_ for a list
+        of available commands.
+
+        Example:
+
+        .. code-block:: python
+
+            from hyprpy import Hyprland
+
+            instance = Hyprland()
+            instance.dispatch(["cyclenext", "prev"])
+
+        :param arguments: A list of strings containing the arguments of the dispatch command.
+        :type arguments: list[str]
+        :return: `None` if the command succeeded, otherwise a string indicating errors.
+        :rtype: str or None
+        """
+
+        dispatch_response = self.command_socket.send_command('dispatch', flags=['-j'], args=arguments)
+        dispatch_error = dispatch_response if dispatch_response != 'ok' else None
+        return dispatch_error
+
 
     def get_windows(self) -> List['Window']:
         """Returns all :class:`~hyprpy.components.windows.Window`\\ s currently managed by the instance.
-    
+
         :return: A list containing :class:`~hyprpy.components.windows.Window` objects.
         """
 
         windows_data = json.loads(self.command_socket.send_command('clients', flags=['-j']))
         return [Window(window_data, self) for window_data in windows_data]
 
     def get_window_by_address(self, address: str) -> Union['Window', None]:
@@ -82,25 +107,25 @@
         assertions.assert_is_hexadecimal_string(address)
         for window in self.get_windows():
             if window.address_as_int == int(address, 16):
                 return window
 
     def get_active_window(self) -> 'Window':
         """Returns the currently active :class:`~hyprpy.components.windows.Window`.
-    
+
         :return: The currently active :class:`~hyprpy.components.windows.Window`.
         """
 
         window_data = json.loads(self.command_socket.send_command('activewindow', flags=['-j']))
         return Window(window_data, self)
 
 
     def get_workspaces(self) -> List['Workspace']:
         """Returns all :class:`~hyprpy.components.workspaces.Workspace`\\ s currently managed by the instance.
-    
+
         :return: A list containing :class:`~hyprpy.components.workspaces.Workspace`\\ s.
         """
 
         workspaces_data = json.loads(self.command_socket.send_command('workspaces', flags=['-j']))
         return [Workspace(workspace_data, self) for workspace_data in workspaces_data]
 
     def get_workspace_by_id(self, id: int) -> Union['Workspace', None]:
@@ -132,18 +157,18 @@
         """
 
         assertions.assert_is_string(name)
         for workspace in self.get_workspaces():
             if workspace.name == name:
                 return workspace
 
-    
+
     def get_monitors(self) -> List['Monitor']:
         """Returns all :class:`~hyprpy.components.monitors.Monitor`\\ s currently managed by the instance.
-    
+
         :return: A list containing :class:`~hyprpy.components.monitors.Monitor`\\ s.
         """
 
         monitors_data = json.loads(self.command_socket.send_command('monitors', flags=['-j']))
         return [Monitor(monitor_data, self) for monitor_data in monitors_data]
 
     def get_monitor_by_id(self, id: int) -> Union['Monitor', None]:
```

### Comparing `hyprpy-0.1.5/hyprpy/components/monitors.py` & `hyprpy-0.1.6/hyprpy/components/monitors.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/hyprpy/components/windows.py` & `hyprpy-0.1.6/hyprpy/components/windows.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/hyprpy/components/workspaces.py` & `hyprpy-0.1.6/hyprpy/components/workspaces.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/hyprpy/data/__init__.py` & `hyprpy-0.1.6/hyprpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/hyprpy/data/models.py` & `hyprpy-0.1.6/hyprpy/data/models.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/hyprpy/data/validators.py` & `hyprpy-0.1.6/hyprpy/data/validators.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/hyprpy/utils/assertions.py` & `hyprpy-0.1.6/hyprpy/utils/assertions.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/hyprpy/utils/shell.py` & `hyprpy-0.1.6/hyprpy/utils/shell.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/hyprpy/utils/signals.py` & `hyprpy-0.1.6/hyprpy/utils/signals.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/hyprpy/utils/sockets.py` & `hyprpy-0.1.6/hyprpy/utils/sockets.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/hyprpy.egg-info/PKG-INFO` & `hyprpy-0.1.6/hyprpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python bindings for the Hyprland compositor.
 Author: Julian Lobbes
 Author-email: julian@lobbes.dev
 Project-URL: repo, https://github.com/ulinja/hyprpy
 Project-URL: docs, https://hyprpy.lobbes.dev/
 Keywords: hyprland,wayland,compositor,window manager
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -100,9 +100,8 @@
 
 Hyprpy is in active development! Please file an issue if you find any bugs or have a feature request.
 
 Your contributions are greatly appreciated.
 
 ### Roadmap
 
-- [ ] dispatchers for components
-- [ ] ???
+- [ ] include [dispatchers in components API](https://github.com/ulinja/hyprpy/issues/11)
```

### Comparing `hyprpy-0.1.5/hyprpy.egg-info/SOURCES.txt` & `hyprpy-0.1.6/hyprpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.5/setup.cfg` & `hyprpy-0.1.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hyprpy
-version = 0.1.5
+version = 0.1.6
 description = Python bindings for the Hyprland compositor.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Julian Lobbes
 author_email = julian@lobbes.dev
 project_urls = 
 	repo = https://github.com/ulinja/hyprpy
```

