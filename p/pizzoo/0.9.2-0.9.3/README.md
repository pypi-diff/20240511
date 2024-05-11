# Comparing `tmp/pizzoo-0.9.2.tar.gz` & `tmp/pizzoo-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizzoo-0.9.2.tar", last modified: Sat May 11 00:52:17 2024, max compression
+gzip compressed data, was "pizzoo-0.9.3.tar", last modified: Sat May 11 00:57:45 2024, max compression
```

## Comparing `pizzoo-0.9.2.tar` & `pizzoo-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 00:52:17.280512 pizzoo-0.9.2/
--rw-rw-rw-   0        0        0     6712 2024-05-11 00:52:17.280512 pizzoo-0.9.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 00:52:17.276511 pizzoo-0.9.2/pizzoo/
--rw-rw-rw-   0        0        0    21798 2024-05-04 08:50:51.000000 pizzoo-0.9.2/pizzoo/__init__.py
--rw-rw-rw-   0        0        0     1444 2024-04-19 15:38:24.000000 pizzoo-0.9.2/pizzoo/_constants.py
--rw-rw-rw-   0        0        0    17046 2024-05-03 00:00:18.000000 pizzoo-0.9.2/pizzoo/_renderers.py
--rw-rw-rw-   0        0        0      705 2024-04-28 16:47:36.000000 pizzoo-0.9.2/pizzoo/_utils.py
--rw-rw-rw-   0        0        0    21871 2024-05-10 19:21:17.000000 pizzoo-0.9.2/pizzoo/game.py
-drwxrwxrwx   0        0        0        0 2024-05-11 00:52:17.279513 pizzoo-0.9.2/pizzoo.egg-info/
--rw-rw-rw-   0        0        0     6712 2024-05-11 00:52:17.000000 pizzoo-0.9.2/pizzoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-11 00:52:17.000000 pizzoo-0.9.2/pizzoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 00:52:17.000000 pizzoo-0.9.2/pizzoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-11 00:52:17.000000 pizzoo-0.9.2/pizzoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-11 00:52:17.000000 pizzoo-0.9.2/pizzoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 00:52:17.281511 pizzoo-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1172 2024-05-11 00:52:13.000000 pizzoo-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:57:45.172341 pizzoo-0.9.3/
+-rw-rw-rw-   0        0        0     6796 2024-05-11 00:57:45.172341 pizzoo-0.9.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 00:57:45.168334 pizzoo-0.9.3/pizzoo/
+-rw-rw-rw-   0        0        0    21798 2024-05-04 08:50:51.000000 pizzoo-0.9.3/pizzoo/__init__.py
+-rw-rw-rw-   0        0        0     1444 2024-04-19 15:38:24.000000 pizzoo-0.9.3/pizzoo/_constants.py
+-rw-rw-rw-   0        0        0    17046 2024-05-03 00:00:18.000000 pizzoo-0.9.3/pizzoo/_renderers.py
+-rw-rw-rw-   0        0        0      705 2024-04-28 16:47:36.000000 pizzoo-0.9.3/pizzoo/_utils.py
+-rw-rw-rw-   0        0        0    21871 2024-05-10 19:21:17.000000 pizzoo-0.9.3/pizzoo/game.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:57:45.171342 pizzoo-0.9.3/pizzoo.egg-info/
+-rw-rw-rw-   0        0        0     6796 2024-05-11 00:57:45.000000 pizzoo-0.9.3/pizzoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-11 00:57:45.000000 pizzoo-0.9.3/pizzoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 00:57:45.000000 pizzoo-0.9.3/pizzoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-11 00:57:45.000000 pizzoo-0.9.3/pizzoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-11 00:57:45.000000 pizzoo-0.9.3/pizzoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 00:57:45.172341 pizzoo-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1172 2024-05-11 00:57:40.000000 pizzoo-0.9.3/setup.py
```

### Comparing `pizzoo-0.9.2/PKG-INFO` & `pizzoo-0.9.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pizzoo
-Version: 0.9.2
+Version: 0.9.3
 Summary: Pizzoo is a library for rendering on pixel matrix screens, with direct support for the Divoom Pixoo64 device, and easy integration for any other one. It includes full animation buffer manipulation, a micro game engine, as well as XML/HTML like templates compilation.
 Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet
 License: MIT
 Keywords: pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED matrix,LED,raspberry,raspberry pi
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Requires-Dist: requests~=2.31.0
 Requires-Dist: Pillow~=10.0.0
 Requires-Dist: bdfparser~=2.2.0
 
 <p align="center">
