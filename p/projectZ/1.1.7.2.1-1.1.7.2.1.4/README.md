# Comparing `tmp/projectZ-1.1.7.2.1.tar.gz` & `tmp/projectZ-1.1.7.2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectZ-1.1.7.2.1.tar", last modified: Wed May  1 12:17:06 2024, max compression
+gzip compressed data, was "projectZ-1.1.7.2.1.4.tar", last modified: Sat May 11 11:41:01 2024, max compression
```

## Comparing `projectZ-1.1.7.2.1.tar` & `projectZ-1.1.7.2.1.4.tar`

### file list

```diff
@@ -1,21 +1,33 @@
-drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     1086 2024-05-01 09:25:03.000000 projectZ-1.1.7.2.1/LICENSE.txt
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2910 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/PKG-INFO
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2416 2024-04-30 21:29:39.000000 projectZ-1.1.7.2.1/README.md
-drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/projectZ/
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      595 2024-05-01 12:14:44.000000 projectZ-1.1.7.2.1/projectZ/__init__.py
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)    15835 2024-05-01 12:11:05.000000 projectZ-1.1.7.2.1/projectZ/async_client.py
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)    15159 2024-05-01 12:10:09.000000 projectZ-1.1.7.2.1/projectZ/client.py
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     4403 2024-05-01 10:03:10.000000 projectZ-1.1.7.2.1/projectZ/requests_builder.py
-drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/projectZ/utils/
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        0 2024-04-30 21:29:39.000000 projectZ-1.1.7.2.1/projectZ/utils/__init__.py
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2017 2024-05-01 10:04:41.000000 projectZ-1.1.7.2.1/projectZ/utils/exceptions.py
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      865 2024-04-30 21:29:39.000000 projectZ-1.1.7.2.1/projectZ/utils/generator.py
-drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/projectZ.egg-info/
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2910 2024-05-01 12:17:05.000000 projectZ-1.1.7.2.1/projectZ.egg-info/PKG-INFO
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      377 2024-05-01 12:17:05.000000 projectZ-1.1.7.2.1/projectZ.egg-info/SOURCES.txt
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        1 2024-05-01 12:17:05.000000 projectZ-1.1.7.2.1/projectZ.egg-info/dependency_links.txt
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)       49 2024-05-01 12:17:05.000000 projectZ-1.1.7.2.1/projectZ.egg-info/requires.txt
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        9 2024-05-01 12:17:05.000000 projectZ-1.1.7.2.1/projectZ.egg-info/top_level.txt
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)       38 2024-05-01 12:17:06.035191 projectZ-1.1.7.2.1/setup.cfg
--rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      905 2024-05-01 12:16:49.000000 projectZ-1.1.7.2.1/setup.py
+drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-11 11:41:01.582053 projectZ-1.1.7.2.1.4/
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     1086 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/LICENSE.txt
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2957 2024-05-11 11:41:01.582053 projectZ-1.1.7.2.1.4/PKG-INFO
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2461 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/README.md
+drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-11 11:41:01.582053 projectZ-1.1.7.2.1.4/projectZ/
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      595 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/__init__.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)    15835 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/async_client.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)    15159 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/client.py
+drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-11 11:41:01.582053 projectZ-1.1.7.2.1.4/projectZ/objects/
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      139 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/objects/ChatMessageTypes.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      169 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/objects/MediaTargets.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-11 11:36:27.000000 projectZ-1.1.7.2.1.4/projectZ/objects/__init__.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     1196 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/objects/constants.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)    21942 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/objects/objects.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      448 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/objects/profile.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     3540 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/objects/ws_types.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     4403 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/requests_builder.py
+drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-11 11:41:01.582053 projectZ-1.1.7.2.1.4/projectZ/utils/
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/utils/__init__.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2017 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/utils/exceptions.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      865 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/utils/generator.py
+drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-11 11:41:01.582053 projectZ-1.1.7.2.1.4/projectZ/ws/
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-11 11:36:43.000000 projectZ-1.1.7.2.1.4/projectZ/ws/__init__.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     3581 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/ws/async_socket.py
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     3610 2024-05-11 11:29:24.000000 projectZ-1.1.7.2.1.4/projectZ/ws/socket.py
+drwxr-xr-x   0 xsarzy    (1000) xsarzy    (1000)        0 2024-05-11 11:41:01.582053 projectZ-1.1.7.2.1.4/projectZ.egg-info/
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)     2957 2024-05-11 11:41:01.000000 projectZ-1.1.7.2.1.4/projectZ.egg-info/PKG-INFO
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      665 2024-05-11 11:41:01.000000 projectZ-1.1.7.2.1.4/projectZ.egg-info/SOURCES.txt
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        1 2024-05-11 11:41:01.000000 projectZ-1.1.7.2.1.4/projectZ.egg-info/dependency_links.txt
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)       49 2024-05-11 11:41:01.000000 projectZ-1.1.7.2.1.4/projectZ.egg-info/requires.txt
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)        9 2024-05-11 11:41:01.000000 projectZ-1.1.7.2.1.4/projectZ.egg-info/top_level.txt
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)       38 2024-05-11 11:41:01.586053 projectZ-1.1.7.2.1.4/setup.cfg
+-rw-r--r--   0 xsarzy    (1000) xsarzy    (1000)      879 2024-05-11 11:37:33.000000 projectZ-1.1.7.2.1.4/setup.py
```

### Comparing `projectZ-1.1.7.2.1/LICENSE.txt` & `projectZ-1.1.7.2.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `projectZ-1.1.7.2.1/PKG-INFO` & `projectZ-1.1.7.2.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,58 @@
-Metadata-Version: 2.1
-Name: projectZ
-Version: 1.1.7.2.1
-Summary: Library for creating projectZ bots and scripts.
-Home-page: https://github.com/xXxCLOTIxXx/projectZ.py
-Download-URL: https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip
-Author: Xsarz
-Author-email: xsarzy@gmail.com
-License: MIT
-Keywords: projectZ.py,projectZ,projectZ-py,projectZ-bot,api,python,python3,python3.x,xsarz,official,async,sync,projz
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <body>
 	<p align="center">
+	    <a href="#"><img src="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/res/logo.png"/></a>
 	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/releases"><img src="https://img.shields.io/github/v/release/xXxCLOTIxXx/projectZ.py" alt="GitHub release" />
 	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="licence" /></a>
 	    <a href="https://pypi.org/project/projectZ/"><img src="https://img.shields.io/pypi/v/projectZ" alt="pypi" /></a>
 	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md"><img src="https://img.shields.io/website?down_message=failing&label=docs&up_color=green&up_message=passing&url=https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md" alt="docs" /></a>
 	</p>
 	<div align="center">
 		<a href="https://github.com/xXxCLOTIxXx/xXxCLOTIxXx/blob/main/sponsor.md">
-			<img src="https://img.shields.io/static/v1?style=for-the-badge&label=Sponsor project&message=%E2%9D%A4&color=ff69b4" alt="Sponsor project"/>
+			<img src="https://img.shields.io/badge/%D0%A1%D0%BF%D0%BE%D0%BD%D1%81%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D1%82%D1%8C-Donate-F79B1F?style=for-the-badge&logo=github&logoColor=FF69B4&color=FF69B4" alt="Sponsor project"/>
 		</a>
-	</div>
-	<table align="center">
-		</tr>
-		<tr> <th colspan="3">More info</th> </tr>
-		<tr>
-			<td>
-				<a href="https://t.me/DxsarzUnion"><img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" height="30px">
-				 Telegram Channel</a>
-			</td>
-			<td>
-				<a href="https://www.youtube.com/channel/UCNKEgQmAvt6dD7jeMLpte9Q"><img src="https://upload.wikimedia.org/wikipedia/commons/0/09/YouTube_full-color_icon_%282017%29.svg" height="30px">
-				 YouTube channel</a>
-			</td>
-			<td>
-				<a href="https://discord.gg/GtpUnsHHT4"><img src="https://www.svgrepo.com/show/353655/discord-icon.svg" height="30px">
-				 Discord Server</a>
-			</td>
-		</tr>
-	</table>
-<h1 align="center">projectZ.py</h1>
-		    
+		<hr>
+		<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=28&duration=2000&pause=2000&color=F79B1F&random=false&width=200&repeat=false&lines=Installation" alt="Installation"/>
+	<p>Git</p>
+	
 ```bash
