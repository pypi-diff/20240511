# Comparing `tmp/pyrotel-0.9.2.tar.gz` & `tmp/pyrotel-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrotel-0.9.2.tar", last modified: Fri Mar 22 22:40:46 2024, max compression
+gzip compressed data, was "pyrotel-0.9.3.tar", last modified: Sat May 11 17:49:06 2024, max compression
```

## Comparing `pyrotel-0.9.2.tar` & `pyrotel-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 22:40:46.611250 pyrotel-0.9.2/
--rw-rw-rw-   0        0        0     1071 2024-02-01 09:40:20.000000 pyrotel-0.9.2/LICENSE
--rw-rw-rw-   0        0        0     1452 2024-03-22 22:40:46.572241 pyrotel-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0      605 2024-03-22 22:15:32.000000 pyrotel-0.9.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 22:40:46.346183 pyrotel-0.9.2/pyrotel/
--rw-rw-rw-   0        0        0       55 2024-03-22 22:35:04.000000 pyrotel-0.9.2/pyrotel/__init__.py
--rw-rw-rw-   0        0        0    28475 2024-03-22 22:27:49.000000 pyrotel-0.9.2/pyrotel/client.py
--rw-rw-rw-   0        0        0     3092 2024-02-29 09:45:28.000000 pyrotel-0.9.2/pyrotel/util.py
-drwxrwxrwx   0        0        0        0 2024-03-22 22:40:46.543233 pyrotel-0.9.2/pyrotel.egg-info/
--rw-rw-rw-   0        0        0     1452 2024-03-22 22:40:45.000000 pyrotel-0.9.2/pyrotel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-03-22 22:40:45.000000 pyrotel-0.9.2/pyrotel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 22:40:45.000000 pyrotel-0.9.2/pyrotel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-03-22 22:40:45.000000 pyrotel-0.9.2/pyrotel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-22 22:40:45.000000 pyrotel-0.9.2/pyrotel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 22:40:46.621253 pyrotel-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1007 2024-03-22 22:14:09.000000 pyrotel-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:49:06.200256 pyrotel-0.9.3/
+-rw-rw-rw-   0        0        0     1090 2024-05-11 17:46:39.000000 pyrotel-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0     1387 2024-05-11 17:49:06.200256 pyrotel-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2024-05-11 17:47:31.000000 pyrotel-0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 17:49:06.022193 pyrotel-0.9.3/pyrotel/
+-rw-rw-rw-   0        0        0      354 2024-05-11 17:16:30.000000 pyrotel-0.9.3/pyrotel/__init__.py
+-rw-rw-rw-   0        0        0    28618 2024-04-20 21:47:29.000000 pyrotel-0.9.3/pyrotel/client.py
+-rw-rw-rw-   0        0        0     3595 2024-04-21 18:52:58.000000 pyrotel-0.9.3/pyrotel/util.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:49:06.180054 pyrotel-0.9.3/pyrotel.egg-info/
+-rw-rw-rw-   0        0        0     1387 2024-05-11 17:49:05.000000 pyrotel-0.9.3/pyrotel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-05-11 17:49:05.000000 pyrotel-0.9.3/pyrotel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 17:49:05.000000 pyrotel-0.9.3/pyrotel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-11 17:49:05.000000 pyrotel-0.9.3/pyrotel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-11 17:49:05.000000 pyrotel-0.9.3/pyrotel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 17:49:06.200256 pyrotel-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2024-05-11 17:47:36.000000 pyrotel-0.9.3/setup.py
```

### Comparing `pyrotel-0.9.2/PKG-INFO` & `pyrotel-0.9.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2070 7972  : 2.1..Name: pyr
 00000020: 6f74 656c 0d0a 5665 7273 696f 6e3a 2030  otel..Version: 0
-00000030: 2e39 2e32 0d0a 5375 6d6d 6172 793a 2070  .9.2..Summary: p
+00000030: 2e39 2e33 0d0a 5375 6d6d 6172 793a 2070  .9.3..Summary: p
 00000040: 7972 6f74 656c 2069 7320 6120 6c69 6272  yrotel is a libr
 00000050: 6172 7920 666f 7220 7465 6c65 6772 616d  ary for telegram
 00000060: 2062 6f74 732e 0d0a 486f 6d65 2d70 6167   bots...Home-pag
 00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000080: 622e 636f 6d2f 4572 6661 6e2d 4261 6661  b.com/Erfan-Bafa
 00000090: 6e64 6568 2f70 7972 6f74 656c 0d0a 4175  ndeh/pyrotel..Au
 000000a0: 7468 6f72 3a20 4572 6661 6e20 4261 6661  thor: Erfan Bafa
