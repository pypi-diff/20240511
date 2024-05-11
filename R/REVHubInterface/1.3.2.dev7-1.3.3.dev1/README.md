# Comparing `tmp/revhubinterface-1.3.2.dev7.tar.gz` & `tmp/revhubinterface-1.3.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.2.dev7.tar", last modified: Wed May  8 01:55:06 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.3.dev1.tar", last modified: Sat May 11 07:42:48 2024, max compression
```

## Comparing `revhubinterface-1.3.2.dev7.tar` & `revhubinterface-1.3.3.dev1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.811960 revhubinterface-1.3.2.dev7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.811960 revhubinterface-1.3.2.dev7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73572 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface-mac.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 01:55:06.000000 revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/flatpak/flatpak-pip-generator
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 01:55:02.000000 revhubinterface-1.3.2.dev7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:55:06.815960 revhubinterface-1.3.2.dev7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:42:48.569395 revhubinterface-1.3.3.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:42:48.561395 revhubinterface-1.3.3.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:42:48.561395 revhubinterface-1.3.3.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-11 07:42:48.565395 revhubinterface-1.3.3.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:42:48.565395 revhubinterface-1.3.3.dev1/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61200 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:42:48.565395 revhubinterface-1.3.3.dev1/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-11 07:42:48.000000 revhubinterface-1.3.3.dev1/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-11 07:42:48.000000 revhubinterface-1.3.3.dev1/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 07:42:48.000000 revhubinterface-1.3.3.dev1/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-11 07:42:48.000000 revhubinterface-1.3.3.dev1/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-11 07:42:48.000000 revhubinterface-1.3.3.dev1/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 07:42:48.000000 revhubinterface-1.3.3.dev1/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:42:48.565395 revhubinterface-1.3.3.dev1/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/flatpak/flatpak-pip-generator
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/org.unofficialrevport.REVHubInterface.Devel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/org.unofficialrevport.REVHubInterface.Source.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/org.unofficialrevport.REVHubInterface.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-11 07:42:43.000000 revhubinterface-1.3.3.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 07:42:48.569395 revhubinterface-1.3.3.dev1/setup.cfg
```

### Comparing `revhubinterface-1.3.2.dev7/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.3.dev1/.github/workflows/pyinstaller.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 on:
   push:
     branches:
-      - trigger-actions
+      - main
 
 jobs:
   pyinstaller-build-mac:
     runs-on: macos-latest
     steps:
       - name: Create Executable
         uses: sayyid5416/pyinstaller@v1
         with:
           python_ver: '3.12'
           pyinstaller_ver: '==6.6.0'
-          spec: 'REVHubInterface-mac.spec'
+          spec: 'REVHubInterface.spec'
           requirements: 'requirements.txt'
           upload_exe_with_name: 'REVHubInterface_Mac_Binary'
-          options: --onefile, --name "REVHubInterface", --windowed,
       - name: Make DMG
         uses: QQxiaoming/create-dmg-action@v0.0.2
         with:
           name: 'REVHubInterface_Mac_DMG'
           srcdir: './dist'
       - name: Upload DMG
         uses: actions/upload-artifact@v4
@@ -33,23 +32,21 @@
         uses: sayyid5416/pyinstaller@v1
         with:
           python_ver: '3.12'
           pyinstaller_ver: '==6.6.0'
           spec: 'REVHubInterface.spec'
           requirements: 'requirements.txt'
           upload_exe_with_name: 'REVHubInterface_Windows'
-          options: --onefile, --name "REVHubInterface", --windowed,
   pyinstaller-build-linux:
     runs-on: ubuntu-latest
     steps:
       - name: Create Executable
         uses: sayyid5416/pyinstaller@v1
         with:
           python_ver: '3.12'
           pyinstaller_ver: '==6.6.0'
           spec: 'REVHubInterface.spec'
           requirements: 'requirements.txt'
           upload_exe_with_name: 'REVHubInterface_Linux'
