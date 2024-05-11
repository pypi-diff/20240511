# Comparing `tmp/radiacode-0.3.2.tar.gz` & `tmp/radiacode-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radiacode-0.3.2.tar", max compression
+gzip compressed data, was "radiacode-0.3.3.tar", max compression
```

## Comparing `radiacode-0.3.2.tar` & `radiacode-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1070 2023-12-11 09:18:44.124390 radiacode-0.3.2/LICENSE
--rw-r--r--   0        0        0     1520 2023-12-11 09:18:44.124390 radiacode-0.3.2/README.md
--rw-r--r--   0        0        0     1303 2023-12-11 09:18:44.124390 radiacode-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      147 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode/__init__.py
--rw-r--r--   0        0        0      694 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode/bytes_buffer.py
--rw-r--r--   0        0        0        0 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode/decoders/__init__.py
--rw-r--r--   0        0        0     4000 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode/decoders/databuf.py
--rw-r--r--   0        0        0     1573 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode/decoders/spectrum.py
--rw-r--r--   0        0        0     8305 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode/radiacode.py
--rw-r--r--   0        0        0        0 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode/transports/__init__.py
--rw-r--r--   0        0        0     1720 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode/transports/bluetooth.py
--rw-r--r--   0        0        0     1937 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode/transports/usb.py
--rw-r--r--   0        0        0     2500 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode/types.py
--rw-r--r--   0        0        0     1296 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode-examples/README.md
--rw-r--r--   0        0        0     1215 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode-examples/README_ru.md
--rw-r--r--   0        0        0      933 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode-examples/basic.py
--rw-r--r--   0        0        0     2309 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode-examples/narodmon.py
--rw-r--r--   0        0        0     1760 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode-examples/radiacode-exporter.py
--rwxr-xr-x   0        0        0    11387 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode-examples/show-spectrum.py
--rw-r--r--   0        0        0     4456 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode-examples/webserver.html
--rw-r--r--   0        0        0     3383 2023-12-11 09:18:44.124390 radiacode-0.3.2/radiacode-examples/webserver.py
--rw-r--r--   0        0        0     2655 1970-01-01 00:00:00.000000 radiacode-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-11 11:21:36.425989 radiacode-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2010 2024-05-11 11:21:36.425989 radiacode-0.3.3/README.md
+-rw-r--r--   0        0        0     1289 2024-05-11 11:21:36.425989 radiacode-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      147 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode/__init__.py
+-rw-r--r--   0        0        0      694 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode/bytes_buffer.py
+-rw-r--r--   0        0        0        0 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode/decoders/__init__.py
+-rw-r--r--   0        0        0     4000 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode/decoders/databuf.py
+-rw-r--r--   0        0        0     1573 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode/decoders/spectrum.py
+-rw-r--r--   0        0        0     8801 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode/radiacode.py
+-rw-r--r--   0        0        0        0 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode/transports/__init__.py
+-rw-r--r--   0        0        0     2041 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode/transports/bluetooth.py
+-rw-r--r--   0        0        0     1936 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode/transports/usb.py
+-rw-r--r--   0        0        0     2500 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode/types.py
+-rw-r--r--   0        0        0     1296 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode-examples/README.md
+-rw-r--r--   0        0        0     1215 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode-examples/README_ru.md
+-rw-r--r--   0        0        0     1874 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode-examples/basic.py
+-rw-r--r--   0        0        0     2309 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode-examples/narodmon.py
+-rw-r--r--   0        0        0     1760 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode-examples/radiacode-exporter.py
+-rwxr-xr-x   0        0        0    14256 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode-examples/show-spectrum.py
+-rw-r--r--   0        0        0     4456 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode-examples/webserver.html
+-rw-r--r--   0        0        0     3383 2024-05-11 11:21:36.425989 radiacode-0.3.3/radiacode-examples/webserver.py
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 radiacode-0.3.3/PKG-INFO
```

### Comparing `radiacode-0.3.2/LICENSE` & `radiacode-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `radiacode-0.3.2/README.md` & `radiacode-0.3.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -31,7 +31,12 @@
 - install [python poetry](https://python-poetry.org/docs/#installation)
 - clone this repository
 - install and run:
 ```
 $ poetry install
 $ poetry run python3 radiacode-examples/basic.py --bluetooth-mac 52:43:01:02:03:04 # or without --bluetooth-mac for USB connection
 ```
+
+## MacOS
+The library used to communicate over Bluetooh (```bluepy```) is [not supported](https://github.com/IanHarvey/bluepy/issues/44) on MacOS. Only the USB connection is available on Apple devices. A ```USB Serial Number```, obtainable from the ```Device Info``` menu on the device itself, can be specified if more than one Radiacode is connected via USB at the same time.
+
+Make sure ```libusb``` is installed on your system, if you use ```Brew``` you can run: ```brew install libusb```
```