@@ -46,46 +46,42 @@
 000002d0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
 000002e0: 726b 646f 776e 0d0a 4c69 6365 6e73 652d  rkdown..License-
 000002f0: 4669 6c65 3a20 4c49 4345 4e53 450d 0a52  File: LICENSE..R
 00000300: 6571 7569 7265 732d 4469 7374 3a20 7265  equires-Dist: re
 00000310: 7175 6573 7473 0d0a 5265 7175 6972 6573  quests..Requires
 00000320: 2d44 6973 743a 2063 6f6c 6f72 616d 610d  -Dist: colorama.
 00000330: 0a0d 0a23 2320 7079 726f 7465 6c20 302e  ...## pyrotel 0.
-00000340: 392e 3276 0d0a 0d0a 3c68 3320 616c 6967  9.2v....<h3 alig
+00000340: 392e 3376 0d0a 0d0a 3c68 3320 616c 6967  9.3v....<h3 alig
 00000350: 6e3d 2263 656e 7465 7222 3e70 7972 6f74  n="center">pyrot
 00000360: 656c 2069 7320 6120 6c69 6272 6172 7920  el is a library 
 00000370: 666f 7220 7465 6c65 6772 616d 2062 6f74  for telegram bot
 00000380: 732e 3c2f 6833 3e0d 0a0d 0a3e 2023 2320  s.</h3>....> ## 
 00000390: 496e 7374 616c 6c20 616e 6420 5570 6461  Install and Upda
 000003a0: 7465 3a0d 0a60 6060 7079 7468 6f6e 0d0a  te:..```python..
 000003b0: 7069 7020 696e 7374 616c 6c20 7079 726f  pip install pyro
 000003c0: 7465 6c0d 0a60 6060 0d0a 0d0a 3e20 2323  tel..```....> ##
 000003d0: 2053 5441 5254 3a0d 0a60 6060 7079 7468   START:..```pyth
 000003e0: 6f6e 0d0a 6672 6f6d 2070 7972 6f74 656c  on..from pyrotel
 000003f0: 2069 6d70 6f72 7420 436c 6965 6e74 0d0a   import Client..
-00000400: 696d 706f 7274 2061 7379 6e63 696f 0d0a  import asyncio..
-00000410: 0d0a 6170 7020 3d20 436c 6965 6e74 2822  ..app = Client("
-00000420: 4150 495f 544f 4b45 4e22 290d 0a0d 0a61  API_TOKEN")....a
-00000430: 7379 6e63 2064 6566 2062 6f74 2829 3a0d  sync def bot():.
-00000440: 0a09 666f 7220 6d73 6720 696e 2061 7070  ..for msg in app
-00000450: 2e6f 6e5f 6d65 7373 6167 6528 293a 0d0a  .on_message():..
-00000460: 0909 6966 206d 7367 2e74 6578 7420 3d3d  ..if msg.text ==
-00000470: 2022 2f73 7461 7274 223a 0d0a 0909 0961   "/start":.....a
-00000480: 7070 2e73 656e 645f 6d65 7373 6167 6528  pp.send_message(
-00000490: 6d73 672e 6368 6174 5f69 642c 2022 6865  msg.chat_id, "he
-000004a0: 6c6c 6f20 6d79 2064 6561 722e 5c6e 7765  llo my dear.\nwe
-000004b0: 6c63 6f6d 6520 746f 206d 7920 626f 7420  lcome to my bot 
-000004c0: 3a29 222c 2072 6570 6c79 5f74 6f5f 6d65  :)", reply_to_me
-000004d0: 7373 6167 655f 6964 3d6d 7367 2e6d 6573  ssage_id=msg.mes
-000004e0: 7361 6765 5f69 6429 0d0a 0d0a 6966 205f  sage_id)....if _
-000004f0: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
-00000500: 696e 5f5f 223a 0d0a 0961 7379 6e63 696f  in__":...asyncio
-00000510: 2e72 756e 2862 6f74 2829 290d 0a60 6060  .run(bot())..```
-00000520: 0d0a 0d0a 3e20 2323 2053 6f63 6961 6c20  ....> ## Social 
-00000530: 4d65 6469 613a 0d0a 3c61 2068 7265 663d  Media:..<a href=
-00000540: 2268 7474 7073 3a2f 2f74 2e6d 652f 7065  "https://t.me/pe
-00000550: 7273 6961 6e5f 7079 223e 5445 4c45 4752  rsian_py">TELEGR
-00000560: 414d 3c2f 613e 3c62 723e 0d0a 3c61 2068  AM</a><br>..<a h
-00000570: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000580: 6875 622e 636f 6d2f 4572 6661 6e2d 4261  hub.com/Erfan-Ba
-00000590: 6661 6e64 6568 2f70 7972 6f74 656c 223e  fandeh/pyrotel">
-000005a0: 4749 5448 5542 3c2f 613e 0d0a            GITHUB</a>..
+00000400: 0d0a 6170 7020 3d20 436c 6965 6e74 2822  ..app = Client("
+00000410: 4150 495f 544f 4b45 4e22 290d 0a0d 0a61  API_TOKEN")....a
+00000420: 7379 6e63 2064 6566 2062 6f74 2829 3a0d  sync def bot():.
+00000430: 0a09 666f 7220 6d73 6720 696e 2061 7070  ..for msg in app
+00000440: 2e6f 6e5f 6d65 7373 6167 6528 293a 0d0a  .on_message():..
+00000450: 0909 6966 206d 7367 2e74 6578 7420 3d3d  ..if msg.text ==
+00000460: 2022 2f73 7461 7274 223a 0d0a 0909 0961   "/start":.....a
+00000470: 7070 2e73 656e 645f 6d65 7373 6167 6528  pp.send_message(
+00000480: 6d73 672e 6368 6174 5f69 642c 2022 6865  msg.chat_id, "he
+00000490: 6c6c 6f20 6d79 2064 6561 722e 5c6e 7765  llo my dear.\nwe
+000004a0: 6c63 6f6d 6520 746f 206d 7920 626f 7420  lcome to my bot 
+000004b0: 3a29 222c 2072 6570 6c79 5f74 6f5f 6d65  :)", reply_to_me
+000004c0: 7373 6167 655f 6964 3d6d 7367 2e6d 6573  ssage_id=msg.mes
+000004d0: 7361 6765 5f69 6429 0d0a 0d0a 6060 600d  sage_id)....```.
+000004e0: 0a0d 0a3e 2023 2320 536f 6369 616c 204d  ...> ## Social M
+000004f0: 6564 6961 3a0d 0a3c 6120 6872 6566 3d22  edia:..<a href="
+00000500: 6874 7470 733a 2f2f 742e 6d65 2f70 6572  https://t.me/per
+00000510: 7369 616e 5f70 7922 3e54 454c 4547 5241  sian_py">TELEGRA
+00000520: 4d3c 2f61 3e3c 6272 3e0d 0a3c 6120 6872  M</a><br>..<a hr
+00000530: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000540: 7562 2e63 6f6d 2f45 7266 616e 2d42 6166  ub.com/Erfan-Baf
+00000550: 616e 6465 682f 7079 726f 7465 6c22 3e47  andeh/pyrotel">G
+00000560: 4954 4855 423c 2f61 3e0d 0a              ITHUB</a>..
```