-          options: --onefile, --name "REVHubInterface", --windowed,
```

### Comparing `revhubinterface-1.3.2.dev7/.github/workflows/python-publish.yml` & `revhubinterface-1.3.3.dev1/.github/workflows/python-publish.yml`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 name: Upload Python Package
 
 on:
   release:
     types: [published]
   push:
     branches:
-      - trigger-actions
+      - main
 
 permissions:
   contents: read
 
 jobs:
   release-build:
     runs-on: ubuntu-latest
```

### Comparing `revhubinterface-1.3.2.dev7/LICENSE.txt` & `revhubinterface-1.3.3.dev1/LICENSE.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Copyright (c) 2024, Unofficial Rev Port team and contributors.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+    * Redistributions of source code must retain the above copyright
+      notice, this list of conditions and the following disclaimer.
+    * Redistributions in binary form must reproduce the above copyright
+      notice, this list of conditions and the following disclaimer in the
+      documentation and/or other materials provided with the distribution.
+    * Neither the name of the Unofficial Rev Port team nor the
+      names of its contributors may be used to endorse or promote products
+      derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE UNOFFICIAL REV PORT TEAM OR CONTRIBUTORS BE LIABLE FOR ANY
+DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+This software is based on the REV Hub Interface tool created by REV, which was released under the following license:
 Copyright (c) 2019, REV Robotics LLC
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
     * Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
```

### Comparing `revhubinterface-1.3.2.dev7/PKG-INFO` & `revhubinterface-1.3.3.dev1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-Metadata-Version: 2.1
-Name: REVHubInterface
-Version: 1.3.2.dev7
-Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: pyft232==0.12
-Requires-Dist: pyserial==3.5
-Requires-Dist: sv-ttk==2.6.0
-
 # REV Hub Interface (Community Edition)
 
 The REV Hub Interface is a piece of software allowing for a direct connection from a REV Expansion Hub and its peripherals to a PC. 
 
 This interface provides a method for teams to prototype with motors, servos, and sensors in a way that is faster and easier than setting up an entire robot control system. It is also a valuable troubleshooting tool that can help isolate the cause of an issue and determine if it is electrical or software related. The REV Hub Firmware can also be updated and recovered through this interface in addition to the Robot Controller Application.
 
