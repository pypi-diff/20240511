# Comparing `tmp/tidevice3-0.8.4.tar.gz` & `tmp/tidevice3-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidevice3-0.8.4.tar", max compression
+gzip compressed data, was "tidevice3-0.9.0.tar", max compression
```

## Comparing `tidevice3-0.8.4.tar` & `tidevice3-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1068 2024-01-29 06:11:50.376104 tidevice3-0.8.4/LICENSE
--rw-r--r--   0        0        0     2275 2024-01-29 06:11:50.376104 tidevice3-0.8.4/README.md
--rw-r--r--   0        0        0     1584 2024-01-29 06:12:15.152151 tidevice3-0.8.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/__init__.py
--rw-r--r--   0        0        0      824 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/__main__.py
--rw-r--r--   0        0        0     4442 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/api.py
--rw-r--r--   0        0        0        0 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/cli/__init__.py
--rw-r--r--   0        0        0     5337 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/cli/app.py
--rw-r--r--   0        0        0     2119 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/cli/cli_common.py
--rw-r--r--   0        0        0     1297 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/cli/developer.py
--rw-r--r--   0        0        0      633 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/cli/exec.py
--rw-r--r--   0        0        0     5289 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/cli/fsync.py
--rw-r--r--   0        0        0     1073 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/cli/list.py
--rw-r--r--   0        0        0      529 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/cli/reboot.py
--rw-r--r--   0        0        0     3700 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/cli/screenrecord.py
--rw-r--r--   0        0        0      697 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/cli/screenshot.py
--rw-r--r--   0        0        0     5755 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/cli/tunneld.py
--rw-r--r--   0        0        0      236 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/utils/__init__.py
--rw-r--r--   0        0        0     1922 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/utils/common.py
--rw-r--r--   0        0        0     5246 2024-01-29 06:11:50.376104 tidevice3-0.8.4/tidevice3/utils/download.py
--rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 tidevice3-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-01-29 06:43:19.984881 tidevice3-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2275 2024-01-29 06:43:19.984881 tidevice3-0.9.0/README.md
+-rw-r--r--   0        0        0     1584 2024-01-29 06:43:32.945052 tidevice3-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/__init__.py
+-rw-r--r--   0        0        0      838 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/__main__.py
+-rw-r--r--   0        0        0     4442 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/api.py
+-rw-r--r--   0        0        0        0 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/__init__.py
+-rw-r--r--   0        0        0     5337 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/app.py
+-rw-r--r--   0        0        0     2129 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/cli_common.py
+-rw-r--r--   0        0        0     1297 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/developer.py
+-rw-r--r--   0        0        0      633 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/exec.py
+-rw-r--r--   0        0        0     5289 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/fsync.py
+-rw-r--r--   0        0        0     1073 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/list.py
+-rw-r--r--   0        0        0      529 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/reboot.py
+-rw-r--r--   0        0        0     2138 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/runwda.py
+-rw-r--r--   0        0        0     3665 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/screenrecord.py
+-rw-r--r--   0        0        0      697 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/screenshot.py
+-rw-r--r--   0        0        0     5755 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/cli/tunneld.py
+-rw-r--r--   0        0        0      236 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/utils/__init__.py
+-rw-r--r--   0        0        0     1922 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/utils/common.py
+-rw-r--r--   0        0        0     5246 2024-01-29 06:43:19.984881 tidevice3-0.9.0/tidevice3/utils/download.py
+-rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 tidevice3-0.9.0/PKG-INFO
```

### Comparing `tidevice3-0.8.4/LICENSE` & `tidevice3-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/README.md` & `tidevice3-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/pyproject.toml` & `tidevice3-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tidevice3"
-version = "0.8.4"
+version = "0.9.0"
 description = "wrapper for pymobiledevice3 for easy use with iphone device"
 homepage = "https://github.com/codeskyblue/tidevice3"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `tidevice3-0.8.4/tidevice3/__main__.py` & `tidevice3-0.9.0/tidevice3/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def main():
     try:
         cli(auto_envvar_prefix='T3')
-    except FatalError as e:
+    except (FatalError, ValueError) as e:
         click.echo(f"Error: {e}")
         sys.exit(1)
     except NoDeviceConnectedError:
         logger.error("No device connected")
         sys.exit(1)
     except BaseException as e:
         click.echo(f"Error: {type(e)} {e}")
```

