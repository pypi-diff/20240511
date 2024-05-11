# Comparing `tmp/anipics-1.5.2.tar.gz` & `tmp/anipics-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipics-1.5.2.tar", max compression
+gzip compressed data, was "anipics-1.5.3.tar", max compression
```

## Comparing `anipics-1.5.2.tar` & `anipics-1.5.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    34519 2024-01-20 19:04:25.749725 anipics-1.5.2/LICENSE
--rw-r--r--   0        0        0      729 2024-01-21 16:14:53.250187 anipics-1.5.2/README.md
--rw-r--r--   0        0        0      297 2024-01-21 16:19:12.732175 anipics-1.5.2/anipics/__init__.py
--rw-r--r--   0        0        0      179 2024-01-21 16:19:12.732175 anipics-1.5.2/anipics/models.py
--rw-r--r--   0        0        0      238 2024-01-21 16:19:12.734175 anipics-1.5.2/anipics/services/__init__.py
--rw-r--r--   0        0        0     1048 2024-01-21 16:19:12.734175 anipics-1.5.2/anipics/services/animepicsx.py
--rw-r--r--   0        0        0     2032 2024-01-21 16:19:12.736175 anipics-1.5.2/anipics/services/nekoslife.py
--rw-r--r--   0        0        0     2942 2024-01-21 16:19:12.736175 anipics-1.5.2/anipics/services/waifupics.py
--rw-r--r--   0        0        0      571 2024-01-21 15:06:57.057592 anipics-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     1530 1970-01-01 00:00:00.000000 anipics-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    34519 2024-01-20 19:04:25.749725 anipics-1.5.3/LICENSE
+-rw-r--r--   0        0        0      728 2024-05-10 20:21:07.857078 anipics-1.5.3/README.md
+-rw-r--r--   0        0        0      297 2024-05-07 15:43:31.902097 anipics-1.5.3/anipics/__init__.py
+-rw-r--r--   0        0        0      179 2024-01-21 16:19:12.732175 anipics-1.5.3/anipics/models.py
+-rw-r--r--   0        0        0      238 2024-01-21 16:19:12.734175 anipics-1.5.3/anipics/services/__init__.py
+-rw-r--r--   0        0        0     1060 2024-05-06 18:31:41.106238 anipics-1.5.3/anipics/services/animepicsx.py
+-rw-r--r--   0        0        0     2036 2024-05-06 18:31:41.143237 anipics-1.5.3/anipics/services/nekoslife.py
+-rw-r--r--   0        0        0     3047 2024-05-06 18:31:41.194235 anipics-1.5.3/anipics/services/waifupics.py
+-rw-r--r--   0        0        0      571 2024-05-07 15:43:22.793311 anipics-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 anipics-1.5.3/PKG-INFO
```

### Comparing `anipics-1.5.2/LICENSE` & `anipics-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anipics-1.5.2/README.md` & `anipics-1.5.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # poetry
 $ poetry add anipics
 ```
 
 ### 🔑 Usage
 
-You can see an example of use [here](/examples/)
+You can see an example of use [here](/examples)
 
 ### Available services
 
 - AnimePicsX
 - NekosLife
 - WaifuPics
```

### Comparing `anipics-1.5.2/anipics/services/nekoslife.py` & `anipics-1.5.3/anipics/services/nekoslife.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 from anipics.models import Models
 
 NekosLifeType = NewType("NekosLifeType", str)
 
 
 class NekosLife:
+    ENDPOINT = "https://nekos.life/api/v2/img/{query}"
+
     class Types:
         wallpaper: NekosLifeType = "wallpaper"
         ngif: NekosLifeType = "ngif"
         tickle: NekosLifeType = "tickle"
         feed: NekosLifeType = "feed"
         gecg: NekosLifeType = "gecg"
         gasm: NekosLifeType = "gasm"
@@ -41,25 +43,23 @@
             query (Union[NekosLifeType, str]): Category of image
 
         Returns:
             Models.Result: Model with `url` parameter
         """
         with httpx.Client() as client:
             return Models.Result(
-                url=client.get(f"https://nekos.life/api/v2/img/{query}").json()["url"]
+                url=client.get(self.ENDPOINT.format(query=query)).json()["url"]
             )
 
     async def async_get(self, query: Union[NekosLifeType, str]) -> Models.Result:
         """Get picture from nekos.life
 
         Args:
             query (Union[NekosLifeType, str]): Category of image
 
         Returns:
             Models.Result: Model with `url` parameter
         """
         async with httpx.AsyncClient() as client:
             return Models.Result(
-                url=(await client.get(f"https://nekos.life/api/v2/img/{query}")).json()[
-                    "url"
-                ]
+                url=(await client.get(self.ENDPOINT.format(query=query))).json()["url"]
             )
```

### Comparing `anipics-1.5.2/anipics/services/waifupics.py` & `anipics-1.5.3/anipics/services/waifupics.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 from anipics.models import Models
 
 WaifuPicsType = NewType("WaifuPicsSFWType", str)
 
 
 class WaifuPics:
+    ENDPOINT = "https://api.waifu.pics/{_type}/{query}"
+
     class Types:
         class SFW:
             waifu: WaifuPicsType = "waifu"
             neko: WaifuPicsType = "neko"
             shinobu: WaifuPicsType = "shinobu"
             megumin: WaifuPicsType = "megumin"
             bully: WaifuPicsType = "bully"
@@ -60,15 +62,17 @@
 
         Returns:
             Models.Result: Model with `url` parameter
         """
         _type = "nsfw" if nsfw else "sfw"
         with httpx.Client() as client:
             return Models.Result(
-                url=client.get(f"https://api.waifu.pics/{_type}/{query}").json()["url"]
+                url=client.get(self.ENDPOINT.format(_type=_type, query=query)).json()[
+                    "url"
+                ]
             )
 
     async def async_get(
         self, query: Union[WaifuPicsType, str], nsfw: bool
     ) -> Models.Result:
         """Get pictire from waifu.pics
 
@@ -79,10 +83,10 @@
         Returns:
             Models.Result: Model with `url` parameter
         """
         _type = "nsfw" if nsfw else "sfw"
         async with httpx.AsyncClient() as client:
             return Models.Result(
                 url=(
-                    await client.get(f"https://api.waifu.pics/{_type}/{query}")
+                    await client.get(self.ENDPOINT.format(_type=_type, query=query))
                 ).json()["url"]
             )
```

### Comparing `anipics-1.5.2/pyproject.toml` & `anipics-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipics"
-version = "1.5.2"
+version = "1.5.3"
 description = "Simple module to get anime pictures"
 authors = ["Daniel <D4n13l3k00@yandex.ru>"]
 readme = "README.md"
 license = "AGPL-3.0"
 repository = "https://github.com/D4n13l3k00/anipics"
 
 [tool.poetry.dependencies]
```

### Comparing `anipics-1.5.2/PKG-INFO` & `anipics-1.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: anipics
-Version: 1.5.2
+Version: 1.5.3
 Summary: Simple module to get anime pictures
 Home-page: https://github.com/D4n13l3k00/anipics
 License: AGPL-3.0
 Author: Daniel
 Author-email: D4n13l3k00@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Project-URL: Repository, https://github.com/D4n13l3k00/anipics
 Description-Content-Type: text/markdown
 
 <div align='center'>
@@ -42,15 +43,15 @@
 
 # poetry
 $ poetry add anipics
 ```
 
 ### 🔑 Usage
 
-You can see an example of use [here](/examples/)
+You can see an example of use [here](/examples)
 
 ### Available services
 
 - AnimePicsX
 - NekosLife
 - WaifuPics
```