### Comparing `pyrotel-0.9.2/README.md` & `pyrotel-0.9.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-00000000: 2323 2070 7972 6f74 656c 2030 2e39 2e32  ## pyrotel 0.9.2
-00000010: 760a 0a3c 6833 2061 6c69 676e 3d22 6365  v..<h3 align="ce
-00000020: 6e74 6572 223e 7079 726f 7465 6c20 6973  nter">pyrotel is
-00000030: 2061 206c 6962 7261 7279 2066 6f72 2074   a library for t
-00000040: 656c 6567 7261 6d20 626f 7473 2e3c 2f68  elegram bots.</h
-00000050: 333e 0a0a 3e20 2323 2049 6e73 7461 6c6c  3>..> ## Install
-00000060: 2061 6e64 2055 7064 6174 653a 0a60 6060   and Update:.```
-00000070: 7079 7468 6f6e 0a70 6970 2069 6e73 7461  python.pip insta
-00000080: 6c6c 2070 7972 6f74 656c 0a60 6060 0a0a  ll pyrotel.```..
-00000090: 3e20 2323 2053 5441 5254 3a0a 6060 6070  > ## START:.```p
-000000a0: 7974 686f 6e0a 6672 6f6d 2070 7972 6f74  ython.from pyrot
-000000b0: 656c 2069 6d70 6f72 7420 436c 6965 6e74  el import Client
-000000c0: 0a69 6d70 6f72 7420 6173 796e 6369 6f0a  .import asyncio.
-000000d0: 0a61 7070 203d 2043 6c69 656e 7428 2241  .app = Client("A
-000000e0: 5049 5f54 4f4b 454e 2229 0a0a 6173 796e  PI_TOKEN")..asyn
-000000f0: 6320 6465 6620 626f 7428 293a 0a09 666f  c def bot():..fo
-00000100: 7220 6d73 6720 696e 2061 7070 2e6f 6e5f  r msg in app.on_
-00000110: 6d65 7373 6167 6528 293a 0a09 0969 6620  message():...if 
-00000120: 6d73 672e 7465 7874 203d 3d20 222f 7374  msg.text == "/st
-00000130: 6172 7422 3a0a 0909 0961 7070 2e73 656e  art":....app.sen
-00000140: 645f 6d65 7373 6167 6528 6d73 672e 6368  d_message(msg.ch
-00000150: 6174 5f69 642c 2022 6865 6c6c 6f20 6d79  at_id, "hello my
-00000160: 2064 6561 722e 5c6e 7765 6c63 6f6d 6520   dear.\nwelcome 
-00000170: 746f 206d 7920 626f 7420 3a29 222c 2072  to my bot :)", r
-00000180: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
-00000190: 6964 3d6d 7367 2e6d 6573 7361 6765 5f69  id=msg.message_i
-000001a0: 6429 0a0a 6966 205f 5f6e 616d 655f 5f20  d)..if __name__ 
-000001b0: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0a09  == "__main__":..
-000001c0: 6173 796e 6369 6f2e 7275 6e28 626f 7428  asyncio.run(bot(
-000001d0: 2929 0a60 6060 0a0a 3e20 2323 2053 6f63  )).```..> ## Soc
-000001e0: 6961 6c20 4d65 6469 613a 0a3c 6120 6872  ial Media:.<a hr
-000001f0: 6566 3d22 6874 7470 733a 2f2f 742e 6d65  ef="https://t.me
-00000200: 2f70 6572 7369 616e 5f70 7922 3e54 454c  /persian_py">TEL
-00000210: 4547 5241 4d3c 2f61 3e3c 6272 3e0a 3c61  EGRAM</a><br>.<a
-00000220: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00000230: 6974 6875 622e 636f 6d2f 4572 6661 6e2d  ithub.com/Erfan-
-00000240: 4261 6661 6e64 6568 2f70 7972 6f74 656c  Bafandeh/pyrotel
-00000250: 223e 4749 5448 5542 3c2f 613e 0a         ">GITHUB</a>.
+00000000: 2323 2070 7972 6f74 656c 2030 2e39 2e33  ## pyrotel 0.9.3
+00000010: 760d 0a0d 0a3c 6833 2061 6c69 676e 3d22  v....<h3 align="
+00000020: 6365 6e74 6572 223e 7079 726f 7465 6c20  center">pyrotel 
+00000030: 6973 2061 206c 6962 7261 7279 2066 6f72  is a library for
+00000040: 2074 656c 6567 7261 6d20 626f 7473 2e3c   telegram bots.<
+00000050: 2f68 333e 0d0a 0d0a 3e20 2323 2049 6e73  /h3>....> ## Ins
+00000060: 7461 6c6c 2061 6e64 2055 7064 6174 653a  tall and Update:
+00000070: 0d0a 6060 6070 7974 686f 6e0d 0a70 6970  ..```python..pip
+00000080: 2069 6e73 7461 6c6c 2070 7972 6f74 656c   install pyrotel
+00000090: 0d0a 6060 600d 0a0d 0a3e 2023 2320 5354  ..```....> ## ST
+000000a0: 4152 543a 0d0a 6060 6070 7974 686f 6e0d  ART:..```python.
+000000b0: 0a66 726f 6d20 7079 726f 7465 6c20 696d  .from pyrotel im
+000000c0: 706f 7274 2043 6c69 656e 740d 0a0d 0a61  port Client....a
+000000d0: 7070 203d 2043 6c69 656e 7428 2241 5049  pp = Client("API
+000000e0: 5f54 4f4b 454e 2229 0d0a 0d0a 6173 796e  _TOKEN")....asyn
+000000f0: 6320 6465 6620 626f 7428 293a 0d0a 0966  c def bot():...f
+00000100: 6f72 206d 7367 2069 6e20 6170 702e 6f6e  or msg in app.on
+00000110: 5f6d 6573 7361 6765 2829 3a0d 0a09 0969  _message():....i
+00000120: 6620 6d73 672e 7465 7874 203d 3d20 222f  f msg.text == "/
+00000130: 7374 6172 7422 3a0d 0a09 0909 6170 702e  start":.....app.
+00000140: 7365 6e64 5f6d 6573 7361 6765 286d 7367  send_message(msg
+00000150: 2e63 6861 745f 6964 2c20 2268 656c 6c6f  .chat_id, "hello
+00000160: 206d 7920 6465 6172 2e5c 6e77 656c 636f   my dear.\nwelco
+00000170: 6d65 2074 6f20 6d79 2062 6f74 203a 2922  me to my bot :)"
+00000180: 2c20 7265 706c 795f 746f 5f6d 6573 7361  , reply_to_messa
+00000190: 6765 5f69 643d 6d73 672e 6d65 7373 6167  ge_id=msg.messag
+000001a0: 655f 6964 290d 0a0d 0a60 6060 0d0a 0d0a  e_id)....```....
+000001b0: 3e20 2323 2053 6f63 6961 6c20 4d65 6469  > ## Social Medi
+000001c0: 613a 0d0a 3c61 2068 7265 663d 2268 7474  a:..<a href="htt
+000001d0: 7073 3a2f 2f74 2e6d 652f 7065 7273 6961  ps://t.me/persia
+000001e0: 6e5f 7079 223e 5445 4c45 4752 414d 3c2f  n_py">TELEGRAM</
+000001f0: 613e 3c62 723e 0d0a 3c61 2068 7265 663d  a><br>..<a href=
+00000200: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000210: 636f 6d2f 4572 6661 6e2d 4261 6661 6e64  com/Erfan-Bafand
+00000220: 6568 2f70 7972 6f74 656c 223e 4749 5448  eh/pyrotel">GITH
+00000230: 5542 3c2f 613e 0d0a                      UB</a>..
```