-  <img src="https://github.com/pabletos/pizzoo/blob/main/docs/docs/assets/images/pizzoo-banner-nobg.png" alt="Pizzoo logo" width="450">
+  <img src="https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/images/pizzoo-banner-nobg.png" alt="Pizzoo logo" width="450">
 </p>
 <p>
 	<a 
 	href='https://ko-fi.com/B0B1PYK0W'
 	target='_blank'
 	rel="noreferrer"
 	>
@@ -51,46 +51,49 @@
 
 * **Game Development Toolkit**:
 	Tap into the possibilities of micro game development with our mini game engine. Design, develop, and deploy small-scale games that can be played right on your LED devices, perfect for creating engaging interactive experiences.
 
 ## Drawing on your device
 Frame manipulation is the core of the `pizzoo` library. Every time the library is created and the `render` method is called, the buffer is filled with a new frame we can use to draw on. Lets start by drawing three pixels on the screen and rendering:
 
-<img align="right" width="160" height="160" src="https://github.com/pabletos/pizzoo/blob/main/docs/docs/assets/images/qs-2.png">
-
 ```python
 pizzoo.cls()
 pizzoo.draw_circle((31, 31), 10, '#00ff00', filled=True) # Green circle, filled
 pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red rectangle, not filled
 pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue line
 pizzoo.draw_line((0, 31), (63, 31), (255, 255, 0)) # Yellow line, tuple rgb color format
 pizzoo.render()
 ```
 
+<p align="center">
+  <img width="320" height="320" src="https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/images/qs-2.png">
+</p>
+
 ## Creating animations
 Aside from simple gif drawing (That is also supported), custom animations can be created using frame-by-frame manipulation. As an example:
 
-<img align="right" width="160" height="160" src="https://github.com/pabletos/pizzoo/blob/main/docs/docs/assets/images/qs-5.gif">
-
 ```python
 '''
 This will create a simple diagonal moving circle
 '''
 for i in range(0, 54):
 	pizzoo.cls()
 	pizzoo.draw_circle((i + 4, i + 4), 2, '#00ff00', filled=True)
 	pizzoo.add_frame()
 pizzoo.render(frame_speed=100)
 ```
 
+<p align="center">
+	<img width="320" height="320" src="https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/images/qs-5.gif">
+</p>
+
+
 ## Rendering templates
 The most powerful feature of this library is the ability of render templates. Custom XML/HTML like templates can be made to create images, Pixoo64 dials and even reusable parts or components.
 
-<img align="right" width="160" height="160" src="https://github.com/pabletos/pizzoo/blob/main/docs/docs/assets/images/qs-6.png">
-
 ```python
 '''
 This template uses custom nodes for Pixoo64 for creating auto-updating dials, as date or time, so these are missing when 
 rendering on any other renderer
 '''
 pizzoo.load_font('amstrad', './files/amstrad_cpc_extended.bdf')
 pizzoo.render_template('''
@@ -112,14 +115,19 @@
 				</section>
 			</section>
 		</rectangle>
 	</pizzoo>
 ''')
 ```
 
