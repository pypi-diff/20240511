# Comparing `tmp/pizzoo-0.9.3.tar.gz` & `tmp/pizzoo-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizzoo-0.9.3.tar", last modified: Sat May 11 00:57:45 2024, max compression
+gzip compressed data, was "pizzoo-0.9.4.tar", last modified: Sat May 11 09:33:35 2024, max compression
```

## Comparing `pizzoo-0.9.3.tar` & `pizzoo-0.9.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 00:57:45.172341 pizzoo-0.9.3/
--rw-rw-rw-   0        0        0     6796 2024-05-11 00:57:45.172341 pizzoo-0.9.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 00:57:45.168334 pizzoo-0.9.3/pizzoo/
--rw-rw-rw-   0        0        0    21798 2024-05-04 08:50:51.000000 pizzoo-0.9.3/pizzoo/__init__.py
--rw-rw-rw-   0        0        0     1444 2024-04-19 15:38:24.000000 pizzoo-0.9.3/pizzoo/_constants.py
--rw-rw-rw-   0        0        0    17046 2024-05-03 00:00:18.000000 pizzoo-0.9.3/pizzoo/_renderers.py
--rw-rw-rw-   0        0        0      705 2024-04-28 16:47:36.000000 pizzoo-0.9.3/pizzoo/_utils.py
--rw-rw-rw-   0        0        0    21871 2024-05-10 19:21:17.000000 pizzoo-0.9.3/pizzoo/game.py
-drwxrwxrwx   0        0        0        0 2024-05-11 00:57:45.171342 pizzoo-0.9.3/pizzoo.egg-info/
--rw-rw-rw-   0        0        0     6796 2024-05-11 00:57:45.000000 pizzoo-0.9.3/pizzoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-11 00:57:45.000000 pizzoo-0.9.3/pizzoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 00:57:45.000000 pizzoo-0.9.3/pizzoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-11 00:57:45.000000 pizzoo-0.9.3/pizzoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-11 00:57:45.000000 pizzoo-0.9.3/pizzoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 00:57:45.172341 pizzoo-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1172 2024-05-11 00:57:40.000000 pizzoo-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:33:35.104435 pizzoo-0.9.4/
+-rw-rw-rw-   0        0        0     6988 2024-05-11 09:33:35.103434 pizzoo-0.9.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 09:33:35.099242 pizzoo-0.9.4/pizzoo/
+-rw-rw-rw-   0        0        0    21798 2024-05-04 08:50:51.000000 pizzoo-0.9.4/pizzoo/__init__.py
+-rw-rw-rw-   0        0        0     1444 2024-04-19 15:38:24.000000 pizzoo-0.9.4/pizzoo/_constants.py
+-rw-rw-rw-   0        0        0    17046 2024-05-03 00:00:18.000000 pizzoo-0.9.4/pizzoo/_renderers.py
+-rw-rw-rw-   0        0        0      705 2024-04-28 16:47:36.000000 pizzoo-0.9.4/pizzoo/_utils.py
+-rw-rw-rw-   0        0        0    21871 2024-05-10 19:21:17.000000 pizzoo-0.9.4/pizzoo/game.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:33:35.102435 pizzoo-0.9.4/pizzoo.egg-info/
+-rw-rw-rw-   0        0        0     6988 2024-05-11 09:33:35.000000 pizzoo-0.9.4/pizzoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-11 09:33:35.000000 pizzoo-0.9.4/pizzoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 09:33:35.000000 pizzoo-0.9.4/pizzoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-11 09:33:35.000000 pizzoo-0.9.4/pizzoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-11 09:33:35.000000 pizzoo-0.9.4/pizzoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 09:33:35.104435 pizzoo-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-05-11 09:26:24.000000 pizzoo-0.9.4/setup.py
```

### Comparing `pizzoo-0.9.3/PKG-INFO` & `pizzoo-0.9.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pizzoo
-Version: 0.9.3
-Summary: Pizzoo is a library for rendering on pixel matrix screens, with direct support for the Divoom Pixoo64 device, and easy integration for any other one. It includes full animation buffer manipulation, a micro game engine, as well as XML/HTML like templates compilation.
+Version: 0.9.4
+Summary: Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.
 Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet
 License: MIT
 Keywords: pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED matrix,LED,raspberry,raspberry pi
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: License :: OSI Approved :: MIT License
@@ -19,39 +19,45 @@
 </p>
 <p>
 	<a 
 	href='https://ko-fi.com/B0B1PYK0W'
 	target='_blank'
 	rel="noreferrer"
 	>