### Comparing `tidevice3-0.8.4/tidevice3/api.py` & `tidevice3-0.9.0/tidevice3/api.py`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/tidevice3/cli/app.py` & `tidevice3-0.9.0/tidevice3/cli/app.py`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/tidevice3/cli/cli_common.py` & `tidevice3-0.9.0/tidevice3/cli/cli_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,10 +52,10 @@
         usbmux_address = ctx.obj['usbmux_address']
         service_provider = connect_service_provider(udid=udid, usbmux_address=usbmux_address)
         with service_provider:
             return ctx.invoke(func, service_provider, *args, **kwargs)
     return update_wrapper(new_func, func)
 
 
-CLI_GROUPS = ["list", "developer", "screenshot", "screenrecord", "fsync", "app", "reboot", "tunneld", "exec"]
+CLI_GROUPS = ["list", "developer", "screenshot", "screenrecord", "fsync", "app", "reboot", "tunneld", "runwda", "exec"]
 for group in CLI_GROUPS:
     __import__(f"tidevice3.cli.{group}")
```

### Comparing `tidevice3-0.8.4/tidevice3/cli/developer.py` & `tidevice3-0.9.0/tidevice3/cli/developer.py`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/tidevice3/cli/exec.py` & `tidevice3-0.9.0/tidevice3/cli/exec.py`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/tidevice3/cli/fsync.py` & `tidevice3-0.9.0/tidevice3/cli/fsync.py`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/tidevice3/cli/list.py` & `tidevice3-0.9.0/tidevice3/cli/list.py`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/tidevice3/cli/reboot.py` & `tidevice3-0.9.0/tidevice3/cli/reboot.py`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/tidevice3/cli/screenrecord.py` & `tidevice3-0.9.0/tidevice3/cli/screenrecord.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,25 +90,24 @@
 @cli.command("screenrecord")
 @click.option("--fps", default=5, help="frame per second")
 @click.option("--show-time/--no-show-time", default=True, help="show time on screen")
 @click.argument("out")
 @pass_rsd
 def cli_screenrecord(service_provider: LockdownClient, out: str, fps: int, show_time: bool):
     """ screenrecord to mp4 """
-    writer = imageio.get_writer(out, fps=fps)#, macro_block_size=1)
+    writer = imageio.get_writer(out, fps=fps)
     frame_index = 0
     try:
         for png_data in limit_fps(iter_screenshot(service_provider), fps, debug=True):
             pil_img = Image.open(io.BytesIO(png_data))
             pil_img = resize_for_ffmpeg(pil_img)
             if show_time:
                 time_str = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
                 draw_text(pil_img, f'Time: {time_str} Frame: {frame_index}')
             
             writer.append_data(np.array(pil_img))
             frame_index += 1
     except KeyboardInterrupt:
         print("")
-        pass
     finally:
         writer.close()
         logger.info("screenrecord saved to %s", out)
```

### Comparing `tidevice3-0.8.4/tidevice3/cli/screenshot.py` & `tidevice3-0.9.0/tidevice3/cli/screenshot.py`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/tidevice3/cli/tunneld.py` & `tidevice3-0.9.0/tidevice3/cli/tunneld.py`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/tidevice3/utils/common.py` & `tidevice3-0.9.0/tidevice3/utils/common.py`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/tidevice3/utils/download.py` & `tidevice3-0.9.0/tidevice3/utils/download.py`

 * *Files identical despite different names*

### Comparing `tidevice3-0.8.4/PKG-INFO` & `tidevice3-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidevice3
-Version: 0.8.4
+Version: 0.9.0
 Summary: wrapper for pymobiledevice3 for easy use with iphone device
 Home-page: https://github.com/codeskyblue/tidevice3
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