-pip install projectZ
+pip install git+https://github.com/xXxCLOTIxXx/projectZ.py.git
 ```
-<h4 align="center">or</h4>
-		    
+<p>pypi</p>
+
 ```bash
-pip install git+https://github.com/xXxCLOTIxXx/projectZ.py.git
+pip install projectZ
 ```
-<p align="center">Library for working with projectZ servers, below you will see code examples</p>
-<h1 align="center">Login example</h1>
+<hr><br>
+<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=28&duration=2000&pause=2000&color=F79B1F&repeat=false&random=false&width=90&lines=Using" alt="Using"/>
+</div>
+<h4 align="center">Login example</h4>
 
 ```python
 import projectZ
 
 client = projectZ.Client()
 client.login(email='email', password='password')
 ```
-
-<h1 align="center">Async login example</h1>
+<br><br>
+<h4 align="center">Async login example</h4>
 
 ```python
 import projectZ
 import asyncio
 
 
 client = projectZ.AsyncClient()
 async def main():
 	await client.login(email='email', password='password')
 
 if __name__ == '__main__':
 	loop = asyncio.get_event_loop()
 	loop.run_until_complete(main())
 ```
-
+<hr><br>
+<div align="center">
+<a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md">
+<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=14&duration=1&pause=31&color=3DACF7&random=false&width=195&lines=Read+the+documentation" alt="=Read the documentation"/>
+</a>
+</div>
 </body>
```