-	<img height='24' style="border:0px; height:24px" src='https://img.shields.io/badge/donate-blue?logo=ko-fi&logoColor=%23ffffff' border='0' alt='Buy Me a Coffee at ko-fi.com' />
+	<img src='https://img.shields.io/badge/donate-blue?logo=ko-fi&logoColor=%23ffffff' border='0' alt='Buy Me a Coffee at ko-fi.com' />
+	</a>
+	<a
+	href="https://pizzoo.pablohuet.com"
+	target="_blank"
+	rel="noreferrer"
+	>
+		<img src="https://img.shields.io/badge/-docs-red?logo=readthedocs&logoColor=white">
 	</a>
 	<a
 	href='https://pypi.org/project/pizzoo/'
 	target='_blank'
 	rel="noreferrer"
 	>
-	<img height='24' style="text-decoration:none;" src="https://img.shields.io/badge/version-0.9.0-blue?logo=pypi&logoColor=%23ffffff"/>
-	</a>
+	<img src="https://img.shields.io/badge/version-0.9.0-blue?logo=pypi&logoColor=%23ffffff"/>
 	</a>
-	<img height='24' style="text-decoration:none;" src="https://img.shields.io/badge/status-beta-yellow"/>
+	<img src="https://img.shields.io/badge/status-beta-yellow"/>
 </p>
 
 Pizzoo is a robust Python library designed for developers who want to unlock the full potential of matrix LED displays, particularly the Pixoo64, a 64x64 pixel LED display, and extend its functionalities to various other devices. Whether you're looking to create dynamic animations, develop interactive games, or integrate unique display functionalities, Pizzoo provides you with the tools and flexibility to innovate and express your creative ideas.
 
 ## Features
 
 * **Full Animation Creation and Control**:
 	With frame-by-frame programatic drawing capabilities you can craft detailed animations directly on your LED display, allowing you to visually conceptualize, iterate, and render animations seamlessly.
 
 * **Template Rendering**:
 	Our built-in compiler supports an XML/HTML-like language for template processing. This facilitates the design of UIs with relative positioning, defined areas, and reusable components, helping you creating fast and reusable interfaces.
 
 * **Flexible integration with any device**:
-	The Renderer class can be easily extended to support additional methods and integrate with various hardware. This ensures that Pizzoo can adapt to your specific project and hardware requirements.
+	Even with the Pixoo64 being the default target, the Renderer class can be easily extended to support additional methods and integrate with various hardware. This ensures that Pizzoo can adapt to your specific project and hardware requirements.
 
 * **Game Development Toolkit**:
 	Tap into the possibilities of micro game development with our mini game engine. Design, develop, and deploy small-scale games that can be played right on your LED devices, perfect for creating engaging interactive experiences.
 
 ## Drawing on your device
 Frame manipulation is the core of the `pizzoo` library. Every time the library is created and the `render` method is called, the buffer is filled with a new frame we can use to draw on. Lets start by drawing three pixels on the screen and rendering:
 
