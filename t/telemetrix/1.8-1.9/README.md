# Comparing `tmp/telemetrix-1.8.tar.gz` & `tmp/telemetrix-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telemetrix-1.8.tar", last modified: Mon Nov 29 16:09:47 2021, max compression
+gzip compressed data, was "telemetrix-1.9.tar", last modified: Fri Feb 11 23:39:25 2022, max compression
```

## Comparing `telemetrix-1.8.tar` & `telemetrix-1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2021-11-29 16:09:47.199628 telemetrix-1.8/
--rw-rw-r--   0 afy       (1000) afy       (1000)       21 2021-11-29 15:48:23.000000 telemetrix-1.8/MANIFEST.in
--rw-rw-r--   0 afy       (1000) afy       (1000)     3318 2021-11-29 16:09:47.199628 telemetrix-1.8/PKG-INFO
--rw-rw-r--   0 afy       (1000) afy       (1000)     2423 2021-11-29 16:07:23.000000 telemetrix-1.8/README.md
--rw-rw-r--   0 afy       (1000) afy       (1000)     2425 2021-11-29 16:06:39.000000 telemetrix-1.8/pypi_desc.md
--rw-rw-r--   0 afy       (1000) afy       (1000)       38 2021-11-29 16:09:47.199628 telemetrix-1.8/setup.cfg
--rw-rw-r--   0 afy       (1000) afy       (1000)     1150 2021-11-29 16:06:39.000000 telemetrix-1.8/setup.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2021-11-29 16:09:47.199628 telemetrix-1.8/telemetrix/
--rw-rw-r--   0 afy       (1000) afy       (1000)        0 2020-11-27 18:58:16.000000 telemetrix-1.8/telemetrix/__init__.py
--rw-rw-r--   0 afy       (1000) afy       (1000)     4084 2021-11-29 16:06:39.000000 telemetrix-1.8/telemetrix/private_constants.py
--rw-rw-r--   0 afy       (1000) afy       (1000)    86855 2021-11-29 16:06:39.000000 telemetrix-1.8/telemetrix/telemetrix.py
-drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2021-11-29 16:09:47.199628 telemetrix-1.8/telemetrix.egg-info/
--rw-rw-r--   0 afy       (1000) afy       (1000)     3318 2021-11-29 16:09:47.000000 telemetrix-1.8/telemetrix.egg-info/PKG-INFO
--rw-rw-r--   0 afy       (1000) afy       (1000)      292 2021-11-29 16:09:47.000000 telemetrix-1.8/telemetrix.egg-info/SOURCES.txt
--rw-rw-r--   0 afy       (1000) afy       (1000)        1 2021-11-29 16:09:47.000000 telemetrix-1.8/telemetrix.egg-info/dependency_links.txt
--rw-rw-r--   0 afy       (1000) afy       (1000)        9 2021-11-29 16:09:47.000000 telemetrix-1.8/telemetrix.egg-info/requires.txt
--rw-rw-r--   0 afy       (1000) afy       (1000)       11 2021-11-29 16:09:47.000000 telemetrix-1.8/telemetrix.egg-info/top_level.txt
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2022-02-11 23:39:25.485752 telemetrix-1.9/
+-rw-rw-r--   0 afy       (1000) afy       (1000)       21 2021-11-29 16:14:01.000000 telemetrix-1.9/MANIFEST.in
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3318 2022-02-11 23:39:25.485752 telemetrix-1.9/PKG-INFO
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2423 2021-11-29 16:14:01.000000 telemetrix-1.9/README.md
+-rw-rw-r--   0 afy       (1000) afy       (1000)     2425 2021-11-29 16:14:01.000000 telemetrix-1.9/pypi_desc.md
+-rw-rw-r--   0 afy       (1000) afy       (1000)       38 2022-02-11 23:39:25.485752 telemetrix-1.9/setup.cfg
+-rw-rw-r--   0 afy       (1000) afy       (1000)     1150 2022-02-11 15:19:10.000000 telemetrix-1.9/setup.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2022-02-11 23:39:25.485752 telemetrix-1.9/telemetrix/
+-rw-rw-r--   0 afy       (1000) afy       (1000)        0 2020-11-27 18:58:16.000000 telemetrix-1.9/telemetrix/__init__.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)     4084 2022-02-11 15:19:10.000000 telemetrix-1.9/telemetrix/private_constants.py
+-rw-rw-r--   0 afy       (1000) afy       (1000)    87210 2022-01-18 20:53:24.000000 telemetrix-1.9/telemetrix/telemetrix.py
+drwxrwxr-x   0 afy       (1000) afy       (1000)        0 2022-02-11 23:39:25.485752 telemetrix-1.9/telemetrix.egg-info/
+-rw-rw-r--   0 afy       (1000) afy       (1000)     3318 2022-02-11 23:39:25.000000 telemetrix-1.9/telemetrix.egg-info/PKG-INFO
+-rw-rw-r--   0 afy       (1000) afy       (1000)      292 2022-02-11 23:39:25.000000 telemetrix-1.9/telemetrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 afy       (1000) afy       (1000)        1 2022-02-11 23:39:25.000000 telemetrix-1.9/telemetrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 afy       (1000) afy       (1000)        9 2022-02-11 23:39:25.000000 telemetrix-1.9/telemetrix.egg-info/requires.txt
+-rw-rw-r--   0 afy       (1000) afy       (1000)       11 2022-02-11 23:39:25.000000 telemetrix-1.9/telemetrix.egg-info/top_level.txt
```

### Comparing `telemetrix-1.8/PKG-INFO` & `telemetrix-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telemetrix
-Version: 1.8
+Version: 1.9
 Summary: Remotely Control And Monitor Arduino-Core devices
 Home-page: https://github.com/MrYsLab/telemetrix
 Author: Alan Yorinks
 Author-email: MisterYsLab@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/MrYsLab/telemetrix
 Keywords: telemetrix,Arduino,Protocol,Python