+<p align="center">
+	<img width="320" height="320" src="https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/images/qs-6.png">
+</p>
+
+
 There's also have a dedicated section for this on our docs.
 
 ## Do you want to know more?
 [Here's](pizzoo.pablohuet.com) a dedicated page for documentation with a lot of examples so you can get quickly started.
 
 ## Contribute and/or donate
 This library was created and is maintained by a single developer, consider contributing with pull requests, new integrations, proposals or [simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pizzoo Version: 0.9.2 Summary: Pizzoo is a library
+Metadata-Version: 2.1 Name: pizzoo Version: 0.9.3 Summary: Pizzoo is a library
 for rendering on pixel matrix screens, with direct support for the Divoom
 Pixoo64 device, and easy integration for any other one. It includes full
 animation buffer manipulation, a micro game engine, as well as XML/HTML like
 templates compilation. Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet License: MIT Keywords:
 pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED
 matrix,LED,raspberry,raspberry pi Classifier: Development Status :: 4 - Beta
@@ -31,38 +31,41 @@
 to your specific project and hardware requirements. * **Game Development
 Toolkit**: Tap into the possibilities of micro game development with our mini
 game engine. Design, develop, and deploy small-scale games that can be played
 right on your LED devices, perfect for creating engaging interactive
 experiences. ## Drawing on your device Frame manipulation is the core of the
 `pizzoo` library. Every time the library is created and the `render` method is
 called, the buffer is filled with a new frame we can use to draw on. Lets start
-by drawing three pixels on the screen and rendering: [https://github.com/
-pabletos/pizzoo/blob/main/docs/docs/assets/images/qs-2.png]```python pizzoo.cls
-() pizzoo.draw_circle((31, 31), 10, '#00ff00', filled=True) # Green circle,
-filled pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red
+by drawing three pixels on the screen and rendering: ```python pizzoo.cls()
+pizzoo.draw_circle((31, 31), 10, '#00ff00', filled=True) # Green circle, filled
+pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red
 rectangle, not filled pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue
 line pizzoo.draw_line((0, 31), (63, 31), (255, 255, 0)) # Yellow line, tuple
-rgb color format pizzoo.render() ``` ## Creating animations Aside from simple
-gif drawing (That is also supported), custom animations can be created using
-frame-by-frame manipulation. As an example: [https://github.com/pabletos/
-pizzoo/blob/main/docs/docs/assets/images/qs-5.gif]```python ''' This will
-create a simple diagonal moving circle ''' for i in range(0, 54): pizzoo.cls()
-pizzoo.draw_circle((i + 4, i + 4), 2, '#00ff00', filled=True) pizzoo.add_frame
-() pizzoo.render(frame_speed=100) ``` ## Rendering templates The most powerful
-feature of this library is the ability of render templates. Custom XML/HTML
-like templates can be made to create images, Pixoo64 dials and even reusable
-parts or components. [https://github.com/pabletos/pizzoo/blob/main/docs/docs/
-assets/images/qs-6.png]```python ''' This template uses custom nodes for
-Pixoo64 for creating auto-updating dials, as date or time, so these are missing
-when rendering on any other renderer ''' pizzoo.load_font('amstrad', './files/
-amstrad_cpc_extended.bdf') pizzoo.render_template(''' - Long text wrapped Cool
-''') ``` There's also have a dedicated section for this on our docs. ## Do you
-want to know more? [Here's](pizzoo.pablohuet.com) a dedicated page for
-documentation with a lot of examples so you can get quickly started. ##
-Contribute and/or donate This library was created and is maintained by a single
-developer, consider contributing with pull requests, new integrations,
-proposals or [simply by doing a small donation on ko-fi](https://ko-fi.com/
-B0B1PYK0W). ## Special thanks This library exists thanks to other libraries
-that were an inspiration, specially the [Pixoo](https://github.com/
-SomethingWithComputers/pixoo) library by SomethingWithComputers and the
-[Matrix-Fonts](https://github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font
-collection by trip5.
+rgb color format pizzoo.render() ```
+   [https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/
+                               images/qs-2.png]
+## Creating animations Aside from simple gif drawing (That is also supported),
+custom animations can be created using frame-by-frame manipulation. As an
+example: ```python ''' This will create a simple diagonal moving circle ''' for
+i in range(0, 54): pizzoo.cls() pizzoo.draw_circle((i + 4, i + 4), 2,
+'#00ff00', filled=True) pizzoo.add_frame() pizzoo.render(frame_speed=100) ```
+   [https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/
+                               images/qs-5.gif]
+## Rendering templates The most powerful feature of this library is the ability
+of render templates. Custom XML/HTML like templates can be made to create
+images, Pixoo64 dials and even reusable parts or components. ```python ''' This
+template uses custom nodes for Pixoo64 for creating auto-updating dials, as
+date or time, so these are missing when rendering on any other renderer '''
+pizzoo.load_font('amstrad', './files/amstrad_cpc_extended.bdf')
+pizzoo.render_template(''' - Long text wrapped Cool ''') ```
+   [https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/
+                               images/qs-6.png]
+There's also have a dedicated section for this on our docs. ## Do you want to
+know more? [Here's](pizzoo.pablohuet.com) a dedicated page for documentation
+with a lot of examples so you can get quickly started. ## Contribute and/or
+donate This library was created and is maintained by a single developer,
+consider contributing with pull requests, new integrations, proposals or
+[simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W). ##
+Special thanks This library exists thanks to other libraries that were an
+inspiration, specially the [Pixoo](https://github.com/SomethingWithComputers/
+pixoo) library by SomethingWithComputers and the [Matrix-Fonts](https://
+github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font collection by trip5.
```

### Comparing `pizzoo-0.9.2/pizzoo/__init__.py` & `pizzoo-0.9.3/pizzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.2/pizzoo/_constants.py` & `pizzoo-0.9.3/pizzoo/_constants.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.2/pizzoo/_renderers.py` & `pizzoo-0.9.3/pizzoo/_renderers.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.2/pizzoo/_utils.py` & `pizzoo-0.9.3/pizzoo/_utils.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.2/pizzoo/game.py` & `pizzoo-0.9.3/pizzoo/game.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.2/pizzoo.egg-info/PKG-INFO` & `pizzoo-0.9.3/pizzoo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pizzoo
-Version: 0.9.2
+Version: 0.9.3
 Summary: Pizzoo is a library for rendering on pixel matrix screens, with direct support for the Divoom Pixoo64 device, and easy integration for any other one. It includes full animation buffer manipulation, a micro game engine, as well as XML/HTML like templates compilation.
 Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet
 License: MIT
 Keywords: pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED matrix,LED,raspberry,raspberry pi
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Requires-Dist: requests~=2.31.0
 Requires-Dist: Pillow~=10.0.0
 Requires-Dist: bdfparser~=2.2.0
 
 <p align="center">
-  <img src="https://github.com/pabletos/pizzoo/blob/main/docs/docs/assets/images/pizzoo-banner-nobg.png" alt="Pizzoo logo" width="450">
+  <img src="https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/images/pizzoo-banner-nobg.png" alt="Pizzoo logo" width="450">
 </p>
 <p>
 	<a 
 	href='https://ko-fi.com/B0B1PYK0W'
 	target='_blank'
 	rel="noreferrer"
 	>
@@ -51,46 +51,49 @@
 
 * **Game Development Toolkit**:
 	Tap into the possibilities of micro game development with our mini game engine. Design, develop, and deploy small-scale games that can be played right on your LED devices, perfect for creating engaging interactive experiences.
 
 ## Drawing on your device
 Frame manipulation is the core of the `pizzoo` library. Every time the library is created and the `render` method is called, the buffer is filled with a new frame we can use to draw on. Lets start by drawing three pixels on the screen and rendering:
 
-<img align="right" width="160" height="160" src="https://github.com/pabletos/pizzoo/blob/main/docs/docs/assets/images/qs-2.png">
-
 ```python
 pizzoo.cls()
 pizzoo.draw_circle((31, 31), 10, '#00ff00', filled=True) # Green circle, filled
 pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red rectangle, not filled
 pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue line
 pizzoo.draw_line((0, 31), (63, 31), (255, 255, 0)) # Yellow line, tuple rgb color format
 pizzoo.render()
 ```
 
+<p align="center">
+  <img width="320" height="320" src="https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/images/qs-2.png">
+</p>
+
 ## Creating animations
 Aside from simple gif drawing (That is also supported), custom animations can be created using frame-by-frame manipulation. As an example:
 
-<img align="right" width="160" height="160" src="https://github.com/pabletos/pizzoo/blob/main/docs/docs/assets/images/qs-5.gif">
-
 ```python
 '''
 This will create a simple diagonal moving circle
 '''
 for i in range(0, 54):
 	pizzoo.cls()
 	pizzoo.draw_circle((i + 4, i + 4), 2, '#00ff00', filled=True)
 	pizzoo.add_frame()
 pizzoo.render(frame_speed=100)
 ```
 
+<p align="center">
+	<img width="320" height="320" src="https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/images/qs-5.gif">
+</p>
+
+
 ## Rendering templates
 The most powerful feature of this library is the ability of render templates. Custom XML/HTML like templates can be made to create images, Pixoo64 dials and even reusable parts or components.
 
-<img align="right" width="160" height="160" src="https://github.com/pabletos/pizzoo/blob/main/docs/docs/assets/images/qs-6.png">
-
 ```python
 '''
 This template uses custom nodes for Pixoo64 for creating auto-updating dials, as date or time, so these are missing when 
 rendering on any other renderer
 '''
 pizzoo.load_font('amstrad', './files/amstrad_cpc_extended.bdf')
 pizzoo.render_template('''
@@ -112,14 +115,19 @@
 				</section>
 			</section>
 		</rectangle>
 	</pizzoo>
 ''')
 ```
 
+<p align="center">
+	<img width="320" height="320" src="https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/images/qs-6.png">
+</p>
+
+
 There's also have a dedicated section for this on our docs.
 
 ## Do you want to know more?
 [Here's](pizzoo.pablohuet.com) a dedicated page for documentation with a lot of examples so you can get quickly started.
 
 ## Contribute and/or donate
 This library was created and is maintained by a single developer, consider contributing with pull requests, new integrations, proposals or [simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pizzoo Version: 0.9.2 Summary: Pizzoo is a library
+Metadata-Version: 2.1 Name: pizzoo Version: 0.9.3 Summary: Pizzoo is a library
 for rendering on pixel matrix screens, with direct support for the Divoom
 Pixoo64 device, and easy integration for any other one. It includes full
 animation buffer manipulation, a micro game engine, as well as XML/HTML like
 templates compilation. Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet License: MIT Keywords:
 pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED
 matrix,LED,raspberry,raspberry pi Classifier: Development Status :: 4 - Beta
@@ -31,38 +31,41 @@
 to your specific project and hardware requirements. * **Game Development
 Toolkit**: Tap into the possibilities of micro game development with our mini
 game engine. Design, develop, and deploy small-scale games that can be played
 right on your LED devices, perfect for creating engaging interactive
 experiences. ## Drawing on your device Frame manipulation is the core of the
 `pizzoo` library. Every time the library is created and the `render` method is
 called, the buffer is filled with a new frame we can use to draw on. Lets start
-by drawing three pixels on the screen and rendering: [https://github.com/
-pabletos/pizzoo/blob/main/docs/docs/assets/images/qs-2.png]```python pizzoo.cls
-() pizzoo.draw_circle((31, 31), 10, '#00ff00', filled=True) # Green circle,
-filled pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red
+by drawing three pixels on the screen and rendering: ```python pizzoo.cls()
+pizzoo.draw_circle((31, 31), 10, '#00ff00', filled=True) # Green circle, filled
+pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red
 rectangle, not filled pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue
 line pizzoo.draw_line((0, 31), (63, 31), (255, 255, 0)) # Yellow line, tuple
-rgb color format pizzoo.render() ``` ## Creating animations Aside from simple
-gif drawing (That is also supported), custom animations can be created using
-frame-by-frame manipulation. As an example: [https://github.com/pabletos/
-pizzoo/blob/main/docs/docs/assets/images/qs-5.gif]```python ''' This will
-create a simple diagonal moving circle ''' for i in range(0, 54): pizzoo.cls()
-pizzoo.draw_circle((i + 4, i + 4), 2, '#00ff00', filled=True) pizzoo.add_frame
-() pizzoo.render(frame_speed=100) ``` ## Rendering templates The most powerful
-feature of this library is the ability of render templates. Custom XML/HTML
-like templates can be made to create images, Pixoo64 dials and even reusable
-parts or components. [https://github.com/pabletos/pizzoo/blob/main/docs/docs/
-assets/images/qs-6.png]```python ''' This template uses custom nodes for
-Pixoo64 for creating auto-updating dials, as date or time, so these are missing
-when rendering on any other renderer ''' pizzoo.load_font('amstrad', './files/
-amstrad_cpc_extended.bdf') pizzoo.render_template(''' - Long text wrapped Cool
-''') ``` There's also have a dedicated section for this on our docs. ## Do you
-want to know more? [Here's](pizzoo.pablohuet.com) a dedicated page for
-documentation with a lot of examples so you can get quickly started. ##
-Contribute and/or donate This library was created and is maintained by a single
-developer, consider contributing with pull requests, new integrations,
-proposals or [simply by doing a small donation on ko-fi](https://ko-fi.com/
-B0B1PYK0W). ## Special thanks This library exists thanks to other libraries
-that were an inspiration, specially the [Pixoo](https://github.com/
-SomethingWithComputers/pixoo) library by SomethingWithComputers and the
-[Matrix-Fonts](https://github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font
-collection by trip5.
+rgb color format pizzoo.render() ```
+   [https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/
+                               images/qs-2.png]
+## Creating animations Aside from simple gif drawing (That is also supported),
+custom animations can be created using frame-by-frame manipulation. As an
+example: ```python ''' This will create a simple diagonal moving circle ''' for
+i in range(0, 54): pizzoo.cls() pizzoo.draw_circle((i + 4, i + 4), 2,
+'#00ff00', filled=True) pizzoo.add_frame() pizzoo.render(frame_speed=100) ```
+   [https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/
+                               images/qs-5.gif]
+## Rendering templates The most powerful feature of this library is the ability
+of render templates. Custom XML/HTML like templates can be made to create
+images, Pixoo64 dials and even reusable parts or components. ```python ''' This
+template uses custom nodes for Pixoo64 for creating auto-updating dials, as
+date or time, so these are missing when rendering on any other renderer '''
+pizzoo.load_font('amstrad', './files/amstrad_cpc_extended.bdf')
+pizzoo.render_template(''' - Long text wrapped Cool ''') ```
+   [https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/
+                               images/qs-6.png]
+There's also have a dedicated section for this on our docs. ## Do you want to
+know more? [Here's](pizzoo.pablohuet.com) a dedicated page for documentation
+with a lot of examples so you can get quickly started. ## Contribute and/or
+donate This library was created and is maintained by a single developer,
+consider contributing with pull requests, new integrations, proposals or
+[simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W). ##
+Special thanks This library exists thanks to other libraries that were an
+inspiration, specially the [Pixoo](https://github.com/SomethingWithComputers/
+pixoo) library by SomethingWithComputers and the [Matrix-Fonts](https://
+github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font collection by trip5.
```

### Comparing `pizzoo-0.9.2/setup.py` & `pizzoo-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 long_description = open('%s\\README.md' % 'C:\\Users\\Usuario\\Documents\\Projects\\pizzoo').read()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name="pizzoo",
-    version="0.9.2",
+    version="0.9.3",
     author="Pablo Huet",
     description="Pizzoo is a library for rendering on pixel matrix screens, with direct support for the Divoom Pixoo64 device, and easy integration for any other one. It includes full animation buffer manipulation, a micro game engine, as well as XML/HTML like templates compilation.",
     long_description=long_description,
 	long_description_content_type='text/markdown',
 	license="MIT",
     keywords="pixoo, pixoo64, divoom, screen, pixel, matrix, render, buffer, LED matrix, LED, raspberry, raspberry pi",
     url="https://github.com/pabletos/pizzoo#readme",
```