-This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows).
+This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows). Though initially created by REV, this version of the software is **not maintained by or affiliated with REV.**  Do **not** contact REV support about any issues you experience with this software, instead you may create a GitHub Issue or ask in https://discord.gg/pU2fesSTqF. 
+
+This software is licensed under the BSD-3-Clause license. The full text is availiable in the LICENSE.txt file.
 
 ## Installing the software
 
 Start by downloading the latest version of the software from [the Releases page](https://github.com/unofficial-rev-port/REVHubInterface/releases).  An `.exe` is provided for Windows systems, a Flatpak for Linux systems (soon to be published on Flathub), and a `.DMG` for macOS.
 Alternately, you can download it from PyPi:
 
 1. Install Python 3
```

### Comparing `revhubinterface-1.3.2.dev7/README.md` & `revhubinterface-1.3.3.dev1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,26 @@
+Metadata-Version: 2.1
+Name: REVHubInterface
+Version: 1.3.3.dev1
+Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: pyft232==0.12
+Requires-Dist: pyserial==3.5
+Requires-Dist: sv-ttk==2.6.0
+
 # REV Hub Interface (Community Edition)
 
 The REV Hub Interface is a piece of software allowing for a direct connection from a REV Expansion Hub and its peripherals to a PC. 
 
 This interface provides a method for teams to prototype with motors, servos, and sensors in a way that is faster and easier than setting up an entire robot control system. It is also a valuable troubleshooting tool that can help isolate the cause of an issue and determine if it is electrical or software related. The REV Hub Firmware can also be updated and recovered through this interface in addition to the Robot Controller Application.
 
-This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows).
+This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows). Though initially created by REV, this version of the software is **not maintained by or affiliated with REV.**  Do **not** contact REV support about any issues you experience with this software, instead you may create a GitHub Issue or ask in https://discord.gg/pU2fesSTqF. 
+
+This software is licensed under the BSD-3-Clause license. The full text is availiable in the LICENSE.txt file.
 
 ## Installing the software
 
 Start by downloading the latest version of the software from [the Releases page](https://github.com/unofficial-rev-port/REVHubInterface/releases).  An `.exe` is provided for Windows systems, a Flatpak for Linux systems (soon to be published on Flathub), and a `.DMG` for macOS.
 Alternately, you can download it from PyPi:
 
 1. Install Python 3
```

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.3.dev1/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface/REVADC.py` & `revhubinterface-1.3.3.dev1/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.3.dev1/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.3.dev1/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.3.dev1/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.3.dev1/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface/REVModule.py` & `revhubinterface-1.3.3.dev1/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.3.dev1/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface/REVServo.py` & `revhubinterface-1.3.3.dev1/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.3.dev1/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.3.dev1/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface-mac.spec` & `revhubinterface-1.3.3.dev1/REVHubInterface.spec`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- mode: python ; coding: utf-8 -*-
 from PyInstaller.utils.hooks import collect_all
+from PyInstaller.utils.hooks import collect_data_files
 
 datas = []
+datas += collect_data_files('sv_ttk')
 binaries = []
 hiddenimports = []
 tmp_ret = collect_all('REVHubInterface')
 datas += tmp_ret[0]; binaries += tmp_ret[1]; hiddenimports += tmp_ret[2]
 
 
 block_cipher = None
```

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.3.dev1/REVHubInterface.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.2.dev7
+Version: 1.3.3.dev1
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
 
 # REV Hub Interface (Community Edition)
 
 The REV Hub Interface is a piece of software allowing for a direct connection from a REV Expansion Hub and its peripherals to a PC. 
 
 This interface provides a method for teams to prototype with motors, servos, and sensors in a way that is faster and easier than setting up an entire robot control system. It is also a valuable troubleshooting tool that can help isolate the cause of an issue and determine if it is electrical or software related. The REV Hub Firmware can also be updated and recovered through this interface in addition to the Robot Controller Application.
 
-This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows).
+This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows). Though initially created by REV, this version of the software is **not maintained by or affiliated with REV.**  Do **not** contact REV support about any issues you experience with this software, instead you may create a GitHub Issue or ask in https://discord.gg/pU2fesSTqF. 
+
+This software is licensed under the BSD-3-Clause license. The full text is availiable in the LICENSE.txt file.
 
 ## Installing the software
 
 Start by downloading the latest version of the software from [the Releases page](https://github.com/unofficial-rev-port/REVHubInterface/releases).  An `.exe` is provided for Windows systems, a Flatpak for Linux systems (soon to be published on Flathub), and a `.DMG` for macOS.
 Alternately, you can download it from PyPi:
 
 1. Install Python 3
```

### Comparing `revhubinterface-1.3.2.dev7/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.3.dev1/REVHubInterface.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 .gitignore
 LICENSE.txt
 README.md
-REVHubInterface-mac.spec
 REVHubInterface.sh
 REVHubInterface.spec
+org.unofficialrevport.REVHubInterface.Devel.svg
+org.unofficialrevport.REVHubInterface.Source.svg
+org.unofficialrevport.REVHubInterface.svg
 pyproject.toml
 requirements.txt
 .github/workflows/pyinstaller.yml
 .github/workflows/python-publish.yml
 REVHubInterface/REV2mSensor.py
 REVHubInterface/REVADC.py
 REVHubInterface/REVColorSensorV3.py
```

### Comparing `revhubinterface-1.3.2.dev7/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.3.dev1/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.3.dev1/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/flatpak/python3-requirements.json` & `revhubinterface-1.3.3.dev1/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev7/pyproject.toml` & `revhubinterface-1.3.3.dev1/pyproject.toml`

 * *Files identical despite different names*