### Comparing `projectZ-1.1.7.2.1/projectZ/__init__.py` & `projectZ-1.1.7.2.1.4/projectZ/__init__.py`

 * *Files identical despite different names*

### Comparing `projectZ-1.1.7.2.1/projectZ/async_client.py` & `projectZ-1.1.7.2.1.4/projectZ/async_client.py`

 * *Files identical despite different names*

### Comparing `projectZ-1.1.7.2.1/projectZ/client.py` & `projectZ-1.1.7.2.1.4/projectZ/client.py`

 * *Files identical despite different names*

### Comparing `projectZ-1.1.7.2.1/projectZ/requests_builder.py` & `projectZ-1.1.7.2.1.4/projectZ/requests_builder.py`

 * *Files identical despite different names*

### Comparing `projectZ-1.1.7.2.1/projectZ/utils/exceptions.py` & `projectZ-1.1.7.2.1.4/projectZ/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `projectZ-1.1.7.2.1/projectZ/utils/generator.py` & `projectZ-1.1.7.2.1.4/projectZ/utils/generator.py`

 * *Files identical despite different names*

### Comparing `projectZ-1.1.7.2.1/projectZ.egg-info/PKG-INFO` & `projectZ-1.1.7.2.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,71 @@
 Metadata-Version: 2.1
 Name: projectZ
-Version: 1.1.7.2.1
+Version: 1.1.7.2.1.4
 Summary: Library for creating projectZ bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/projectZ.py
 Download-URL: https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Keywords: projectZ.py,projectZ,projectZ-py,projectZ-bot,api,python,python3,python3.x,xsarz,official,async,sync,projz
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <body>
 	<p align="center">
+	    <a href="#"><img src="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/res/logo.png"/></a>
 	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/releases"><img src="https://img.shields.io/github/v/release/xXxCLOTIxXx/projectZ.py" alt="GitHub release" />
 	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="licence" /></a>
 	    <a href="https://pypi.org/project/projectZ/"><img src="https://img.shields.io/pypi/v/projectZ" alt="pypi" /></a>
 	    <a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md"><img src="https://img.shields.io/website?down_message=failing&label=docs&up_color=green&up_message=passing&url=https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md" alt="docs" /></a>
 	</p>
 	<div align="center">
 		<a href="https://github.com/xXxCLOTIxXx/xXxCLOTIxXx/blob/main/sponsor.md">