### Comparing `pyrotel-0.9.2/pyrotel/client.py` & `pyrotel-0.9.3/pyrotel/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 from .util import message
 from colorama import Fore
 import requests
 from subprocess import getoutput as cmd
 
 # dev by Erfan-Bafandeh - persian py
 
-lib_name = "pyrotel"
-
-print("Loading . .")
-
-version = requests.get(f"https://pypi.org/pypi/{lib_name}/json").json()["info"]["version"]
-
-libs = cmd("pip freeze").split("\n")
-
-for i in range(len(libs)):
-    info = libs[i].split("==")
-    if info[0] == lib_name:
-        last_version = info[1]
-if last_version != version:
-    print(f"""
+class Client:
+    def __init__(self, token: str, timeout: float = 10, debug_mode: bool = True, version_check: bool = True, welcome_message: bool = True) -> None:
+        self.token = token
+        self.timeout = timeout
+        self.debug_mode = debug_mode
+        lib_name = "pyrotel"
+        if version_check:
+            print("Loading . .")
+
+            version = requests.get(f"https://pypi.org/pypi/{lib_name}/json").json()["info"]["version"]
+
+            libs = cmd("pip freeze").split("\n")
+
+            for i in range(len(libs)):
+                info = libs[i].split("==")
+                if info[0] == lib_name:
+                    last_version = info[1]
+            if last_version != version:
+                print(f"""
 you have a new update !
 
 lib name: {Fore.LIGHTCYAN_EX}{lib_name}{Fore.RESET}
 version: {Fore.LIGHTCYAN_EX}{last_version}{Fore.RESET}
 new vesion: {Fore.LIGHTCYAN_EX}{version}{Fore.RESET}
-""")
-
-print(f"""
+            """)
+            if welcome_message:
+                print(f"""
 Welcome to {lib_name} {Fore.LIGHTCYAN_EX}{version}{Fore.RESET} library.
 
-dev by {Fore.LIGHTYELLOW_EX}Erfan Bafandeh.{Fore.RESET}
-""")
-
-class Client:
-
-    def __init__(self, token: str, timeout: float = 10, debug_mode: bool = True) -> None:
-        self.token = token
-        self.timeout = timeout
-        self.debug_mode = debug_mode
+Devloped by {Fore.LIGHTYELLOW_EX}Erfan Bafandeh.{Fore.RESET}
+            """)
 
     def request(self, method: str, json: dict = {}, files: dict = {}) -> dict:
         url = f"https://api.telegram.org/bot{self.token}/{method}"
         if json != {} and files != {}:
             response = requests.post(url=url, data=json, files=files).json()
         elif json != {}:
             response = requests.post(url=url, data=json).json()