@@ -130,7 +136,9 @@
 [Here's](pizzoo.pablohuet.com) a dedicated page for documentation with a lot of examples so you can get quickly started.
 
 ## Contribute and/or donate
 This library was created and is maintained by a single developer, consider contributing with pull requests, new integrations, proposals or [simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W).
 
 ## Special thanks
 This library exists thanks to other libraries that were an inspiration, specially the [Pixoo](https://github.com/SomethingWithComputers/pixoo) library by SomethingWithComputers and the [Matrix-Fonts](https://github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font collection by trip5.
+
+Also I want to give a special thanks [to my lovely fiancee](https://github.com/srtashadowfax) for all his support while developing this library, both technical and emotional ðŸ’–
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,50 +1,51 @@
-Metadata-Version: 2.1 Name: pizzoo Version: 0.9.3 Summary: Pizzoo is a library
-for rendering on pixel matrix screens, with direct support for the Divoom
-Pixoo64 device, and easy integration for any other one. It includes full
-animation buffer manipulation, a micro game engine, as well as XML/HTML like
-templates compilation. Home-page: https://github.com/pabletos/pizzoo#readme
-Author: Pablo Huet License: MIT Keywords:
+Metadata-Version: 2.1 Name: pizzoo Version: 0.9.4 Summary: Pizzoo is a easy-to-
+use library for rendering on pixel matrix screens like the Pixoo64, featuring
+easy new device integration, animation tools, and XML template rendering
+support. Home-page: https://github.com/pabletos/pizzoo#readme Author: Pablo
+Huet License: MIT Keywords:
 pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED
 matrix,LED,raspberry,raspberry pi Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics Classifier: License :: OSI Approved
 :: MIT License Description-Content-Type: text/markdown Requires-Dist:
 requests~=2.31.0 Requires-Dist: Pillow~=10.0.0 Requires-Dist: bdfparser~=2.2.0
                                  [Pizzoo logo]
-_[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-_f_i_._c_o_m_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_v_e_r_s_i_o_n_-_0_._9_._0_-
-_b_l_u_e_?_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_%_2_3_f_f_f_f_f_f_]
-[https://img.shields.io/badge/status-beta-yellow]
+_[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-_f_i_._c_o_m_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_d_o_c_s_-
+_r_e_d_?_l_o_g_o_=_r_e_a_d_t_h_e_d_o_c_s_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_v_e_r_s_i_o_n_-
+_0_._9_._0_-_b_l_u_e_?_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_%_2_3_f_f_f_f_f_f_][https://img.shields.io/badge/status-
+beta-yellow]
 Pizzoo is a robust Python library designed for developers who want to unlock
 the full potential of matrix LED displays, particularly the Pixoo64, a 64x64
 pixel LED display, and extend its functionalities to various other devices.
 Whether you're looking to create dynamic animations, develop interactive games,
 or integrate unique display functionalities, Pizzoo provides you with the tools
 and flexibility to innovate and express your creative ideas. ## Features *
 **Full Animation Creation and Control**: With frame-by-frame programatic
 drawing capabilities you can craft detailed animations directly on your LED
 display, allowing you to visually conceptualize, iterate, and render animations
 seamlessly. * **Template Rendering**: Our built-in compiler supports an XML/
 HTML-like language for template processing. This facilitates the design of UIs
 with relative positioning, defined areas, and reusable components, helping you
 creating fast and reusable interfaces. * **Flexible integration with any
-device**: The Renderer class can be easily extended to support additional
-methods and integrate with various hardware. This ensures that Pizzoo can adapt
-to your specific project and hardware requirements. * **Game Development
-Toolkit**: Tap into the possibilities of micro game development with our mini
-game engine. Design, develop, and deploy small-scale games that can be played
-right on your LED devices, perfect for creating engaging interactive
-experiences. ## Drawing on your device Frame manipulation is the core of the
-`pizzoo` library. Every time the library is created and the `render` method is
-called, the buffer is filled with a new frame we can use to draw on. Lets start
-by drawing three pixels on the screen and rendering: ```python pizzoo.cls()
-pizzoo.draw_circle((31, 31), 10, '#00ff00', filled=True) # Green circle, filled
-pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red
-rectangle, not filled pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue
-line pizzoo.draw_line((0, 31), (63, 31), (255, 255, 0)) # Yellow line, tuple
-rgb color format pizzoo.render() ```
+device**: Even with the Pixoo64 being the default target, the Renderer class
+can be easily extended to support additional methods and integrate with various
+hardware. This ensures that Pizzoo can adapt to your specific project and
+hardware requirements. * **Game Development Toolkit**: Tap into the
+possibilities of micro game development with our mini game engine. Design,
+develop, and deploy small-scale games that can be played right on your LED
+devices, perfect for creating engaging interactive experiences. ## Drawing on
+your device Frame manipulation is the core of the `pizzoo` library. Every time
+the library is created and the `render` method is called, the buffer is filled
+with a new frame we can use to draw on. Lets start by drawing three pixels on
+the screen and rendering: ```python pizzoo.cls() pizzoo.draw_circle((31, 31),
+10, '#00ff00', filled=True) # Green circle, filled pizzoo.draw_rectangle((26,
+26), 11, 11, '#ff0000', filled=False) # Red rectangle, not filled
+pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue line pizzoo.draw_line((0,
+31), (63, 31), (255, 255, 0)) # Yellow line, tuple rgb color format
+pizzoo.render() ```
    [https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/
                                images/qs-2.png]
 ## Creating animations Aside from simple gif drawing (That is also supported),
 custom animations can be created using frame-by-frame manipulation. As an
 example: ```python ''' This will create a simple diagonal moving circle ''' for
 i in range(0, 54): pizzoo.cls() pizzoo.draw_circle((i + 4, i + 4), 2,
 '#00ff00', filled=True) pizzoo.add_frame() pizzoo.render(frame_speed=100) ```
@@ -65,7 +66,10 @@
 donate This library was created and is maintained by a single developer,
 consider contributing with pull requests, new integrations, proposals or
 [simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W). ##
 Special thanks This library exists thanks to other libraries that were an
 inspiration, specially the [Pixoo](https://github.com/SomethingWithComputers/
 pixoo) library by SomethingWithComputers and the [Matrix-Fonts](https://
 github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font collection by trip5.
+Also I want to give a special thanks [to my lovely fiancee](https://github.com/
+srtashadowfax) for all his support while developing this library, both
+technical and emotional Ã°Å¸ââ
```

### Comparing `pizzoo-0.9.3/pizzoo/__init__.py` & `pizzoo-0.9.4/pizzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.3/pizzoo/_constants.py` & `pizzoo-0.9.4/pizzoo/_constants.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.3/pizzoo/_renderers.py` & `pizzoo-0.9.4/pizzoo/_renderers.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.3/pizzoo/_utils.py` & `pizzoo-0.9.4/pizzoo/_utils.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.3/pizzoo/game.py` & `pizzoo-0.9.4/pizzoo/game.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.3/pizzoo.egg-info/PKG-INFO` & `pizzoo-0.9.4/pizzoo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pizzoo
-Version: 0.9.3
-Summary: Pizzoo is a library for rendering on pixel matrix screens, with direct support for the Divoom Pixoo64 device, and easy integration for any other one. It includes full animation buffer manipulation, a micro game engine, as well as XML/HTML like templates compilation.
+Version: 0.9.4
+Summary: Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.
 Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet
 License: MIT
 Keywords: pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED matrix,LED,raspberry,raspberry pi
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: License :: OSI Approved :: MIT License
@@ -19,39 +19,45 @@
 </p>
 <p>
 	<a 
 	href='https://ko-fi.com/B0B1PYK0W'
 	target='_blank'
 	rel="noreferrer"
 	>
-	<img height='24' style="border:0px; height:24px" src='https://img.shields.io/badge/donate-blue?logo=ko-fi&logoColor=%23ffffff' border='0' alt='Buy Me a Coffee at ko-fi.com' />
+	<img src='https://img.shields.io/badge/donate-blue?logo=ko-fi&logoColor=%23ffffff' border='0' alt='Buy Me a Coffee at ko-fi.com' />
+	</a>
+	<a
+	href="https://pizzoo.pablohuet.com"
+	target="_blank"
+	rel="noreferrer"
+	>
+		<img src="https://img.shields.io/badge/-docs-red?logo=readthedocs&logoColor=white">
 	</a>
 	<a
 	href='https://pypi.org/project/pizzoo/'
 	target='_blank'
 	rel="noreferrer"
 	>
-	<img height='24' style="text-decoration:none;" src="https://img.shields.io/badge/version-0.9.0-blue?logo=pypi&logoColor=%23ffffff"/>
-	</a>
+	<img src="https://img.shields.io/badge/version-0.9.0-blue?logo=pypi&logoColor=%23ffffff"/>
 	</a>
-	<img height='24' style="text-decoration:none;" src="https://img.shields.io/badge/status-beta-yellow"/>
+	<img src="https://img.shields.io/badge/status-beta-yellow"/>
 </p>
 
 Pizzoo is a robust Python library designed for developers who want to unlock the full potential of matrix LED displays, particularly the Pixoo64, a 64x64 pixel LED display, and extend its functionalities to various other devices. Whether you're looking to create dynamic animations, develop interactive games, or integrate unique display functionalities, Pizzoo provides you with the tools and flexibility to innovate and express your creative ideas.
 
 ## Features
 
 * **Full Animation Creation and Control**:
 	With frame-by-frame programatic drawing capabilities you can craft detailed animations directly on your LED display, allowing you to visually conceptualize, iterate, and render animations seamlessly.
 
 * **Template Rendering**:
 	Our built-in compiler supports an XML/HTML-like language for template processing. This facilitates the design of UIs with relative positioning, defined areas, and reusable components, helping you creating fast and reusable interfaces.
 
 * **Flexible integration with any device**:
-	The Renderer class can be easily extended to support additional methods and integrate with various hardware. This ensures that Pizzoo can adapt to your specific project and hardware requirements.
+	Even with the Pixoo64 being the default target, the Renderer class can be easily extended to support additional methods and integrate with various hardware. This ensures that Pizzoo can adapt to your specific project and hardware requirements.
 
 * **Game Development Toolkit**:
 	Tap into the possibilities of micro game development with our mini game engine. Design, develop, and deploy small-scale games that can be played right on your LED devices, perfect for creating engaging interactive experiences.
 
 ## Drawing on your device
 Frame manipulation is the core of the `pizzoo` library. Every time the library is created and the `render` method is called, the buffer is filled with a new frame we can use to draw on. Lets start by drawing three pixels on the screen and rendering:
 
@@ -130,7 +136,9 @@
 [Here's](pizzoo.pablohuet.com) a dedicated page for documentation with a lot of examples so you can get quickly started.
 
 ## Contribute and/or donate
 This library was created and is maintained by a single developer, consider contributing with pull requests, new integrations, proposals or [simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W).
 
 ## Special thanks
 This library exists thanks to other libraries that were an inspiration, specially the [Pixoo](https://github.com/SomethingWithComputers/pixoo) library by SomethingWithComputers and the [Matrix-Fonts](https://github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font collection by trip5.
+
+Also I want to give a special thanks [to my lovely fiancee](https://github.com/srtashadowfax) for all his support while developing this library, both technical and emotional ðŸ’–
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,50 +1,51 @@
-Metadata-Version: 2.1 Name: pizzoo Version: 0.9.3 Summary: Pizzoo is a library
-for rendering on pixel matrix screens, with direct support for the Divoom
-Pixoo64 device, and easy integration for any other one. It includes full
-animation buffer manipulation, a micro game engine, as well as XML/HTML like
-templates compilation. Home-page: https://github.com/pabletos/pizzoo#readme
-Author: Pablo Huet License: MIT Keywords:
+Metadata-Version: 2.1 Name: pizzoo Version: 0.9.4 Summary: Pizzoo is a easy-to-
+use library for rendering on pixel matrix screens like the Pixoo64, featuring
+easy new device integration, animation tools, and XML template rendering
+support. Home-page: https://github.com/pabletos/pizzoo#readme Author: Pablo
+Huet License: MIT Keywords:
 pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED
 matrix,LED,raspberry,raspberry pi Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics Classifier: License :: OSI Approved
 :: MIT License Description-Content-Type: text/markdown Requires-Dist:
 requests~=2.31.0 Requires-Dist: Pillow~=10.0.0 Requires-Dist: bdfparser~=2.2.0
                                  [Pizzoo logo]
-_[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-_f_i_._c_o_m_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_v_e_r_s_i_o_n_-_0_._9_._0_-
-_b_l_u_e_?_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_%_2_3_f_f_f_f_f_f_]
-[https://img.shields.io/badge/status-beta-yellow]
+_[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-_f_i_._c_o_m_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_d_o_c_s_-
+_r_e_d_?_l_o_g_o_=_r_e_a_d_t_h_e_d_o_c_s_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_v_e_r_s_i_o_n_-
+_0_._9_._0_-_b_l_u_e_?_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_%_2_3_f_f_f_f_f_f_][https://img.shields.io/badge/status-
+beta-yellow]
 Pizzoo is a robust Python library designed for developers who want to unlock
 the full potential of matrix LED displays, particularly the Pixoo64, a 64x64
 pixel LED display, and extend its functionalities to various other devices.
 Whether you're looking to create dynamic animations, develop interactive games,
 or integrate unique display functionalities, Pizzoo provides you with the tools
 and flexibility to innovate and express your creative ideas. ## Features *
 **Full Animation Creation and Control**: With frame-by-frame programatic
 drawing capabilities you can craft detailed animations directly on your LED
 display, allowing you to visually conceptualize, iterate, and render animations
 seamlessly. * **Template Rendering**: Our built-in compiler supports an XML/
 HTML-like language for template processing. This facilitates the design of UIs
 with relative positioning, defined areas, and reusable components, helping you
 creating fast and reusable interfaces. * **Flexible integration with any
-device**: The Renderer class can be easily extended to support additional
-methods and integrate with various hardware. This ensures that Pizzoo can adapt
-to your specific project and hardware requirements. * **Game Development
-Toolkit**: Tap into the possibilities of micro game development with our mini
-game engine. Design, develop, and deploy small-scale games that can be played
-right on your LED devices, perfect for creating engaging interactive
-experiences. ## Drawing on your device Frame manipulation is the core of the
-`pizzoo` library. Every time the library is created and the `render` method is
-called, the buffer is filled with a new frame we can use to draw on. Lets start
-by drawing three pixels on the screen and rendering: ```python pizzoo.cls()
-pizzoo.draw_circle((31, 31), 10, '#00ff00', filled=True) # Green circle, filled
-pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red
-rectangle, not filled pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue
-line pizzoo.draw_line((0, 31), (63, 31), (255, 255, 0)) # Yellow line, tuple
-rgb color format pizzoo.render() ```
+device**: Even with the Pixoo64 being the default target, the Renderer class
+can be easily extended to support additional methods and integrate with various
+hardware. This ensures that Pizzoo can adapt to your specific project and
+hardware requirements. * **Game Development Toolkit**: Tap into the
+possibilities of micro game development with our mini game engine. Design,
+develop, and deploy small-scale games that can be played right on your LED
+devices, perfect for creating engaging interactive experiences. ## Drawing on
+your device Frame manipulation is the core of the `pizzoo` library. Every time
+the library is created and the `render` method is called, the buffer is filled
+with a new frame we can use to draw on. Lets start by drawing three pixels on
+the screen and rendering: ```python pizzoo.cls() pizzoo.draw_circle((31, 31),
+10, '#00ff00', filled=True) # Green circle, filled pizzoo.draw_rectangle((26,
+26), 11, 11, '#ff0000', filled=False) # Red rectangle, not filled
+pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue line pizzoo.draw_line((0,
+31), (63, 31), (255, 255, 0)) # Yellow line, tuple rgb color format
+pizzoo.render() ```
    [https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/
                                images/qs-2.png]
 ## Creating animations Aside from simple gif drawing (That is also supported),
 custom animations can be created using frame-by-frame manipulation. As an
 example: ```python ''' This will create a simple diagonal moving circle ''' for
 i in range(0, 54): pizzoo.cls() pizzoo.draw_circle((i + 4, i + 4), 2,
 '#00ff00', filled=True) pizzoo.add_frame() pizzoo.render(frame_speed=100) ```
@@ -65,7 +66,10 @@
 donate This library was created and is maintained by a single developer,
 consider contributing with pull requests, new integrations, proposals or
 [simply by doing a small donation on ko-fi](https://ko-fi.com/B0B1PYK0W). ##
 Special thanks This library exists thanks to other libraries that were an
 inspiration, specially the [Pixoo](https://github.com/SomethingWithComputers/
 pixoo) library by SomethingWithComputers and the [Matrix-Fonts](https://
 github.com/trip5/Matrix-Fonts/tree/main) matrix bdf font collection by trip5.
+Also I want to give a special thanks [to my lovely fiancee](https://github.com/
+srtashadowfax) for all his support while developing this library, both
+technical and emotional Ã°Å¸ââ
```

### Comparing `pizzoo-0.9.3/setup.py` & `pizzoo-0.9.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 long_description = open('%s\\README.md' % 'C:\\Users\\Usuario\\Documents\\Projects\\pizzoo').read()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name="pizzoo",
-    version="0.9.3",
+    version="0.9.4",
     author="Pablo Huet",
-    description="Pizzoo is a library for rendering on pixel matrix screens, with direct support for the Divoom Pixoo64 device, and easy integration for any other one. It includes full animation buffer manipulation, a micro game engine, as well as XML/HTML like templates compilation.",
+    description="Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.",
     long_description=long_description,
 	long_description_content_type='text/markdown',
 	license="MIT",
     keywords="pixoo, pixoo64, divoom, screen, pixel, matrix, render, buffer, LED matrix, LED, raspberry, raspberry pi",
     url="https://github.com/pabletos/pizzoo#readme",
     packages=['pizzoo'],
     install_requires=[
```