```

### Comparing `telemetrix-1.8/README.md` & `telemetrix-1.9/README.md`

 * *Files identical despite different names*

### Comparing `telemetrix-1.8/pypi_desc.md` & `telemetrix-1.9/pypi_desc.md`

 * *Files identical despite different names*

### Comparing `telemetrix-1.8/setup.py` & `telemetrix-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 setup(
     name='telemetrix',
     packages=['telemetrix'],
     install_requires=['pyserial'],
 
-    version='1.8',
+    version='1.9',
     description="Remotely Control And Monitor Arduino-Core devices",
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     author='Alan Yorinks',
     author_email='MisterYsLab@gmail.com',
     url='https://github.com/MrYsLab/telemetrix',
```

### Comparing `telemetrix-1.8/telemetrix/private_constants.py` & `telemetrix-1.9/telemetrix/private_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     STEPPER_TARGET_POSITION = 16
     STEPPER_CURRENT_POSITION = 17
     STEPPER_RUNNING_REPORT = 18
     STEPPER_RUN_COMPLETE_REPORT = 19
     FEATURES = 20
     DEBUG_PRINT = 99
 
-    TELEMETRIX_VERSION = "1.8"
+    TELEMETRIX_VERSION = "1.9"
 
     # reporting control
     REPORTING_DISABLE_ALL = 0
     REPORTING_ANALOG_ENABLE = 1
     REPORTING_DIGITAL_ENABLE = 2
     REPORTING_ANALOG_DISABLE = 3
     REPORTING_DIGITAL_DISABLE = 4
```

### Comparing `telemetrix-1.8/telemetrix/telemetrix.py` & `telemetrix-1.9/telemetrix/telemetrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -763,16 +763,16 @@
         callback returns a data list:
 
         [pin_type, pin_number, pin_value, raw_time_stamp]
 
         The pin_type for digital input pins with pullups enabled = 11
 
         """
-        self._set_pin_mode(pin_number, PrivateConstants.AT_INPUT_PULLUP, callback=
-        callback)
+        self._set_pin_mode(pin_number, PrivateConstants.AT_INPUT_PULLUP,
+                           callback=callback)
 
     def set_pin_mode_digital_output(self, pin_number):
         """
         Set a pin as a digital output pin.
 
         :param pin_number: arduino pin number
         """
@@ -1059,47 +1059,59 @@
         If you are trying to use constant speed movements, you should call setSpeed()
         after calling moveTo().
 
         :param motor_id: motor id: 0 - 3
 
         :param position: target position. Maximum value is 32 bits.
         """
-
+        if position < 0:
+            polarity = 1
+        else:
+            polarity = 0
+        position = abs(position)
         if not self.stepper_info_list[motor_id]['instance']:
             if self.shutdown_on_exception:
                 self.shutdown()
             raise RuntimeError('stepper_move_to: Invalid motor_id.')
 
         position_bytes = list(position.to_bytes(4, 'big', signed=True))
 
         command = [PrivateConstants.STEPPER_MOVE_TO, motor_id]
         for value in position_bytes:
             command.append(value)
+        command.append(polarity)
         self._send_command(command)
 
     def stepper_move(self, motor_id, relative_position):
         """
         Set the target position relative to the current position.
 
         :param motor_id: motor id: 0 - 3
 
         :param relative_position: The desired position relative to the current
                                   position. Negative is anticlockwise from
                                   the current position. Maximum value is 32 bits.
         """
+        if relative_position < 0:
+            polarity = 1
+        else:
+            polarity = 0
+
+        relative_position = abs(relative_position)
         if not self.stepper_info_list[motor_id]['instance']:
             if self.shutdown_on_exception:
                 self.shutdown()
             raise RuntimeError('stepper_move: Invalid motor_id.')
 
         position_bytes = list(relative_position.to_bytes(4, 'big', signed=True))
 
         command = [PrivateConstants.STEPPER_MOVE, motor_id]
         for value in position_bytes:
             command.append(value)
+        command.append(polarity)
         self._send_command(command)
 
     def stepper_run(self, motor_id, completion_callback=None):
         """
         This method steps the selected motor based on the current speed.
 
         Once called, the server will continuously attempt to step the motor.
```

### Comparing `telemetrix-1.8/telemetrix.egg-info/PKG-INFO` & `telemetrix-1.9/telemetrix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telemetrix
-Version: 1.8
+Version: 1.9
 Summary: Remotely Control And Monitor Arduino-Core devices
 Home-page: https://github.com/MrYsLab/telemetrix
 Author: Alan Yorinks
 Author-email: MisterYsLab@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/MrYsLab/telemetrix
 Keywords: telemetrix,Arduino,Protocol,Python
```