@@ -58,25 +56,14 @@
 
 description: {response["description"]}
 note: if you can't debug this error, you can send a message to pyrotel lib support in telegram massenger.
 support: {Fore.LIGHTCYAN_EX}t.me/ppy_sup{Fore.RESET}""")
             return response
 
     def on_message(self):
-        '''Use this method to receive updates
-        Example:
-            from balepy import Client
-
-            client = Client('token', timeout=10)
-            def main():
-                for update in client.on_message():
-                    print(update.text)
-
-            main()
-        '''
         payload: dict = {
             'offset': -1, 'limit': 100
         }
         while True:
             update = self.request('getupdates', json=payload)
             payload['offset'] = 1
             if (update != None) and (update['ok']) and (update['result'] != []):
@@ -84,15 +71,21 @@
 
         payload['offset'] = update['result'][len(update['result'])-1]['update_id'] + 1
         payload['limit'] = 1
         while True:
             responce = self.request('getupdates', json=payload)
             if responce != None and responce['result'] != []:
                 payload['offset'] += 1
-                yield message(responce['result'][0])
+                yield message(responce['result'][0], self.token)
+
+    def start_handler(self, func):
+        async def wrapper():
+            for msg in self.on_message():
+                await func(msg)
+        return wrapper
 
     async def get_updates(self) -> dict:
         return self.request("getupdates")
 
     async def set_webhook(self, url: str) -> dict:
         payload = {
             "url":url
```

### Comparing `pyrotel-0.9.2/pyrotel/util.py` & `pyrotel-0.9.3/pyrotel/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# dev by amirali irvany
+from . import client
+
 class message:
 
-    def __init__(self, data: dict) -> str:
+    def __init__(self, data: dict, token: str) -> str:
         self.data: dict = data
+        self.token: str = token
 
     @property
     def message(self):
         if 'callback_query' in self.data:
             return self.data['callback_query']['message']
         elif 'message' in self.data:
             return self.data['message']
@@ -108,8 +110,15 @@
                 return 'document'
         elif 'audio' in self.message:
             if 'caption' in self.message:
                 return 'audioCaption'
             else:
                 return 'audio'
         else:
-            return None
+            return None
+    async def reply(self, 
+                    text: str, 
+                    disable_notification: bool = False, 
+                    reply_markup: dict = "", 
+                    ):
+        app = client.Client(self.token, version_check=False, welcome_message=False)
+        await app.send_message(self.message['chat']['id'], text, reply_to_message_id=self.message['message_id'], disable_notification=disable_notification, reply_markup=reply_markup)
```

### Comparing `pyrotel-0.9.2/pyrotel.egg-info/PKG-INFO` & `pyrotel-0.9.3/pyrotel.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2070 7972  : 2.1..Name: pyr
 00000020: 6f74 656c 0d0a 5665 7273 696f 6e3a 2030  otel..Version: 0
-00000030: 2e39 2e32 0d0a 5375 6d6d 6172 793a 2070  .9.2..Summary: p
+00000030: 2e39 2e33 0d0a 5375 6d6d 6172 793a 2070  .9.3..Summary: p
 00000040: 7972 6f74 656c 2069 7320 6120 6c69 6272  yrotel is a libr
 00000050: 6172 7920 666f 7220 7465 6c65 6772 616d  ary for telegram
 00000060: 2062 6f74 732e 0d0a 486f 6d65 2d70 6167   bots...Home-pag
 00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000080: 622e 636f 6d2f 4572 6661 6e2d 4261 6661  b.com/Erfan-Bafa
 00000090: 6e64 6568 2f70 7972 6f74 656c 0d0a 4175  ndeh/pyrotel..Au
 000000a0: 7468 6f72 3a20 4572 6661 6e20 4261 6661  thor: Erfan Bafa
@@ -46,46 +46,42 @@
 000002d0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
 000002e0: 726b 646f 776e 0d0a 4c69 6365 6e73 652d  rkdown..License-
 000002f0: 4669 6c65 3a20 4c49 4345 4e53 450d 0a52  File: LICENSE..R
 00000300: 6571 7569 7265 732d 4469 7374 3a20 7265  equires-Dist: re
 00000310: 7175 6573 7473 0d0a 5265 7175 6972 6573  quests..Requires
 00000320: 2d44 6973 743a 2063 6f6c 6f72 616d 610d  -Dist: colorama.
 00000330: 0a0d 0a23 2320 7079 726f 7465 6c20 302e  ...## pyrotel 0.
-00000340: 392e 3276 0d0a 0d0a 3c68 3320 616c 6967  9.2v....<h3 alig
+00000340: 392e 3376 0d0a 0d0a 3c68 3320 616c 6967  9.3v....<h3 alig
 00000350: 6e3d 2263 656e 7465 7222 3e70 7972 6f74  n="center">pyrot
 00000360: 656c 2069 7320 6120 6c69 6272 6172 7920  el is a library 
 00000370: 666f 7220 7465 6c65 6772 616d 2062 6f74  for telegram bot
 00000380: 732e 3c2f 6833 3e0d 0a0d 0a3e 2023 2320  s.</h3>....> ## 
 00000390: 496e 7374 616c 6c20 616e 6420 5570 6461  Install and Upda
 000003a0: 7465 3a0d 0a60 6060 7079 7468 6f6e 0d0a  te:..```python..
 000003b0: 7069 7020 696e 7374 616c 6c20 7079 726f  pip install pyro
 000003c0: 7465 6c0d 0a60 6060 0d0a 0d0a 3e20 2323  tel..```....> ##
 000003d0: 2053 5441 5254 3a0d 0a60 6060 7079 7468   START:..```pyth
 000003e0: 6f6e 0d0a 6672 6f6d 2070 7972 6f74 656c  on..from pyrotel
 000003f0: 2069 6d70 6f72 7420 436c 6965 6e74 0d0a   import Client..
-00000400: 696d 706f 7274 2061 7379 6e63 696f 0d0a  import asyncio..
-00000410: 0d0a 6170 7020 3d20 436c 6965 6e74 2822  ..app = Client("
-00000420: 4150 495f 544f 4b45 4e22 290d 0a0d 0a61  API_TOKEN")....a
-00000430: 7379 6e63 2064 6566 2062 6f74 2829 3a0d  sync def bot():.
-00000440: 0a09 666f 7220 6d73 6720 696e 2061 7070  ..for msg in app
-00000450: 2e6f 6e5f 6d65 7373 6167 6528 293a 0d0a  .on_message():..
-00000460: 0909 6966 206d 7367 2e74 6578 7420 3d3d  ..if msg.text ==
-00000470: 2022 2f73 7461 7274 223a 0d0a 0909 0961   "/start":.....a
-00000480: 7070 2e73 656e 645f 6d65 7373 6167 6528  pp.send_message(
-00000490: 6d73 672e 6368 6174 5f69 642c 2022 6865  msg.chat_id, "he
-000004a0: 6c6c 6f20 6d79 2064 6561 722e 5c6e 7765  llo my dear.\nwe
-000004b0: 6c63 6f6d 6520 746f 206d 7920 626f 7420  lcome to my bot 
-000004c0: 3a29 222c 2072 6570 6c79 5f74 6f5f 6d65  :)", reply_to_me
-000004d0: 7373 6167 655f 6964 3d6d 7367 2e6d 6573  ssage_id=msg.mes
-000004e0: 7361 6765 5f69 6429 0d0a 0d0a 6966 205f  sage_id)....if _
-000004f0: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
-00000500: 696e 5f5f 223a 0d0a 0961 7379 6e63 696f  in__":...asyncio
-00000510: 2e72 756e 2862 6f74 2829 290d 0a60 6060  .run(bot())..```
-00000520: 0d0a 0d0a 3e20 2323 2053 6f63 6961 6c20  ....> ## Social 
-00000530: 4d65 6469 613a 0d0a 3c61 2068 7265 663d  Media:..<a href=
-00000540: 2268 7474 7073 3a2f 2f74 2e6d 652f 7065  "https://t.me/pe
-00000550: 7273 6961 6e5f 7079 223e 5445 4c45 4752  rsian_py">TELEGR
-00000560: 414d 3c2f 613e 3c62 723e 0d0a 3c61 2068  AM</a><br>..<a h
-00000570: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000580: 6875 622e 636f 6d2f 4572 6661 6e2d 4261  hub.com/Erfan-Ba
-00000590: 6661 6e64 6568 2f70 7972 6f74 656c 223e  fandeh/pyrotel">
-000005a0: 4749 5448 5542 3c2f 613e 0d0a            GITHUB</a>..
+00000400: 0d0a 6170 7020 3d20 436c 6965 6e74 2822  ..app = Client("
+00000410: 4150 495f 544f 4b45 4e22 290d 0a0d 0a61  API_TOKEN")....a
+00000420: 7379 6e63 2064 6566 2062 6f74 2829 3a0d  sync def bot():.
+00000430: 0a09 666f 7220 6d73 6720 696e 2061 7070  ..for msg in app
+00000440: 2e6f 6e5f 6d65 7373 6167 6528 293a 0d0a  .on_message():..
+00000450: 0909 6966 206d 7367 2e74 6578 7420 3d3d  ..if msg.text ==
+00000460: 2022 2f73 7461 7274 223a 0d0a 0909 0961   "/start":.....a
+00000470: 7070 2e73 656e 645f 6d65 7373 6167 6528  pp.send_message(
+00000480: 6d73 672e 6368 6174 5f69 642c 2022 6865  msg.chat_id, "he
+00000490: 6c6c 6f20 6d79 2064 6561 722e 5c6e 7765  llo my dear.\nwe
+000004a0: 6c63 6f6d 6520 746f 206d 7920 626f 7420  lcome to my bot 
+000004b0: 3a29 222c 2072 6570 6c79 5f74 6f5f 6d65  :)", reply_to_me
+000004c0: 7373 6167 655f 6964 3d6d 7367 2e6d 6573  ssage_id=msg.mes
+000004d0: 7361 6765 5f69 6429 0d0a 0d0a 6060 600d  sage_id)....```.
+000004e0: 0a0d 0a3e 2023 2320 536f 6369 616c 204d  ...> ## Social M
+000004f0: 6564 6961 3a0d 0a3c 6120 6872 6566 3d22  edia:..<a href="
+00000500: 6874 7470 733a 2f2f 742e 6d65 2f70 6572  https://t.me/per
+00000510: 7369 616e 5f70 7922 3e54 454c 4547 5241  sian_py">TELEGRA
+00000520: 4d3c 2f61 3e3c 6272 3e0d 0a3c 6120 6872  M</a><br>..<a hr
+00000530: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000540: 7562 2e63 6f6d 2f45 7266 616e 2d42 6166  ub.com/Erfan-Baf
+00000550: 616e 6465 682f 7079 726f 7465 6c22 3e47  andeh/pyrotel">G
+00000560: 4954 4855 423c 2f61 3e0d 0a              ITHUB</a>..
```

### Comparing `pyrotel-0.9.2/setup.py` & `pyrotel-0.9.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup, find_packages
-
-setup(
-    name = 'pyrotel',
-    version = '0.9.2',
-    author= 'Erfan Bafandeh',
-    author_email = 'user.enbh@gmail.com',
-    description = 'pyrotel is a library for telegram bots.',
-    keywords = ['Bot', 'Robot', 'pyrotel', 'telegram', 'telegrambot'],
-    long_description = open("README.md", encoding="utf-8").read(),
-    python_requires="~=3.6",
-    long_description_content_type = 'text/markdown',
-    url = 'https://github.com/Erfan-Bafandeh/pyrotel',
-    packages = find_packages(),
-    install_requires = ["requests", "colorama"],
-    classifiers = [
-    	"Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
-        "License :: OSI Approved :: MIT License",
-    ]
-)
+from setuptools import setup, find_packages
+
+setup(
+    name = 'pyrotel',
+    version = '0.9.3',
+    author= 'Erfan Bafandeh',
+    author_email = 'user.enbh@gmail.com',
+    description = 'pyrotel is a library for telegram bots.',
+    keywords = ['Bot', 'Robot', 'pyrotel', 'telegram', 'telegrambot'],
+    long_description = open("README.md", encoding="utf-8").read(),
+    python_requires="~=3.6",
+    long_description_content_type = 'text/markdown',
+    url = 'https://github.com/Erfan-Bafandeh/pyrotel',
+    packages = find_packages(),
+    install_requires = ["requests", "colorama"],
+    classifiers = [
+    	"Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "License :: OSI Approved :: MIT License",
+    ]
+)
```