### Comparing `radiacode-0.3.2/pyproject.toml` & `radiacode-0.3.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 [tool.poetry]
 name = "radiacode"
-version = "0.3.2"
+version = "0.3.3"
 description = "Library for RadiaCode-101"
 authors = ["Maxim Andreev <andreevmaxim@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cdump/radiacode"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
 ]
 include = ["radiacode-examples/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-bluepy = "^1.3"
+bluepy = { version = "^1.3", markers = "sys_platform != 'darwin'" }
 pyusb = "^1.2"
 aiohttp = {version = "^3.9", optional = true}
 prometheus-client = {version = "^0.19", optional = true}
 matplotlib = {version = "^3.7", optional = true}
 numpy = {version = "^1.26", optional = true}
 pyyaml = {version = "^6.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1"
 mypy = "^1.7"
-black = "^23.11"
 
 [tool.poetry.extras]
 examples = ["aiohttp", "prometheus-client", "matplotlib", "numpy", "pyyaml"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 130
-target-version = ["py310"]
-skip-string-normalization = true
-
 [tool.ruff]
 extend-select = ["B", "Q"]
 line-length = 130
 target-version = "py310"
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "single"
 
+[tool.ruff.format]
+quote-style = "single"
+
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
```

### Comparing `radiacode-0.3.2/radiacode/bytes_buffer.py` & `radiacode-0.3.3/radiacode/bytes_buffer.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.3.2/radiacode/decoders/databuf.py` & `radiacode-0.3.3/radiacode/decoders/databuf.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.3.2/radiacode/decoders/spectrum.py` & `radiacode-0.3.3/radiacode/decoders/spectrum.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.3.2/radiacode/radiacode.py` & `radiacode-0.3.3/radiacode/radiacode.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import struct
+import platform
 from typing import List, Optional, Union
 
 from radiacode.bytes_buffer import BytesBuffer
 from radiacode.decoders.databuf import decode_VS_DATA_BUF
 from radiacode.decoders.spectrum import decode_RC_VS_SPECTRUM
 from radiacode.transports.bluetooth import Bluetooth
 from radiacode.transports.usb import Usb
@@ -21,15 +22,19 @@
     def __init__(
         self,
         bluetooth_mac: Optional[str] = None,
         serial_number: Optional[str] = None,
         ignore_firmware_compatibility_check: bool = False,
     ):
         self._seq = 0
-        if bluetooth_mac is not None:
+
+        # Bluepy doesn't support MacOS: https://github.com/IanHarvey/bluepy/issues/44
+        self._bt_supported = platform.system() != 'Darwin'
+
+        if bluetooth_mac is not None and self._bt_supported is True:
             self._connection = Bluetooth(bluetooth_mac)
         else:
             self._connection = Usb(serial_number=serial_number)
 
         # init
         self.execute(b'\x07\x00', b'\x01\xff\x12\xff')
         self._base_time = datetime.datetime.now()
@@ -109,15 +114,15 @@
     def fw_version(self) -> tuple[tuple[int, int, str], tuple[int, int, str]]:
         r = self.execute(b'\x0a\x00')
         boot_minor, boot_major = r.unpack('<HH')
         boot_date = r.unpack_string()
         target_minor, target_major = r.unpack('<HH')
         target_date = r.unpack_string()
         assert r.size() == 0
-        return ((boot_major, boot_minor, boot_date), (target_major, target_minor, target_date))
+        return ((boot_major, boot_minor, boot_date), (target_major, target_minor, target_date.strip('\x00')))
 
     def hw_serial_number(self) -> str:
         r = self.execute(b'\x0b\x00')
         serial_len = r.unpack('<I')[0]
         assert serial_len % 4 == 0
         serial_groups = [r.unpack('<I')[0] for _ in range(serial_len // 4)]
         assert r.size() == 0
@@ -165,14 +170,21 @@
         assert r.size() == 0
 
     # used in spectrum_channel_to_energy
     def energy_calib(self) -> List[float]:
         r = self.read_request(VS.ENERGY_CALIB)
         return list(r.unpack('<fff'))
 
+    def set_energy_calib(self, coef: List[float]) -> None:
+        assert len(coef) == 3
+        pc = struct.pack('<fff', *coef)
+        r = self.execute(b'\x27\x08', struct.pack('<II', int(VS.ENERGY_CALIB), len(pc)) + pc)
+        retcode = r.unpack('<I')[0]
+        assert retcode == 1
+
     def set_language(self, lang='ru') -> None:
         assert lang in {'ru', 'en'}, 'unsupported lang value - use "ru" or "en"'
         self.write_request(VSFR.DEVICE_LANG, struct.pack('<I', bool(lang == 'en')))
 
     def set_device_on(self, on: bool):
         assert not on, 'only False value accepted'
         self.write_request(VSFR.DEVICE_ON, struct.pack('<I', bool(on)))
```

### Comparing `radiacode-0.3.2/radiacode/transports/usb.py` & `radiacode-0.3.3/radiacode/transports/usb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import struct
-
 import usb.core
 
 from radiacode.bytes_buffer import BytesBuffer
 
 
 class DeviceNotFound(Exception):
     pass
```

### Comparing `radiacode-0.3.2/radiacode/types.py` & `radiacode-0.3.3/radiacode/types.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.3.2/radiacode-examples/README.md` & `radiacode-0.3.3/radiacode-examples/README.md`

 * *Files identical despite different names*

### Comparing `radiacode-0.3.2/radiacode-examples/README_ru.md` & `radiacode-0.3.3/radiacode-examples/README_ru.md`

 * *Files identical despite different names*

### Comparing `radiacode-0.3.2/radiacode-examples/narodmon.py` & `radiacode-0.3.3/radiacode-examples/narodmon.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.3.2/radiacode-examples/radiacode-exporter.py` & `radiacode-0.3.3/radiacode-examples/radiacode-exporter.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.3.2/radiacode-examples/show-spectrum.py` & `radiacode-0.3.3/radiacode-examples/show-spectrum.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,23 +7,49 @@
 
   Calculates and shows in an animated display:
 
    - counts:      accumulated number of counts/sec
    - count rate:  count rate
    - dose rate:   energy deposit in crystal, i.e. sum(counts*energies).
    - total dose:  total sum of deposited energies
+
+
+  Command line options:
+
+    Usage: show-spectrum.py [-h] [-b BLUETOOTH_MAC] [-r] [-R] [-q]
+            [-i INTERVAL] [-f FILE] [-t TIME] [-H HISTORY]
+
+    Read and display gamma energy spectrum from RadioCode 102, 
+    show differential and updated cumulative spectrum, 
+    optionally store data to file in yaml format.  
+
+    Options:
+      -h, --help          show this help message and exit
+      -b BLUETOOTH_MAC, --bluetooth-mac BLUETOOTH_MAC  bluetooth MAC address of device
+      -s SERIAL_NUMBER, --serial-number SERIAL_NUMBER  serial number of device
+      -r, --restart       restart spectrum accumulation
+      -R, --Reset         reset spectrum stored in device
+      -q, --quiet         no status output to terminal
+      -i INTERVAL, --interval INTERVAL update interval
+      -f FILE, --file FILE  file to store results
+      -t TIME, --time TIME  run time in seconds
+      -H HISTORY, --history HISTORY  number of rate-history points to store in file
+
+   Hint: use option -R to reset spectrum data in RadiaCode device
+     
 """
 
 import argparse
 import sys
 import time
 import numpy as np
 import yaml
 import matplotlib as mpl
 import matplotlib.pyplot as plt
+import matplotlib.patches as patches
 from radiacode import RadiaCode
 
 # set backend and matplotlib style
 mpl.use('Qt5Agg')
 plt.style.use('dark_background')
 
 # some constants
@@ -34,113 +60,133 @@
 depositedE2dose = keV2J * 1e6 / m_sensor  # dose rate in µGy/h
 
 
 class appColors:
     """Define colors used in this app"""
 
     title = 'goldenrod'
-    text1 = 'linen'
-    text2 = 'lime'
-    text3 = 'red'
+    text1 = 'blue'
+    text2 = 'green'
+    text3 = 'lightgreen'
+    text4 = 'red'
     bg = 'black'
     line1 = '#F0F0C0'
     marker1 = 'orange'
     auxline = 'red'
 
 
 def plot_RC102Spectrum():
     # Helper functions for conversion of channel numbers to energies
     global a0, a1, a2  # calibration constants
-    # approx. calibration, overwritten by first  retrieved spectrum
+    # approx. calibration, overwritten by first retrieved spectrum
     a0 = 0.17
     a1 = 2.42
     a2 = 0.0004
 
+    global mpl_active  # flag indicating that matplotlib figure exists
+    mpl_active = False
+
     def Chan2En(C):
         # convert Channel number to Energy
         #  E = a0 + a1*C + a2 C^2
         return a0 + a1 * C + a2 * C**2
 
     def En2Chan(E):
         # convert Energies to Channel Numbers
         # inverse E = a0 + a1*C + a2 C^2
         c = a0 - E
         return (np.sqrt(a1**2 - 4 * a2 * c) - a1) / (2 * a2)
 
+    def on_mpl_window_closed(ax):
+        # detect when matplotlib window is closed
+        global mpl_active
+        print('    !!! Graphics window closed')
+        mpl_active = False
+
     # end helpers ---------------------------------------
 
     # ------
     # parse command line arguments
     # ------
-    parser = argparse.ArgumentParser(description='read and display spectrum from RadioCode 102')
-    parser.add_argument('--bluetooth-mac', type=str, nargs='+', required=False, help='bluetooth MAC address of device')
-    parser.add_argument(
-        '-n',
-        '--noreset',
-        action='store_const',
-        const=True,
-        default=False,
-        help='do not reset spectrum stored in device',
+    parser = argparse.ArgumentParser(
+        description='Read and display gamma energy spectrum from RadioCode 102, '
+        + 'show differential and updated cumulative spectrum, '
+        + 'optionally store data to file in yaml format.'
     )
+    parser.add_argument('-b', '--bluetooth-mac', type=str, required=False, help='bluetooth MAC address of device')
+    parser.add_argument('-s', '--serial-number', type=str, required=False, help='serial number of device')
+    parser.add_argument('-r', '--restart', action='store_true', help='restart spectrum accumulation')
+    parser.add_argument('-R', '--Reset', action='store_true', help='reset spectrum stored in device')
+    parser.add_argument('-q', '--quiet', action='store_true', help='no status output to terminal')
     parser.add_argument('-i', '--interval', type=float, default=1.0, help='update interval')
     parser.add_argument('-f', '--file', type=str, default='', help='file to store results')
     parser.add_argument('-t', '--time', type=int, default=36000, help='run time in seconds')
-    parser.add_argument('-H', '--history', type=int, default=500, help='number of rate history points')
+    parser.add_argument('-H', '--history', type=int, default=500, help='number of rate-history points to store in file')
     args = parser.parse_args()
 
     bluetooth_mac = args.bluetooth_mac
-    reset_spectrum = not args.noreset
+    serial_number = args.serial_number
+    restart_accumulation = args.restart
+    reset_device_spectrum = args.Reset
+    quiet = args.quiet
     dt_wait = args.interval
     timestamp = time.strftime('%y%m%d-%H%M', time.localtime())
     print(args.file)
     filename = args.file + '_' + timestamp + '.yaml' if args.file != '' else ''
     NHistory = args.history
     run_time = args.time
     rate_history = np.zeros(NHistory)
 
-    print(f'\n *==* script {sys.argv[0]} executing')
+    if not quiet:
+        print(f'\n *==* script {sys.argv[0]} executing')
+        if bluetooth_mac is not None:
+            print(f'    connecting via Bluetooth, MAC {bluetooth_mac}')
+        elif serial_number is not None:
+            print(f'    connect via USB to device with SN {serial_number}')
+        else:
+            print('    connect via USB')
 
     # ------
     # initialize and connect to RC10x device
     # ------
-    rc = RadiaCode(bluetooth_mac=bluetooth_mac)
+    rc = RadiaCode(bluetooth_mac=bluetooth_mac, serial_number=serial_number)
     serial = rc.serial_number()
     fw_version = rc.fw_version()
     status_flags = eval(rc.status().split(':')[1])[0]
     a0, a1, a2 = rc.energy_calib()
     # get initial spectrum and meta-data
-    if reset_spectrum:
+    if reset_device_spectrum:
         rc.spectrum_reset()
     spectrum = rc.spectrum()
     # print(f'### Spectrum: {spectrum}')
     counts0 = np.asarray(spectrum.counts)
     NChannels = len(counts0)
     Channels = np.asarray(range(NChannels)) + 0.5
     Energies = Chan2En(Channels)
     duration_s = spectrum.duration.total_seconds()
-    countsum0 = np.sum(np.asarray(spectrum.counts))
     _t0 = time.time()
     t_start = _t0  # start time of acquisition from device
-    T0 = _t0 - duration_s  # start time of accumulation
 
     print(f'### Found device with serial number: {serial}')
     print(f'    Firmware: {fw_version}')
     print(f'    Status flags: 0x{status_flags:x}')
     print(f'    Calibration coefficientes: a0={a0:.6f}, a1={a1:.6f}, a2={a2:.6f}')
     print(f'    Number of spectrum channels: {NChannels}')
     print(f'    Spectrum accumulation since {spectrum.duration}')
 
     # ------
     # initialize graphics display
     # -------
     # create a figure with two sub-plots
-    fig = plt.figure('Gamma Spectrum', figsize=(8.0, 8.0))
-    fig.suptitle('Radiacode Spectrum   ' + time.asctime(), size='large', color=appColors.title)
-    fig.subplots_adjust(left=0.12, bottom=0.1, right=0.95, top=0.85, wspace=None, hspace=0.1)  #
+    fig = plt.figure('GammaSpectrum', figsize=(8.0, 8.0))
+    fig.suptitle('Radiacode: $\gamma$-ray spectrum   ' + time.asctime(), size='large', color=appColors.title)
+    fig.subplots_adjust(left=0.12, bottom=0.1, right=0.95, top=0.88, wspace=None, hspace=0.1)  #
     gs = fig.add_gridspec(nrows=15, ncols=1)
+    mpl_active = True
+    fig.canvas.mpl_connect('close_event', on_mpl_window_closed)
 
     # 1st plot for cumulative spectrum
     axE = fig.add_subplot(gs[:-6, :])
     axE.set_ylabel('Cumulative counts', size='large')
     axE.set_xlim(0.0, Energies[NChannels - 1])
     plt.locator_params(axis='x', nbins=12)
     axE.grid(linestyle='dotted', which='both')
@@ -190,50 +236,69 @@
         0.7,
         0.75,
         '     ',
         transform=axE.transAxes,
         color=appColors.text2,
         alpha=0.7,
     )
+
+    # textbox and background
+    rect = patches.Rectangle((0.65, 0.73), 0.34, 0.26, angle=0.0, color='white', alpha=0.7, transform=axE.transAxes)
+    axE.add_patch(rect)
+
     text_diff_statistics = axEdiff.text(
         0.75,
         0.55,
         '     ',
         transform=axEdiff.transAxes,
-        color=appColors.text2,
+        color=appColors.text3,
         alpha=0.7,
     )
+
     # plot in non-blocking mode
     plt.ion()  # interactive mode, non-blocking
     plt.show()
 
     # ---
     # initialize and start read-out loop
     # ---
     print(f'### Collecting data for {run_time:d} s')
+    print('  type  <ctrl>+c to stop  ', end='\r')
+
     toggle = ['  \\ ', '  | ', '  / ', '  - ']
     itoggle = 0
     icount = -1
     total_time = 0
+    previous_counts = counts0.copy()
+    if restart_accumulation:
+        counts = np.zeros(len(counts0))
+        T0 = t_start
+    else:
+        counts = counts0.copy()
+        T0 = t_start - duration_s  # start time of accumulation
+
+    countsum0 = np.sum(counts)
+
     time.sleep(dt_wait - time.time() + t_start)
     try:
-        while total_time < run_time:
+        while total_time < run_time and mpl_active:
             _t = time.time()  # start time of loop
             icount += 1
             # dt = _t - _t0  # last time interval
             _t0 = _t
             total_time = int(10 * (_t - T0)) / 10  # active time rounded to 0.1s
             spectrum = rc.spectrum()
-            counts = np.asarray(spectrum.counts)
-            if not any(counts):
+            actual_counts = np.asarray(spectrum.counts)
+            if not any(actual_counts):
                 time.sleep(dt_wait)
                 print(' accumulation time:', total_time, ' s', ' !!! waiting for data', end='\r')
                 continue
-            counts_diff = counts - counts0
-            counts0[:] = counts
+            counts_diff = actual_counts - previous_counts
+            previous_counts[:] = actual_counts
+            counts += counts_diff
             # some statistics
             countsum = np.sum(counts)
             rate = (countsum - countsum0) / dt_wait
             rate_history[icount % NHistory] = rate
             rate_av = countsum / total_time
             hrates[icount % num_history_points] = rate
             depE = np.sum(counts_diff * Energies)  # in keV
@@ -264,23 +329,24 @@
                 + f'dose: {total_dose:.3g} µGy  \n'
                 + f'av. doserate: {av_doserate:.3g} µGy/h'
             )
             text_diff_statistics.set_text(f'rate: {rate:.3g} Hz\n' + f'dose: {doserate:.3g} µGy/h')
             # draw data
             fig.canvas.draw_idle()
             # update status text in terminal
-            print(
-                toggle[itoggle],
-                ' active:',
-                total_time,
-                's  ',
-                f'counts: {countsum:.5g}, rate: {rate:.3g} Hz, dose: {doserate:.3g} µGy/h',
-                '    (<ctrl>+c to stop)      ',
-                end='\r',
-            )
+            if not quiet:
+                print(
+                    toggle[itoggle],
+                    ' active:',
+                    total_time,
+                    's  ',
+                    f'counts: {countsum:.5g}, rate: {rate:.3g} Hz, dose: {doserate:.3g} µGy/h',
+                    '    (<ctrl>+c to stop)      ',
+                    end='\r',
+                )
             itoggle = itoggle + 1 if itoggle < 3 else 0
             # wait for corrected wait interval)
             fig.canvas.start_event_loop(max(0.9 * dt_wait, dt_wait * (icount + 2) - (time.time() - t_start)))
         # --> end while true
 
         print('\n' + sys.argv[0] + ': exit after ', total_time, ' s of data accumulation ...')
 
@@ -298,15 +364,16 @@
                 else np.concatenate((rate_history[icount + 1 :], rate_history[: icount + 1])).tolist(),
                 ecal=[a0, a1, a2],
                 spectrum=counts.tolist(),
             )
             with open(filename, 'w') as f:
                 f.write(yaml.dump(d, default_flow_style=None))
 
-        input('    type <ret> to close down graphics window  --> ')
+        if mpl_active:
+            input('    type <ret> to close down graphics window  --> ')
 
         ### get dose info from device
         #  for v in rc.data_buf():
         #    print(v.dt.isoformat(), v)
 
 
 if __name__ == '__main__':
```

### Comparing `radiacode-0.3.2/radiacode-examples/webserver.html` & `radiacode-0.3.3/radiacode-examples/webserver.html`

 * *Files identical despite different names*

### Comparing `radiacode-0.3.2/radiacode-examples/webserver.py` & `radiacode-0.3.3/radiacode-examples/webserver.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.3.2/PKG-INFO` & `radiacode-0.3.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radiacode
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library for RadiaCode-101
 Home-page: https://github.com/cdump/radiacode
 License: MIT
 Author: Maxim Andreev
 Author-email: andreevmaxim@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: examples
 Requires-Dist: aiohttp (>=3.9,<4.0) ; extra == "examples"
-Requires-Dist: bluepy (>=1.3,<2.0)
+Requires-Dist: bluepy (>=1.3,<2.0) ; sys_platform != "darwin"
 Requires-Dist: matplotlib (>=3.7,<4.0) ; extra == "examples"
 Requires-Dist: numpy (>=1.26,<2.0) ; extra == "examples"
 Requires-Dist: prometheus-client (>=0.19,<0.20) ; extra == "examples"
 Requires-Dist: pyusb (>=1.2,<2.0)
 Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "examples"
 Project-URL: Repository, https://github.com/cdump/radiacode
 Description-Content-Type: text/markdown
@@ -60,7 +60,11 @@
 - clone this repository
 - install and run:
 ```
 $ poetry install
 $ poetry run python3 radiacode-examples/basic.py --bluetooth-mac 52:43:01:02:03:04 # or without --bluetooth-mac for USB connection
 ```
 
+## MacOS
+The library used to communicate over Bluetooh (```bluepy```) is [not supported](https://github.com/IanHarvey/bluepy/issues/44) on MacOS. Only the USB connection is available on Apple devices. A ```USB Serial Number```, obtainable from the ```Device Info``` menu on the device itself, can be specified if more than one Radiacode is connected via USB at the same time.
+
+Make sure ```libusb``` is installed on your system, if you use ```Brew``` you can run: ```brew install libusb```
```