-			<img src="https://img.shields.io/static/v1?style=for-the-badge&label=Sponsor project&message=%E2%9D%A4&color=ff69b4" alt="Sponsor project"/>
+			<img src="https://img.shields.io/badge/%D0%A1%D0%BF%D0%BE%D0%BD%D1%81%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D1%82%D1%8C-Donate-F79B1F?style=for-the-badge&logo=github&logoColor=FF69B4&color=FF69B4" alt="Sponsor project"/>
 		</a>
-	</div>
-	<table align="center">
-		</tr>
-		<tr> <th colspan="3">More info</th> </tr>
-		<tr>
-			<td>
-				<a href="https://t.me/DxsarzUnion"><img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" height="30px">
-				 Telegram Channel</a>
-			</td>
-			<td>
-				<a href="https://www.youtube.com/channel/UCNKEgQmAvt6dD7jeMLpte9Q"><img src="https://upload.wikimedia.org/wikipedia/commons/0/09/YouTube_full-color_icon_%282017%29.svg" height="30px">
-				 YouTube channel</a>
-			</td>
-			<td>
-				<a href="https://discord.gg/GtpUnsHHT4"><img src="https://www.svgrepo.com/show/353655/discord-icon.svg" height="30px">
-				 Discord Server</a>
-			</td>
-		</tr>
-	</table>
-<h1 align="center">projectZ.py</h1>
-		    
+		<hr>
+		<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=28&duration=2000&pause=2000&color=F79B1F&random=false&width=200&repeat=false&lines=Installation" alt="Installation"/>
+	<p>Git</p>
+	
 ```bash
-pip install projectZ
+pip install git+https://github.com/xXxCLOTIxXx/projectZ.py.git
 ```
-<h4 align="center">or</h4>
-		    
+<p>pypi</p>
+
 ```bash
-pip install git+https://github.com/xXxCLOTIxXx/projectZ.py.git
+pip install projectZ
 ```
-<p align="center">Library for working with projectZ servers, below you will see code examples</p>
-<h1 align="center">Login example</h1>
+<hr><br>
+<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=28&duration=2000&pause=2000&color=F79B1F&repeat=false&random=false&width=90&lines=Using" alt="Using"/>
+</div>
+<h4 align="center">Login example</h4>
 
 ```python
 import projectZ
 
 client = projectZ.Client()
 client.login(email='email', password='password')
 ```
-
-<h1 align="center">Async login example</h1>
+<br><br>
+<h4 align="center">Async login example</h4>
 
 ```python
 import projectZ
 import asyncio
 
 
 client = projectZ.AsyncClient()
 async def main():
 	await client.login(email='email', password='password')
 
 if __name__ == '__main__':
 	loop = asyncio.get_event_loop()
 	loop.run_until_complete(main())
 ```
-
+<hr><br>
+<div align="center">
+<a href="https://github.com/xXxCLOTIxXx/projectZ.py/blob/main/docs/main.md">
+<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=14&duration=1&pause=31&color=3DACF7&random=false&width=195&lines=Read+the+documentation" alt="=Read the documentation"/>
+</a>
+</div>
 </body>
```

### Comparing `projectZ-1.1.7.2.1/setup.py` & `projectZ-1.1.7.2.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from setuptools import setup, find_packages
-from platform import system
 
 with open("README.md", "r") as file:
 	long_description = file.read()
 
 link = 'https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip'
-ver = '1.1.7.2.1'
+ver = '1.1.7.2.1.4'
 
 setup(
 	name = "projectZ",
 	version = ver,
 	url = "https://github.com/xXxCLOTIxXx/projectZ.py",
 	download_url = link,
 	license = "MIT",
```

